# IRC

School 42 project: (group)

Server : ```./ircser <port 6665-6669> <keyword>```
Client : cd Client/ ```./sic -h <localhost> -p <port> [-n <nickname>] [-k <keyword>]```

Recreate an IRC chat [Internet Relay Chat: TCP/IP protocol to communicate by message on the internet] with the following basic commands:

**ALL USERS**
- PASS		password
- NICK		nickname
- USER		username
- JOIN		#channel *key*
- TOPIC		#channel *:topic*
- PRIVMSG	receiver :text_to_be_sent
- PART		#channel *:reason*
- LIST		*channel*
- QUIT		*:message*

**OPERATORS'S CHANNEL**
- KICK		#channel nickname *:comment*
- INVITE	nickname #channel
- TOPIC		#channel *:topic*
- MODE		#channel +|- i|t|k|o|l *limit* *user*

>	_Various information_
- Operator's channel only :
	- INVITE : Send an invitation to someone to enter a specific channel
	- KICK : Kick someone from the channel and send a notification to all user's channel
	- MODE : Change the channel’s mode by an operator
		- i : Set/remove Invite-only channel
		- t : Set/remove the restrictions of the TOPIC command to channel operators
		- k : Set/remove the channel key (password)
		- o : Give/take channel operator privilege
		- l : Set/remove the user limit to channel

- All users :
	- PASS : Set the password for the connection with server
	- NICK : Set the Nickname
	- USER : Set the Username		
	- JOIN : Create or join a channel(s)
	- TOPIC : Display or set a specific channel topic
	- PART : To exit a a one or more channel(s)
	- LIST : List all the channels or the member's channel if the channel is specified
	- PRIVMSG : Send a message to a user(s) or a channel(s)  
	- QUIT : Quit the server with or without a reason

## IRC protocol
- The IRC protocol uses a system of servers and clients to allow users to connect to discussion channels in real time.
- IRC clients must connect to an IRC server using a nickname, username and password, then they can join public or private chat channels.
- IRC commands are used to perform actions, such as joining a channel, leaving a channel, sending a private message, etc.
- IRC channel operators are users who have special privileges on a channel, such as kicking other users or changing channel settings.
