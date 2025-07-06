# LocalChat: lightweight IRC-like chat application

LocalChat is a lightweight IRC-like chat application that allows local users
to communicate. It can be used as a replacement for
[`write`](https://linux.die.net/man/1/write), e.g., for collaborative remote
administration tasks.

Features:

- Multi user chatting.
- Multi channel support.
- Join and leave notifications.
- Own messages highlighting.
- History retention, visible when a user joins the conversation.
- Configurable nickname by setting the `${USER}` environment variable.


## Installation

Install dependencies and clone the source code:

    apt install splitvt
    git clone https://github.com/jfjlaros/localchat.git


## Usage

Start the application with the following commands:

    cd localchat
    ./localchat

Or, if you want to join an other channel, e.g., "mychannel":

    ./localchat mychannel

The interface contains two windows. In the top window, we see the
conversation, in the bottom window, we can write a message to add to the
conversation.

![screenshot](https://github.com/jfjlaros/localchat/blob/master/screenshot.png)

The application can be closed by pressing Ctrl+C.

A backup of a conversation can be made by copying its log file, e.g.:

    cp /tmp/.localchat/main ~/localchat.main.log
