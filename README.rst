========================
 Colloquy speech plugin
========================

-----------------------------------------------------
 A text-to-speech plugin for the Colloquy IRC client
-----------------------------------------------------

:author: James Tatum, <jtatum@gmail.com>

Forked Changes
==============
:author: James Shawn Carnley, <wrenchpilot@gmail.com>

Very simple filtering for Twitch live streaming based on hardcoded values. 
Currently filters out: 
* "nightbot"
* "moobot"
* "!songrequest"
* "!sq" - custom command for song requests by title

TODO:
* Make the filters configurable via the /speech command
* Store filters via ini file...

Installation
============
Drop speech.py into one of these locations::

  ~/Library/Application Support/Colloquy/PlugIns (current user)
  /Library/Application Support/Colloquy/PlugIns (all users)
  /Network/Library/Application Support/Colloquy/PlugIns (all users on the network)

If Colloquy is running, reload the plugin with /reload plugins

Usage
=====
/speech on
  Enable speech. That's pretty much all you have to do to use this plugin.
  The computer will begin speaking every line of text in channel.

/speech off
  Disable the plugin

/speech voices
  Display a list of available voices

/speech voice
  Select a speaking voice, for instance **/speech voice agnes**

/speech nick
  Use **/speech nick on** to enable speaking the nickname before each message.
  This can be disabled with **/speech nick off**

/speech help
  Produce a list of all commands available in the speech plugin.
