# Introduction
This Document will serve as a playbook of sorts. a quick reference to situational and useful commands. The Goal of this is to be a Living document. A place to store all the commands I've used along with a brief description of their purpose. that way I can easily re-use them in the future.

# Best Practices
The commands in this document will be edited in such a way that they are easily copy and pasted. doing so required the use of environment variables. 

For example:
`nmap 127.0.0.1` can't be copy and pasted easily whereas `nmap $TARGET_IP` can.

For this reason, to start off any shell session we will want to set these environment variables using a command similar to the following:
`export TARGET_IP=127.0.0.1`

All the commands in this playbook will assume these variables are set.

**Note:** *Every new shell session you will need to re-set these variables as they do not persist to other sessions.*
