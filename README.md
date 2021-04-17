# Getting mods

> NOTE: you need to own BTD6 on steam obviously

**if you already have a mod move to the next section**

get them from one or more of the discord servers linked below. It is recommended that you get familiar with installing and loading mods before you begin making them.


# Access the Mods folder
The BTD6 Steam folder can be found by right click BTD6 in your library, then go to Properties>Local Files>Browse Local Files.
By default, they can be found here

Windows: `Program Files (x86)\Steam\steamapps\common\BloonsTD6`

# Downloads and Installation
> make sure antivirus is turned off as they often cause problems

1. download [Gurren_core.dll](https://cdn.discordapp.com/attachments/504783182755921930/799372741056528414/Gurren_Core.dll), [BloonsTD6_Mod_Helper.dll](https://github.com/gurrenm3/BloonsTD6-Mod-Helper/releases) and [MelonLoader](https://github.com/HerpDerpinstine/MelonLoader/releases/download/v0.2.7.4/MelonLoader.Installer.exe)

2. install/run **melonloader** from [here.](https://github.com/LavaGang/MelonLoader.Installer/releases/latest/download/MelonLoader.Installer.exe) You should see this screen

<img src="https://cdn.discordapp.com/attachments/761529691491270656/831433661270065172/unknown.png"/>

Click on Settings and enable alpha releases. Make sure version 0.3.0 is selected.

Click the "select" button.

3. go to the BTD6 directory and click on `BloonsTD6.exe`, then click open:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776980387477061662/Screenshot_1315.png"/>

4. on the melonloader window, click the install button

now launch the game and close it. then put Gurren_core.dll and BloonsTD6_Mod_Helper.dll in the mods folder (**important**)

If all goes well, the BTD6 directory should look something like this:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776968486269616159/Screenshot_1311.png"/>

**IMPORTANT: BloonsTD6_Mod_Helper.dll and Gurren_core.dll need to be in the Mods directory at all times, never remove or disable them**

# Loading Mods

1. if the mod comes in a zip file, extract it
2. put the mod's `.dll` in the "Mods" directory
<img src = "https://cdn.discordapp.com/attachments/699781597515481159/776967989944647710/Screenshot_1309.png"/>

Make sure not to use the same mod twice as it breaks melonloader.

> `.dll.disabled` files are disabled `.dll` mods. This is usually automatically done with the mod manager. you can also manually rename or move the files to disable them.

## Hacker pool

Using mods in  coop, races and odyssey can get your account flagged. By default the game doesn't let you access these modes if your Mods folder isn't empty.
To avoid getting flagged, turn off your internet if you use the speed hack. Alternatively, setup a Windows virtual machine and use a second Steam account to play mods (much safer). Mods that modify how much monkey money, XP, or trophies you have will also get you flagged. If you are flagged, you will have 2 leaves above your settings icon and you will no longer be able to play public coop games or submit race times.


## Common Mods

[Fire Rate Changer](https://github.com/Timotheeee/btd6_mods/blob/master/rate_changer/rate_changer.dll)

[Speedhack](https://github.com/Timotheeee/btd6_mods/blob/master/speedhackmelon/speedhackmelon.dll) (use keys 6 to 9 to change the speed)

## How to temporarily disable melonloader

If you rename version.dll to anything else you can temporarily disable melonloader. This is useful for playing coop, races and odyssey without getting flagged.

# Troubleshooting

### Mods that used to work before no longer work after a btd6 update

Update your mods by downloading their newest versions.

### The game crashes when loading into a map

if you have nkhook in your mods folder, remove it. The mods that used to require it no longer need it.

### Console gives an error

- Make sure you put Gurren_core.dll and BloonsTD6_Mod_Helper.dll in the "Mods" folder and that they aren't disabled

- Make sure you read the requirements of the mods you are using. Some mods haven't been updated for the latest version of the game, such as the leaked expansion and many of the old nexus mods.

- Make sure there are no zip files in your Mods folder

### Console says the mods are loaded but nothing has changed in the game

You probably have a duplicate mod

### The mod manager crashes or doesn't work

You don't need the mod manager anyways

### MSVCP140.dll was not found

Download visual c++ from the official microsoft website

### Failed to load Il2cpp

redownload the game and reinstall melonloader

### The game crashes when loading a save file, or my profile is corrupted

if you used the jukebox mod, reinstall it and then remove all custom songs before getting rid of it.

if you used the free trophies mod from the nexus then your save file is broken and there's no fix. Don't use that mod.

### After installing melonloader, there's no "Mods" folder

Launch the game and close it

### Installing melonloader takes ages

If it takes more than a few minutes, restart it. maybe your internet connection is unstable. Make sure not to highlight any text in the console. if you do it by accident, press enter.


### Other issues

if you can't find the solution to your problem here, ask in the "help requests" channel in the "BTD6 Mods and Discussions" discord. Make sure to post screenshots and explanations of what you already tried and what the errors are, as well as the list of mods that you used/tried to use.

# Useful Links
## Discord Servers
[BTD6 Mods and Discussions](https://discord.gg/hENWNsd5pY) : Most public mods are here

[Inferno Server](https://discord.gg/mZuRncU7ec) : Where Tewtiy gets his mods (note that most of them aren't public, especially the old ones)


## Optional
there are 2 main mod managers: [this one](https://github.com/TDToolbox/BTD6-Mod-Manager/releases/latest) and [this one](https://github.com/Inferno-Dev-Team/Inferno-Mod-Manager/releases/latest)
mod managers are currently unnecessary and rather inflexible for `.dll` modding; it is as simple as dragging and dropping files into the folder


# How to make mods

## Prerequisites

-  [Visual Studio](https://visualstudio.microsoft.com/) (not Visual Studio code). If you are a rich person, use [Rider](https://www.jetbrains.com/rider/) because its better
- some knowledge of c#, though java is close enough



## Tips

It is generally a good idea to start by downloading an existing mod and then modifying it as it will take care of all the references. Start by downloading the speedhack for example, fix all the dll references and the paths in the properties file and then compile it with ctrl+shift+b to make sure it works.

this video series covers the basics of how to make a mod:
[A good tutorial covering the basics of BTD6 Modding](https://www.youtube.com/watch?v=5wXzWSIJm2I&list=PLWFKnf1pcvUuBUrVQouhvhxqOSQRjst7D&index=6)

these 3 objects have a ton of useful stuff, use visual studio or decompilers to see what's available:

`InGame.instance`

`InGame.instance.bridge`

`Game.instance`

you can use [dnSpy](https://github.com/dnSpy/dnSpy/releases/tag/v6.1.8) (recomended) or [dotPeek](https://www.jetbrains.com/decompiler/) on `Assembly-CSharp.dll` to see (most) of the games functions/methods/classes.

A lot of mods are open source, their code can give you an idea on how to do things.

Most mods use something known as harmony patches. The can be used to run code both before and after the game's functions are called, and can also be used to modify/read parameters and return values.

This mod: https://github.com/sinai-dev/UnityExplorer/releases/download/3.1.4/UnityExplorer.MelonLoader.Il2Cpp.zip makes it possible to view the unity scene.

if you want to import your own 3d models into the game, you will need to create an asset bundle using the 2018 unity version, then use AssetBundle.LoadFromMemory(File.ReadAllBytes(@"bundle"))

gurren's mod helper makes modding easier: https://github.com/gurrenm3/BloonsTD6-Mod-Helper/releases

## Editing the gamemodel

the gamemodel defines everything from towers to bloons to difficulties.

For a better overview of how it works here is the whole thing converted to JSON (without towers): https://cdn.discordapp.com/attachments/793858401977106462/808040397750140968/entiremodel.json

here is the JSON for each individual tower: https://cdn.discordapp.com/attachments/504782676805550113/806879236610457615/towers.zip

if you want to create a custom tower you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/handkanonier/Main.cs) as a template.

if you want to modify existing towers you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/no_rng/Main.cs) as a template.


## How to install mods on Linux

https://gist.github.com/BowDown097/1f35312036c347c40c400f362ac780fd

# Credits

hosted by: [hemidemisemipresent](https://github.com/hemisemidemipresent)

maintained by: [hemidemisemipresent](https://github.com/hemisemidemipresent) and [Timotheeee]()

If you want to change something here, contact `hemidemisemipresent#0301` / `Timotheeee1#0538` on discord or [create a fork and make a pull request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on the [github repo](https://github.com/hemisemidemipresent/btd6-modding-tutorial)
