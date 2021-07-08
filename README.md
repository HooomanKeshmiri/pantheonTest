
# pantheonTest: Test Drupal website on Pantheon platform
This is a basic Drupal website that was developed through Pantheon and Lando. The goal of this project was to get familiar with both making content directly with Drupal as well as using Lando to initialize the website.
#
## Description:
This application is website that can be navigated by anyone made in Drupal. It can be used by anyone to get familiar with both using Drupal. It is recommended that if you are to download the files and launch the website that you use Lando to both initialize and launch the site. The Lando installation guide will be posted further below. To develop the web page Drupal was used as this is a predecessor to a project that I will be on using Drupal and I needed to learn how to use Drupal effectively. Issues arose when attempting to use a drupal8 recipe directly from lando as opposed to pantheon, and editing files would not fix the issue that arose and I plan to solve this issue in the future.

#

## Installation:

Downloading Lando: https://docs.lando.dev/basics/installation.html

To use this web page first download the code base from github. Following that install Lando on your device and in the repository that you cloned.  

 Type `lando start` to have lando build the app. Following that it will display a URL that is the name you set in the `.lando.yml` file followed by .lndo.site. Then type `lando pull` to pull the pantheon database to your local machine. Then you can either copy the URL into your browser or type `open firstDrupalSite.lndo.site` to open the webpage. After that the website should open and you should be able to interact with the drupal website.

#

## Usage:
The usage of this web page is extremely simple and like every other webpage. If you would like to edit the page you can visit the developmental tools in the Drupal GUI.

#### Module / Theme Editing 
In drupal there are some default themes that you can install for the website but you can also download external ones. Using `lando composer require drupal/a_theme:(version)`. This also applies to modules that you would like to install.

## Troubleshooting
Some issues may occur while using/editing this site.  Somethings to try:

`lando drush cr all` clears the cache of current site and you can use `lando restart` to restart the wbesite. You can also use `lando rebuild -y` to rebuild the website in your Docker.

Finally if the above don't work you can destroy the site as a last measure. `lando destroy` to destroy the site for a rebuild.
#
Credits:
Hooman Keshmiri
Farnoosh Johnson