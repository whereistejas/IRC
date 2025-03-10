# How to do IRC the right way (Part 1)

IRC which stands for Internet Relay Chat is one of the oldest methods of chatting across the internet. This piece of technology is as old as the internet, itself. Like, all great things about the internet it started with a Swede writing a program.

## What is IRC and why should you bother with it?

IRC is a text-based communication protocol. In very simple terms, it allows users to create #channels (or as we call them, chat rooms) where a group of people can chat together. It also offers numerous features like file transfers and SSL encryption. 

IRC networks are a great learning place. Numerous FOSS projects have their own IRC channels, where newbie users can go for help. One such channel is `#irssi`. It is also a great place to meet new people, with tons of experience.

IRC is an old-school technology. It is dying. In it's hayday IRC was the next dominant form of communication over the internet after email. Thus, it can be said, that using IRC is a way of saving a cultural symbol, from turning to ruin.

IRC is free and open. Contrary to what many may have you believe, it has a very simplistic design. However, it is not new-user friendly. For all it's ease, it has a few major issues.

## How does IRC work?

Like any communication protocol, it involves a client and server. The server, an IRC server, may be public or private.

One IRC network will have numerous IRC servers under it's wings. To connect to the IRC, you need both the netowrk and server address.

There are numerous IRC clients just as we have numerous email clients. While, the choice of a client is very subjective, for the purpose of demonstration we will be using `irssi`. While, the choice of a client is very subjective, for the purpose of demonstration we will be using `irssi`. Every Linux distribution offers `irssi` as a binary in it's package repos. You can install it on Fedora like this: `sudo dnf install irssi -y`.

![](images/part1/irssi-ui.png)

## Let's get started.

1. Launch `irssi` in your terminal. You will be greeted by a weird-looking TUI. At the bottom, you will find a prompt. It will have the word `status` on it's left corner. This is like a window indicator. Currently you are in the `status` window which shows you all the information you are receiving from the network and server.

2. Type `/network` and press `<Enter>`. `irssi` will show you a list of networks that are stored in `irssi` by default. We wish to connect to the `Freenode` network.
![](images/part1/irssi-network-list.png)

3. Type `/connect Freenode` and press `<Enter>`. You will notice that you have connected to the `Freenode` network. Your `nick` is the name of the `$USER` you are logged in as. Your `nick` is like your User ID. Most people will reserve an unique `nick`, in order to prevent other people from impersonating them. `<Pg-Up>` and `<Pg-Down>` will help you scroll in the window. You will see a bunch of other stuff saying that you are not registered. For the purpose of this demonstration, you can safely ignore it.
![](images/part1/irssi-connect.png)

4. The next task is to join a channel. Type `/join #tejas` and press `<Enter>`. You will probably see a new window pop up and notice that the prompt title has changed from `status` to `#tejas`.
![](images/part1/irssi-join.png)

5. Say Hi!

6. Type `/msg whereistejas Hey! I made it here!` and press `<Enter>`. This will send a personal message to me. If, I'm online, we can have a nice chat. (P.S. I'm always online).

7. Let's try joining another channel called `#irssi`. To switch between different channels in `irssi` use `<Alt> + <No. Key>`. For example, `<Alt>+2` will take you back to the `#tejas` channel.

8. In case you need help, type `/help`.

9. Figure out how to quit on your own.

That wasn't difficult at all, was it?

## Conclusion

Now that you know how to connect to an IRC network and join a channel, you are ready to meet tons of new people. This is also the point, where we can start talking about the drawbacks of IRC:

1. There is no way to save or log messages that are sent to you when you are offline, i.e., not connected to an IRC network.

2. There is no way of recovering messages from a previous session in the current session, i.e., you lose everything once you `/quit`.

3. You can connect only one client to a network with one `nick`, i.e., you can only connect from one place at a time.

However, there are ways of overcoming the above mentioned issues, which will be part of the next article. We can see at once, how the above metioned issues are connected with one another.
