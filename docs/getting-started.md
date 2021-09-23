# Getting started

_**Please note:** the design system is currently being updated while Studio 24 is working on the W3C redesign project. These
instructions are currently intended for W3C to test the design system. We plan to release a tagged version of the design
system once this work is done (in November)._

## In a standalone project

### Installing via Composer
You can install the Design System via [Composer](https://getcomposer.org/) via:

```
composer require w3c/website-templates-bundle:dev-main
```

This requires PHP 7.4+

_Please note, this currently works best within a Symfony project. We are working on improved methods to install the Design 
System for non-Symfony sites._

### Installing via ZIP file

You can also download a [ZIP archive file](/assets/assets.zip) of the frontend assets and use these within your project.

_Todo: Review with W3C whether we can get users to point directly to the WSC assets on beta.w3.org / w3.org_

### Frontend assets
This will install the built front-end assets for the Design System into `vendor/w3c/website-templates-bundle/public/dist/assets`

You can then copy these into your project codebase. 

If you wish to use the SASS files, you can find these in `vendor/w3c/website-templates-bundle/assets-src`

If you wish to copy our build process for frontend assets see `vendor/w3c/website-templates-bundle/package.json` file.

### HTML templates

You can create HTML templates based on the examples in the Design System. For example the [Default template](https://design-system.w3.org/code/default.html) 
contains all the global styles required for pages.

If you wish to use Twig templates, you can use the Twig templates in `vendor/w3c/website-templates-bundle/design-system-templates`
as a starting point.

For Symfony projects please see below on how to integrate the design system using the bundle system.

## In a Symfony project

For usage instructions on how to install the W3C Design System as a [Symfony bundle](https://symfony.com/doc/current/bundles.html)
see the [w3c-website-templates-bundle README](https://github.com/w3c/w3c-website-templates-bundle/blob/main/README.md).

Please note these contain complex Twig templates designed to be integrated into the [W3C frontend website project](https://github.com/w3c/w3c-website-frontend).

_Todo: review with W3C if we can bridge the gap between the Symfony template bundle & the design system and move usage docs here_

_Todo: review with W3C how portable these Twig bundle templates really are between different Symfony projects_