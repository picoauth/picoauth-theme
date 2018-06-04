# PicoAuth theme

The default theme for Pico CMS that can be used with the PicoAuth plugin. This theme **depends on the PicoAuth plugin** and will not work without it.

Feel free to use this theme as a template for your own customized theme for a Pico website using the PicoAuth plugin.

## Features

* Adds a login bar to the top of each page with an option to log in, register (if enabled).
* For a logged user it displays a username, an option to logout and link to the page to change password (if enabled).
* Can also display a small profile picture next to the username (if configured in PicoAuth).
* Displays an option to *Close locks session* (if PageLock module is configured and at least 1 lock has been unlocked)
* This theme is responsive.
* Structure of the forms (login, registration, etc.) is kept default.

## Installation
The recommended way of installation is using composer:
```
composer require picoauth/picoauth-theme
```

After the installation is complete, in Pico `config.yml` set `theme: picoauth-theme`.

## Screenshot
![Theme header](https://i.imgur.com/6Fqb5Y8.png)

## How to use

This theme contains only a set of simple Twig templates. The CSS is loaded from the PicoAuth plugin files (the plugin must be installed).
The key part of this theme is `index.twig` which applies the default layout from PicoAuth to the whole Pico CMS website and also adds a login bar to the top of each page.

### Customization

Refer to the *Theme customization* section of the [PicoAuth Documentation](https://github.com/picoauth/picoauth/wiki) for the full reference on how to create/customize themes when using PicoAuth.
