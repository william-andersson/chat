# Simple terminal chat application
![Screenshot](https://github.com/william-andersson/chat/blob/main/Screenshot.png)

## Make it work

Set this up on a ssh server for users to chat with each other :smiley:<br>
Run **sudo toolbox-chat-setup --init** or **sudo ./setup.sh --init** to create the server.<br>
Default server location is /srv/toolbox-chat and the default chatroom is "default".<br>


> [!NOTE]
> :blue_square: Only private messages are sent to offline users.<br>
> :blue_square: Ability to change chatrooms (setup beforehand with **sudo toolbox-chat-setup --add**).<br>
> :blue_square: The WORDLIST file created can be populated with "forbidden" words separated with spaces.<br>

>[!TIP]
> :green_square: Ban user by changing owner of corresponding /srv/toolbox-chat/default/username file to root.<br>
> :green_square: Send message to everyone as admin via command line with **sudo toolbox-chat --admin \<ROOM\> \<"MESSAGE"\>**.<br>

## Usage
Run toolbox-chat and press the following keys to...

> * *w - start typing a message*
> * *u - list all users (online users show up in green)*
> * *l - list available chatrooms*
> * *c - change chatroom*
> * *r - resend message if wrong nickname was entered*
> * *h - for help*
> * *q - to quit*

All messages are sent to every user unless the message starts with @username<br>

## Limitations

- Only shorter messages work, return key = send
