# Season 2: Goat Magic

During 1.19, we started work on a new feature called Goat Magic. This is a feature meant to bring in additional capabilities (inspired from many sources) onto the server, in order to provide a more unique experience.

This feature is still in development, however, we will be releasing a beta version to the server for players to enjoy. This will allow players to access the new content and provide feedback to help improve the experience. At the moment, this feature is behind netherite.

As it is in beta, there will be bugs and potentially major changes to this custom content. For example, we will be releasing tools to make building easier, which currently generate instant results. However, as we work on the feature more, we will begin to slow down how the building mechanic works, which will result in slower build times. Certain spells may be added or purged over time, depending on their state.

As new features are worked on, we may see it replace existing custom capabilities either in this MC Version or in the next major version. For example, we use commands to teleport home/spawn, and so forth. Eventually, these may be replaced by spells that perform the same functionality and add additional immersion. Having item-variants of commands was always an objective of mine, however, it is difficult to provide a command initially then replace it with an item, as players tend to get upset about this change. I'm hoping that this feature can be made available at the start of the season, versus later on.

Another aspect is documentation. We don't want to rely on a website for documentation, as we want to provide that in game. However, that has proven to be challenging and even time consuming. Overtime, we will aim to slowly bridge the gap. 

## Controls

We are limited on how we can intercept controls from the player. We cannot add support for additional keys or actions, like in modded.

In this document, you'll see references to `left click`, `right click`, and `shift right click`. This is implied that you are holding the item, looking at air or a block, and performing left or right click with that item. `shift` is your `sneak`. 

# Jeff

You'll need to find a goat named `Jeff`. Jeff has a low chance of spawning with a group of Goats. Once you find Jeff, this will start a mini-quest. At the conclusion of the quest, you'll get a `Magical Goat Horn`.

# Magical Goat Horn

This item does nothing by itself, however, it can be used to open up a portal.
## Crafting

<img src="/assets/items/magical-goat-horn-crafting.png" />

You'll need 8 essences with one goat horn. Surround the goat horn with the essence and you'll get a magical goat horn.

## Uses

You know the Ancient City that was released in 1.19 and there is a structure that looks like a portal. This item may just open up a portal.

# Essence

This item has a random chance of dropping.

## Consumable

You can consume this item to receive mana.

# Spellbook

This is a single tool that allows you to select and cast spells.

* **Note**: You need to craft a spellbook, in order to use a spellbook.
* **Note**: You'll need to identify and learn spells, to begin using magic. 

## Crafting

<img src="/assets/items/spellbook-crafting.png" />

You'll need 8 essence and 1 book. This will give you a spellbook.

* **Note**: This will change in the future.

## Controls

* Sneak - Right-click -> Open GUI
* Right-click -> Cast [Dependent on spell]
* Left-click -> Cast [Dependent on spell]

## Spells

There are currently 20 spells.

## Building Spells

Certain blocks may have certain colors. When it comes to building:

* Green outlines -> Buildable
* Red outlines -> Not enough resources or blocked.
* Yellow outlines -> Area is protected.

With building spells, you need to have resources on hand (with mana) to build. As you cast a building spell, you have the option of `rollback` as needed.

Not everything is supported, as this proven to be time-consuming and challenging.

* Blocks with "facing" do not rotate, such as observers, pistons, etc.
* Entities, such as item frames, are not included.
* Stairs do not change shapes.
* Water/Lava/Waterlogged are ignored.

### Extend

Inspired by Builder's wand. This will allow you to select a block and extend an area, similar to builder's wand.

To select a block, open the GUI, go to "Options", and click a block in your inventory. It should change the block inside the GUI to match.

From there, close the inventory and hover over a block. This should generate a preview. If you want to build there, you can do `right click`. 

### Copy

**Note**: This may see some changes in the future.

This is a spell paired with `Paste`. This allows you to select an area and save it. It is intentionally limited to one selection *per player*.

To select an area:
* Open GUI -> Make sure 'Spell Mode' is on 'Select'
* Left click to select position 1.
* Right click to select position 2.
* Open GUI -> Click on 'Spell Mode' to cycle modes until it is on 'Save'. Close GUI.
* Right click to save.

### Paste

**Note**: This requires a selection from `Copy`.

Once you have a selection, you can do the following:

* Left click to select an anchor. This will preview the selection at the new location.
* You can change rotation/flip by open GUI and going to the options.
* To paste, just Right Click.

### Rollback

**Note**: This is paired with any of the building spells.

You may want to undo certain operations. This spell stores the last 10 building operations (from the player) and gives you the ability to undo it.

To select a rollback:

* Open up the GUI -> Go to Options -> Select a rollback
* Right click to rollback.  

# Unidentified / Identified Spells

During your travels, you may encounter an 'Unidentified scroll'. When it is unidentified, you can "right click" to identify it. However, this will only work when you discover magic (by crafting a spellbook).

Once you identify a spell, you have the option of learning it (by right clicking again) or giving it away. 

## Mirror Dimension

The mirror dimension is a new, experimental world. This isn't your average world.

* Resets daily with a different seed.
* Infinitely monster scaling. Mobs will get harder, so fully enchanted armor will only last you so far. 
* New Loot
  * Majority of the new items being released will be done via the Mirror Dimension. 
* Always night time. There may be a way to set it to day though...
* Sleeping and flying are not recommended... You are welcome to try. Heh. 
* You cannot /sethome.
* If you die in the world, you won't be punished for it. You'll spawn at your bed (or spawn) with your stuff. However, you will be locked out for a period of time.
* Currently the world is heavily focused on Player vs Mobs. At the same time, we know that it isn't for everyone. We may introduce other methods within this world. 

This feature is still in development, so expect more content in the future. Having it reset daily gives us more opportunity to be more creative in what we can do here and it does allow content/loot to reset. 

