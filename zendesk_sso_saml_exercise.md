# Exercise: SSO Integration with SAML for Zendesk

## Objective

Integrate **Single Sign-On (SSO)** using **SAML** between **Okta** and
**Zendesk** so that users can authenticate to Zendesk through Okta.

------------------------------------------------------------------------

## Prerequisites

-   Okta Admin access
-   Zendesk Admin account
-   User email in Okta must match the Zendesk user email

------------------------------------------------------------------------

## Step 1: Create a Trial Account on Zendesk

1.  Go to: https://www.zendesk.com/register/
2.  Create a **Zendesk trial account**.
3.  Note the **Zendesk domain name** (example:
    `yourcompany.zendesk.com`).

------------------------------------------------------------------------

## Step 2: Add Zendesk Application in Okta

1.  Login to **Okta Admin Console**.

2.  Navigate to:

    Applications → Applications → Browse App Catalog

3.  Search for **Zendesk**.

4.  Click **Add Integration**.

5.  Provide the following details:

    -   Zendesk Subdomain
    -   Application label (optional)

6.  Click **Done**.

------------------------------------------------------------------------

## Step 3: Configure SAML in Zendesk

1.  Login to **Zendesk Admin Center**.

2.  Navigate to:

    Security → Single Sign-On (SSO)

3.  Enable **SAML SSO**.

4.  Select **Okta** as Identity Provider (IdP).

------------------------------------------------------------------------

## Step 4: Copy SAML Details from Okta

In **Okta Application Settings**, locate:

-   Identity Provider Single Sign-On URL
-   Identity Provider Issuer
-   X.509 Certificate

Copy these values.

------------------------------------------------------------------------

## Step 5: Configure Zendesk SAML Settings

Paste the following values in Zendesk SSO configuration:

-   **Entity ID / Issuer**
-   **SAML SSO URL**
-   **X.509 Certificate**

Save the configuration.

------------------------------------------------------------------------

## Step 6: Configure Application Username

1.  Go to **Okta Admin Console → Applications → Zendesk**.

2.  Edit **Sign On Settings**.

3.  Change **Application username format** to:

    Email

4.  Save changes.

------------------------------------------------------------------------

## Step 7: Assign Users to Zendesk Application

1.  Navigate to:

    Okta Admin Console → Directory → People

2.  Create a **new user**.

3.  Ensure the **email ID matches the Zendesk user email**.

4.  Assign the **Zendesk application** to that user.

------------------------------------------------------------------------

## Step 8: Test SSO Login

1.  Login to **Okta End-User Dashboard**.
2.  Click **Zendesk application icon**.
3.  Verify that the user is **successfully logged into Zendesk using
    SSO**.

------------------------------------------------------------------------

## Expected Result

Users should be able to login to **Zendesk directly from Okta without
entering separate credentials**, confirming successful **SAML SSO
integration**.

------------------------------------------------------------------------

## Lab Validation Checklist

-   Okta Zendesk application created
-   SAML parameters configured correctly
-   User assigned to application
-   Successful SSO login verified
