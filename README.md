# colour_chat
A minetest CSM mod for changing the colour of text sent to the server.
[First version](https://github.com/red-001/colour_chat) was made by red-001, more features were added by me. Pastel added by dhausmig.

## chat commands:  
(note: all colours must be a 6 letter hex code with a "#" - eg: "#ffffff")

    .get_colour <name>                         -  get the hex value from a colour name
    .get_color <name>                          -  same as get_colour, but with different spelling
    .set_colour [<col1> [<col2> [<times>]]]    -  Set the default chat colour to either one solid colour, or a fade between two colours. 'times' is how many times to fade between them. Leave blank to reset to white.
    .set_color [<col1> [<col2> [<times>]]]     -  same as .set_colour, but with american spelling.
	.set_max [<max>]                           -  set the maximum character limit. for servers that dont use the default. Leave blank to reset to 500
    .rainbow <message>                         -  send a message with rainbow colours.
    .pastel <message>                          -  similar to rainbow, but easier to read.
    .alternate [<col1> <col2>] <message>       -  alternate between two colours.
    .fade <col1> <col2> [<times>] <message>    -  fade message between two colours, fade multiple times  -  works with long messages!!
    .custom <message with colours>             -  send a message with custom colour changes. Use "#------" anywhere in the text to change colours.
    .msg <playername> <message>                -  send a private message, the same as "/msg", but with your colours applied to it
    .mw <message>                              -  send a message with a red "MODERATOR WARNING:  ".
    .say <message>                             -  send a plain, white message.


- [Forum Topic](https://forum.minetest.net/viewtopic.php?f=53&t=20152)

changes:
    
- messages can fade through colours multiple times
- short messages don't fade
- .alternate uses users colours instead of red and green if no parameters are given
- moderator warning now gives a warning before sending the message
- comments and code cleaned up a little
- the maximum message length can be changed with a command for servers that don't use the default.
