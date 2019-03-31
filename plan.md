## Current Projects

### pyxedit (pyxedit)

A python wrapper to xedit

### NPC Stylizer (npc-stylizer)

A tool that allows users to pick and choose which npc is to be replaced by which
npc replacer mod.

Mods to support: ANY

### NPC Facebook (npc-facebook)

**Script To Generate FormList**

skyrim-builder modlist to install the following:

- any required body replacer (UNP, CBBE, SOS, etc..., and custom body textures)
- any required hair mods (ApachiiSkyHair, etc...)
- the list of NPC overhaul mods
- salt and wind retextures
- (install body replacer separately)
- (install base hair mods separately)
- (install Salt and Wind retextures _with_ the base mod they modify)

user launch program:

- user is prompted the path to the Skyrim folder, if the folder is a protected
  folder, user is warned to run everything as administrator (or simply told to
  install Skyrim somewhere else)

- user is given the option to install SKSE; if user already has SKSE user may
  chooes not to do this step

- user is prompted to provide the archive of a Mod Organizer 2 standalone
  executable, as well as a folder to work in (work dir may be auto-created)

- program installs Mod Organizer 2
- program configures Mod Organizer 2
- program installs the list of mods with Mod Organizer 2
- program opens all mods with pyxedit to generate a list of NPCs affected
- program uses NpcFacebookTemplate.esp as a template to generate NpcFacebook.esp
- program packages NpcFacebook.esp together with the template files and the
  NPCs list as a mod
- the generated mod is in turn installed into Mod Organizer 2

- user is given the option to launch Skyrim via Mod Organizer 2; once in game,
  user is told to go to MCM menu for NPC Facebook and press the button there

- in-game, mod script will cycle through the list of NPCs read in from the
  file, and photoshoots each of them (properly framed against a nice backdrop -
  maybe somewhere in riverwood; timescale is forced to pass very slowly and
  weather is repeated forced to be 81a to ensure optimum lighting conditions)

- once complete, player is told to exit the game

- during the photoshoot session, a timestamp is logged at beginning and end to
  mark the duration of the session

- once outside of the game, user can click the button to retrieve images; this
  will inspect the screenshot output directory, retrieve the files based on the
  timestamp window, and then renames/processes the files based on NPC order

- the end 'facebook' folder can be incrementally updated with photoshoots from
  each mod

### Skyrim Builder (skyrim-builder)

A tool that attempts a 1-button install of skyrim modlists.

# Current Plan

1. develop pyxedit in conjunction with a npc stylizer script; needs of script dictates pyxedit high level API
2. develop the `npc-facebook.esp` plugin, where on a button push it will take photos of a list of NPCs provided via a text file
3. iterate with npc-stylizer, npc-facebook, and pyxedit until stylizer functionality is all working
4. publish pyxedit 0.1 privately (let ElMinister know about this)
5. officially begin npc-stylizer project to reuse code from the skyrim-builder framework
6. implement UI workflow for npc-stylizer
7. once npc-stylizer is ready for public, announce and publish npc-stylizer together with pyxedit 1.0
8. continue working towards skyrim-builder


# test section

```python
import foo

def whatever():
    foo.whatever
```