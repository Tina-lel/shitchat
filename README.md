# shitchat
a shitty, unsecure, plain text chat, with file sharing, multiple chat rooms and user lists, via sftp. written in bash lol (slapped together in 20 minutes because i was bored lol).

Warning:
-
This is not secure at all, and you should NOT use this at all lol. use this at your own risk.

Dependencies:
-
sshfs

rsync (optional for file uploading and downloading)

Ussage:
-

git clone https://github.com/Tina-lel/shitchat && cd shitchat

chmod +x chat && chmod +x config

open up the "config" file with a text editor of your choice and find the #GENERAL CONFIG START part, replace "MyName" with another name, "ReplaceMe" with a status (for example "Playing Minecraft" or something) and "/home/user/Downloads" with a dir where you want downloaded files to be safed to. next, scroll down to the "#SFTP CONFIG START" part. (you need to enter an sftp address, a user, a password, and a user writeable remote directory on the SFTP server (wich must contain a plain text file called "main") ), then save the file.

run ./chat mount, and enter the password, for your sshd server.

then run ./chat chat

and then select a chat room (you can create new ones by entering a name, wich is not already present.)

to chat press ctrl+c wich will open the "msgbox", for a list of commands type !help or read the bottom part of the readme.

if you did not exit via !exit in the message box, run ./chat umount, to unmount the sftp share.

Updating:
-

run ./chat sync, wich does everything for you

Commands:
-

chat: the main chat

mount: mounts the SFTP share

umount: unmounts the SFTP share

sync: sync's "chat" form github

help: displays the help message

help_msgbox: displays msgbox commands

readme: displays this file

Msgbox commands:
-

!exit: exits the chat, writes user file, and unmounts the SFTP share

!back: goes back to the chat selection screen

!users: list all users

!upload: uploads files to the SFTP share

!download: downloads files from the SFTP share

!help: displays a help message
