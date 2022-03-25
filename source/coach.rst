.. -*- coding: utf-8; -*-

=================================================
Online Coach
=================================================

-------------------------------------------------
Introduction
-------------------------------------------------

The online coach is a privileged client that can connect to the server in official games. It
has the capability of receiving global and noise-free information about the objects on the
field. In order to encourage research in this area there are special coach contests since
2001. This way, research groups that do not want to develop a team of player clients
can participate in the RoboCup challenge by focusing on the online coach. Additionally,
in order to make it possible to use a single coach with a variety of teams, a standard
coach language (CLang) has been developed that can be used to communicate with the
players.

See Section 7.4 and 7.5 for details about the commands that can be used by the online
coach and messages that will be sent by the server.

How to connect to an online coach 
By default, port 6002 is used Online_coach. You need to pay attention to the following points when connecting: 
1）There is no need to notify the server when it starts Online_coach is about to connect, the options -coach and -coach_w_referee are trainer-specific; 
2）The connection method is basically the same as that of the player, but the connection must be successful after at least one of the players of their own side is successful, and this order is related to whether the Online_coach is successful; 
3）Online_coach needs to send initialization information to the server, including its own team name, that is, to identify the server, otherwise the server will not be processed, and also specify the protocol version used.
