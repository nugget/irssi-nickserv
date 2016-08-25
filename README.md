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
