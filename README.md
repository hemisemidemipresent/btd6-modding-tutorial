# Downloads and Installation

Download [the mod helper](https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll) and [MelonLoader](https://github.com/LavaGang/MelonLoader.Installer/releases/latest/download/MelonLoader.Installer.exe).

Run the **melonloader** installer. You should see this screen

<img src="https://cdn.discordapp.com/attachments/761529691491270656/870680857940209694/unknown.png"/>

Go to the "Settings" tab on the right of the installer. Enable the "Show ALPHA Pre-Releases" option.

<img src="https://cdn.discordapp.com/attachments/859064232262762497/1057496273906839632/image.png"/>

Go back to the "Automated" tab on the left of the installer.

Click the "select" button.

Navigate to the BTD6 directory, which by default is located at: `C:\Program Files (x86)\Steam\steamapps\common\BloonsTD6` and click on `BloonsTD6.exe`, then click open:

<img src="https://cdn.discordapp.com/attachments/699781597515481159/776980387477061662/Screenshot_1315.png"/>

On the melonloader window, click the install button (install the latest release)

Now launch the game to generate the "Mods" folder. 
If you get the MSVCP140.dll was not found error, or the game doesn't launch at all then install [visual c++](https://aka.ms/vs/16/release/vc_redist.x64.exe). 
If you get an error like "Access to the path '...' is denied" then run turn off your antivirus, reinstall melonloader and run the game as administrator.

Now put **`Btd6ModHelper.dll`** in the "Mods" folder (**important**)

If all goes well, the Mods directory should look like this:

<img src="https://cdn.discordapp.com/attachments/859064232262762497/1008077519242657822/unknown.png"/>

**IMPORTANT: `Btd6ModHelper.dll` needs to be in the Mods directory at all times. If you don't have the mod helper, the game will not save progress and most mods will not work.**


## Common Mods

[Fire Rate Changer](https://github.com/Timotheeee/btd6_mods/blob/master/rate_changer/rate_changer.dll) (custom speed hypersonic, press F9 to use)

[Speedhack](https://github.com/Timotheeee/btd6_mods/blob/master/speedhackmelon/speedhackmelon.dll) (use keys 6,7,8,9 to change the speed)


# Loading Mods

You can get mods from these discord servers:

[BTD6 Mods and Discussions](https://discord.gg/hENWNsd5pY) : Most public mods are here

[Inferno Server](https://discord.gg/cqRqrvjv68) : Where Tewtiy gets his mods (note that most of them aren't public)

Avoid using Nexus mods as the vast majority of them are outdated/stolen.

1. if the mod comes in a zip file, extract it
2. put the mod's `.dll` in the `Mods` directory
3. make sure that there are no zip files or duplicate mods in the `Mods` directory

To disable some mods, you can manually move the files to another directory.

## Hacker pool

By default the game doesn't let you access public coop, races, collection events, the trophy store and odyssey if you are using mods (to prevent cheating). 
Using mods that give your account an advantage such as infinite money/xp/trophies/knowledge mods will get your account flagged. 
To protect your account, setup a Windows virtual machine and use a second Steam account to play mods (can also be done without a virtual machine but it's pretty annoying to switch between accounts). 
If you are flagged, you will have 2 leaves above your settings icon and you will no longer be able to play public coop games, play contested territory or submit race times. 
Using the speedhack in singleplayer is usually fine, unless you abuse it to grind monkey money faster and then get a top 50 time in a race.

## How to disable mods

Move `version.dll`, the `Melonloader` folder and the `Mods` folder **entirely out of the BTD6 directory** (put them in a folder on your Desktop for example). 




# Troubleshooting

## The console says "il2cpp_init detour failed: One of the dependant libraries is missing"

You need to install the .Net 6 Runtime [https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-6.0.12-windows-x64-installer)

## The console says "No compatibility layer found"

You need to download the mod helper, download the latest release here: [https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll](https://github.com/gurrenm3/BTD-Mod-Helper/releases/latest/download/Btd6ModHelper.dll)
also make sure that it is **not in a zip file** and **not in a folder**. It should be a dll file directly inside of the "Mods" folder.

## The mods are in the Mods folder but they don’t work

Make sure you are using the latest version of the mod helper (check the link above). Make sure your mods are in the dll format directly inside of the "Mods" folder. They should not be in a zip. Game updates sometimes break mods and not all mod developers update their mods. Avoid using nexus mods as the vast majority of them are outdated/low quality/stolen.
If you still have problems, join one of the 2 discord servers above and then send the `latest.log` located in the **Melonloader** folder in the help channel. 

## The game does not open at all, or gives an MSVCP140.dll was not found error

Install this: [https://aka.ms/vs/16/release/vc_redist.x64.exe](https://aka.ms/vs/16/release/vc_redist.x64.exe)






# How to make mods

## Prerequisites

-   [Visual Studio](https://visualstudio.microsoft.com/) (not Visual Studio code)
-   Some basic knowledge of [c#](https://docs.microsoft.com/en-us/dotnet/csharp/), though if you already know Java, it is close enough

## Tips

It is generally a good idea to start by downloading an existing mod and then modifying it as it will include all the nescessary files. Start by downloading the speedhack for example, fix all the paths of the dll references and the paths in the properties file and then compile it with ctrl+shift+b to make sure it works.

Mods usually reference Melonloader.dll, the mod helper and most of the files in the Managed folder.

The [Mod helper wiki](https://github.com/gurrenm3/BTD-Mod-Helper/wiki) has a bunch of useful documentation.

These 3 objects have a ton of useful stuff, use visual studio or decompilers to see what's available:

`InGame.instance`

`InGame.instance.bridge`

`Game.instance`

You can use [dnSpy](https://github.com/dnSpy/dnSpy/releases/tag/v6.1.8) (recomended) or [dotPeek](https://www.jetbrains.com/decompiler/) on `Assembly-CSharp.dll` to see (most) of the games functions/methods/classes.

A lot of mods are open source, their code can give you an idea on how to do things.

Most mods use something known as harmony patches. The can be used to run code both before and after the game's functions are called, and can also be used to modify/read parameters and return values.

[UnityExplorer mod](https://github.com/sinai-dev/UnityExplorer/releases/download/3.1.4/UnityExplorer.MelonLoader.Il2Cpp.zip) makes it possible to view the unity scene.

If you want to import your own 3D models into the game, you will need to create an asset bundle using the 2018 unity version, then use

```cs
AssetBundle.LoadFromMemory(File.ReadAllBytes(@"bundle"))
```

## Editing the gamemodel

The gamemodel defines everything from towers to bloons to difficulties.

For a better overview of how it works here is [the whole thing converted to JSON (without towers)](https://cdn.discordapp.com/attachments/504783182755921930/869939855923236944/entiremodel.json)

[Here](https://cdn.discordapp.com/attachments/504783182755921930/869939786734010418/Towers.zip) is the JSON for each individual tower

If you want to create a custom tower you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/handkanonier/Main.cs) as a template. Creating custom towers mostly involves copying existing behaviors and pasting them together. Use the JSON above to see how towers are defined. Use [this video](https://www.youtube.com/watch?v=NSINBN3em6w) as a guide.

If you want to modify existing towers you can use [this](https://github.com/Timotheeee/btd6_mods/blob/master/no_rng/Main.cs) as a template.

## [How to install mods on Linux]
Install MelonLoader with [this guide](https://melonwiki.xyz/#/?id=linux-instructions). Make sure you put Mod Helper in the Mods folder.

# Credits

Hosted by: [hemidemisemipresent](https://github.com/hemisemidemipresent)

Maintained by: [hemidemisemipresent](https://github.com/hemisemidemipresent) and [Timotheeee](https://github.com/Timotheeee/btd6_mods)

If you want to change something here, contact `hemidemisemipresent#0301` / `Timotheeee1#0538` on discord or [create a fork and make a pull request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on the [github repo](https://github.com/hemisemidemipresent/btd6-modding-tutorial)
