# Simple repository to explain datapack changes (for VS2)

Just making this repo to showcase how you, a mod pack author, can make some datapacks that change how existing mods work.

## Function

The root of this is `datapack`, essentially that folder is a functioning 1.20.1 datapack which can be zipped up (and is zipped up as `vs2weightchange.zip`). The base of the folder needs a `pack.mcmeta`, and the `pack_format` in that pack needs to be roughly equivalent to what version minecraft you're playing on.

[Check the pack format here](https://minecraft.wiki/w/Data_pack#Pack_format)

For 1.20.1 this is `15`

## What to change

Go to `datapack/data/valkyrienskies/vs_mass` and edit `datapack_mass_changes.json`. Add as many entries as you like. The mass seems to be multiplied by 10, so 10 = 100, 20 = 200, 200 = 2000 etc.

Once you're done, zip up the `datapack` folder, and it's now a `datapack.zip`. Check the `datapack.zip` included in this repo for an example of the file structure

## Where to put it

By default, these packs need to go into a world's datapack folder. You can find this here;

`(pack_root)/saves/(world_name)/datapacks/`

Alternatively you can add this great mod: https://www.curseforge.com/minecraft/mc-mods/drp-global-datapack and put it into `(pack_root)/resourcepacks` and it'll propogate out to all new saves

## Structure

I found out the structure from going to the VS2 github, this folder here: https://github.com/ValkyrienSkies/Valkyrien-Skies-2/tree/1.18.x/main/common/src/main/resources/data/valkyrienskies/vs_mass

