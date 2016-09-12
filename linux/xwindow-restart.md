# Problem Description

Shadow windows appearing on screen when moving any window (term/google chrome) around desktop.

# Platform
Ubuntu Xenial 16.04

# Reference

http://askubuntu.com/questions/1220/how-to-restart-x-window-server-from-command-line

# Workaround procedure

$ sudo systemctl restart lightdm.service
