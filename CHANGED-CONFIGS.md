# Changed Configs (W.I.P.)

This is a condensed overview of which configs have been adjusted, how, and in cases where relevant, why.

Simplemenu, bisecthosting, simple rcp and Keybindings

# Options

# Mods

## bclib
bclib can be used to sync config differences between client and server, which is not always preferable. As an example, if you disable the thick fog effects for BetterNether, but the server has it enabled, bclib will undo that client-side change if you agree to sync. If you want to enforce a particular experience, you can of course adjust the server-related settings to your liking.

### *(config/defaultoptions/extra/config/config/bclib/client.json)*
- "didShowWelcome [default: false]": true,
- "check [default: true]": false
- "showUpdateInfo [default: true]": false,

### *(config/defaultoptions/extra/config/config/bclib/server.json)*
- "enabled [default: true]": false,

## Inventory Profiles Next
IPN can be helpful when it comes to a multitude of inventory management tasks, such as auto-replacing blocks in your hotbar when your stack runs out. Normally there is a GUI button below the inventory, but it has been disabled to reduce clutter, and reduce the chance of UI overlap. Armor and tools with durability will not warn you when they are about to break, nor be auto-replaced. The experience has been, that getting spammed with durability messages in the mid-to-late game is more annoying than it is useful. Once Mending is acquired, this feature is just too intrusive. A few hotkey features were removed related to moving items between inventories with the scroll wheel, as you tend to keep doing it by accident, wondering where your stuff went. The hotkey for sorting your inventory was changed to the middle mouse button, as pressing "R" on an item will trigger REI or similar to open the crafting recipes instead.

### *(config/defaultoptions/extra/config/config/inventoryprofilesnext/inventoryprofiles.json)*
"ModSettings":
- "first_run": false

"GuiSettings": {
- "enable_profiles_ui": "value": false
- "continuous_crafting_saved_value": false

"LockedSlotsSettings": {
- "locked_slots_empty_hotbar_as_semi_locked": "value": false

"AutoRefillSettings": {
- "refill_armor": "value": false
- "refill_before_tool_break": "value": false
- "visual_durability_notification": "value": false
- "audio_durability_notification": "value": false
- "visual_replace_success_notification": "value": false
- "audio_replace_success_notification": "value": false
- "visual_replace_failed_notification": "value": false
- "audio_replace_failed_notification": "value": false

"ScrollSettings": {
- "scroll_full_stack": "main": "keys": ""
- "scroll_leave_last": "main": "keys": ""
- "scroll_spread": "main": "keys": ""
- "scroll_throw": "main": "keys": ""

"Hotkeys":
- "sort_inventory": "main": "keys": "BUTTON_3"
- "scroll_to_chest": "main": "keys": ""
- "scroll_to_inventory": "main": "keys": ""

## jade
Configured the Jade overlay to be transparent and located in the top left. The intention is to make it less intrusive to the visual space.

### *(config/defaultoptions/extra/config/config/jade/jade.json)*

## Roughly Enough Items
REI has been configured to provide a better overview of what you can make, but also to improve performance and load times.

### *(config/defaultoptions/extra/config/config/roughlyenoughitems/collapsible.json5)*
- A ton of collapsible entries for the various blocks and items. 18000+ lines of text, so it is "easier" to just check the categories ingame instead.

### *(config/defaultoptions/extra/config/config/roughlyenoughitems/config.json5)*
- A few adjustments to sorting method, appearance and performance.

## Simply Swords
The weapons provided in this mod are already quite powerful. As a slight balancing measure, the gem sockets on unique weapons have been disabled, as they already have unique effects.

### *(config/defaultoptions/extra/config/config/simplyswords_main/general.json5)*
- "enableUniqueGemSockets": false

## Let's Do Vinery
Infinite bone meal is just a bit too overpowered, and circumvents reasons to make midgame farms that produce bone meal.

### *(config/defaultoptions/extra/config/vinery/config.json5)*
- "enable_wine_maker_set_bonus": false,

## Alex's Mobs
Just craft the book if you want it, reduces clutter for new players and makes the start just that bit less confusing.

### *(config/defaultoptions/extra/config/alexsmobs.toml)*
- giveBookOnStartup = false

## Betterf3
Modules have been reduced a bit to avoid clutter from overwhelming information that the average player is unlikely to use.

### *(config/defaultoptions/extra/config/betterf3.json)*

## Copycats+
Some Copycats have been disabled in order to keep the available selection more clean and closer to what is already present in either vanilla or other mods. The level of fidelity provided by e.g. Chisels and Bits was outside the scope of this pack in the first place, and is probably not well suited for a persistent server in terms of stability and performance anyway.

### *(config/defaultoptions/extra/config/copycats-common.toml)*
- copycat_board = false
- copycat_byte = false
- copycat_ghost_block = false
- copycat_half_layer = false
- copycat_half_panel = false
- copycat_layer = false
- copycat_slice = false
- copycat_slope_layer = false
- copycat_vertical_slice = false

## Create Connected
Create Connected includes a selection of copycat blocks from before the various modders behind Copycats+ collaborated on merging their additions. These copycats have naturally been disabled due to them already being present elsewhere.

### *(config/defaultoptions/extra/config/create_connected-common.toml)*
- copycat_beam = false
- copycat_block = false
- copycat_board = false
- copycat_fence = false
- copycat_fence_gate = false
- copycat_slab = false
- copycat_stairs = false
- copycat_vertical_step = false
- copycat_wall = false

## Deathbackup
Disabled the chat message, as there is no need for the reminder.

### *(config/defaultoptions/extra/config/deathbackup.json5)*
- "sendBackupReminderMessageToThoseWithAccessOnDeath": false

## Doubledoors
Disabled opening of multiple fence gates and trapdoors, as they are commonly used as part of decorative builds, in cases where opening multiple trapdoors for instance, would be really annoying when building.

### *(config/defaultoptions/extra/config/doubledoors.json5)*
- "enableFenceGates": false
- "enableTrapdoors": false

## Everycomp
Disabled generation of wood types for Building But Better's layer blocks, as they have been disabled entirely (similar reasons to Copycats+ changes).

### *(config/defaultoptions/extra/config/everycomp-entries.toml)*
[entries.wood_type.bbb]
- layer = false

## Freecam
Freecam is just really good when building on a larger scale. Being unable to pass through solid blocks just makes it kinda useless or annoying to use. If people want to use x-ray cheating methods for mining, then that is their choice.

### *(config/defaultoptions/extra/config/freecam.toml)*
- "Ignore All Collision" = true

## Icarus
Changes were made so that Icarus wings are mainly cosmetic, and on parity with normal Elytra wings. Only difference is that you can do loops with Icarus wings. This makes the wings better balanced with the ones added from other mods.

### *(config/defaultoptions/extra/config/icarus.jsonc)*
- "armor_slows": false
- "wings_speed": 0.0
- "wings_durability": 432
- "required_food_amount": 0.0
- "max_height_enabled": false

## Item Obliterator
Can be used to prevent players from acquiring specific items or blocks that are troublesome by deleting them when they are picked up. Very useful in cases where there is no other way to prevent those items/blocks fram spwaning outright. I think we can all agree that having a mob spawner produce Ender Dragons is probably a bad idea.

### *(config/defaultoptions/extra/config/item_obliterator.json5)*
"blacklisted_items":
- "minecraft:wither_spawn_egg"
- "minecraft:ender_dragon_spawn_egg"
- "minecraft:warden_spawn_egg"
- "alexsmobs:spawn_egg_warped_mosco"
- "alexsmobs:spawn_egg_cachalot_whale"
- "alexsmobs:spawn_egg_void_worm"
- "alexsmobs:spawn_egg_laviathan"
- "alexsmobs:spawn_egg_bunfungus"
- "alexsmobs:spawn_egg_farseer"
- "deeperdarker:shriek_worm_spawn_egg"
- "deeperdarker:stalker_spawn_egg"
- "enlightend:void_laviathan_spawn_egg"

## Kiwi

## Lighty

## Mini Effects

## More Culling

## Mouse Tweaks

## Packedup

## Servercore

## Small Ships

## Enhanced Mob Spawners

## Supplementaries

## Wilder Nature

## Xaero's Minimap

## Xaero's Worldmap


































