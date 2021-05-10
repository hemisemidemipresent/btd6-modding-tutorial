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

1. download [Gurren_core.dll](https://cdn.discordapp.com/attachments/504783182755921930/799372741056528414/Gurren_Core.dll), [BloonsTD6_Mod_Helper.dll](https://github.com/gurrenm3/BTD-Mod-Helper/releases) and [MelonLoader](https://github.com/LavaGang/MelonLoader.Installer/releases/latest/download/MelonLoader.Installer.exe)

2. Run the **melonloader** installer. You should see this screen

<img src="https://cdn.discordapp.com/attachments/761529691491270656/831433661270065172/unknown.png"/>

Click on Settings and enable alpha releases. Make sure version 0.3.0 is selected.

Click the "select" button.

3. go to the BTD6 directory and click on `BloonsTD6.exe`, then click open:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776980387477061662/Screenshot_1315.png"/>

4. on the melonloader window, click the install button

now launch the game and close it. then put Gurren_core.dll and BloonsTD6_Mod_Helper.dll in the mods folder (**important**)

If all goes well, the BTD6 directory should look something like this:

<img src="https://cdn.discordapp.com/attachments/761529691491270656/833016709900009499/unknown.png"/>

**IMPORTANT: BloonsTD6_Mod_Helper.dll and Gurren_core.dll need to be in the Mods directory at all times, never remove or disable them**

# Loading Mods

1. if the mod comes in a zip file, extract it
2. put the mod's `.dll` in the "Mods" directory
3. make sure that there are no zip files or duplicate mods in the "Mods" directory

to disable some mods, you can manually move the files to another directory.

## Hacker pool

By default the game doesn't let you access coop, races and odyssey if your Mods folder isn't empty, to prevent cheating. Using mods that give your account an advantage such as infinite money/xp/trophies/knowledge mods or abusing the speedhack to grind faster will get your account flagged. To protect your account, setup a Windows virtual machine and use a second Steam account to play mods (can also be done without a virtual machine but it's pretty annoying to switch between accounts). If you are flagged, you will have 2 leaves above your settings icon and you will no longer be able to play public coop games or submit race times.

## How to temporarily disable melonloader

If you rename version.dll to anything else you can temporarily disable melonloader. This is useful for playing coop, races and odyssey without having to uninstall melonloader. make sure your mods folder is empty or these gamemodes won't be available.

## Common Mods

[Fire Rate Changer](https://github.com/Timotheeee/btd6_mods/blob/master/rate_changer/rate_changer.dll) (custom speed hypersonic, press F9 to use)

[Speedhack](https://github.com/Timotheeee/btd6_mods/blob/master/speedhackmelon/speedhackmelon.dll) (use keys 6 to 9 to change the speed)


# Troubleshooting

### Assembly Generator exited with code -2

Reinstall melonloader using the latest version (enable alphas in the installer's settings first)

### The mods are in the Mods folder but they don't work

- If you have nkhook in your mods folder, remove it. The mods that used to require it no longer need it. A few mods haven't been updated but those were mostly broken already.

- Most of the mods on the Nexus no longer work and have been abandoned by their creator. Remove broken abandoned mods and search for up to date alternatives in the discord servers.

- Make sure you put Gurren_core.dll and BloonsTD6_Mod_Helper.dll in the "Mods" folder and that they aren't disabled

- Make sure there are no zip files in your Mods folder

### The mod manager crashes or doesn't work

You don't need the mod manager anyways

### Mods that used to work before no longer work after a btd6 update

Update your mods by downloading their newest versions, and update the mod helper if you haven't done so already. Some mods have been abandoned by their creator and no longer work. 

### Could not resolve type with token [...] BloonsTD6_Mod_Helper

The BloonsTD6_Mod_Helper has been renamed to BTD_Mod_Helper for compatibility with future games (sorry for the inconvenience). Update every mod that uses the mod helper, they now require the BTD_Mod_Helper instead.

### Could not load type ... while decoding custom attribute

Same as above

### Could not resolve type with token [...] BTD_Mod_Helper

The BloonsTD6_Mod_Helper has been renamed to BTD_Mod_Helper for compatibility with future games (sorry for the inconvenience). You need to download the new BTD_Mod_Helper from the link above in the tutorial. (There's a good chance you will then get the error above)

### Caching Steam ID ... [API loaded no]

Restart steam then try again. If that doesn't work try running BTD6 as administrator

### MSVCP140.dll was not found

Download visual c++ from the official microsoft website

### Failed to load Il2cpp

redownload the game and reinstall melonloader

### The game crashes when loading a save file, or my profile is corrupted

if you used the jukebox mod, reinstall it and then remove all custom songs before getting rid of it.

### After installing melonloader, there's no "Mods" folder

Launch the game and close it

### Installing melonloader takes ages

If it takes more than a few minutes, restart it. maybe your internet connection is unstable. Make sure not to highlight any text in the console. if you do it by accident, press enter.

### [INTERNAL FAILURE] Failed to Execute Assembly Generator!

turn off the firewall and run BTD6 as administrator


### Other issues

if you can't find the solution to your problem here, ask in the "help requests" channel in the "BTD6 Mods and Discussions" discord. Make sure to post screenshots and explanations of what you already tried and what the errors are, as well as the list of mods that you used/tried to use.

# Useful Links
## Discord Servers
[BTD6 Mods and Discussions](https://discord.gg/hENWNsd5pY) : Most public mods are here

[Inferno Server](https://discord.gg/mZuRncU7ec) : Where Tewtiy gets his mods (note that most of them aren't public)


## Optional
there are 2 main mod managers: [this one](https://github.com/TDToolbox/BTD6-Mod-Manager/releases/latest) and [this one](https://github.com/Inferno-Dev-Team/Inferno-Mod-Manager/releases/latest)
mod managers are currently unnecessary and rather inflexible for `.dll` modding; it is as simple as dragging and dropping files into the folder.


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

For a better overview of how it works here is the whole thing converted to JSON (without towers): https://cdn.discordapp.com/attachments/505179324488613909/836926751463440404/entiremodel.zip

here is the JSON for each individual tower: https://cdn.discordapp.com/attachments/505179324488613909/836926742404923412/Towers.7z

if you want to create a custom tower you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/handkanonier/Main.cs) as a template.

if you want to modify existing towers you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/no_rng/Main.cs) as a template.


## How to install mods on Linux

https://gist.github.com/BowDown097/1f35312036c347c40c400f362ac780fd

# Credits

hosted by: [hemidemisemipresent](https://github.com/hemisemidemipresent)

maintained by: [hemidemisemipresent](https://github.com/hemisemidemipresent) and [Timotheeee]()

If you want to change something here, contact `hemidemisemipresent#0301` / `Timotheeee1#0538` on discord or [create a fork and make a pull request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on the [github repo](https://github.com/hemisemidemipresent/btd6-modding-tutorial)
