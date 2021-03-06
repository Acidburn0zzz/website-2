.. _daycamp_03:

Documentation, IRC, and Package Managers
========================================

More about Man Pages
--------------------

* the manual (rtfm)::

    $ man <program>
    $ man man

* use ``/phrase`` to search for ``phrase`` in the document; ``n`` for next match
  and ``N`` for previous match
* else::

    $ <program> --help

Documentation
-------------

Man pages, blogs you find by Googling, StackOverflow

.. figure:: /static/google.gif
    :align: center
    :scale: 50%

*  Contribute to community
    * Correct it if it's wrong
    * Remind them what newbies don't know
    * Write your own
* For your future self as well
* Start now

IRC
---

.. figure:: /static/multiple_networks.gif
    :scale: 40%
    :align: center

* Internet Relay Chat
* Very old (RFC 1459 May 1993)
* Works on everything (no GUI needed)
* The people you want to listen to are there
* Oregon State ran one of the first servers ever!

A Client
--------

.. note:: Switch to a terminal and show example

Use irssi or weechat in screen

.. code-block:: bash

    # This step is optional, but persistent IRC is cool
    $ ssh <username>@<preferred shell host>

    # start screen with the name 'irc'
    $ screen -S irc

    # start your client in the 0th window of the screen session
    $ irssi
    # or
    $ weechat-curses

    # exit irc screen with CTRL+a, CTRL+d
    # exit ssh session with CTRL+d or 'exit'
    # to get back to irc:
    $ ssh <username>@<preferred shell host>
    $ screen -dr IRC

Networks
--------

.. figure:: /static/multiple_networks.gif
    :scale: 30%
    :align: center

::

    /connect irc.freenode.net

    /nick <myawesomenickname>
    /msg nickserv register <password> <email>

    /nick <myawesomenickname>
    /msg nickserv identify <password>

Channels
--------

::

    /join #osu-lug
    /join #devopsbootcamp

:``/list``:
  - tells all channels on network
  - Don't do this on Freenode!
:``/topic``: tells you the current channel's topic
:``/names``: tells you who's here

Commands
--------

* take action with ``/me does thing```
* everything else starting with / is a command

::

    /say $thing
    /join, /part, /whois <nick>, /msg, /help <command>

Note that nothing shows up in the channel when you run a ``/whois`` command; it
shows up either in your status buffer or your conversation with the person.

.. rst-class:: codeblock-sm

::

    12:04 -!- _test_ [~test@c-50-137-46-63.hsd1.or.comcast.net]
    12:04 -!-  ircname  : Example User
    12:04 -!-  channels : #ExampleChannel
    12:04 -!-  server   : moorcock.freenode.net [TX, USA]
    12:04 -!-  hostname : c-50-137-46-63.hsd1.or.comcast.net 50.137.46.63
    12:04 -!-  idle     : 0 days 0 hours 2 mins 38 secs [signon: Wed Nov  6
    12:00:30
                          2013]
    12:04 -!- End of WHOIS

Useful tricks
-------------

* Tab-complete works on nicknames. use it.
* Highlight when people say your name
* Symbols are *not* part of names; they mark status in channel (such as @)
* Logging (expect it); \`/set autolog on\`
* chanserv and nickserv are good bots to know
    * hamper is also a bot

Screen & Irssi Hints
--------------------

* Paste with ctrl+shift+v
    * PuTTY defaults to right-click to paste
* To get back ``screen -dr IRC``
* Can you use ``man screen`` to find out what the d and r flags mean?

::

 SCREEN(1)                                                               SCREEN(1)

 NAME
        screen - screen manager with VT100/ANSI terminal emulation

 SYNOPSIS
        screen [ -options ] [ cmd [ args ] ]
        screen -r [[pid.]tty[.host]]
        screen -r sessionowner/[[pid.]tty[.host]]
 Manual page screen(1) line 1 (press h for help or q to quit)

Etiquette
---------

* Don't ask to ask
    * Ask detailed and specific questions about your problem
* Show that you're worth helping
* Read the topic
    * ``/topic``
    * Output only shows up in your channel, not to everyone else
* Pastebin code
* Choose your nick carefully

Terminology
-----------

* ping/pong

.. figure:: /static/jargon.jpg
    :align: right
    :scale: 50%

* tail
* hat
* nick
* netsplit
* kick/ban/k-line
* common emotes
    * ``o/`` AND  ``\o`` high fives
    * ``/me &`` means afk

Asking for help
---------------

It's okay to ask.

#. What should be happening?
#. What's actually happening?
#. Google it
#. Skim the manuals of each component
#. Identify a friend, mentor, or IRC channel who could help
#. When they're not busy, give them a quick synopsis of points 1 and 2,
   mentioning what possibilities you've ruled out by searching.

**Contributions = expertise + time**

Review
------

* How do you start an irc client?
    * How often should you need to start your IRC client?
* How do you reconnect to a screen session?
* Give an example of something which you should not do in IRC
