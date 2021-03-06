![GlassChat 3](http://assets.gingergaming.com/img/glasschat/logo.png)
![Developed with <3 by Tiger and Alex](http://assets.gingergaming.com/img/glasschat/authors.png)
![Notice: Current build is not ready for use yet.](http://assets.gingergaming.com/img/glasschat/build-notready.png)

Did you ever want to chat with other players in [Minecraft](http://minecraft.net), but without using the main chat? No? Well, now you do, because we present to you: GlassChat3.
In GlassChat 3, you can send messages directly, without the server knowing, to other players. No plugins or extra mods required!

![](http://assets.gingergaming.com/img/glasschat/title-features.png)
- Fast and secure chatting (no public rednet)
- No plugins required.
- Multi-dimensional: works everywhere, thanks to Terminal Glasses!
- Positioned in the top-left corner of your screen, so you'll be able to follow two chats at the same time.
- 100% free and open source.
- Nicknames
- Colored chat
- Easily add custom commands
- Basic IRC commands
- And way more!



![Downloads](http://assets.gingergaming.com/img/glasschat/title-downloads.png)
- Pastebin installer for **server**: `Y5R5R9Cv`.
- Pastebin installer for **client**: `zfmzr5vH`.

![Getting Started](http://assets.gingergaming.com/img/glasschat/title-gettingstarted.png)
GlassChat 3 requires [ComputerCraft](http://computercraft.info) and [OpenPeripheral Addons](http://openmods.info/). 
The FTB Direwolf 1.6.4 modpack has all these mods already installed. This version of GlassChat was developed on a live server with FTB Direwolf20 1.6.4 v1.0.18. GlassChat also needs the HTTP API to be enabled in your CCcraft.conf  server file.

**Building your Cluster**

Firstly, you'll need to build a GlassChat Cluster. A cluster exists out of a server and clients. 
All computers used need to be [Advanced Computers](http://ftbwiki.org/Advanced_Computer). 
Clients need to have a [Terminal Glasses Bridge](http://wiki.technicpack.net/Terminal_Glasses_Bridge). 

Both the server and it's clients need to be connected with eachother using a ComputerCraft modem and network cables. You could swap the modem and cables with wireless modems, but rednet can't handle too many wireless requests per second. 

For small setups it's okay to use wireless modems (*Heads-up: You will need to change `rednet.broadcast()` to `rednet.send()` at the server files, collect all the connected client ID's, put those in a foreach loop and add some form of security*), but for large clusters, we recommend using network cables and a normal modem.

Below you can see an example setup of a GlassChat Cluster using a modem and network cables. This cluster has two clients and one server. Theoretically, you can add as much clients to a cluster as you want. Per cluster, there can only be one server.

![An example of a GlassChat Cluster](http://assets.gingergaming.com/img/glasschat/setup.png)

Now that you've set up your GlassChat Cluster, you'll need to make 1 [Terminal Glasses](http://wiki.technicpack.net/Terminal_Glasses) for every client you have. You now need to link each Terminal Glasses with a Client. Do this by right-clicking the Terminal Glasses Bridge connected to the client. Your glasses are now linked to your client.

**Installing the Software**

Okay, so now that we've got all the hardware set up, let's start installing the software!

- **Installing the Server's software** 
Go to your server and enter `pastebin get Y5R5R9Cv update`. You can view the pastebin code [here](http://pastebin.com/Y5R5R9Cv) if you don't trust us ;)
Once the download is ready, run `update`. The computer will now download the server startup.lua from GitHub and put it in the `startup` file. When that's finished, the computer will reboot. That's it for the server part!

- **Installing the Client's software** 
Go to your client and enter `pastebin get zfmzr5vH update`. You can view the pastebin code [here](http://pastebin.com/zfmzr5vH) if you don't trust us ;)
Once the download is ready, run `update`. The computer will now download the client startup.lua from GitHub and put it in the `startup` file. The installer will now prompt you for a username. Enter the name you want to be known as in the chat (No worries, you can always change your nickname later). 
Now the installer will prompt you for the Server's Cluster ID. Go back to your server and look for the `ID: xxx` at the top of the screen. That's the Server's Cluster ID. Enter that ID at your client. The installer will now finish the setup and reboot your client.

![How it works](http://assets.gingergaming.com/img/glasschat/title-how.png)
![GlassChat communication explained.](http://assets.gingergaming.com/img/glasschat/glasschat-map.png)

*Heads-up: If you want your cluster to work when not being there, eg. in another world or far away, you'll have to chunkload the whole cluster with a Chunkloader of some sorts.*

![Using GlassChat](http://assets.gingergaming.com/img/glasschat/title-usingglasschat.png)
To be able to chat, you need to wear [your Terminal Glasses linked to your Client](https://github.com/lesander/GlassChat3#how-to-get-started).

**Sending Messages**

To send a message, type `$$` in the chat bar, followed by your message. For example: `$$Hello world!` or `$$ Hello world!`.

**Client Commands**

The GlassChat Client has several commands available. All commands start with `$$gc`, followed by the actual command. Here's a list of all the commands:
- `$$gc help` list all commands.
- `$$gc info` list all connected clients, their nicknames and the Server Cluster ID.
- `$$gc users` list all connected clients and their nicknames.
- `$$gc version` output the version of your GlassChat client.
- `$$gc update` update your GlassChat client.
- `$$gc reboot` reboot your GlassChat client.
- `$$gc nick {input}` set a new nickname, where `{input}` is your new nickname.

**Server Commands**

The GlassChat Server also has some commands available to make life easier. Commands can be submitted by pressing the key of the command inside the Server's terminal.
- Press `U` to **Update** all connected clients.
- Press `R` to **Reboot** all connected clients.
- Press `S` to **update and restart** the server.
- Press `K` to **kill/stop** the server.

![FAQ](http://assets.gingergaming.com/img/glasschat/title-faq.png)
Content soon to come...

![All errors explained](http://assets.gingergaming.com/img/glasschat/title-errors.png)
Content soon to come...



----------
**This documentation is under construction, and so is GlassChat 3!**

GlassChat, developed by [Toomas Tamm](http://github.com/tiiger87) and [Sander Laarhoven](http://github.com/lesander).

*GlassChat3 is licensed under the terms of the GNU GENERAL PUBLIC LICENSE Version 2, wich can be found under the name `LICENSE` in your distribution.*
