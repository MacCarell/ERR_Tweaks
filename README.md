# Posture Bar Mod Config/Textures
Install [Elden Mod Loader](https://www.nexusmods.com/eldenring/mods/117?tab=files) into your `ELDEN RING/Game` folder, then drag and drop my `Game` folder into your `ELDEN RING` folder, overriding `mod_loader_config.ini`.
Make sure you are playing in Borderless Windowed mode, otherwise you will run into issues. It's generally better than fullscreen anyway.
  - All credit to Mordrog for the [Posture Bar Mod](https://www.nexusmods.com/eldenring/mods/3405/?tab=description)
    - Download it from Nexus and endorse so he gets those sweet donation points for cash.
  - I have included the `.xcf` files for use with GIMP if you want to edit them at all yourself.

# Functional Changes
## Latest update supported (1.2.1)
### DISCLAIMERS
- **!! Before replacing files, ensure I have updated this repo to the latest edition of Reforged.**
- **!! Keep backups. I fuck up on occasion.**
- **!! If you encounter issues, revert your files to the original Reforged files before seeking technical assistance or reporting bugs.**
- **!! Backup your saves! Say for instance you put a CGS-only ash of war on Forked Greatsword then update ERR and load the game without my tweaks. Not good, probably.**

## Basic
Drag and drop the `mod` folder into your Reforged folder, overwriting `regulation.bin` and other files.

#### Changes
- Increased Short Sword crit mult by 30
- Changed Forked Greatsword into a curved greatsword with thrusting heavy/crit attacks
- Reduced Warped Axe Light attack recovery to be more like vanilla
- (Not anymore) Made Inescapable Frenzy quicker and increased its distance


## Advanced (Requires Smithbox)
Use the following steps within Smithbox when importing each of the various files.
Smithbox changes are pretty much version independent.
For animation changes, just use the basic steps for c0000.anibnd.dcx (make sure versions up to date).

### Crit Damage Changes
- Go to Param Editor -> EquipParamWeapon
- Click *Data -> Import CSV -> Specific Field -> throwAtkRate* and paste in the text from throwAtkRate.csv
#### Changes
- Increased Short sword crit mult by 30

### Moveset Changes
- Go to Param Editor -> EquipParamWeapon
- Click *Data -> Import CSV -> All Fields and paste in the text from forked-greatsword.csv
#### Changes
- Changed Forked Greatsword into a curved greatsword with thrusting r2 attacks.

### Row Names
- Go to the Param Editor and then to the param category which matches a folder name
- Click *Data -> Import CSV -> Row Names* then paste in the text from that folder's row-names.csv file
#### Changes
- Named various status effect rows so they are easier to identify in Smithbox
- Imported community row names and trimmed up/edited a bit where necessary

### (Draft) Frenzy/Blight Bolts
- These share the same icon as the frenzy/blight arrows, and they are named "?weaponName?" because changing names involves more than just param work
- Go to Param Editor, then within the following param categories, click *Data -> Import CSV -> All Fields* then paste in the text from `New/frenzy-blight-bolts.csv` which should be in each folder named according to the param category. (e.g. `EquipMtrlSetParam/New/frenzy-blight-bolts.csv`)
  - EquipMtrlSetParam
    - The recipes to craft the bolts
  - EquipParamWeapon
    - The bolts themselves
  - ShopLineupParam_Recipe
    - The association from the crafting books to the recipes
