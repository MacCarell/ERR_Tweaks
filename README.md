# Within Smithbox
Use the following steps within Smithbox when importing each of the various files

## Row Names
- Go to the Param Editor and then to the param category which matches a folder name
- Click *Data -> Import CSV -> Row Names* then paste in the text from that folder's row-names.csv file
#### Changes
- Named various status effect rows so they are easier to identify in Smithbox
- Imported community row names and trimmed up/edited a bit where necessary

## Crit Damage Changes
- Go to Param Editor -> EquipParamWeapon
- Click *Data -> Import CSV -> Specific Field -> throwAtkRate* and paste in the text from throwAtkRate.csv
#### Changes
- Increased Short sword crit mult by 30

## Moveset Changes
- Go to Param Editor -> EquipParamWeapon
- Click *Data -> Import CSV -> All Fields -> wepmotionCategory* and paste in the text from forked-greatsword.csv
#### Changes
- Changed Forked Greatsword into a curved greatsword with thrusting r2 attacks

## Frenzy/Blight Bolts
- These share the same icon as the frenzy/blight arrows, and they are named "?weaponName?" because changing names involves more than just param work
- Go to Param Editor, then within the following param categories, click *Data -> Import CSV -> All Fields* then paste in the text from `New/frenzy-blight-bolts.csv` which should be in each folder named according to the param category. (e.g. `EquipMtrlSetParam/New/frenzy-blight-bolts.csv`)
  - EquipMtrlSetParam
    - The recipes to craft the bolts
  - EquipParamWeapon
    - The bolts themselves
  - ShopLineupParam_Recipe
    - The association from the crafting books to the recipes
