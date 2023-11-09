This is a readme just for the nukefire module of tintin-helper.

First, read the tintin-helper readme as it explains the basic concepts
and setup. Then come back and read this one.

Player files:
You do not need an account file for nukefire. Just a player file.
Your player file should look something like this:
```
#nop Sample player file

#list modules_on_connect create layout nukefire nukefire/regen nukefire/class/cyborg;

#var char_name {<name>}
#var char_password {<password>}
#var layout_preference {full}
#var comms-session {com}
#var cont_key <keyword for a container>

log on
#config log plain
#tick {idle} {#cr} {135}
```
Name should be all lower case. Player file should be saved as:

`name_nukefire.player`

in your players folder.

To connect multiple sessions:
Connect your first session as normal, such as:

>connect goliath

Once your first session is connected, return to the default session in
tintin by using #gts.
Then connect to your next char:

>connect img

Sessions will be named: nukefire:<name of char>. You can switch between
them like #nukefire:goliath, or alias something shorter.

There are various issues with this package as is. As the dev team
at nukefire works on mud side things, some of them will be resolved.
Others will not. This is still a work in progress. Feel free to message
me on discord/slack or raise issues on github.