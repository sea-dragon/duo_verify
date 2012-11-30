# Overview
Sample PHP code for calling the Duo Verify API

## Author
Jack Wink
Last Update: 2011-08-15

# Setup

## Configuration
Define the following values at the top of the `duo_verify.php` file:

- `HOST`  = API hostname
- `IKEY`  = Integration key
- `SKEY`  = Secret key
- `PHONE` = E.164-formatted phone number of the call recipient. Spaces and dashes are optional. For example, a US number could look like "+1 555 555-5555" or "+15555555555"

## PHP Version
This sample code relies on functions available starting PHP 5.1.2.  You will need to be able to call `hash_hmac()` with a SHA1 digest.

# Running
Run `duo_verify.php` (e.g. from the command line `php duo_verify.php`) after you configured the file (See above).  It will call you, give you a pin, and then ask you for the pin.  It will poll the call status throughout the phone call.

# Need Help?
Please see the Duo Verify documentation:

<http://www.duosecurity.com/docs/duoverify>
