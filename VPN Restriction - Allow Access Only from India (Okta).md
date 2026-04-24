# VPN Restriction - Allow Access Only from India (Okta)

Restrict user login access in Okta to only **India region** and block access from other locations using Network Zones and Global Session Policies.

---

## Step 1: Login to Okta Admin Console
- Access your Okta Admin Dashboard

---

## Step 2: Create Network Zone (India)

1. Navigate to:
   **Security → Networks**
2. Click **Add Zone**
3. Select **Dynamic Zone**

### Configure:
- **Zone Name:** Indian
- ❌ Uncheck: Block access from IPs matching conditions listed in this zone
- **IP Type:** Any
- **Location:** India
- *(Optional)* Add State/Region

4. Click **Save**

---

## Step 3: Configure Global Session Policy

1. Navigate to:
   **Security → Global Session Policy**
2. Click **Add New Rule**

### Configure Rule:
- **Rule Name:** Network - Block
- **Exclude Users:** (Optional – specify users to exclude)

### Policy Conditions:
- **IF User's IP is:** Not in zone → Indian  
- **Identity Provider:** Any  
- **Authenticates via:** Any  
- **Behavior:** Any  
- **Risk:** Any  

### Action:
- **THEN Access is:** Denied  

3. Click **Save**

---

## Step 4: Testing

1. Connect to a **VPN outside India**
2. Try logging in as an end user

### Expected Result:
- Login request should be **blocked**
- Access denied due to non-Indian location

---

## Outcome
- Users can only log in from India  
- All other regions are blocked  

---

## ⚠️ Notes
- Ensure correct rule order in policies  
- Always exclude at least one admin user to avoid lockout  
- Test using non-admin account  

---

## 🚀 Conclusion
This setup enforces **location-based access control**, aligning with Zero Trust principles by restricting access based on geographic location.
