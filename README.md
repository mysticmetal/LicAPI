# LicAPI

[![Build Status](https://travis-ci.org/m1guelpf/LicAPI.svg?branch=master)](https://travis-ci.org/m1guelpf/LicAPI)   [![Code Climate](https://codeclimate.com/github/m1guelpf/LicAPI/badges/gpa.svg)](https://codeclimate.com/github/m1guelpf/LicAPI)

A PHP API to manage license info

## What is LicAPI?

LicAPI is an script that allows you to manage, verify and return data from your licenses.

## Demo:

You can see a demo of the script at [https://demo.miguelpiedrafita.com/LicAPI/admin.php](https://demo.miguelpiedrafita.com/LicAPI/admin.php) using username&password 'licapi' (without the '') or test the verification function at [https://demo.miguelpiedrafita.com/LicAPI/test.html](https://demo.miguelpiedrafita.com/LicAPI/test.html) or by GET at [https://demo.miguelpiedrafita.com/LicAPI/api.php?license=test](ttps://demo.miguelpiedrafita.com/LicAPI/api.php?license=test).

## Requirements:

- PHP >4.1
- MySQL database

## Installation:

- Upload all the files to your server.
- Create a MySQL Database.
- Import database info from licapi.sql.
- Open config.php, fill your database info and change
```php
$debug = false;
``` 

to
```php
$debug = true;
```
- Run the script with license test (do api.php?license=test).
- If the script doesn't show any errors, you're OK!
- **REMEMBER TO TURN $debug BACK TO false!!!**
- Change the demo info with your own custom info using the admin.php page.
- Enjoy!

## Errors:

All the interesting activity is logged to the table 'activity' with an activityId. The activityId can be used to identify errors in production or to log any strange activity. Only IP Adress, User-Agent, ActivityId and ActivityTitle is logged.

## Credits:

- [Miguel Piedrafita](https://projects.miguelpiedrafita.com)
- [PHP](https://php.net)
- [MySQL](https://mysql.com)

Copyright (C) Miguel Piedrafita. Use of this work is subject to Mozilla Public License 2.0
