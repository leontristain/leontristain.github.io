## Current Projects

### pyxedit (pyxedit)

A python wrapper to xedit

### NPC Stylizer (npc-stylizer)

A tool that allows users to pick and choose which npc is to be replaced by which
npc replacer mod.

Mods to support:
* Seranaholic
* Valerica
* The Ordinary Women
* The Men of Winter
* Pandorable's NPCs
* Pandorable's NPCs - Dawnguard
* Realistic Faces
* Improved Bards
* Fresh Faces
* Botox For Skyrim
* Metalsabers Beautiful Ladies of Skyrim
* Distinct People
* Inhabitants of Skyrim
* Bijin AIO
* Metalsabers Beautiful Orcs of Skyrim
* Migal's Hearthfires Bards
* Followers Hirelings and Housecarls
* Distinct Husbands
* Metalsabers Beautiful Vampires of Skyrim
* Massive NPC Facelift Overhaul
* Diversity - An NPC Overhaul
* WICO - Windsong Immersive Character Overhaul
* People - Cathedral Concept
* Total Character Makeover

### NPC Facebook (npc-facebook)

**Script To Generate FormList**

 - download and unpack all above mods
 - take input all the mod folders
 - find all below files across all mod folders and collect form ids:
    data/meshes/actors/character/FaceGenData/FaceGeom/*/(form_id).nif
    data/textures/actors/character/FaceGenData/FaceTint/*/(form_id).dds
 - in pyxedit, open up NpcFacebookBase.esp
 - copy all records to a new NpcFacebook.esp
 - in NpcFacebook.esp, empty formlist
 - in NpcFacebook.esp, add the overall set of form ids to formlist
 - save NpcFacebook.esp to a new mod and copy over scripts
 - and we're done!

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