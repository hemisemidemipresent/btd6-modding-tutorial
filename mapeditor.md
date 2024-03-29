note: if your Windows is set to a language that uses commas instead of periods to represent decimals (like polish), then the map editor doesn't work.

# How to use the map editor
- Start by copying the files from the [zip](https://github.com/Timotheeee/btd6_mods/blob/master/map_editor/map_editor.zip) into your Mods folder. The mods folder should have include the mod helper, the 2 dll files from the map editor and the map_editor folder.
- go in the map_editor folder, make a copy of the "example" folder and rename it to the name of your map
- Now go in that new folder and open info.txt, you will be able to change the music and difficulty (0 = beginner, 3 = expert etc)
- Replace "image.png" with the image of your map (make sure the new file is called image.png)
- Now launch the game and enter your map, so you can start defining what the paths and areas should be.

## defining paths
press F1, click around, press F1 again when you're done. You can define multiple tracks. Before moving on, make sure you pressed F1 to finish up the last track you made.

## defining areas
Areas define collisions and where towers can be placed. They are defined by pressing F2, but first you need to tell the mod what type of area you want.
- Pressing 0 will select the type of "track" (default)
- Pressing 1 will select the type of "water"
- Pressing 2 will select the type of "land"
- Pressing 3 will select the type of "unplaceable" (there doesn't seem to be a difference between "track" and this one)
- Pressing 4 will toggle whether or not the area should block line of sight. (by default, it doesn't)

After defining the area type, press F2. Now click around to define a polygon, then press F2 again when you're done. It is highly recommended to start by making the entire map a "land" area (by clicking in all 4 corners) and then drawing the water/walls on top of that (placing towers in a spot that has no area defined crashes the game). Polygons autocomplete themselves (unless the area blocks LOS!) and the newest areas are stacked on top of the older ones.

## undoing changes
in the map's folder you can edit or delete the paths.txt and areas.txt files to undo your recent changes or to start from scratch.

## end
Once you are done defining your map, close the game. You can now remove the map editor mod if you want to, but keep the map loader. When you restart the game, your map will load and should be playable.

## available music
MusicBTD5JazzA
MusicCityA
MusicCoopA
MusicDarkA
MusicSailsAgain
MusicUpbeat1A
MusicUpbeat2A
MusicUpbeat3A

# How to use the map loader
- Extract map_editor.zip in your Mods folder
- Delete map_editor.dll
- If someone sent you a zip file with a map in it, just extract it into the map_editor folder.

# Troubleshooting
## The game crashes when entering the custom map, after defining the tracks and areas.
You probably messed up while editing. you can edit or delete the paths.txt and areas.txt files to try to fix the problem or to start from scratch. Alternatively you can send those 2 files and your latest.log file in the help channel of one of the modding discord servers.

## If you can't find your map in the map list
make sure you don't end up with a "map_editor" folder inside of another "map_editor" folder

## The game crashes when placing towers
You need to start by defining the entire map as "land". (read the above sections again)



