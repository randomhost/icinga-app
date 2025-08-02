# randomhost/icinga-app

<!-- TOC -->
* [1. Purpose](#1-purpose)
* [2. Check Commands](#2-check-commands)
* [3. Notification Commands](#3-notification-commands)
* [4. License](#4-license)
<!-- TOC -->

## 1. Purpose

This is a meta package for installing check and notification commands provided
by the various `randomhost/icinga-*` packages.

Available check and notification scripts will be installed to `vendor/bin/`.

## 2. Check Commands

The following check commands are available:

* `icinga-check-minecraft-playercount`

  Checks the amount of players on the server.

  **Command line parameters**

  | Parameter             | Description                             |
  |-----------------------|-----------------------------------------|
  | `--host`              | Minecraft server IP address or hostname |
  | `--port`              | Query port                              |
  | `--thresholdWarning`  | Threshold to trigger the WARNING state  |
  | `--thresholdCritical` | Threshold to trigger the CRITICAL state |

## 3. Notification Commands

The following notification commands are available:

* `icinga-notify-nma-push`

  Sends notifications using [CM.com][1].

  **Command line parameters**

  | Parameter   | Description                                              |
  |-------------|----------------------------------------------------------|
  | `--type`    | Notification type                                        |
  | `--service` | Service name                                             |
  | `--host`    | Host name                                                |
  | `--address` | Host address                                             |
  | `--state`   | Service state                                            |
  | `--time`    | Notification time                                        |
  | `--output`  | Check plugin output                                      |
  | `--phone`   | Phone number in international format (e.g. +12065550199) |
  | `--apikey`  | CM.com API key                                           |

## 4. License

See LICENSE.txt for full license details.


[1]: https://cm.com
