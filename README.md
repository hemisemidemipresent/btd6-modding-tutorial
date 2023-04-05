# Downloads and Installation

If run into any issues while installing, then check the troubleshooting section down below.

**IMPORTANT**: Mods that were last updated before december 26th 2022 **NO LONGER WORK** (because of some melonloader changes made around that time). Also, to use Melonloader you now need to download and install [.NET 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer). If you don't have it, you will get an error when launching the game. And Windows 7 is no longer supported.

Download [the mod helper](https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll) and [MelonLoader](https://github.com/LavaGang/MelonLoader/releases/download/v0.6.1/MelonLoader.x64.zip)

Open the Melonloader zip you just downloaded, then select all of the files in the zip and copy them

<img src="https://cdn.discordapp.com/attachments/761529691491270656/1067357050935451688/image.png"/>

Navigate to the BTD6 directory, which by default is located at: `C:\Program Files (x86)\Steam\steamapps\common\BloonsTD6`

Paste the files from the zip into the BTD6 directory

<img src="https://cdn.discordapp.com/attachments/761529691491270656/1067359077820280852/image.png"/>

Download [.NET 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer) and install it

<img src="https://cdn.discordapp.com/attachments/761529691491270656/1091098817958531162/image.png"/>


Now launch the game to generate the "Mods" folder. If you get the MSVCP140.dll was not found error, or the game doesn't launch at all then install [visual c++](https://aka.ms/vs/16/release/vc_redist.x64.exe) and then restart your pc. 

Put **`Btd6ModHelper.dll`** in the "Mods" folder

If all goes well, the Mods directory should look like this:

<img src="https://cdn.discordapp.com/attachments/859064232262762497/1008077519242657822/unknown.png"/>

**IMPORTANT: `Btd6ModHelper.dll` needs to be in the Mods directory at all times. If you don't have the mod helper, the game will not save progress and most mods will not work.**

If you are using the **`Epic Games`** version of the game, then you will also need to follow [this tutorial](https://github.com/Baydock/BTD6EpicGamesModCompat/) to make melonloader work.

To create your own mods, watch [this video](https://www.youtube.com/watch?v=NSINBN3em6w) and check out the tips down below.

## How to uninstall Melonloader

delete the melonloader, mods, plugins, userdata, userlibs folders as well as dobby.dll, notice.txt and version.dll

## Common Mods

[Fire Rate Changer](https://github.com/Timotheeee/btd6_mods/blob/master/rate_changer/rate_changer.dll) (custom speed hypersonic, press F9 to use)

[Speedhack](https://github.com/Timotheeee/btd6_mods/blob/master/speedhackmelon/speedhackmelon.dll) (use keys 6,7,8,9 to change the speed)


# Obtaining Mods

The mod helper adds a new button to the bottom right of the main menu which allows you to access the mod browser, where you can find a bunch of mods as well as mod repositories.

You can also get mods from these discord servers:

[BTD6 Mods and Discussions](https://discord.gg/hENWNsd5pY) : Most public mods are here

[1330 Studios](https://discord.gg/cqRqrvjv68) : Most public mods are here too. Tewtiy also gets his mods from here (note that some of them aren't public, especially older ones)

Avoid using Nexus mods as the vast majority of them are outdated/stolen.

To download mods from github, try to find a dll file and download it. If there is no dll file, then check if there are any releases

To disable some mods, you can manually move the files to another directory.

## Hacker pool

By default the game doesn't let you access public coop, races, collection events, the trophy store and odyssey if you are using mods (to prevent cheating). 
Using mods that give your account an advantage such as infinite money/xp/trophies/knowledge mods will get your account flagged. 
To protect your account, setup a Windows virtual machine and use a second Steam account to play mods (can also be done without a virtual machine but it's pretty annoying to switch between accounts). 
If you are flagged, you will have 2 leaves above your settings icon and you will no longer be able to play public coop games, play contested territory or submit race times. 
Using the speedhack in singleplayer is usually fine, unless you abuse it to grind monkey money faster and then get a top 50 time in a race. 
Using mods in private coop is risky, it is best to use an account that you don't care about and also make sure that every player is using the same mods with the same configurations. If you do get flagged, you will still be able to play private coop.


# Troubleshooting

## The console or a popup window says "il2cpp_init detour failed"

You need to install the .Net 6 Runtime [https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer)

## A popup window says "failed to initialize: failed to find bootstrap"

You didn't uninstall melonloader correctly. you need to delete the melonloader, mods, plugins, userdata, userlibs folders as well as dobby.dll, notice.txt and version.dll

## A popup window says "failed to initialize: failed to load library"

Rename your btd6 folder to "BloonsTD6". If that doesn't work, change the language of Windows to english. If that still doesn't work, reinstall the game with your antivirus turned off. It's not entirely clear what causes this error.

## The console says "Could not load file or assembly ..."

Reinstall Melonloader with your antivirus turned off

## The game is not saving

Make sure you have the mod helper, you can download the latest release here: [https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll](https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll)

If you are trying to uninstall, read the section above

## The game crashes while loading mods

-Make sure you have the mod helper, you can download the latest release here: [https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll](https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll)

-Make sure you are not using any mods that were last updated before december 26th 2022

-If that doesn't solve it, navigate to the Melonloader folder and check the "latest.log" file. if it doesn't contain any errors then check the console errors and see if you can figure it out yourself. if not, join one of the discord servers linked above and post the log file or a screenshot of the console in the help channel.

## The mods are in the Mods folder but they don’t work

Make sure you are using the latest version of the mod helper (check the link above). Make sure your mods are in the dll format directly inside of the "Mods" folder. They should not be in a zip. Game updates sometimes break mods and not all mod developers update their mods. Avoid using nexus mods as the vast majority of them are outdated/low quality/stolen.
If you still have problems, join one of the 2 discord servers above and then send the `latest.log` located in the **Melonloader** folder in the help channel. 

## The game does not open at all, or gives an MSVCP140.dll was not found error

Install this: [https://aka.ms/vs/16/release/vc_redist.x64.exe](https://aka.ms/vs/16/release/vc_redist.x64.exe)




# How to make mods

## Prerequisites

-   [Visual Studio](https://visualstudio.microsoft.com/) (not Visual Studio code)
-   Some basic knowledge of [c#](https://docs.microsoft.com/en-us/dotnet/csharp/), though if you already know Java, it is close enough

## getting started
Read [this](https://github.com/gurrenm3/BTD-Mod-Helper/wiki/Getting-Started). The mod helper wiki also has a bunch of useful info about the game's structure.

## Tips

A lot of mods are open source, their code can give you an idea on how to do things.

Most mods use something known as harmony patches. The can be used to run code both before and after the game's functions are called, and can also be used to modify/read parameters and return values.

[UnityExplorer mod](https://github.com/Baydock/UnityExplorer-NewML/releases/latest) makes it possible to view the unity scene.

If you want to import your own 3D models into the game, you will need to create an asset bundle using the unity version the game uses, check your melonloader log or console to see this, then use

```cs
AssetBundle.LoadFromMemory(File.ReadAllBytes(@"bundle"))
```

## Editing the gamemodel

The gamemodel defines everything from towers to bloons to difficulties.

For a better overview of how it works here is [the whole thing converted to JSON (without towers)](https://cdn.discordapp.com/attachments/504783182755921930/869939855923236944/entiremodel.json)

[Here](https://cdn.discordapp.com/attachments/504783182755921930/869939786734010418/Towers.zip) is the JSON for each individual tower

You can also get newer json files by going into the in-game mod helper settings, there should be an option to dump the gamemodel there.

If you want to create a custom tower you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/handkanonier/Main.cs) as a template. Creating custom towers mostly involves copying existing behaviors and pasting them together. Use the JSON above to see how towers are defined. Use [this video](https://www.youtube.com/watch?v=NSINBN3em6w) as a guide.

If you want to modify existing towers you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/no_rng/Main.cs) as a template.

## [How to install mods on Linux]
Install MelonLoader with [this guide](https://melonwiki.xyz/#/?id=linux-instructions). Make sure you put Mod Helper in the Mods folder.

# Credits

Hosted by: [hemidemisemipresent](https://github.com/hemisemidemipresent)

Maintained by: [hemidemisemipresent](https://github.com/hemisemidemipresent), [Timotheeee](https://github.com/Timotheeee/btd6_mods) and [Silentstorm](https://github.com/Onixiya)

If you want to change something here, contact `hemidemisemipresent#0301` / `Timotheeee1#1337` / `Silentstorm#5336` on discord or [create a fork and make a pull request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on the [github repo](https://github.com/hemisemidemipresent/btd6-modding-tutorial)
