# Symfony PHP CodeSniffer Coding Standard (PCG Cube flavor)

A coding standard to check against the [Symfony coding standards](http://symfony.com/doc/current/contributing/code/standards.html),
based on excellent [escapestudios/symfony2-coding-standard](https://github.com/djoos/Symfony2-coding-standard) repository.

_Important note:_ Please be careful using this library, as it is for internal usage, and probably will not be maintained

## Differences

The following standards has been modified:

- added the Symfony.Commenting.FunctionComment.MissingParamType
- removed the Symfony.Commenting.FunctionComment.SpacingAfterParamType
- removed the Symfony.Commenting.Annotations.Invalid
- removed the Symfony.Functions.Arguments.Invalid
- removed the Squiz.Strings.ConcatenationSpacing.PaddingFound

## Installation

### Composer

This standard can be installed with the [Composer](https://getcomposer.org/) dependency manager.

1. [Install Composer](https://getcomposer.org/doc/00-intro.md)

2. Install the coding standard as a dependency of your project

        composer require --dev karen-nalbandian/symfony-coding-standard:dev-master

3. Add the coding standard to the PHP_CodeSniffer install path

        vendor/bin/phpcs --config-set installed_paths vendor/karen-nalbandian/symfony-coding-standard

4. Check the installed coding standards for "Symfony"

        vendor/bin/phpcs -i

5. Done!

        vendor/bin/phpcs /path/to/code

### Stand-alone

1. Install [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer)

2. Checkout this repository

        git clone https://github.com/karen-nalbandian/symfony-coding-standard.git

3. Add the coding standard to the PHP_CodeSniffer install path

        phpcs --config-set installed_paths /path/to/symfony-coding-standard

   Or copy/symlink this repository's "Symfony"-folder inside the phpcs `Standards` directory

4. Check the installed coding standards for "Symfony"

        phpcs -i

5. Done!

        phpcs /path/to/code
