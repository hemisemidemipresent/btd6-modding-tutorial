# Getting mods

> NOTE: you need to own BTD6 on steam obviously

**if you already have a mod move to the next section**

get them from one or more of the discord servers linked below. It is recommended that you get familiar with installing and loading mods before you begin making them.
> **NOTE: There are no plans for Mac support. For Mac users, it is recommended to emulate Windows to play mods. ~~Like seriously if you are using a mac you should know that they are an ass to do hacky things with~~**

# Access the Mods folder
The BTD6 Steam folder can be found by right click BTD6 in your library, then go to Properties>Local Files>Browse Local Files.
By default, they can be found here

Windows: `Program Files (x86)\Steam\steamapps\common\BloonsTD6`

Linux: `~/.steam/steam/steamapps/common/BloonsTD6` (note that linux does not support DLL mods)

# Downloads and Installation
> make sure antivirus is turned off as they often cause problems

1. download [NKHook6](https://github.com/TDToolbox/NKHook6/releases/download/41/NKHook6.dll) and [MelonLoader](https://github.com/HerpDerpinstine/MelonLoader/releases/download/v0.2.7.4/MelonLoader.Installer.exe)

2. install/run **melonloader** (NKHook6 will be dealt with later). You should see this screen

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776979212472549406/Screenshot_1313.png"/>
Click the "select" button.

3. go to the BTD6 directory and click on `BloonsTD6.exe`, then click open:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776980387477061662/Screenshot_1315.png"/>

4. on the melonloader window, click the install button

now launch the game and close it. then put NKHook6.dll in the mods folder

If all goes well, the BTD6 directory should look something like this:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776968486269616159/Screenshot_1311.png"/>

**IMPORTANT: NKHook6.dll needs to be in the Mods directory at all times, never remove or disable it**

# Loading Mods

1. if the mod comes in a zip file, extract it
2. put the mod's `.dll` in the "Mods" directory
<img src = "https://cdn.discordapp.com/attachments/699781597515481159/776967989944647710/Screenshot_1309.png"/>

Make sure not to use the same mod twice.

> `.dll.disabled` files are disabled `.dll` mods. This is usually automatically done with the mod manager. you can also manually rename the files to disable them.

> never use mods in coop, races and odyssey, your account will **likely** be flagged. Turn off internet if you use a speed mod. (not compulsory). Alternatively, setup a Windows WM and use a second Steam account to play mods.

## Optional
there are 2 main mod managers: [this one](https://github.com/TDToolbox/BTD6-Mod-Manager/releases/latest) and [this one](https://github.com/Inferno-Dev-Team/Inferno-Mod-Manager/releases/latest)
mod managers are currently unnecessary and rather inflexible for `.dll` modding; it is as simple as dragging and dropping files into the folder

## .btd6mod files
this is an outdated format that you should avoid using. if you still want to use it, use this: https://www.nexusmods.com/bloonstd6/mods/41

# Troubleshooting

### after installing melonloader, there's no "Mods" folder

launch the game and close it

### installing melonloader takes ages

if it takes more than a few minutes, restart it. maybe your internet connection is unstable.

### the mod manager crashes or doesn't work

you don't need the mod manager anyways

### console says eventregistry not found

make sure you put nkhook6.dll in the "Mods" folder

### console gives another error

make sure you have no duplicate nkhook

make sure you have no duplicate mods

make sure you read the requirements of the mods you are using. some of them require [gurren_core.dll](https://cdn.discordapp.com/attachments/504783182755921930/799372741056528414/Gurren_Core.dll) for example, or your nkhook version might be outdated.

make sure you aren't using both expansion mods at once.

### failed to load Il2cpp

redownload the game and reinstall melonloader

# Useful Links
## Discord Servers
[BTD6 Mods and Discussions](https://discord.gg/hENWNsd5pY) : Most public mods are here

[NKHook6](https://discord.gg/GUPggzaczS) : the discord for discussing [NKHook6](https://github.com/TDToolbox/NKHook6), which is the forerunning easiest way to make mods

[Inferno Server](https://discord.gg/mZuRncU7ec) : Where Tewtiy gets his mods (note that most of them aren't public)

## Common Mods

[Fire Rate Changer](https://github.com/Timotheeee/btd6_mods/blob/master/rate_changer/rate_changer.dll)

[Speedhack](https://github.com/Timotheeee/Speed_mod/blob/main/speedhackmelon/speedhackmelon.dll)

## How to make mods

It is generally a good idea to start by downloading an existing mod and then modifying it as it will take care of all the references. Start by downloading the speedhack for example, fix all the dll references and the paths in the properties file and then compile it with ctrl+shift+b to make sure it works.

this video series can also help:
[A good tutorial covering the basics of BTD6 Modding](https://www.youtube.com/watch?v=5wXzWSIJm2I&list=PLWFKnf1pcvUuBUrVQouhvhxqOSQRjst7D&index=6)

[NKhook Documentation](https://github.com/TDToolbox/BTD-Docs/tree/master/Unity%20Engine/Btd6/NKHook6)

a few tips:
these 3 objects have a ton of useful stuff, use visual studio to see what's available:
InGame.instance.
InGame.instance.bridge.
Game.instance.

you can use DNspy on assembly-csharp.dll to see the game's functions.

a lot of mods are open source, their code can give you an idea on how to do things.

## Credits

hosted by: hemidemisemipresent
maintained by: hemidemisemipresent and timotheeee












