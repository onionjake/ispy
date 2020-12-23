ispy
====

ispy is a monitoring program, to monitor what is on the screens of linux
computers.


server
======

The server program is called "ispy".


client
======

The client program is called "my-little-eye".  To install with systemd,
do the following as root:

  git clone $source.git /usr/local/ispy
  ln -s /usr/local/ispy/my-little-eye.service /etc/systemd/user
  systemctl --global enable my-little-eye

The service will start on next login, or can be started with:

  systemctl --user start my-little-eye


