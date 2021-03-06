# Getting Started with a new Magento Application
There are a steps involved in preparing your local development environment for Magento 2 development.

1. [Setting up composer](#setting-up-composer)
2. [Setting up your Magento Account](#setting-up-your-magento-account)
3. [Configuring Composer](#configuring-composer)
4. [Creating your Magento 2 Project](#creating-your-magento-2-project)
4. [Setting up Mage2Docker](#setting-up-mage2docker)

## Setting up composer
Magento 2 utilizes composer to manage its dependencies, including itself. To realistically work with Magento, you will need composer. How you install composer is up to you, but we've provided some basic documentation on how to do this on "cleanly" on a few platforms.

> If you already have composer installed, you can skip to [Setting up your Magento account](#setting-up-your-magento-account).

1. Windows
    * [Installing PHP & Composer through WSL (Preferred)](./composer/on-windows.md)
    * [Installing Composer Natively](https://getcomposer.org/doc/00-intro.md#installation-windows)
2. [MacOS]
    * [Installing PHP and Composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-macos)

## Setting up your Magento Account
[The process of creating a Magento account is fully documented by Magento and you should follow their process](https://docs.magento.com/m2/ce/user_guide/magento/magento-account-create.html). 

## Configuring Composer

In case you have not done so, we will add your Magento composer authentication credentials to your local `auth.json`.

First check to see if you have a credentials file under `~/.composer/auth.json`.

```bash
cat ~/.composer/auth.json
```

If you have a `auth.json` file here, you have most likely already configured your credentials and can skip to the next step.

If you don't see your credentials there, [you can follow the Magento 2 guide to find your credentials](https://devdocs.magento.com/guides/v2.3/install-gde/prereq/connect-auth.html) and copy the `auth.json.sample` [found in the Magento 2 repo](https://github.com/magento/magento2) to your user's `auth.json` file: `~/.composer/auth.json` file and fill out the required credentials.

```bash
cp /path/to/magento/project/auth.json.sample ~/.composer/auth.json
``` 

## Creating your Magento 2 Project
[We recommend creating your Magento 2 project with composer.](https://devdocs.magento.com/guides/v2.3/install-gde/composer.html)

## Setting up Mage2Docker.
Now that you have a local Magento 2 project, you can follow along with the [existing project setup](./existing-project.md).