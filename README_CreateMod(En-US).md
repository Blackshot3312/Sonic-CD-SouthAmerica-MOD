# How to Create a Sonic CD Music Mod

I'm creating a quick guide on how to make mods for Sonic CD, explaining how the game's file structure works. In this guide, I'll be using **SCDSteamModManager** as a reference.

## Folder structure
The folder should be structured as:
`/ModFolderName/Data/Music`

You can choose whether to modify the American or Japanese version of the music, represented by the directories /JP/ or /US/, respectively. The past tracks should go into the `/Music/` folder directly, before /JP/ or /US/.

## Naming Convention
If you want to base your mod on mine or modify it, feel free to do so! Here’s the naming system:

> A = Present
> 
> B = Past
> 
> C = Good Future
> 
> D = Bad Future

Numbers correspond to specific stages:

> 1 = Palmtree Panic
> 
> 3 = Collision Chaos
> 
> 4 = Tidal Tempest
> 
> 5 = Quartz Quadrant
> 
> 6 = Wacky Workbench
> 
> 7 = Startdust Speedway
> 
> 8 = Metallic Madness

Example: `R3B.ogg (Collision Chaos Past)` or `R8C.ogg (Metallic Madness Good Future)`

Past tracks, or ending 'B' tracks, should be placed in the /music/ folder. Meanwhile, endings A, C, or D should go in their respective folders based on the soundtrack region you plan to modify. In the end, the structure should be:
```
/Music/JP/ (example) R1A, R1C, R1D...
/Music/US/ (example) R1A, R1C, R1D...
/Music/ R1B, R3B, R4B...
```
The **music format must be in .ogg.**

## Mod.ini edit (Manifest)

The `mod.ini` file will be located in the root of your mod folder. It contains the mod’s information so that **SCDSteamModManager** knows what it's dealing with. It's very simple—you can copy the details below, delete everything after the equal sign, and replace it with your own information.

```
Name=Mod Name
Author=Author
Version=1.0
Description=Mod Description
GitHubRepo=Link to the GitHub repository
GitHubAsset=Link to the .git in your repository
UpdateUrl=I left this blank, but maybe it's used for something else
```
The GitHub link isn't mandatory, but it's good to have in case you want to update and notify the launcher.
