Commands
=========

.. note::
    <args> - required argument
    [args] - optional argument



Administration commands
-----------------------

Prefix
~~~~~~~~~~~~~~~~~~~~~~~

Description: Set custom prefix for bot (prefix is only used to help command) if prefix not given will be set to default

Required Permission: ADMINISTRATOR

.. code-block:: console

    usage: /prefix [prefix]


Clear
~~~~~~~~~~~~~~~~~~~~~~~

Description: Clear chat by given amount or message author

Required Permission: ADMINISTRATOR or MANAGE_MESSAGES

Args:

* Amount: number of message to delete
* User: Author of message to delete

.. code-block:: console

    Usage: /clear [amount] [user]


Logs
~~~~

Required Permission: ADMINISTRATOR

Set
"""
Description: Set a log channel for selected event if channel not given logs will be unset

Args: 

* Events:

    - Message - message edite, delate, ...
    - Voice - user join, leave from voice channel
    - User - user change profile, name, ...
    - Server - server name change, image, ...

* channel: Channel where logs will be send


.. code-block:: console

    Usage: /logs set <event> [channel]

Show
""""
Description: Show current logs channels

.. code-block:: console

    Usage: /logs show



Automessage
~~~~~~~~~~~~~~~~~~~~~~~

Required Permission: ADMINISTRATOR
Automessage limit: 2

Add
""""

Description: Add auto message to your server

Args:
            * country-code: 2-digit code of country to get time zone, `Country Codes <https://www.iban.com/country-codes>`_
            * job-name: Name under will be show auto message
            * channel: Channel where auto message will be send
            * hour: Hour when auto message will be send between 0 and 23
            * minutes: Minutes when auto message will be send between 0 and 59
            * day-month: Day of month when auto message will be send between 1 and 31
            * month: Number of month when auto message will be send between 1 and 12
            * day-week: One day of week SUN - SAT 

.. code-block:: console

    Usage: /automessage add <country-code> <job-name> <channel> <hour> <minutes> [day-month] [month] [day-week]

Delete
""""""

Description: Deleting auto message by name

Args: 
    * Name:  Name of auto message you want to delete

.. code-block:: console

    Usage: /automessage delete <name>

Show
""""
Description: Show list of server auto messages

.. code-block:: console

    Usage: /automessage show

Change status
""""""""""""""
Description: Change status of auto message from running to idle and vice versa 

Args: 
    * Name of auto message you want to change status

.. code-block:: console

    Usage: /automessage change-status <name>

Other
-----------------------

Ping
~~~~~~~~~~~~~~~~~~~~~~~

Description: Show bot response time in ms

.. code-block:: console

    Usage: /ping

Help
~~~~~~~~~~~~~~~~~~~~~~~

Its Help 


Stats
~~~~~~~~~~~~~~~~~~~~~~~

Description: Show bot statistic

.. code-block:: console

    Usage: /stats


Contact
~~~~~~~~~~~~~~~~~~~~~~~

Description: Contact to bot owner to reporte bugs or send a feature proposition

Args:

* Title: title of the message
* Content: content of the message

.. code-block:: console

    Usage: /contact <title> <content>

Radio
~~~~~~

Play
""""

Description: Search for radio and sellect to play

Args:
            * name: name of the radio station
            * tag: tag like pop, most clicked
            * country-code: 2-digit code of country you want search radio
            * order-by: order radio station by name, language, clicktrend, votes

.. code-block:: console

    Usage: /radio play [tag] [name] [country-code] [order-by]

Leave
""""""

Description: Stop playing and leave bot from channel

.. code-block:: console

    Usage: /radio leave 

Now-playing
""""""""""""

Description: Show now playing radio station

.. code-block:: console

    Usage: /radio now-playing 

Random
""""""
Description: Play random radio station

.. code-block:: console

    Usage: /radio random

Follow
~~~~~~~


Create
""""

Description: Create profile to follow other users. 

.. warning::

    You can delete your profile after 30 days

Args:
            * Privacy-options: Public - Everyone see your profile and can follow Unpublic - Everyone can follow you but your profile is hide Private - You need to accept all following requests and your profile is hide 
            * Notification: All - all notification Only following join - only join to channel notification Olny system notification - notification from bot like follow request Disable - Disable all notification 
            * Color: Color to set on your profile need hex like `#f1c40f <https://www.color-hex.com/color/f1c40f>`_

.. code-block:: console

    Usage: /profile create <privacy-options> <notification> [color]

Delete
""""""

Description: Delete your profile with following and followers. 

.. warning::

    We can't be able to restore you profile after deleting

.. code-block:: console

    Usage: /profile delete

Display
""""""""""""

Description: Display your or given user profile if public

Args:
            * User: User to see thier profile

.. code-block:: console

    Usage: /profile display [user]

Follow
""""""
Description: Follow a user or send request if profile is private

Args: 
            * User: User to follow

.. code-block:: console

    Usage: /profile follow <user>

Unfollow
""""""""
Description: Unfollow a user

Args: 
            * User to unfollow

.. code-block:: console

    Usage: /profile unfollow <user>

Show followers
""""""""""""""
Description: Showing yours or user followers list if profile is public

Args: 
            * User: User to see thier followers

.. code-block:: console

    Usage: /profile show followers [user]

Show following
""""""""""""""

Description: Showing your or user following list if profile is public. You can also unfollow user from list

Args: 
            * User: User to see thier following

.. code-block:: console

    Usage: /profile show following [user]

Show follow-request
"""""""""""""""""""

Description: Showing your follow request list if profile is private

.. code-block:: console

    Usage: /profile show follow-request

Settings color
""""""""""""""

Description: Set new color of your profile

Args: 
            * color: new color given in hex like `#f1c40f <https://www.color-hex.com/color/f1c40f>`_

.. code-block:: console

    Usage: /profile settings color <color>

Settings privacy
""""""""""""""""

Description: Set privacy of your profile

Args: 
            * Privacy-options: Public - Everyone see your profile and can follow Unpublic - Everyone can follow you but your profile is hide Private - You need to accept all following requests and your profile is hide

.. code-block:: console

    Usage: /profile settings privacy <privacy-options>

Settings notification
"""""""""""""""""""""

Description: Set notification for your profile

Args: 
            * Notification: 
                - All - all notification 
                - Only following join - only join to channel notification 
                - Olny system notification - notification from bot like follow request 
                - Disable - Disable all notification

.. code-block:: console

    Usage: /profile settings notification <notification>


Documentation created by:

  * `Sadowski Krystian <https://github.com/Sadowski-Krystian>`_
  * Gummun