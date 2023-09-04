# Downloads and Installation

If run into any issues while installing, then check the [troubleshooting section](https://hemisemidemipresent.github.io/btd6-modding-tutorial/#troubleshooting) down below.

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

If you are using the **`Epic Games`** version of the game, then you will also need to follow [this tutorial](https://github.com/GrahamKracker/BTD6EpicGamesModCompat/) to make melonloader work.

There is a common problem where some anti-viruses delete certain melonloader files. This is usually not an issue with Windows Defender. If you are using another anti-virus, then add an exception to the melonloader folder.

To create your own mods, watch [this video](https://www.youtube.com/watch?v=NSINBN3em6w) and check out the tips down below.

## How to uninstall Melonloader

delete the melonloader, mods, plugins, userdata, userlibs folders as well as dobby.dll, notice.txt and version.dll

## Common Mods

[Fire Rate Changer](https://github.com/Timotheeee/btd6_mods/blob/master/rate_changer/rate_changer.dll) (custom speed hypersonic, press F9 to use)

[Speedhack](https://github.com/Timotheeee/btd6_mods/blob/master/speedhackmelon/speedhackmelon.dll) (use keys 6,7,8,9 to change the speed)

[Race Button](https://github.com/Timotheeee/btd6_mods/blob/master/racemod/racemod.dll) and [Round changer](https://github.com/Timotheeee/btd6_mods/raw/master/round_changer/round_changer.dll) (press F8 to use)


# Obtaining Mods

The mod helper adds a new button to the bottom right of the main menu which allows you to access the mod browser, where you can find a bunch of mods as well as mod repositories.

You can also get mods from this discord server:

[BTD6 Mods and Discussions](https://discord.gg/hENWNsd5pY)

Avoid using Nexus mods as the vast majority of them are outdated/stolen.

To download mods from github, try to find a dll file and download it. If there is no dll file, then check if there are any releases.

To disable some mods, you can manually move the files to another directory.

## Hacker pool

By default the game doesn't let you access public coop, races, collection events, the trophy store and odyssey if you are using mods (to prevent cheating). 
Using mods that give your account an advantage such as infinite money/xp/trophies/knowledge mods will get your account flagged. 
To protect your main account it is recommended to play on an alternate account. If you don't want to do this, turning off your internet connection is also an effective way to avoid getting flagged while using mods in singleplayer/challenge editor (although not guaranteed to always work). 
If you are flagged, you will have 2 leaves above your settings icon and you will no longer be able to play public coop games, play contested territory or submit race times. 
Using the speedhack in singleplayer is usually fine, unless you abuse it to grind monkey money faster and then get a top 50 time in a race. Turn off your internet while using it to be safer. Using speedhack in odyssey is guaranteed to get you flagged.
Using mods in private coop is risky, it is best to use an account that you don't care about and also make sure that every player is using the same mods with the same configurations. If you do get flagged, you will still be able to play private coop.


# Troubleshooting

## The console or a popup window says "il2cpp_init detour failed"

You need to install the .Net 6 Runtime [https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer)

## A popup window says "failed to initialize: failed to find bootstrap"

You didn't uninstall melonloader correctly. you need to delete the melonloader, mods, plugins, userdata, userlibs folders as well as dobby.dll, notice.txt and version.dll

## A popup window says "failed to initialize: failed to load library"

The path to the BTD6 exe file should not have any special characters. This includes dashes **`-`** and modified letters like **`À`**

## The console says "Could not load file or assembly ..."

Delete the MelonLoader folder, then reinstall Melonloader with your antivirus turned off. If you get the exact same error again, try replacing the melonloader folder with these [files](https://cdn.discordapp.com/attachments/500665135711387680/1121347870885412974/MelonLoader.zip)

## The console says "1 Plugin loaded" and then gets stuck
Use [this](https://nightly.link/LavaGang/MelonLoader/workflows/build/alpha-development) melonloader version

## The game is not saving

Make sure you have the mod helper, you can download the latest release here: [https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll](https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll)

If you are trying to uninstall, read the section above

## The game crashes while loading mods, or the mods are not working

-Make sure you have the mod helper, you can download the latest release here: [https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll](https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll)

-Make sure you are not using any mods that were last updated before december 26th 2022

-Make sure your mods are in the dll format directly inside of the "Mods" folder. They should not be in a zip or in a subfolder. 

-Game updates sometimes break mods and not all mod developers update their mods. 

-Avoid using nexus mods as the vast majority of them are outdated/low quality/stolen.

-If none of the above tips solve the problem, navigate to the Melonloader folder and check the "latest.log" file. If you see that a specific mod appears to be causing errors, remove it or check for a new version. If the log file doesn't contain any errors then check if the console does. You can also try removing each mod one by one until you find the one that is causing issues. If you can't figure it out yourself, join the discord server linked above and post the log file or a screenshot of the console in the help channel.

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

[UnityExplorer mod](https://github.com/GrahamKracker/UnityExplorer) makes it possible to view the unity scene.

If you want to import your own 3D models into the game, you will need to create an asset bundle using the unity version the game uses, check your melonloader log or console to see this, then use

```cs
AssetBundle.LoadFromMemory(File.ReadAllBytes(@"bundle"))
```

## Editing the gamemodel

The gamemodel defines everything from towers to bloons to difficulties.

For a better overview of how it works here is [the whole thing converted to JSON](https://github.com/Btd6ModHelper/btd6-game-data)

[Here]((https://github.com/Btd6ModHelper/btd6-game-data/tree/main/Towers)) is the JSON for each individual tower

You can also get newer json files by going into the in-game mod helper settings, there should be an option to dump the gamemodel there.

If you want to create a custom tower you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/handkanonier/Main.cs) as a template. Creating custom towers mostly involves copying existing behaviors and pasting them together. Use the JSON above to see how towers are defined. Use [this video](https://www.youtube.com/watch?v=NSINBN3em6w) as a guide.

If you want to modify existing towers you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/no_rng/Main.cs) as a template.

## [How to install mods on Linux]
Install MelonLoader with [this guide](https://melonwiki.xyz/#/?id=linux-instructions). Make sure you put Mod Helper in the Mods folder.

# Credits

Hosted by: [hemidemisemipresent](https://github.com/hemisemidemipresent)

Maintained by: [hemidemisemipresent](https://github.com/hemisemidemipresent), [Timotheeee](https://github.com/Timotheeee/btd6_mods) and [Silentstorm](https://github.com/Onixiya)

If you want to change something here, contact `hemidemisemipresent#0301` / `Timotheeee1#1337` / `Silentstorm#5336` on discord or [create a fork and make a pull request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on the [github repo](https://github.com/hemisemidemipresent/btd6-modding-tutorial)
