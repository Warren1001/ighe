# In-game Hero Editor for D2R

I tried my best to establish a pattern for cube recipes, here are the changes:
- Akara's Misc page has a lot of items for sale.
- Sell and buy values are drastically modified. Sell values are in the millions and buy values are close to 1.
- New characters start with a Cube in their inventory. If a brand new character does not start with a Cube, the mod is not installed correctly.
- Some vendors may sell different items than they usually do, I started work on changing what vendors sell a while back but didn't get too far and don't remember how much I've done.
- Added a bunch of cube recipes. All original cube recipes are untouched.
- Added 1 unique small charm with hacky stuff on it.
- You can teleport in town.

The unique small charm is obtained by cubing 1 stamina potion by itself. It gives three things:
- An Aura of Death. This Aura grants a massive amount of experience gained and instantly kills everything in a wide radius (a couple screens from you) every tick. It also makes you semi-immortal and grants a ton of movement speed and faster cast rate.
- Teleport. This is not the same Teleport that Sorceress has, though it functions the exact same way.
- Summon Diablo. This will literally summon Diablo on top of you. This is to streamline the rushing of a new character. This will be explained in more detail below.

The purpose of the charm is for rushing/quest completing. You must toss it on the ground if you plan to use the character outside of the mod. If you try to load a character that has the charm with the unmodded game or another mod, the game will crash on load (or it just won't let you load that character, don't remember which happens). You will hit level 99 by the time you finish Hell using the rushing method.

This mod contains status effect indicators for the Assassin's charge-up skills. They were made by Bonesy, taken from his D2RLaunch application (I edited the textures slightly and changed the order of the icons). Full credits to him:
- [D2R Modding Discord](https://discord.gg/gEshQt2dRT)
- [D2R Modding Website](https://www.d2rmodding.com)

If you do not want the status effect indicators, delete the `data/hd/overlays/` and `data/hd/vfx/` directories and their contents.

## How to Install
1. Download as a ZIP. If you don't know how to do this, click Code at the top left of the site. Above the descriptions for the files to the right, there is another green box that says Code. Click it and press Download ZIP.
2. Navigate to your D2R install.
3. Navigate to the mods folder. If you do not have one, just create one. Your path should be `{D2R base folder}\mods`.
4. Extract the contents of the ZIP file into the mods folder. If you've done it correctly, you should see a path similar to `{D2R base folder}\mods\ighe\...`.
5. Go to Battle.net and click the Gear Icon next to Play for D2R, then click Game Settings.
6. Tick the box that is labeled `Additional command line arguments`.
7. Paste the following into the text box that shows up: `-mod ighe -txt -enablerespec`. The `-enablerespec` option grants free respecs by Alt + Left Clicking on the stat point allocation buttons in the character screen. If you don't want this, just remove it. There is no way provided by the mod to easily acquire a Token of Absolution.

## How to Get a Character Started

Using an external hero editor makes this process much easier, but if you can't be bothered (some editors don't give you the proper stat values based on your character and level, so I just do it in-game), then there's a way to get to Hell and level 99 very quickly.
1. Go to Akara and sell one of your scrolls you start with. Buy something worth 1 gold. Sell that. Now you have infinite gold. Buy a Stamina Potion and an El Rune.
2. Cube the Stamina Potion by itself. This is the unique small charm. Read above for more information about it.
3. Cube the El Rune by itself. This will open a portal to Andariel. Walk in, walk out, she will die from the portal location, you don't need to get close to her.
4. Go to Act 2. Cube the Eld Rune by itself. Go in portal. Duriel is dead. Teleport to Tyrael. Go to town and talk to Jerhyn, Meshif, etc.
5. Go to Act 3. Cube the Tir Rune by itself. Go in portal. Count to three. Teleport on the Hell Gate and go through it.
6. Cube whatever rune is next by itself. Go in portal. Select the Summon Diablo skill. Cast it. Go back to town and talk to Tyrael.
7. Cube whatever rune is next by itself. Go in portal. Exit the game. Go to Nightmare and start from Step 3 again.

Once you get into Hell, you should be level 99. If you wanted to be a lower level, sucks to suck, just use an external hero editor.

Now you use a combination of Gambling, Akara, and the Horadric Cube to get everything you need.

## New Cube Recipes

For anything that is numerical, counting is done with runes. El Rune is 1. Eld Rune is 2. etc

To add a socket to an item, use the numerical equivalent rune for the number of sockets you want on the item. If the recipe doesn't work, that item can't have that many sockets. Check the item level if you think it should.
- Item + El Rune = Item with 1 Socket
- Item + Eld Rune = Item with 2 Sockets
- ...etc

In the event you have an item whose item level is too low for sockets or a specific rarity:
- Item + Hel Rune = Item with `item level = 99`

To change the rarity of an item, use the associated perfect gem color. Since there isn't a gold gem (Unique) and Normal and Superior items are both white:
- Item + Perfect Skull = Item with Normal Quality
- Item + Perfect Diamond = Item with Superior Quality
- Item + Perfect Sapphire = Item with Magic Quality
- ...etc
- Item + Perfect Amethyst = Item with Unique Quality

If you change an item quality to the same item quality it already has, this will effectively reroll the item.

To change the tier of an item, use a Perfect Ruby.
- Normal Item + Perfect Ruby = Exceptional Item
- Exceptional Item + Perfect Ruby = Elite Item

There is no way to downgrade, D2R doesn't seem to support this. If you need to go down a tier, you'll have to acquire that manually (I use Gambling).

To make an item ethereal:
- Item + Zod Rune = Ethereal Item

Cubing a Tome of Town Portal by itself will open the Cow Portal for convenience. The original recipe still exists.

### To acquire skiller Grand Charms:

The numerical order is based on the order of the skill tabs on the skill tree in-game. For example, Cold Spells is the first skill tab on the skill tree in-game for the Sorceress, so Cold Spells = 1. Lightning Spells = 2. etc
- Magic Grand Charm + numerical rune of the skill tree tab order = New Magic Grand Charm with Tab Skill.

Examples:
- As a Sorceress: Magic Grand Charm + El Rune = New Magic Grand Charm with +1 to Cold Skills
- As an Amazon: Magic Grand Charm + El Rune = New Magic Grand Charm with +1 to Javelin and Spear Skills

There is no way currently to easily roll crafted items. I plan to make the recipes refund the materials and allow you to use the crafted item to roll again, but I'm lazy.
There is no way to acquire specific Rare items or any other Magic items besides blindly rerolling. Consider using an external hero editor for this.
