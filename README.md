# UAL Webform Spambot

This is a Drupal 7 module that allows you to check Webform submissions against the [Stop
 Forum Spam](https://www.stopforumspam.com/) database.  Currently, it only supports a single Webform
 and is geared toward the "Contact Us" form on the Special Collections and main Library website.

## Installation

* Install the [Spambot module](https://www.drupal.org/project/spambot) and enable it.
* Clone this repo into the correct modules folder for your Drupal installation.
* Enable this module.
* (Optional) Set the `ual_webform_spambot_form_id` variable to the correct form id for the webform you'd like to protect.
You can do this using `drush vset`.  By default, this variable is set to `webform_client_form_41`, which is the `form_id`
of the "Contact Us" form on http://new.library.arizona.edu.
* (Optional) Set the `ual_webform_spambot_email_field` variable to the correct field name for the email field on your webform.
You can do this using `drush vset` as well.  By default, this variable is set to `your_email`, which is the correct value for the "Contact Us" form on http://new.library.arizona.edu.
