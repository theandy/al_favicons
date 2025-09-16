# Favicons for your TYPO3 Website
***
Creates Favicons in different sizes and ads web app manifest. Supports favicons for dark mode.

# Installation
* `/usr/bin/php8.1 composer.phar req andreas-loewer/al-favicons:@dev`
* Include the AL Favicons (al_favicons) to your TypoScript

# Configuration
## Options
* You can set your Options (files and other configuration options) in constant editor
## Optional configuration
### Name of the webmanifest file
If not set, the manifest file ist renders as `<link rel="manifest" href="/?type=8422">` in your source code.
To use a name instead of ?type=8422, you can add this type to the site configuration (the .yaml file):

    map:
      site.webmanifest: 8422

This results in `<link rel="manifest" href="/site.webmanifest">`.

## Adaptive SVG Favicon
This extension supports files for dark and light mode. The .ico and .png files can be provided seperately.
The .svg file should adapt to the color scheme automatically. See the example svg in this extension.
