irssi
=====

XMPP
----

    /xmppconnect -host <hostname> <jid>

where `<jid>` is the username, complete with `@hostname.domainname` as
required.

Seeing who is online
--------------------

To do this one needs to check the "roster"

    /roster

Chat rooms
----------

Join a chat room on `jabber.ccc.de`

    /join <room_name>@conference.jabber.ccc.de

Accept connection request
-------------------------

Similarly to accepting an authorisation request in other chat clients, when
using the XMPP module for `irssi` and someone wishes to be a contact, then
you need to "accept them to your presence".  You will see a message like
this:

    <user>@jabber.ccc.de: wants to subscribe to your presence (accept or deny?)

To accept this request one uses the following command:

    /presence accept <user>@jabber.ccc.de

To add people to the roster, use this command:

    /presence subscribe <user>@jabber.ccc.de
