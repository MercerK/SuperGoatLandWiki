# Lands

- **Wiki**: https://github.com/Angeschossen/Lands/wiki
- **Plugin**:
  https://www.spigotmc.org/resources/lands-land-claim-plugin-grief-prevention-protection-gui-management-nations-wars-1-16-support.53313/

Lands is a powerful claim plugin that provides a ton of customization, allowing users to claim large areas and define
subareas, all with unique roles and rules.

/land claim to claim chunk /land unclaim to unclaim chunk /land selection to select area. /land menu to open up menu to
see all claims. You can click on an option to further edit it. /land map to see chunks claimed around you. /land trust
or /lands untrust to provide permissions to player. /land invites to see invites. /land rename to rename.

There are three terminologies to know.

Lands, Chunks, and Areas.

A land is a container for chunks and areas. Chunk is the 16x256x16. Area is a player defined region within a land.

You can have one or multiple lands, housing many chunks. These chunks do not have to be connected, so in theory, you can
have one land, but many chunks all over. Within a land, you can define many areas (which can have unique roles and
permissions). For example, you want to make a public sheep farm, but want to protect certain blocks. You can setup an
area to allow certain blocks, but make the default disallow everything else to the visitor.

For those that do not have a land or want to create a new one, you can create a land by doing `/land create`. This
creates a brand new "land" and may claim the chunk you are on.

You can expand the land by using `/land selection` or a golden shovel. To edit an existing land, you will need to do
`/land edit {YOUR_LAND_HERE}`. Once you made a selection, you can do `/land selection assign {YOUR_LAND_HERE}`.

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
