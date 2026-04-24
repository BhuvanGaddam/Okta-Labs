# Okta IAM Lab -- User Creation

## Objective

The objective of this exercise is to create a new user in the Okta Admin
Console and verify that the user can successfully log in to the Okta
dashboard.

------------------------------------------------------------------------

## Step 1 -- Access Okta Admin Console

1.  Log in to your Okta Admin Console.
2.  Navigate to the user management section.

Okta Admin Console → Directory → People

------------------------------------------------------------------------

## Step 2 -- Create a New User

1.  Click **Add Person**.
2.  Enter the required user details.

Example:

  Field           Example
  --------------- ----------------------
  First Name      Test
  Last Name       User
  Username        testuser@example.com
  Primary Email   testuser@example.com

3.  Click **Save**.

------------------------------------------------------------------------

## Step 3 -- Verify User Creation

1.  After saving, the user will appear in the **People** directory.
2.  Verify that the user profile information is correct.

------------------------------------------------------------------------

## Step 4 -- Test User Login

1.  Open a **new browser tab** or **incognito window**.
2.  Navigate to the Okta login page.
3.  Log in using the newly created user credentials.

------------------------------------------------------------------------

## Expected Outcome

-   The user should be successfully created in the Okta directory.
-   The user should be able to log in to the Okta dashboard.
-   The administrator should be able to view the user profile in the
    **People** section.

------------------------------------------------------------------------

## Learning Outcome

After completing this exercise, you will understand:

-   How to create users in Okta
-   How to manage users in the Okta directory
-   Basic identity provisioning in an IAM platform
