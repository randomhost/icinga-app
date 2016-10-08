randomhost/icinga-app
=====================

This is a meta package for installing check and notification commands provided
by the various `randomhost/icinga-*` packages.

Available check and notification scripts will be installed to `vendor/bin/`.

Check commands
--------------

The following check commands are available:

* `icinga-check-minecraft-playercount`
    
    Checks the amount of players on the server.
    
    **Command line parameters**
    
    | Parameter           | Description                             |
    | ------------------- | --------------------------------------- |
    | --host              | Minecraft server IP address or hostname |
    | --port              | Query port                              |
    | --thresholdWarning  | Threshold to trigger the WARNING state  |
    | --thresholdCritical | Threshold to trigger the CRITICAL state |

Notification commands
---------------------

The following notification commands are available:

* `icinga-notify-nma-push`

    Sends notifications using [NotifyMyAndroid][0].
    
    **Command line parameters**
    
    | Parameter           | Description             |
    | ------------------- | ----------------------- |
    | --type              | Notification type       |
    | --service           | Service name            |
    | --host              | Host name               |
    | --address           | Host address            |
    | --state             | Service state           |
    | --time              | Notification time       |
    | --output            | Check plugin output     |
    | --apikey            | NotifyMyAndroid API key |

License
-------

See LICENSE.txt for full license details.


[0]: http://notifymyandroid.com
