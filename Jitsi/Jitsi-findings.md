Currently the two files in this folder provide the setup for the server and client for traffic shaping

The current setup is a central jitsi server on an intel nuc. The fireqos-server is placed on it to restrict traffic to the needed speed. Then fireqos.conf is placed on both clients which connect to the given link

TODO: Add pictures here


Next steps:

Setup a server that can simulate multiple jitsi clients outlined here:
https://community.jitsi.org/t/tutorial-loadtesting-jitsi-with-malleusjitsificus-on-a-selenium-grid/33302
