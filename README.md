# DDEV Magento2 Environment Setup

This repository provides a streamlined setup for a Magento 2 environment, ideal for demo purposes, module development, and theme development in isolation.

## Purpose

This project was created for those times when you need a clean development environment to contribute to an open-source module or theme quickly.
It's not intended to be a one-size-fits-all solution for all Magento 2 related work, but rather an automated version of [Magento 2 Quickstart by DDEV](https://ddev.readthedocs.io/en/stable/users/quickstart/#magento).

## Setup Procedure

To get started, clone this repository and run `ddev start`.
The setup command will guide you through the process, but feel free to press <kbd>Enter</kbd> at each step.
If you need to run the installation again, use `ddev install-magento`.

## System Components

- [DDEV](https://ddev.com/) >= 1.22.4
- Magento 2 from [Magento](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/composer.html) or [Mage-OS](https://devdocs.mage-os.org/) repository.
- Configurable Magento 2 version (default: latest stable), compatible with:
- [Elasticsearch](https://github.com/ddev/ddev-elasticsearch) 7
- [Redis 7](https://github.com/ddev/ddev-redis-7)
- [MariaDB](https://ddev.readthedocs.io/en/latest/users/extend/database-types/) 10.6
- [PHP](https://ddev.readthedocs.io/en/latest/users/configuration/config/#php_version) 8.2

The default dependencies align with the [system requirements](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/system-requirements.html) for the latest stable version.

### Noteworthy Features

- [xdebug](https://ddev.readthedocs.io/en/latest/users/debugging-profiling/step-debugging/) 3
- [Email Capture and Review](https://ddev.readthedocs.io/en/latest/users/usage/developer-tools/#email-capture-and-review-mailpit) ([Mailpit](https://github.com/axllent/mailpit))
- [Node.js](https://ddev.readthedocs.io/en/latest/users/extend/customization-extendibility/#using-nodejs-with-ddev) 20
- [gum](https://github.com/Morgy93/ddev-gum)
- [composer](https://ddev.readthedocs.io/en/latest/users/usage/developer-tools/#ddev-and-composer) 2
- [nginx](https://ddev.readthedocs.io/en/latest/users/configuration/config/#webserver_type) 1.24

For [additional services and add-ons](https://ddev.readthedocs.io/en/latest/users/extend/additional-services/), run `ddev get --list --all`.
