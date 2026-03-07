# In-game Hero Editor for D2R

The purpose of this mod is to have an in-game testing tool that is significantly more convenient for item generation than an external hero editor. It remains as close to unmodded as possible, modifying nothing existing, and only adding new mechanics. With that said, some things have to be altered to make features of this mod possible:
- All monsters are capable of dropping Latent Sunders if a grand charm rolls unique.
- Items not usually sold by Akara added by this mod may display weirdly in the vendor screen and after buying them, but they should work all the same.

It is important to note that items found naturally while playing with this mod will still contribute to your Chronicle. You won't get banned if you accidentally log into online with the mod, but several things won't work correctly and give you errors, such as vendoring.

I tried my best to establish a pattern for cube recipes, here are the changes:
- Akara's Misc page has a lot of items for sale.
- Sell and buy values are drastically modified. Sell values are in the millions and buy values are close to 1.
- New characters start with a Cube in their inventory. If a brand new character does not start with a Cube, the mod is not installed correctly.
- Some vendors may sell different items than they usually do, I started work on changing what vendors sell a while back but didn't get too far and don't remember how much I've done.
- Made all item bases gamble-able.
- Added a bunch of cube recipes. All original cube recipes are untouched.
- Added 2 unique small charms with hacky stuff on it for rushing and testing purposes.
- You can use the Teleport clone skill provided by the two cheat charms to teleport in town and in Duriel's Chamber.
- You can carry as many unique charms without any restrictions.
- Unique items can drop an unlimited amount of times per game instead of the usual limit of 1.
- ~~Unique, set, runeword, and crafted (only the crafted modifiers) items all roll perfectly.~~ Removed, I will make a separate mod for this in the future.
- ~~Superior affixes all roll perfectly.~~
  - ~~Automods and affixes on magic, rare, and crafted (except for the crafted modifiers) items do not roll perfectly at the moment.~~

New items:
- **Cheat Item - Death**:
  - Obtained by crafting a stamina potion by itself.
  - An Aura of Death while equipped, granting a massive amount of experience gained, debuffs all enemies forcing them to -100 Magic Resistance and applies 100,000 magic damage to everything within 40 yards (~1 screen) every tick, and grants a ton of movement speed and faster cast rate. Game crashes on Mephisto if I set the range any higher.
  - Teleport Clone. This is not the same Teleport that Sorceress has, though it functions the exact same way.
  - Summon Diablo. This will literally summon Diablo on top of you. This is to streamline the rushing of a new character. This will be explained in more detail below.
- **Cheat Item - Immortality**:
  - Obtained by crafting an antidote potion by itself.
  - An Aura of Immortality while equipped, granting psuedo immortality (extremely high life regeneration every tick, immediately clearing poison damage, 100,000 damage reduction and magic damage reduction, and 500% Poison Resist). I'm not yet sure how to make someone fully immune to poison damage as it ignores damage reduction.
  - Teleport Clone. This is not the same Teleport that Sorceress has, though it functions the exact same way.

These two items **must** be dropped before uninstalling/unloading the mod or else your unmodded game will crash while loading.

The purpose of the Death charm is for rushing/quest completing. You will hit level 99 by the time you finish Hell using the rushing method. Please note that "loading a character" means launching the game, as all characters are loaded when the game launches. So your game will crash on load if it tries to load the hacky charm without the mod.
The purpose of the Immortality charm is for testing purposes. The aura will share with allied units within 50 yeards (2 screens).

## How to Install
1. [Download the ZIP](https://github.com/Warren1001/ighe/archive/refs/heads/main.zip).
2. Navigate to your D2R install.
3. Navigate to the mods folder. If you do not have one, just create one. Your path should be `{D2R base folder}\mods`.
4. Extract the `ighe` folder inside the `ighe-main` folder from the ZIP file into the mods folder. If you've done it correctly, you should see a path similar to `{D2R base folder}\mods\ighe\ighe.mpq\...`. You do not need the rest of the files.
5. Go to Battle.net and click the Gear Icon next to Play for D2R, then click Game Settings.
6. Tick the box that is labeled `Additional command line arguments`.
7. Paste the following into the text box that shows up: `-mod ighe -txt -enablerespec`. The `-enablerespec` option grants free respecs by Alt + Left Clicking on the stat point allocation buttons in the character screen (only if you've allocated points to that stat). If you don't want this, just remove it.
8. When updating this mod, **do not** drag and drop the mod files and replace the old ones. Delete the old mod folder entirely before installing a new version.

## How to Get a Character Started

Using an external hero editor makes this process much easier, but if you can't be bothered (some editors don't give you the proper stat values based on your character and level, so I just do it in-game), then there's a way to get to Hell and level 99 very quickly.
1. Go to Akara and sell one of your scrolls you start with. Buy something worth 1 gold. Sell that. Now you have infinite gold. Buy a Stamina Potion, Antidote Potion, and an El Rune.
2. Cube the Stamina Potion by itself. This is the Death charm. Cube the Antidote potion by itself. This is the Immortality charm. Read above for more information about these charms.
3. Cube the El Rune by itself. This will open a portal to Andariel. Teleport near her, then teleport back to the portal and go back to town.
4. Go to Act 2. Cube the Eld Rune by itself. Go in portal. Duriel is dead. Teleport to Tyrael (you can teleport through the walls with this mod). Go to town and talk to Jerhyn, Meshif, etc.
5. Go to Act 3. Cube the Tir Rune by itself. Go in portal. Walk closer to Mephisto until he's dead then go through the Hell Gate.
6. Cube the Nef Rune by itself. Go in portal. Select the Summon Diablo skill. Cast it. Go back to town and talk to Tyrael.
7. Cube the Eth Rune by itself. Go in portal. Exit the game. Go to Nightmare and start from Step 3 again.

Once you get into Hell, you should be level 99. If you wanted to be a lower level, sucks to suck, just use an external hero editor.

Now you use a combination of Gambling, Akara, and the Horadric Cube to get everything you need.

## New Cube Recipes

For anything that is numerical, counting is done with runes. El Rune is 1. Eld Rune is 2. etc

To add a socket to an unsocketed item, use the numerical equivalent rune for the number of sockets you want on the item. If the recipe doesn't work, that item can't have that many sockets. Check the item level if you think it should. Items that are already socketed cannot have their socket count modified.
- Item + El Rune = Item with 1 Socket
- Item + Eld Rune = Item with 2 Sockets
- ...etc

In the event you have an item whose item level is too low for sockets or a specific rarity:
- Item + Hel Rune = Item with `item level = 99`

If you want to remove the sockets of an item without destroying them:
- Socketed Item + Hel Rune + Scroll of Identify = Open Socketed Item + Socket Items

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
- As a Warlock: Magic Grand Charm + Tir Rune = New Magic Grand Charm with +1 to Demon Skills

### Sunder Charms

New recipes are the original recipes without the shards needed.
The materials will be refunded allowing you to craft again.
A Renewed Sunder charm can be used to craft itself again using the same ingredients as the Latent recipe.
Additionally, once you have a Renewed Sunder charm, you can also use the Unique recipe (Perfect Amethyst) to reroll into any Renewed Sunder charm.

### Colossal Jewels

Akara sells two jewels. The one closest to the runes is the normal jewel. The other one is the colossal jewel base. You can craft Colossal Jewels using the Unique recipe (Perfect Amethyst) with the colossal jewel base.

### Other

For Crafted items, the recipe is the same however you only need the rune and a Scroll of Identify. The gem and the jewel are no longer needed. The recipe will return the rune and scroll for you to craft again.
Additionally, you can use crafted items to re-roll the craft, so you don't need to keep getting magic items.
Lastly, the item level of the crafted item is always the item level of the original item. The item level will never change. Character level no longer matters.
The original crafting recipes still exist.

There is no way to acquire specific Rare items or any other Magic items besides blindly rerolling. Consider using an external hero editor for this.
