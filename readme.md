# SilverStripe AMP HTML
Converts pages to Google Amp HTML. For more information about AMP HTML see [Google AMP Project Homepage](https://www.ampproject.org).

## Requirements
* SilverStripe 3.2.x

## Installation
**Composer (recommended):**

`composer require thezenmonkey/silverstripe-amp`

If you prefer you may also install manually:

* Download the module from here LINK
* Extract the downloaded archive into your site root so that the destination folder is called silverstripe-amp, opening the extracted folder should contain _config.php in the root along with other files/folders
* Run dev/build?flush=all to regenerate the manifest

##  Usage
The module automatically adds a link to your MetaTags pointing to the AMP HTML version of the page `http://yousite.com/page-name/amp.html`.

A custom controller then renders your content using an AMP HTML version of the Page Template. `<img />` tags are automatically converted to `<amp-img />` before render.

### Themes and Custom Page Types

The base Page type is `Amp.ss`, which can be overidden in your theme like any SilvserStripe Template. Custom Page Types can be rendered using `ClassName-Amp.ss` in your theme.

## To Do
This is an initial commit as proof of concept as such
* Add Base Styling to Match Simple Theme
* Create Modular Schema System
* Add Configurable Scripts for Common Amp Components

