# shitchat
a shitty, unsecure, plain text chat, via sftp (slapped together in 20 minutes because i was bored lol)

Warning:
-
This is not secure at all, and you should NOT use this at all lol. use this at your own risk

Dependencies:
-
sshfs

Ussage:
-

git clone https://github.com/Tina-lel/shitchat && cd shitchat

run chmod +x chat

open up the "chat" file with a text editor of your choice and scroll down to the "SFTP CONFIG START" part. (you need to enter an sftp address, a user, a password, and a user writeable remote directory on a SFTP server (wich must contain a file called "main.txt") ), then save the file.

run ./chat mount, and enter the password, for your sshd server

then run ./chat chat, and enter a name

to chat press ctrl+c wich will open the "newmsg" box, enter "!exit", to exit

if you did not exit via !exit in the message box, run ./chat umount, to unmount the sftp share

Installation (dont):
-

first, follow the instructions above, and make sure its working. then run "sudo cp chat /usr/local/bin/" and enter your password.

Note: if you need to edit the SFTP server details, open the file /usr/local/bin/chat with a text editor, and edit the details, as explained above.

Commands:
-

chat: the main chat

mount: mounts the SFTP share

umount: unmounts the SFTP share

help: displays the help message

readme: displays this file

Msgbox commands:
-

!exit: exits the chat, and unmounts the SFTP share
