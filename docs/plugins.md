# Plugins

Super GoatLand uses plugins to enhance and improve the survival multiplayer experience. These are some of the key ones
to be aware of:

- Blocklocker. Allows the player to protect chests/doors with a sign.
- Death Chests. When you die, your items go into a death chest. This is locked to you and no one else.
- Dynmap. A web interface of the currently explored world: https://map.supergoat.land.
- Essentials. Provides 1 home. This is the only source of command teleportation.
- Lands. Players can claim their land. This is completely optional, as our community does not grief/steal.
- Harbor. A balanced mechanism to support multiple players sleeping, instead of the entire server.
- Mythical Trinkets. Custom items.
- Portals. Allows us to setup waypoints between fixed locations.

## Advanced Armor Stands

### Description

Stand next to an armor stand and type `/aa` into chat to open up the advanced armor stand options.

### More Info

- **Plugin**: https://www.spigotmc.org/resources/advanced-armor-stands.38513/

## Autorank

### Description

Our rank plugin!

### More Info

- `/ar check` provides your playtime & current progress
- `/ar leaderboard` shows top 5

## Deathchests

### Description

When you die, your items go into a chest!

### More Info

- You can see your deathchests by running `/dc list`.
- You can only have 10 death chests. Make sure to go through and clear out old death chests. A death chest will only
  last for an hour until it expires. After an hour, items will drop.
- There is a known bug where a "death chest" would get destroyed. Don't worry. You can try placing a chest where it may
  of been destroyed and it may restore it. If that does not work, reach out to a staff member.

## Essentials

### Description

Provides a bunch of helper capabilities.

### Trade Signs

You can use essential signs for trading.

<img src="/assets/essentials/tradesign.png">

### More Info

- You can set home and teleport to a home. You can only have one home.
  - `/sethome`: sets home
  - `/home`: teleports home
- `/spawn`: teleports to spawn
- Wiki: https://wiki.mc-ess.net/wiki

## Lands

### Description

Lands is a powerful claim plugin that provides a ton of customization, allowing users to claim large areas and define
subareas, all with unique roles and rules.

### Context

There are three terminologies to know.

Lands, Chunks, and Areas.

A land is a container for chunks and areas. Chunk is the 16x256x16. Area is a player defined region within a land.

You can have one or multiple lands, housing many chunks. These chunks do not have to be connected, so in theory, you can
have one land, but many chunks all over. Within a land, you can define many areas (which can have unique roles and
permissions). For example, you want to make a public sheep farm, but want to protect certain blocks. You can setup an
area to allow certain blocks, but make the default disallow everything else to the visitor.

For those that do not have a land or want to create a new one, you can create a land by doing `/land create`. This
creates a brand new "land" and may claim the chunk you are on.

### Commands

- `/land create` to create a new container.
- `/land edit` to select a container to edit.
- `/land edit here` to select the container you are currently standing in.
- `/land claim` to claim chunk; this will be added to the current container selected.
- `/land unclaim` to unclaim chunk
- `/land selection` to select area.
- `/land menu` to open up menu to see all claims. You can click on an option to further edit it.
- `/land map` to see chunks claimed around you.
- `/land trust` or `/lands untrust` to provide permissions to player.
- `/land invites` to see invites.
- `/land rename` to rename.
- You can expand the land by using `/land selection` or a golden shovel. To edit an existing land, you will need to do
  `/land edit {YOUR_LAND_HERE}`. Once you made a selection, you can do `/land selection assign {YOUR_LAND_HERE}`.
- `/wild` teleports to wild.

### More Info

- **Wiki**: https://github.com/Angeschossen/Lands/wiki
- **Plugin**:
  https://www.spigotmc.org/resources/lands-land-claim-plugin-grief-prevention-protection-gui-management-nations-wars-1-16-support.53313/

### Update Roles

You can update the permissions for roles within the land and/or area.

- `/land edit {YOUR_LAND_HERE}` OR `/lands menu` -> Select land
- Go to `roles`.
- Click the target role.
- Add or deny any permissions for that role.

Roles, at the lands level, applies to the primary lands area and any newly created areas. However, existing areas within
a "land" won't get updated. You'll need to update those manually.

### Protect specific areas

You can protect areas in the nether (like on the nether roof) and other areas, with minimal impact to other players now.

1. Create a land, as normal, and add the selection to your land.
2. `/lands menu` -> Select land -> Select Areas -> Create new area (pick a name)
3. Make sure to do `/land edit YOUR_LAND_HERE`
4. Then use a golden shovel and select the entire area (make sure to include height as needed or it won't work
   correctly)
5. And then you `/selection assign NAME_OF_AREA`
6. Once you assign the selection to the area, go to Land GUI and modify the "Default" area under areas, and edit
   "Visitor". Modify actions and ensure all actions are enabled. This allows visitors to break/place blocks everywhere
   (outside of subareas) as needed.
7. Go to the `NAME_OF_AREA` area, and modify visitor to disable all actions (or what you don't want them to have)

If you do it right, players will still be able to access the nether underneath your area and you'll be able to protect
your area as needed.

## Shopkeeper

### Description

Players can buy a shopkeeper, which allows for item trading.

### More Info

- **Wiki**: https://github.com/Shopkeepers/Shopkeepers-Wiki/wiki/Creating-Shops
- **Plugin**: https://www.spigotmc.org/resources/shopkeepers.80756/

You can open up a player shop by buying a Shopkeeper at spawn (3 diamonds). There are a few items to note before you put
one down.

- You'll most likely want to change the shop type. To do so, you'll need to hold the egg in your hand and left click the
  air (look up). This cycles the shop type. I recommend "Trade shop" to allow trading of items. "Buy shop" allows you to
  buy items, sell shop allows you to sell items for emeralds.

- Once you selected a shop, you'll want to put down a chest (this is the inventory), select the chest by
  SNEAK-RIGHT_CLICK on the chest, and then SNEAK-RIGHT_CLICK on a block. This will place a shopkeeper and associate it
  to the chest.

- You'll need to put items in the chest first (what you want to sell/buy/trade). You can then SNEAK-RIGHT_CLICK on the
  villager to edit the prices and customizations of the villager. To set a price in a "Trade Shop", drag an item to
  first (or second) "slot" beneath the item.

- Once you do all that, you should be able to see the trades.

- If you delete the shopkeeper, you lose the egg altogether (intentional), so please place the shopkeeper in a location
  you'll want to use. As it is a new plugin, an admin or staff member can help out. We don't want to make it a
  punishment due to a lack of understanding, however, we want to provide a currency dump in the server.

https://dev.bukkit.org/projects/shopkeepers https://www.youtube.com/watch?v=t51LIXbf7Bs
