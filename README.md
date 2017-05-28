# SimpleUserManager
Simple User Manager Functions for ProcessWire.

This module provides basic front-end user registration, email verification, login, password reset, and profile management functions.

**Note:** This module ues the PHPMailer (included) to send emails.

## Registration
The following data is collected during user registration. All fields are required. If a company name does not exist, the company name becomes a concatenation of the user's first and last names.
* First Name
* Last Name
* Company Name
* Email Address

## Email Verification
Upon submitting the registration form, a verification email is sent to the user-supplied email address. The verification email contains a token which the user must enter in the verification form to complete the verification process. This token is valid for a specified time period and defined in the module config settings. The user may request another verification email be sent should the current verification expire.

## User Login
The user provides the email address and password defined during registration in order to log in. The user has three (default config setting) attempts to log in, after which the account is temporarily disabled for a specified time period (config setting). The user may log in again after this time period has expired.

## Password Reset
A password reset (forgot password) token is sent to the email address defined during registration. The same expiration exists for password reset as for email verification. The password reset form requests a new password and verify new password entries. If the passwords match, the user is redirected to the login form where they can log in with the new credentials.

## Profile Management
The user profile consists of the data collected during registration and the following additional fields.
* User Avatar
* ???
