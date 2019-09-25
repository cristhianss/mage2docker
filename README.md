# Mage2Docker

> Get rid of your "it works on my machine" arguments.

This project intends to create a performant, replicable, and production-like Magento 2 local development environment that leverages Docker.

<div align="center">
    <a href="https://github.com/magento/magento2" target="_blank">
    <img src="https://img.shields.io/badge/magento-2.X-brightgreen.svg?logo=magento&amp;longCache=true" 
    alt="Supported Magento Versions">
    </a>
    <a href="https://hub.docker.com/r/graycore/magento-php" target="_blank">
    <img src="https://img.shields.io/docker/pulls/graycore/magento-php.svg?label=magento-php%20docker%20pulls" 
    alt="Docker Hub Pulls - Magento php">
    </a>
    <a href="https://hub.docker.com/r/graycore/magento-nginx/" target="_blank">
    <img src="https://img.shields.io/docker/pulls/graycore/magento-nginx.svg?label=nginx%20docker%20pulls" 
    alt="Docker Hub Pulls - Nginx">
    </a>
    <a href="https://github.com/graycoreop/mage2docker/graphs/commit-activity" target="_blank"><img src="https://img.shields.io/badge/maintained%3F-yes-brightgreen.svg" alt="Maintained - Yes" /></a>
    <a href="https://github.com/graycore/mage2docker/blob/master/LICENSE.md" target="_blank"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License MIT"/></a>
  <a href="https://gitter.im/graycoreio/mage2docker" target="_blank"><img src="https://img.shields.io/badge/chat-%23mage2docker%20on%20Gitter-brightgreen.svg" alt="chat #mutagen-sync in Slack"/></a>

</div>

## Prerequisites

- Hardware

  - 16GB RAM
  - 4 Cores

- Docker

  - [MacOS](https://docs.docker.com/docker-for-mac/install)
  - [Windows](https://docs.docker.com/docker-for-windows/install/)

    - This does NOT support docker toolbox. All docker toolbox issues will be immediately closed.

  - [Ubuntu](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

- PHP w/ Composer

  - Windows

    - [WSL (Windows Subsystem for Linux)](./docs/stories/composer/on-windows.md)

  - [MacOS](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-macos)

## Features

- :clock1: **5 Minute** Setup
- :fire: Fast (~250ms Out-of-the-box)
- :tada: Blackfire Performance Profiling
- :evergreen_tree: Alpine Linux

## Use Cases (User Stories)

We intend to support the following common use cases:

- [Working with an existing Magento 2 Project](./docs/stories/existing-project.md)
- [Starting a new Magento 2 Project](./docs/stories/new-project.md)
- [Building Extensions for Magento as composer packages](./docs/stories/extensions.md)
- [Running Unit and Integration Tests](./docs/stories/testing.md)
- [Complete Teardown and Reinstall](./docs/stories/reinstalling.md)
- [Using Blackfire Profiler to run performance tests](./docs/stories/blackfire.md)
- [Autocomplete Support during Local Development](./docs/stories/autocomplete.md)

## Frequently Asked Questions

To avoid unnecessary Issues, there is documentation on commonly asked questions:

- [What commands do I need to know and where are they run?]()
- [Why are there two places to run composer?]()
- [Glossary of Terms]()
