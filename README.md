# IRCRelay
IRCRelay reports game events from your server to an IRC channel and allows admins to control their servers or chat with users ingame from IRC. Written for SourceMod, and compiled in SourcePawn 1.10.0.

Administrate your server directly from IRC using commands like msg, kick, rcon, players, info, and more (command character customizable). 

## Why this branch?
IRCRelay is great, until you're trying to connect other relays *to* it. [BosaikNet](http://bosaik.net/)'s Team Fortress 2 server is connected to both IRC and Discord, via [Discord-IRC](https://github.com/reactiflux/discord-irc). While it is possible to use the command-sending feature within Discord-IRC to send messages to in-game users, it's a mess for IRC users (Discord-IRC sends a line before a command to indicate which Discord user sent that command) and it's much more work to talk into the TF2 server than out of it. The biggest change made in this branch is that **all** IRC messages in a channel are sent to the in-game chat. I've also moved the trigger indicator from the IRC bot's username over to its realname, which let me change the IRC bot's username to the same value as its nickname. I feel this makes more sense. 

In the future, I'll be making changes to the channel name parser to fix the case-sensitivity issue. I'll probably add some other stuff as well (announcing when players join/leave), but I need to actually learn SourceMod scripting to do that. 
