# UserManager
Basic User Manager Functions for ProcessWire.

This module provides basic front-end user registration, email verification, login, password reset, and profile management functions.

## Registration
The following data is collected during user registration. All fields are required. If a company name does not exist, the company name becomes a concatenation of the user's first and last names.
* First Name
* Last Name
* Company Name
* Email Address
* Password

Upon submitting the registration form, a verification email is sent to the user-supplied email address. The verification email contains a link to complete the verification process. This link is valid for a specified time period and defined in the module config settings. The user may request another verification email be sent should the current verification expire.

