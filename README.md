# UAL Webform Spambot

This is a Drupal 7 module that allows you to check Webform submissions against the [Stop
 Forum Spam](https://www.stopforumspam.com/) database.  Currently, it only supports a single Webform
 and is geared toward the "Contact Us" form on the Special Collections and main Library website.

## Installation

* Install the [Spambot module](https://www.drupal.org/project/spambot) and enable it.
* Clone this repo into the correct modules folder for your Drupal installation.
* Copy `defines.php.dist` to `defines.php`.
* Edit `defines.php` and set `UAL_WEBFORM_SPAMBOT_FORM_ID` to the correct value for the webform.
You may have to figure this out by editing this module's `ual_webform_spambot_form_alter()` function
and adding a call to `die($form_id)` or `dpm($form_id)`.
* Set `UAL_WEBFORM_SPAMBOT_EMAIL_ADDRESS_FIELD` to the form key of the field that contains the submitter's
email address.
* Enable this module.
