# Getting mods

> NOTE: you need BTD6 on steam obviously

**if you already have a mod move to the next section**

get them from one or more of the discord servers linked below. It is reccomended that you get familiar with installing and loading mods before you begin making them.
> **NOTE: There are no plans for Mac support. For Mac users, it is reccomended emulating Windows to play mods. ~~Like seriously if you are using a mac you should know that they are an ass to do hacky things with~~**

# Access the Mods folder
The BTD6 Steam folder can be found by right click BTD6 in your library, then go to Properties>Local Files>Browse Local Files.
By default, they can be found here

Windows: `Program Files (x86)\Steam\steamapps\common\BloonsTD6`

Linux: `~/.steam/steam/steamapps/common/BloonsTD6` 

This should bring you to the BTD6 directory.

# Downloads and Installation
> make sure antivirus is turned off as they often cause problems

1. download [NKHook6](https://github.com/TDToolbox/NKHook6/releases/download/24/NKHook6.dll) and [MelonLoader](https://github.com/HerpDerpinstine/MelonLoader/releases/download/v0.2.7.4/MelonLoader.Installer.exe)

2. install/run **melonloader** (NKHook6 will be dealt with later). You should see this screen

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776979212472549406/Screenshot_1313.png"/>
Click the "select" button.

3. go to the BTD6 directory and click on `BloonsTD6.exe`, then click open:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776980387477061662/Screenshot_1315.png"/>

4. on the melonloader window, click the install button

If all goes well, the BTD6 directory should look something like this:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776968486269616159/Screenshot_1311.png"/>

## Optional
there are 2 main mod managers: [this one](https://github.com/TDToolbox/BTD6-Mod-Manager/releases/latest) and [this one](https://github.com/Inferno-Dev-Team/Inferno-Mod-Manager/releases/latest)
mod managers are currently unnecessary and rather inflexible for `.dll` modding; it is as simple as dragging and dropping files into the folder

# Loading Mods

1. put `NKHook6.dll` in a folder called "Mods" in the game's directory
2. put the mod's `.dll` to that same directory. 
<img src = "https://cdn.discordapp.com/attachments/699781597515481159/776967989944647710/Screenshot_1309.png"/>

> NOTE: you dont **need** the mod manager for this

Make sure there are no useless `.zip` files in the mods directory as they can cause problems. Also make sure not to use the same mod twice.

> `.dll.disabled` files are disabled `.dll` mods. This is usually automatically done with the mod manager

> never use mods in coop, races and odyssey, your account will **likely** be flagged. Turn off internet if you use a speed mod. (not compulsory)

can you add this to the tutorial:

# Troubleshooting

### after installing melonloader, there's no console

launch the game and close it

### console says eventregistry not found

make sure you put nkhook6.dll in the "Mods" folder

### console gives another error

make sure you have no duplicate nkhook

make sure you have no duplicate mods

make sure you read the requirements of the mods you are using. some of them require gurren_core.dll for example, or your nkhook version might be outdated.

make sure you aren't using both expansion mods at once.

# Useful Links
## Discord Servers
[BTD6 Mods and Discussions](https://discord.gg/hENWNsd5pY) : Most public mods are here

[NKHook6](https://discord.gg/GUPggzaczS) : the discord for discussing [NKHook6](https://github.com/TDToolbox/NKHook6), which is the forerunning easiest way to make mods

[Inferno Server](https://discord.gg/mZuRncU7ec) : Where Tewity gets his mods (note that most of them arent public)
## Videos
[A good tutorial covering the basics of BTD6 Modding](https://youtu.be/tTtJN5gqPrQ?list=PLWFKnf1pcvUuBUrVQouhvhxqOSQRjst7D)

## Common Mods
(tested for v21)

[Fire Rate Changer](https://github.com/Timotheeee/btd6_mods/blob/master/rate_changer/rate_changer.dll)

[Speedhack](https://github.com/Timotheeee/Speed_mod/blob/main/speedhackmelon/speedhackmelon.dll)

## Others
[BTD6 Documentation](https://github.com/TDToolbox/BTD-Docs/tree/master/Unity%20Engine/Btd6)

## Credits

hosted by: hemidemisemipresent
maintained by: hemidemisemipresent and timotheeee
