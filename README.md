# Laravel Themes Installer
[![Latest Stable Version](https://poser.pugx.org/prismalms/laravel-themes-installer/v)](//packagist.org/packages/prismalms/laravel-themes-installer) [![Total Downloads](https://poser.pugx.org/prismalms/laravel-themes-installer/downloads)](//packagist.org/packages/prismalms/laravel-themes-installer) [![License](https://poser.pugx.org/prismalms/laravel-themes-installer/license)](//packagist.org/packages/prismalms/laravel-themes-installer)

This package facilitates working with theme packages by enabling the installation of standalone theme packages directly into the `themes/` directory instead of the `vendor/` directory.

For example if your Theme package name is `prismalms/admin-theme` then the package will be installed into `themes/prismalms/admin` directory.

You can specify an alternate directory by including a `theme-dir` in the extra data in your composer.json file:

    "extra": {
        "theme-dir": "custom"
    }

## Installation

1. Ensure you have the `type` set to `laravel-theme` in your theme's `composer.json`
2. Require this package: `composer require prismalms/laravel-themes-installer`
3. Require your bespoke theme using Composer

## Notes

When working on a theme that is version controlled within an app that is also version controlled, you have to commit and push from inside the Theme directory and then `composer update` within the app itself to ensure that the latest version of your theme (dependant upon constraint) is specified in your composer.lock file.

## Related projects
- [Laravel Themes Manager](https://github.com/prismalms/laravel-themes-manager): Develop multi-themes Laravel application with ease.

## Credits
- This project is a modified version of [hexadog/laravel-theme-installer](https://github.com/hexadog/laravel-theme-installer), created as a fork with additional changes.

## License
Laravel Themes Manager is open-sourced software licensed under the [MIT license](LICENSE).
