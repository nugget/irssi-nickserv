## IRSSI NickServ ##

This is an IRSII script which will automate your interactions with the NickServ
ircservices on all your various IRC networks.

It's nice because it is set up to autorespond to NickServ challenges, so even
in the event of a netsplit or services restart your client will happily
re-identify whenever requested.  This is an improvement over just setting your
NickServ password as the connection password, which gets you in the door but
won't retain your nick when things are unstable.

Additionally, you can define a list of channels which your client will join
only after it has successfully identified with NickServ.  Autojoins can often
fail if a channel is set as protected or set to block unregistered users from
joining.  By deferring the join until post-NickServ we handily sidestep this.

## Installation ##

1. Place `nickserv.pl` in `~/.irssi/scripts`
2. Place `nickserv.channels` and `nickserv.users` in `~/.irssi/`
3. Edit the channels and users files to taste (add your nick and passwords and
   channels)
4. If you require a script be run when Irssi starts, you can place the file (or
   better, create a symlink to it) into `~/.irssi/scripts/autorun/`
   Alternatively, if you want more control over the order in which scripts are
   autoloaded, you can place:
   `/SCRIPT LOAD nickserv.pl` in your `~/.irssi/startup` file.

## Credits ##

The original code was writen by Sami Haahtinen / ZaNaGa
The protected channel support was added by David McNett / Nugget
