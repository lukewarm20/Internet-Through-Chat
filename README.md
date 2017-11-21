# Internet-Through-Chat
Internet Through Chat allows clients to access the internet as well as terminals through anything, from IRC to signal to twitter. Anyway text can be placed, a bot can use it as input. 
This is software currently under development. It allows users to access different parts of the internet by things as basic as IRC or as advanced as high top tier chat systems. If a bot can access what you're saying, it can receive it as input.

If you would like to contribute, feel free. This is open source after all.


So how does it work. Well the way that an irc bot works is you tell it some basic intructions, in this case, listen to what the user says, if the user(s) says "!google_search why is the sky blue?" it will then do a google search to find the most appropriate answer.
Same method applies to things like the terminal, if you need to access a vps for example, or even a malicous site, you have a bot do all the work and get all the nasty gunk you would've had to deal with. This means that the vps, could be accessed by you through something like IRC or twitter even.

So how does this even work? VPS through a chatroom?
This sounds crazy but it really is possible, remember, the bot simply just does a task depending on what you say or any given variable. What says a robot can't type in "ls" into a terminal? That's the idea behind this, as well as the whole "going on the internet without going on the internet" idea.


Now keep in mind, this hasn't been built yet (at the time of writing this 11/15/17)
This is the setting, bot and you are in a chatroom, doesn't matter how you got there, point is, the bot and you don't really know each other. You type in some text, specifically, ls, the bot sees this, and types in "ls", just as you did. The whole (or part) terminal is copied (remember it's just text) then sent out to you. Congrats! You have now made contact with a terminal without even connecting to the bloody thing! There will be more to come (like actual code, derp) so stay tuned.


Another way of keeping things inside of communications private is using public and private key cryptography, this is most likely needed to ensure that all communications are secure while still being readable. The readable part of encryption is something you probably already know, if you don't know the to long didn't read version is it takes math, and makes your communication with something or someone private. The way you keep your private and public keys so no one else can see can be done using what will be called in this note "offline encryption/decryption" this is taking a small machine, let's take a rasperry pi zero in this case, to keep our keys, we'll keep the keys all in one (or more) document(s), where the rasperry pi will call to encrypt and decrypt text and files.

Lastly, a concept that would be awesome if its use can be implemented, is a two channel, input output systems. What this means is that you will send a message to a server, so that anyone else can interpret the message, if they have the credentials and keys to do so.


Putting the bot into action:

Let's say we have our three computers, one that will be able to send messages to our server, one to retrieve our messages from the server, and one offline computer to encrypt and decrypt the messages. On the other side, we have our bot, who will be trafficing the data out for our machines. The server will be running for a short time, meaning it will be only on the internet to bring up a tor hidden service. (note: the server may be able to be run on two machines as well? Also could our bot have comnnections to the internet by the two computers used for the input output seperatly?)

When you connect both machines on your end to the server, immediatly kill all other ports, connections, and most importantly, closing off the output on the input machine, and vise versa for the other, and make sure we accept the connection that has been established (router and hidden service), then, we make our message to be delivered to the server, to then be read, and delivered out to the internet.
