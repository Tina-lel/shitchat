# shitchat
a shitty, non encrypted, unsecure, plain text chat, via ftp

Warning:
-
This is not secure at all, and you should NOT use this at all lol. use this at your own risk

dependencies:
-
curlftpfs

ussage:
-
uncomment the line "user_allow_other" in /etc/fuse.conf (requieres root access), in oder to mount the FTP share.

git clone https://github.com/Tina-lel/shitchat

open up the "chat" file with a text editor of your choice and scroll down until you find the #FTP CONIFG part, add your FTP login data (ftp address, user, password, and a user writeable remote directory on the server (wich must contain a file called "main.txt") ), then save the file.

run the chat script (./chat), and wait until you are connected.

to chat press ctrl+c wich will open the "newmsg" box, press ctrl+c again, to exit

after you exited, run ./umount, to unmount the ftp share
