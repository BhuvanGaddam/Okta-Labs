# SSO Integration with SAML for Freshworks Application

## Objective

Integrate **Single Sign-On (SSO)** using **SAML** between **Okta** and
**Freshworks** so users can log in to Freshworks through Okta.

------------------------------------------------------------------------

## Step 1: Create a Trial Account

1.  Go to the Freshworks website: https://www.freshworks.com/
2.  Create a **trial account**.
3.  Note the **Freshworks domain name**.

------------------------------------------------------------------------

## Step 2: Add Freshworks Application in Okta

1.  Login to **Okta Admin Console**.
2.  Navigate to:

Applications → Browse App Catalog

3.  Search for **Freshworks**.
4.  Click **Add Integration**.

------------------------------------------------------------------------

## Step 3: Configure Application Details

1.  Provide the **Application Name**.
2.  Specify the **Freshworks domain name**.
3.  Click **View SAML Instructions**.

------------------------------------------------------------------------

## Step 4: Configure SSO in Freshworks

1.  Navigate to **Freshworks Dashboard**.
2.  Go to:

Admin Settings → SSO

3.  Enable **SSO**.
4.  Select **Okta with SAML**.
5.  Copy the **Customer ID** from Freshworks.

------------------------------------------------------------------------

## Step 5: Configure SAML Parameters

1.  Paste the **Customer ID** into the Okta configuration.
2.  From **Okta SAML Instructions**, copy the following values:

-   Entity ID provided by the IdP\
-   SAML SSO URL\
-   Security Certificate

3.  Paste these values into the **Freshworks SSO Dashboard**.
4.  Click **Configure SSO**.

------------------------------------------------------------------------

## Step 6: Configure Username Format in Okta

1.  Go to:

Okta Admin Console → Applications → Freshworks

2.  Change **Application Username Format** to:

Email

3.  Click **Save**.

------------------------------------------------------------------------

## Step 7: Create and Assign User

1.  Create a **new user in Okta**.
2.  Ensure the **email ID matches the Freshworks account email**.
3.  Assign the **Freshworks application** to the user.

------------------------------------------------------------------------

## Step 8: Test SSO Login

1.  Login to the **Okta End-User Dashboard**.
2.  Click the **Freshworks application**.
3.  Verify that the user **successfully signs in using SSO**.

------------------------------------------------------------------------

## Expected Result

Users should be able to **log in to Freshworks directly from Okta
without entering separate credentials**, confirming successful **SAML
SSO integration**.
