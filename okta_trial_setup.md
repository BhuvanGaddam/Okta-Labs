# Okta Trial Setup Guide

This guide explains how to create a free trial account in Okta and
access the Okta Admin Console to start working with Identity and Access
Management (IAM) features.

------------------------------------------------------------------------

## Overview

Okta provides a free trial environment that allows users to explore
identity management, authentication, and Single Sign-On (SSO)
integrations.

This lab environment will be used for:

-   User management
-   Group management
-   Role-based access control
-   SAML Single Sign-On (SSO) integrations
-   Application integrations

------------------------------------------------------------------------

## Prerequisites

Before starting, ensure you have:

-   A valid email address
-   Internet access
-   A modern web browser (Chrome / Edge / Firefox)

------------------------------------------------------------------------

## Step 1 -- Register for Okta Free Trial

1.  Open the Okta free trial page:

https://www.okta.com/free-trial/

2.  Click **Start Free Trial**

3.  Fill in the registration details:

  Field        Example
  ------------ ------------------
  First Name   John
  Last Name    Doe
  Work Email   john@example.com
  Country      Your Country

4.  Click **Sign Up**

------------------------------------------------------------------------

## Step 2 -- Verify Email

1.  Check your email inbox.
2.  Open the verification email from Okta.
3.  Click the **Activate Account** link.

------------------------------------------------------------------------

## Step 3 -- Create Okta Password

After verification:

1.  Set your **password**
2.  Configure **Multi-Factor Authentication (if prompted)**

------------------------------------------------------------------------

## Step 4 -- Access Okta Admin Console

Once the account is activated:

1.  Login to your Okta tenant.

Example tenant URL:

    https://your-domain.okta.com

2.  Open the **Admin Console**.

You will see the Okta dashboard where you can manage:

-   Users
-   Groups
-   Applications
-   Security Policies

------------------------------------------------------------------------

## Step 5 -- Explore the Admin Dashboard

Key sections inside the **Okta Admin Console**:

### Directory

Manage identities in your organization.

-   People (Users)
-   Groups
-   Profile Editor

### Applications

Manage integrations with third-party applications.

Examples: - Google Workspace - Zendesk - Freshworks

### Security

Configure authentication and security policies.

-   Multi-Factor Authentication
-   Authentication policies
-   Identity providers

### Reports

View logs and security events.

------------------------------------------------------------------------

## Okta Architecture

Okta acts as an **Identity Provider (IdP)** and supports authentication
protocols such as:

-   SAML
-   OAuth
-   OpenID Connect

These protocols allow secure authentication between Okta and external
applications.

------------------------------------------------------------------------

## Expected Outcome

After completing this setup:

-   You will have a working **Okta trial environment**
-   You will be able to access the **Admin Console**
-   You can start creating users, groups, and applications

------------------------------------------------------------------------

## Next Steps

After creating the Okta environment, proceed with the following labs:

1.  User Creation
2.  Group Creation and Rules
3.  Least Privilege Implementation
4.  SAML SSO Integration with Freshworks
5.  SAML SSO Integration with Zendesk

------------------------------------------------------------------------

## Reference

Official Documentation:

https://developer.okta.com/docs/
