# Changed Configs

This is a condensed overview of which configs have been adjusted, how, and in cases where relevant, why. Given the complex nature of modpack configuration, an attempt has been made to document as much as possible, but in some cases, some changes might slip through the cracks.

Default config files related to the visual representation of the modpack main menu and similar modpack-specific features is not documented here, as they do not impact game or server performance/gameplay etc..

NB: Pay attention to the distinction between "defaultoptions" and "defaultconfigs":

- defaultoptions: Refers to the folder located at \config\defaultoptions - and contains various configs that have been altered, and will only replace the default configs provided by mods, as long as there is no config file to be found.
- defaultconfigs: Refers to the folder defaultconfigs located alongisde the "mods" and "config" folder - and contains world-specific config files, which are applied into the saves/"worldname"/serverconfig/ folder. The defaultconfigs will not override any files that are already present, so if this modpack is updated, make sure to consider overwriting them manually.

<div align="center">

# Options
</div>
To provide an easier install and play experience, some default options, including keybinds, have been changed. A list of the more regularly useful keybinds will be listed here.

### *(config/defaultoptions/keybindings.txt)*
- Various keybind defaults were changed to avoid overlap and move more frequently used shortcuts closer to "WASD".
- Some keybinds were completely disabled to make room for others.

### *(config/defaultoptions/options.txt)*

<div align="center">

# Mods - "defaultoptions"
</div>

<div align="center">

## <center>Bclib</center>
</div>

bclib can be used to sync config differences between client and server, which is not always preferable. As an example, if you disable the thick fog effects for BetterNether, but the server has it enabled, bclib will undo that client-side change if you agree to sync. If you want to enforce a particular experience, you can of course adjust the server-related settings to your liking.

### *(config/defaultoptions/extra/config/config/bclib/client.json)*
- "didShowWelcome [default: false]": true,
- "check [default: true]": false
- "showUpdateInfo [default: true]": false,

### *(config/defaultoptions/extra/config/config/bclib/server.json)*
- "enabled [default: true]": false,

<div align="center">

## Inventory Profiles Next
</div>
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

<div align="center">

## Jade
</div>
Configured the Jade overlay to be transparent and located in the top left. The intention is to make it less intrusive to the visual space.

### *(config/defaultoptions/extra/config/config/jade/jade.json)*

<div align="center">

## Roughly Enough Items
</div>
REI has been configured to provide a better overview of what you can make, but also to improve performance and load times.

### *(config/defaultoptions/extra/config/config/roughlyenoughitems/collapsible.json5)*
- A ton of collapsible entries for the various blocks and items. 18000+ lines of text, so it is "easier" to just check the categories ingame instead.

### *(config/defaultoptions/extra/config/config/roughlyenoughitems/config.json5)*
- A few adjustments to sorting method, appearance and performance.

<div align="center">

## Simply Swords
</div>
The weapons provided in this mod are already quite powerful. As a slight balancing measure, the gem sockets on unique weapons have been disabled, as they already have unique effects.

### *(config/defaultoptions/extra/config/config/simplyswords_main/general.json5)*
- "enableUniqueGemSockets": false

<div align="center">

## Let's Do Vinery
</div>
Infinite bone meal is just a bit too overpowered, and circumvents reasons to make midgame farms that produce bone meal.

### *(config/defaultoptions/extra/config/vinery/config.json5)*
- "enable_wine_maker_set_bonus": false,

<div align="center">

## Alex's Mobs
</div>
Just craft the book if you want it, reduces clutter for new players and makes the start just that bit less confusing.

### *(config/defaultoptions/extra/config/alexsmobs.toml)*
- giveBookOnStartup = false

<div align="center">

## Betterf3
</div>
Modules have been reduced a bit to avoid clutter from overwhelming information that the average player is unlikely to use.

### *(config/defaultoptions/extra/config/betterf3.json)*

<div align="center">

## Copycats+
</div>
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

<div align="center">

## Create Connected
</div>
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

<div align="center">

## Deathbackup
</div>
Disabled the chat message, as there is no need for the reminder.

### *(config/defaultoptions/extra/config/deathbackup.json5)*
- "sendBackupReminderMessageToThoseWithAccessOnDeath": false

<div align="center">

## Doubledoors
</div>
Disabled opening of multiple fence gates and trapdoors, as they are commonly used as part of decorative builds, in cases where opening multiple trapdoors for instance, would be really annoying when building.

### *(config/defaultoptions/extra/config/doubledoors.json5)*
- "enableFenceGates": false
- "enableTrapdoors": false

<div align="center">

## Everycomp
</div>
Disabled generation of wood types for Building But Better's layer blocks, as they have been disabled entirely (similar reasons to Copycats+ changes).

### *(config/defaultoptions/extra/config/everycomp-entries.toml)*
[entries.wood_type.bbb]
- layer = false

<div align="center">

## Freecam
</div>
Freecam is just really good when building on a larger scale. Being unable to pass through solid blocks just makes it kinda useless or annoying to use. If people want to use x-ray cheating methods for mining, then that is their choice.

### *(config/defaultoptions/extra/config/freecam.toml)*
- "Ignore All Collision" = true

<div align="center">

## Icarus
</div>
Changes were made so that Icarus wings are mainly cosmetic, and on parity with normal Elytra wings. Only difference is that you can do loops with Icarus wings. This makes the wings better balanced with the ones added from other mods.

### *(config/defaultoptions/extra/config/icarus.jsonc)*
- "armor_slows": false
- "wings_speed": 0.0
- "wings_durability": 432
- "required_food_amount": 0.0
- "max_height_enabled": false

<div align="center">

## Item Obliterator
</div>
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

<div align="center">

## Kiwi
</div>

### *(config/defaultoptions/extra/config/kiwi-client.yaml)*
- tagsTooltip: false
- debugTooltipMsg: false
- NBTTooltip: false

<div align="center">

## Mouse Tweaks
</div>
Disabling the wheel tweak, which otherwise will move inventory items back and forth between chests when scrolling with the mousewheel. This functinality is also present in Inventory Profiles Next, which is also disabled.

### *(config/defaultoptions/extra/config/MouseTweaks.cfg)*
- WheelTweak=0

<div align="center">

## Packedup
</div>
Lots of changes were made to make backpacks balanced, and more convenient to use in end-game, such as making them bigger, allowing nested storage 1 layer deep, and preventing fire from destroying them. For clarity sake, an -> is used to indicate if a value was changed, and all backpacks are listed.

### *(config/defaultoptions/extra/config/packedup-common.toml)*
- maxBagInBagLayer = 1
- canBackpacksBurn = false

[Backpacks.Basic]
- basicRows = 3
- basicColumns = 9 -> 4

[Backpacks.Iron]
- ironRows = 4
- ironColumns = 9

[Backpacks.Copper]
- copperRows = 4
- copperColumns = 9

[Backpacks.Silver]
- silverRows = 5
- silverColumns = 9

[Backpacks.Gold]
- goldRows = 5
- goldColumns = 9

[Backpacks.Diamond]
- diamondRows = 7
- diamondColumns = 9

[Backpacks.Obsidian]
- obsidianRows = 8 -> 9
- obsidianColumns = 9 -> 13

<div align="center">

## Servercore
</div>
Enabled a few extra optimizations that are non-intrusive. The spawn chunks in vanilla are normally always loaded, so disabiling those being loaded can save a bit of performance stress. Villagers in a 1x1 block area will not tick as often and mobs spawning around biome transition areas is a bit more optimized.

### *(config/defaultoptions/extra/config/servercore/config.yml)*
- disable_spawn_chunks = true
- lobotomize_villagers = true

### *(config/defaultoptions/extra/config/servercore/optimizations.yml)*
- fast-biome-lookups: true

<div align="center">

## Small Ships
</div>
Small Ships was slightly adjusted to remove collision damage from sailing into stuff, and also removing the block destruction of cannonballs.

### *(config/defaultoptions/extra/config/smallships-common.toml)*
- shipGeneralCollisionDamage = 0
- shipGeneralCannonDestruction = 0.0

<div align="center">

## TPA++
</div>
Some default settings were changed to make teleporting more balanced. /back has been disabled, as your items are already "saved" from being in a tombstone, removing the time element of reclaiming your stuff.

### *(config/defaultoptions/extra/config/tpaplusplus-config.toml)*
- "Use /back" = false
- "Accept Windup" = 5.0
- "Global Cooldown" = 900 (15minutes)

<div align="center">

## Enhanced Mob Spawners
</div>
Default spawner range was set to vanilla value of 16, but can still be bumped up with the spawner key item. Egg removal was disabled, because it allows a player to disable any dungeon mob spawner with a simple right click. Egg drop chance has been disabled because eggs from some mods like BetterEnd would not drop due to inconsitencies with how the egg items are named. A separate mod handles egg drops instead, but the configs for disabling eggs in this mod are still present for clarity sake.

### *(config/defaultoptions/extra/config/spawnermod.json)*
- "default_spawner_range": 52 -> 16
- "disable_count": 0 -> 1
- "disable_egg_removal_from_spawner": 0 -> 1
- "monster_egg_drop_chance": 1 -> 0

"disable_specific_egg_drops":
- "alexsmobs:warped_mosco": 1
- "alexsmobs:cachalot_whale": 1
- "alexsmobs:void_worm": 1
- "alexsmobs:bunfungus": 1
- "alexsmobs:farseer": 1
- "deeperdarker:shriek_worm": 1
- "deeperdarker:stalker": 1
- "enlightened_end:void_leviathan": 1
- "minecraft:ender_dragon": 1
- "minecraft:warden": 1


<div align="center">

## Supplementaries
</div>
A handful of destructive features were disabled.

### *(config/defaultoptions/extra/config/supplementaries-common.toml)*
[functional.cannon]
- enabled = false

[functional.lumisene]
- enabled = false

[tweaks.throwable_bricks]
- enabled = false

<div align="center">

## Wilder Nature
</div>
Raccoons and bison are already added through Alex's Mobs, so to avoid confusion, these duplicates were disabled.

### *(config/defaultoptions/extra/config/wildernature.toml)*
- raccoonSpawnWeight = 0
- bisonSpawnWeight = 0

<div align="center">

## Xaero's Minimap
</div>
Visual elements were changed to how the minimap is displayed.

<div align="center">

## Xaero's Worldmap
</div>
Visual elements were changed to how the world map is displayed.

# Mods - "defaultconfigs"

<div align="center">

## GraveStone Mod
</div>
Anyone can break the gravestone, to avoid griefing and cases where players didn't pick up their own graves.

### *(defaultconfigs/gravestone-server.toml)*
- only_owners_can_break = false

<div align="center">

## Open Parties and Claims
</div>

A lot of custom entries were added to increase mod compatibility with the claim protection. Many harmless blocks are not protected by default, such as sitting areas like chairs and benches, or anything else that does not come at the cost of the owning player. Doors are accessible by default, to reduce the likelyhood of players getting stuck. Create trains are accessible by default, to reduce problems such as when a player might disembark from their train while inside another player's claim, being unable to get back into the controls. This also makes it easier to create train stations, without the need for further configuration of the claim protection rules.

A lot of categories were created for groups of similar modded blocks, to allow for more freedom and flexibility. Due to the extent of the config entries, they will not be explicitly outlined here. Refer to the "openpartiesandclaims-server.toml" and "openpartiesandclaims-default-player-config.toml" files inside the defaultconfigs folder instead.
