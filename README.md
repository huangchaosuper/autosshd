autosshd
========

Manage all autossh sessions

Installing
====

  sudo make install

Configure & Usage
====
  
  $ cat /etc/autosshd.conf
  autossh -L *:8888:localhost:8888 ipaddr
  autossh -R *:230:192.168.1.66:22 ipaddr
  
  # After modify configure and reload all authssh sessions
  $ autosshd-reload

  # stop all authssh sessions
  $ autosshd-kill


