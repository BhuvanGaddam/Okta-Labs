# Automate Bulk User Creation Using CSV in Okta
Bulk user creation in Okta allows administrators to efficiently onboard multiple users by uploading a CSV file containing user details such as name, email, department, and role. This process automates account provisioning, reduces manual effort, ensures consistency, and can trigger group assignments and application access based on predefined policies.
## Steps

### 1. Login to Okta Admin Console

Login to your Okta Admin Console with administrator credentials.

### 2. Navigate to Import Option

Go to: **Directory → People → More Actions → Import Users from CSV
File**

### 3. Download and Fill Template

-   Download the CSV template.
-   Fill in the mandatory fields.
-   Ensure **username is the email ID**.

#### Sample Users
  -----------------------------------------------------------------------
  First Name  Last Name Email (Username)         Login
  ----------- --------- ------------------------ ------------------------
  
### 4. Upload CSV File

Upload the completed CSV file into Okta.

### 5. Configure Import Settings

-   Select **Import Users**
-   Enable **Automatically activate new users**

### 6. Set Password and Activate

-   Select imported users
-   Click **Set Password and Activate**

### 7. Verify User Access

-   Login to the **End User Dashboard**
-   Use the **temporary password**
-   Verify access to applications

------------------------------------------------------------------------

## Outcome

Bulk users are successfully created and activated in Okta using CSV
import.
