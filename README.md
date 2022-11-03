# shitchat
a shitty, unsecure, plain text chat, via sftp (slapped together in 20 minutes because i was bored lol)

Warning:
-
This is not secure at all, and you should NOT use this at all lol. use this at your own risk

dependencies:
-
sshfs

ussage:
-

git clone https://github.com/Tina-lel/shitchat

run ./perms once, to set the permissions for the scripts (or do it yourself)

open up the "mount" file with a text editor of your choice and edit the lines starting with "export". (sftp address, user, password, and a user writeable remote directory on the server (wich must contain a file called "main.txt") ), then save the file.

run the mount script (./mount), and enter the password, for your sshd server

run the chat script (./chat)

to chat press ctrl+c wich will open the "newmsg" box, press ctrl+c again, to exit

after you exited, run ./umount, to unmount the sftp share
