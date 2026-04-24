# Least Privilege Principle Implementation Use Case

## Read-Only Administrator Role in Okta

### Objective

Demonstrate the implementation of the Least Privilege Principle by
assigning a Read-Only Administrator role to a user in Okta.

------------------------------------------------------------------------

### Configuration Steps

1.  Log in to the Okta Admin Console.
2.  Navigate to **Directory \> People**.
3.  Select the required **User**.
4.  Go to **Admin Roles**.
5.  Click **Add Individual Admin Privileges**.
6.  Select the role **Read-Only Administrator**.
7.  Click **Save Changes**.

------------------------------------------------------------------------

### Validation Steps

1.  Open a new **Incognito / Private Browser tab**.
2.  Log in using the **assigned user account**.
3.  Access the **Okta Admin Console**.

------------------------------------------------------------------------

### Expected Result

-   The user successfully logs in to the Okta Admin Console.
-   The user is granted **Read-Only Administrator privileges**.
-   The user can **view configurations but cannot modify them**,
    enforcing the Least Privilege Principle.
