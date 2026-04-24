# Disable Self-Service Password Reset (SSPR) in Okta

## Objective
Disable the **Self-Service Password Reset (SSPR)** feature for specific users using Password Policy rules in Okta.

---

## Step 1: Navigate to Password Policy
1. Login to Okta Admin Console
2. Go to:
   
   **Security → Authentication → Okta Account Management Policy → Password Policy**

---

## Step 2: Create New Rule
1. Click on **Add New Rule**
2. Configure the following:

- **Rule Name:** Password reset restriction
- **Exclude Users:** Specify users to exclude from this policy (if needed)

---

## Step 3: Define Conditions
- **IF User's IP is:** Anywhere

---

## Step 4: Disable Self-Service Options
Under **THEN Users can perform self-service**, uncheck all options:

- ❌ Password change (from account settings)
- ❌ Password reset
- ❌ Unlock account

---

## Step 5: Create Rule
- Click **Create Rule** to apply the configuration

---

## Step 6: Testing the Configuration
1. Go to Okta End User Dashboard/Login Page
2. Click on **Forgot Password**
3. Enter the user credentials

### Expected Result:
- Password reset should **NOT work**
- User will not be able to reset password using self-service

---

## Outcome
- SSPR is successfully disabled
- Only admins can reset passwords

---

## ⚠️ Notes
- Ensure the rule is applied to the correct users/groups
- Keep SSPR enabled for normal users if required
- Recommended to disable SSPR only for **privileged/admin accounts**

---

## 🚀 Conclusion
This lab demonstrates how to restrict password reset capabilities in Okta using policy rules, improving security for sensitive accounts.

