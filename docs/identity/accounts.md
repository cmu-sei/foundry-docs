# Accounts

This is where Identity administrators track Identity users. Things administrators can do here include:

- Searching for user accounts
- Creating new accounts
- Creating override codes
- Sending email to users
- Enabling and disabling accounts
- Changing an account's *role*
- Generating a passcode
- Adding an email address

*Administrator* and *manager* roles are denoted by a star in the Identity user interface.

![admin star](img/star.png)

## Update an existing account

Use the **Search** field to find the account you want to update.

- **State:** Enable or Disable an account.
- **Role:** Change an account's role to *member* or *manager*. A *member* can only act on their own account (i.e., update profile, configure 2FA). A *manager* can act on other accounts (i.e., enable or disable, generate authorization codes, add email address, create new accounts). 
- **Code:** Generate an authorization to provide to an account trying to log into Identity.
- **Email:** Add an additional email address to the account.

!!! info
    There is an *administrator* role available; however, it must be enabled in the database. Contact your Identity administrator for help with this role.

## Create a new account

At the bottom of the Accounts screen, click **New Account**. Enter the account information like this: `First Last <email@some.site>`. You can enter an initial password here; but it's recommended to leave that field blank. Users can use the **Reset my password** option at their first login attempt.

## New Override Code

At the bottom of the Accounts screen, click **New Override**. Add a global code for registration and password resets in no email deployment.

!!! info
    Reminder that you must be an *admin* or *manager* in order to create accounts and override codes.