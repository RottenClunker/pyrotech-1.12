**1.5.25**

  * **Fixed:**
    * Sawmill should only play the final work complete sound once  

---

**1.5.24**

  * **Changed:**
    * Improve CompostBinRecipe#getRecipe loading time [(#379)](https://github.com/codetaylor/pyrotech-1.12/pull/379)

---

**1.5.23**

  * **Fixed:**
    * Soaking pot voids items in recipes resulting in stacks over the max stack size [(#381)](https://github.com/codetaylor/pyrotech-1.12/issues/381)

---

**1.5.22**

  * **Fixed:**
    * ToP displays sawmill recipes result amounts incorrectly [(#376)](https://github.com/codetaylor/pyrotech-1.12/issues/376)

---

**1.5.21**

  * **Fixed:**
    * Pyrotech buckets delete objects when placing water [(#375)](https://github.com/codetaylor/pyrotech-1.12/issues/375)

---

**1.5.20**

  * **Fixed:**
    * Empty bucket Crucible recipe output displayed in Waila

---

**1.5.19**

  * **Fixed:**
    * Milk buckets shouldn't stack and void on use [(#374)](https://github.com/codetaylor/pyrotech-1.12/issues/374)

---

**1.5.18**

  * **Fixed:**
    * Irregular behavior when transferring items from the rock bag into containers

---

**1.5.17**

  * **Fixed:**
    * Rendering issue when Crude Drying Rack placed above Drying Rack

---

**1.5.16**

  * **Fixed:**
    * Slag should scale with respect to the amount of ore in the bloomery and not the bloomery capacity [(#369)](https://github.com/codetaylor/pyrotech-1.12/issues/369)

  * **Changed:**
    * Improved ore compat error logging

---

**1.5.15**

  * **Fixed:**
    * Rock Bag ToP error [(#366)](https://github.com/codetaylor/pyrotech-1.12/issues/366)

---

**1.5.14**

  * **Fixed:**
    * Compost Bin ToP error [(#364)](https://github.com/codetaylor/pyrotech-1.12/issues/364)

---

**1.5.13**

  * **Changed:**
    * Updated ru_ru.lang [(#358)](https://github.com/codetaylor/pyrotech-1.12/pull/358)
    
  * **Added:**
    * Russian guidebook translation [(#358)](https://github.com/codetaylor/pyrotech-1.12/pull/358)
    
---

**1.5.12**

  * **Fixed:**
    * Infinite fuel exploit [(#356)](https://github.com/codetaylor/pyrotech-1.12/issues/356)

  * **Changed:**
    * Wooden Buckets can no longer be used as fuel

---

**1.5.11**

  * **Changed:**
    * Updated zh_cn.lang [(#353)](https://github.com/codetaylor/pyrotech-1.12/pull/353)

---

**1.5.10**

  * **Fixed:**
    * Dense redstone crystals don't play sounds on a dedicated server and spam error in client log [(#350)](https://github.com/codetaylor/pyrotech-1.12/issues/350)

---

**1.5.9**

  * **Changed:**
    * Updated zh_cn.lang [(#345)](https://github.com/codetaylor/pyrotech-1.12/pull/345)

---

**1.5.8**

  * **Fixed:**
    * Broken bloom block item stack display name

---

**1.5.7**

  * **Fixed:**
    * Rock Bag voids contents when placed and replaces a block, ie. tall grass, rocks [(#341)](https://github.com/codetaylor/pyrotech-1.12/issues/341)

---

**1.5.6**

  * **Required:**
    * Athenaeum >= 1.19.2 [(#338)](https://github.com/codetaylor/pyrotech-1.12/issues/338)

---

**1.5.5**

  * **Fixed:**
    * Soaking Pot should require campfire when specified in ZS
    * Hwyla / ToP should not indicate Soaking Pot needs a campfire if it has one lit below

---

**1.5.4**

  * **Fixed:**
    * Torches don't attach to walls [(#334)](https://github.com/codetaylor/pyrotech-1.12/issues/334)

---

**1.5.3**

  * **Fixed:**
    * Torches don't ignite on client connected to server [(#333)](https://github.com/codetaylor/pyrotech-1.12/issues/333)

---

**1.5.2**

  * **Fixed:**
    * Red Sandstone Rock can't be placed in rock bags [(#332)](https://github.com/codetaylor/pyrotech-1.12/issues/332)
    * Netherrack Gib can't be placed in rock bags

---

**1.5.1**

  * **Fixed:**
    * Refractory Tank empty recipe is messed up [(#331)](https://github.com/codetaylor/pyrotech-1.12/issues/331)

---

# 1.5.0

  * **Added:**
    * Config option to disable throwing rocks / clumps `THROW_ENABLED` [(#301)](https://github.com/codetaylor/pyrotech-1.12/issues/301)
    * Oredict:
        * `milk` now contains:
            * `minecraft:milk`
            * wooden, clay, and stone milk bucket from Pyrotech
        * `toolSharp` contains swords and axes, sans wooden sword
        * `mulchNitrogen` now contains `pyrotech:rock_netherrack`
        * `rock` now contains `pyrotech:rock:10`
    * Red Sandstone Rocks
    * Straw Bed
        * Single-use bed that does not set a spawn point
    * Netherrack Rocks
        * Drop from Netherrack with low tier tools
        * Spread netherrack `ModuleCoreConfig.ROCKS.NETHERRACK_SPREAD_RADIUS`
    * Dense Redstone Ore
        * Spawns in caves between height 5 and 25 in the overworld
        * Drops Dense Redstone and Redstone when harvested with an iron+ tier pickaxe
        * Chance to spawn Redstone Ore below the dense ores
        * Added worldgen module config values:
            * `ENABLED`
            * `DIMENSION_WHITELIST`
            * `DIMENSION_BLACKLIST`
            * `CHANCE_TO_SPAWN`
            * `CHANCE_TO_SPAWN_REDSTONE_ORE`
            * `VERTICAL_BOUNDS`
    * Dense Redstone
        * Anvil hammer recipe to convert Dense Redstone into Redstone
    * Redstone Tools
        * Made from Dense Redstone
        * Redstone tools have a small chance to activate when damaged, giving them unique properties.
        * Added tools module config values:
            * `ACTIVE_DURATION_TICKS`
            * `ACTIVE_DAMAGE_CHANCE`
            * `INACTIVE_ACTIVATION_CHANCE`
            * `ACTIVE_ACTIVATION_CHANCE`
            * `ACTIVE_HARVEST_SPEED_SCALAR`
            * `ACTIVE_SWORD_DAMAGE_SCALAR`
            * `PROXIMITY_REPAIR_CHANCE`
    * Dense Quartz Ore
        * Spawns in the lower half of the nether
        * Drops Dense Quartz and Quartz when harvested with an iron+ tier pickaxe
        * Chance to spawn Quartz Ore below the dense ores
        * Added worldgen module config values:
            * `ENABLED`
            * `DIMENSION_WHITELIST`
            * `DIMENSION_BLACKLIST`
            * `CHANCE_TO_SPAWN`
            * `CHANCE_TO_SPAWN_QUARTZ_ORE`
            * `VERTICAL_BOUNDS`
    * Dense Quartz
        * Anvil pickaxe recipe to convert Dense Quartz into Quartz
    * Dense Quartz Tools
        * Made from Dense Quartz
        * Dense Quartz tools perform better in The Nether.
        * Added tools module config values:
            * `ACTIVE_HARVEST_SPEED_SCALAR`
            * `ACTIVE_SWORD_DAMAGE_SCALAR`
    * Strange Tuber drops from tall grass and grassy dirt
        * Edible
        * Higher drop chance when not using a shovel
        * Added config values:
            * `STRANGE_TUBER_HUNGER`
            * `STRANGE_TUBER_SATURATION`
    * Marshmallow roasting mechanic:
        * Added config values:
            * `ROASTING_RANGE_BLOCKS`
            * `ROASTING_DURATION_TICKS`
            * `ROASTING_DURATION_VARIANCE_PERCENTAGE`
            * `ROASTING_BURN_DURATION_TICKS`
        * Marshmallows:
            * Short speed effect when eaten
            * Added config values:
                * `MARSHMALLOW_HUNGER`
                * `MARSHMALLOW_SATURATION`
                * `MARSHMALLOW_SPEED_DURATION_TICKS`
                * `MAX_MARSHMALLOW_SPEED_DURATION_TICKS`
        * Roasted Marshmallows:
            * Speed effect when eaten
            * Added config values:
                * `ROASTED_MARSHMALLOW_HUNGER`
                * `ROASTED_MARSHMALLOW_SATURATION`
                * `ROASTED_MARSHMALLOW_SPEED_DURATION_TICKS`
                * `MAX_ROASTED_MARSHMALLOW_SPEED_DURATION_TICKS`
                * `ROASTED_MARSHMALLOW_EFFECT_POTENCY_DURATION_TICKS`
        * Burned Marshmallows:
            * Added config values:
                * `BURNED_MARSHMALLOW_HUNGER`
                * `BURNED_MARSHMALLOW_SATURATION`
                * `BURNED_MARSHMALLOW_SLOW_DURATION_TICKS`
                * `ENABLE_BURNED_MARSHMALLOW_BROADCAST_MESSAGE`
                * `ENABLE_BURNED_MARSHMALLOW_EAT_BROADCAST_MESSAGE`
        * Marshmallow Stick:
            * Sharpen a stick with a sharp tool, `ore:toolSharp`
    * Campfire effects:
        * Added config values:
            * `EFFECTS_START_TIME`
            * `EFFECTS_STOP_TIME`
        * Comfort effect:
            * Applied when in range of a Campfire
            * Applied at night between 19:00 and 5:00
            * Increases hunger and saturation restored from eating
            * Allows player to always eat, regardless of hunger level
            * Added config values:
                * `COMFORT_EFFECT_ENABLED`
                * `COMFORT_HUNGER_MODIFIER`
                * `COMFORT_SATURATION_MODIFIER`
        * Well Fed effect:
            * Applied by eating while max saturation with the Comfort effect
            * Applied at night between 19:00 and 5:00
            * Reduces a player's exhaustion for the effect's duration
            * Added config values:
                * `WELL_FED_EFFECT_ENABLED`
                * `WELL_FED_DURATION_TICKS`
                * `WELL_FED_EXHAUSTION_MODIFIER`
        * Resting effect:
            * Applied when in range of a Campfire
            * Regenerates health slower than the Regeneration effect
            * Increases to Resting II and III by standing still
            * Added config values:
                * `RESTING_EFFECT_ENABLED`
                * `RESTING_REGEN_INTERVAL_TICKS`
                * `RESTING_REGEN_HALF_HEARTS`
                * `RESTING_LEVEL_UP_INTERVAL_TICKS`
        * Well Rested effect:
            * Applied when standing still with Resting III
            * Adds absorption hearts to the player
            * Added config values:
                * `WELL_RESTED_EFFECT_ENABLED`
                * `WELL_RESTED_DURATION_TICKS`
                * `WELL_RESTED_ABSORPTION_HALF_HEARTS`
        * Focused effect:
            * Applied when standing still with Comfort, Well Fed, Resting III, and Well Rested
            * Player gains additional XP while the effect is active
            * Added config values:
                * `FOCUSED_EFFECT_ENABLED`
                * `FOCUSED_MAXIMUM_ACCUMULATED_BONUS`
                * `FOCUSED_ACCUMULATED_BONUS`
                * `FOCUSED_BONUS`
    * Compost Bin
        * Added config values:
            * `ALLOW_AUTOMATION`
            * `SHOW_COMPOST_VALUE_IN_TOOLTIPS`
            * `SHOVEL_WHITELIST`
            * `SHOVEL_BLACKLIST`
            * `MAXIMUM_OUTPUT_ITEM_CAPACITY`
            * `COMPOST_VALUE_REQUIRED_PER_OUTPUT_ITEM`
            * `GENERATED_FOOD_COMPOST_VALUE_RANGE`
            * `COMPOST_DURATION_TICKS`
            * `ADDITIVE_PERCENTILE_SPEED_MODIFIER_PER_LAYER`
            * `MOISTURE_EVAPORATION_RATE_MILLIBUCKETS_PER_TICK`

  * **Changed:**
    * Recipes:
        * Removed mulch crafting recipe
        * Bone and Flint Shears now require Clay Shears to craft
    * OreDict:
        * Removed entry `mulchNitrogen`
    * Torches:
        * Torches are now compatible with TaN's temperature config [(#229)](https://github.com/codetaylor/pyrotech-1.12/issues/229)
    * Soaking Pot:
        * New texture
        * Can now be placed above a campfire
        * Recipes can now require a campfire
        * Waila / ToP now indicates when a recipe is missing a campfire
        * JEI now indicates when a recipe requires a campfire
        * Patchouli template now indicates when a recipe requires a campfire 
    * Campfire:
        * Campfire light level now depends on how much fuel it has
            * Removed campfire `LIGHT_LEVEL` config value
            * Added campfire `MAXIMUM_LIGHT_LEVEL` config value
            * Added campfire `MINIMUM_LIGHT_LEVEL` config value
        * Campfire will now cook faster or slower based on how much fuel it has
            * Added campfire `FUEL_LEVEL_FOR_FULL_COOK_SPEED` config value
        * Campfire will now burn food faster or slower based on how much fuel it has 
            * Burn speed depends on the `FUEL_LEVEL_FOR_FULL_COOK_SPEED` config value
    * Tanks:
        * Tanks can now be stacked vertically to combine into one larger tank [(#105)](https://github.com/codetaylor/pyrotech-1.12/issues/105)
    * World Gen:
        * Improved rock gen compatibility [(#284)](https://github.com/codetaylor/pyrotech-1.12/issues/284)
    * Interaction Framework:
        * Moved configs to Athenaeum config:
            * `core.cfg.client.ALWAYS_SHOW_QUANTITIES`
            * `core.cfg.client.SHOW_INTERACTION_BOUNDS`

  * **Fixed:**
    * ToP/Waila displays incorrect fuel time for brick machines
    * Lang keys in ore compat and custom slag file will now work properly with keys not suffixed with `.name` [(#330)](https://github.com/codetaylor/pyrotech-1.12/issues/330)

  * **Translators:**
    * **New Patchouli Categories**
        * `survive_tools.json`
        * `adapt_tools.json`
    * **New Patchouli Entries**
        * `bloom/dense_redstone.json`
        * `bloom/dense_redstone_ore.json`
        * `bloom/tools_redstone.json`
        * `bloom/dense_quartz.json`
        * `bloom/dense_quartz_ore.json`
        * `bloom/tools_quartz.json`
        * `survive/food_raw.json`
        * `adapt/compost_bin.json`
    * **Changed Patchouli Entries**
        * `adapt/mulch.json`
    * **New Lang Entries:**
        * `pyrotech.effect.comfort`
        * `pyrotech.effect.well.fed`
        * `pyrotech.effect.resting`
        * `pyrotech.effect.well.rested`
        * `pyrotech.effect.focused`
        * `item.pyrotech.marshmallow.name`
        * `item.pyrotech.marshmallow.roasted.name`
        * `item.pyrotech.marshmallow.burned.name`
        * `item.pyrotech.marshmallow.stick.name`
        * `item.pyrotech.marshmallow.on.stick.name`
        * `item.pyrotech.marshmallow.on.stick.roasted.name`
        * `item.pyrotech.marshmallow.on.stick.burned.name`
        * `item.pyrotech.marshmallow.stick.empty.name`
        * `item.pyrotech.dense.redstone.name`
        * `item.pyrotech.redstone.axe.name`
        * `item.pyrotech.redstone.hoe.name`
        * `item.pyrotech.redstone.pickaxe.name`
        * `item.pyrotech.redstone.shovel.name`
        * `item.pyrotech.redstone.sword.name`
        * `item.pyrotech.dense.quartz.name`
        * `item.pyrotech.quartz.axe.name`
        * `item.pyrotech.quartz.hoe.name`
        * `item.pyrotech.quartz.pickaxe.name`
        * `item.pyrotech.quartz.shovel.name`
        * `item.pyrotech.quartz.sword.name`
        * `tile.pyrotech.dense_redstone_ore.name`
        * `tile.pyrotech.dense_quartz_ore.name`
        * `tile.pyrotech.compost_bin.name`
        * `tile.pyrotech.straw_bed.name`
        * `tile.pyrotech.rock_sandstone_red.name`
        * `gui.pyrotech.marshmallow.burned.broadcast.message`
        * `gui.pyrotech.marshmallow.burned.eat.broadcast.message`
        * `gui.pyrotech.tooltip.potency`
        * `gui.pyrotech.tooltip.redstone.activation.chance`
        * `gui.pyrotech.tooltip.redstone.active.durability`
        * `gui.pyrotech.tooltip.redstone.active.efficiency`
        * `gui.pyrotech.tooltip.redstone.active.damage`
        * `gui.pyrotech.tooltip.redstone.active.hoe`
        * `gui.pyrotech.tooltip.compost.value`
        * `gui.pyrotech.waila.moisture.level`
        * `gui.pyrotech.waila.campfire.required`
    * **Changed Lang Entries**
        * `item.pyrotech.mulch.name` from `Potash Mulch` to `Mulch`

---

**1.4.34**

  * **Fixed:**
    * Obsidian hammer is assigned the incorrect material [(#321)](https://github.com/codetaylor/pyrotech-1.12/issues/321)

---

**1.4.33**

  * **Fixed:**
    * Server crash

---

**1.4.32**

  * **Fixed:**
    * Custom cogs aren't properly recognized
    * Custom cogs don't have a cog tooltip
    * Config comment for cogs should not refer to sawmill and sawblades

---

**1.4.31**

  * **Fixed:**
    * Soaking Pot doesn't save progress between game loads

---

**1.4.30**

  * **Changed:**
    * Updated to support changes to the Artisan Worktables API
    * Moved configs to Athenaeum config:
        * `core.cfg.client.ALWAYS_SHOW_QUANTITIES`
        * `core.cfg.client.SHOW_INTERACTION_BOUNDS`

  * **Required:**
    * Athenaeum >= 1.19.0

---

**1.4.29**

  * **Fixed:**
    * Pit Kiln and Soaking Pot output quantities don't respect the output quantities set in the recipe [(#305)](https://github.com/codetaylor/pyrotech-1.12/issues/305)
    * Hwyla and TOP don't display correct Pit Kiln and Soaking Pot output quantities
    
---
    
**1.4.28**

  * **Fixed:**
    * Inserting liquid from stackable containers voids container & liquid [(#236)](https://github.com/codetaylor/artisan-worktables-1.12/issues/236)
    
  * **Required:**
    * Athenaeum >= 1.18.1
    
---

**1.4.27**

  * **API**
    * Bumped version to 2
    * Added `PyrotechAPI.registerHammer(Item, int)`
    
  * **Fixed:**
    * Ghost Image of the Reinforced Shelf model shows missing textures on the side [(#300)](https://github.com/codetaylor/pyrotech-1.12/issues/300)

---

**1.4.26**

  * **Fixed:**
    * Pyrotech bucket crash with Agricraft water tank [(#294)](https://github.com/codetaylor/pyrotech-1.12/issues/294)

---

**1.4.25**

  * **Fixed:**
    * Hothead cosmetic effect should only work for patrons [(#292)](https://github.com/codetaylor/pyrotech-1.12/issues/292)
    * Improved performance of Hothead effect
    
---

**1.4.24**

  * **Fixed:**
    * Self-replicating, infinite lag when pit burn recipe fails to locate the given block [(#291)](https://github.com/codetaylor/pyrotech-1.12/issues/291)
    
  * **Added:**
    * Hothead cosmetic effect for Patreon supporters

---

**1.4.23**

  * **Fixed:**
    * Missing all JEI recipes when CraftTweaker isn't installed [(#285)](https://github.com/codetaylor/pyrotech-1.12/issues/285)
    * ZS method removeWitherForgeRecipes does not work [(#286)](https://github.com/codetaylor/pyrotech-1.12/issues/286)

---

**1.4.22**

  * **Fixed:**
    * Improved config documentation [(#280)](https://github.com/codetaylor/pyrotech-1.12/issues/280)
    * Wither Forge fire does not animate with VanillaFix installed [(#282)](https://github.com/codetaylor/pyrotech-1.12/issues/282)
    
---

**1.4.21**

  * **Fixed:**
    * Worktable eats Silent Gear crafts [(#262)](https://github.com/codetaylor/pyrotech-1.12/issues/262)
    * Item Fire Charge should ignite the following:
        * Campfire
        * Pit Kiln
        * Bloomery / Wither Forge
        * Stone / Brick Machines
        * Pit / Refractory Burn
    * Bloomery fire does not animate with VanillaFix installed
  
---

**1.4.20**

  * **Fixed:**
    * Broken guidebook links [(#270)](https://github.com/codetaylor/pyrotech-1.12/issues/270)
  
  * **Changed:**
    * In the guidebook, renamed `verified fire-starter device` to `verified fire-starting device`

---

**1.4.19**

  * **Fixed:**
    * Snow accumulates on top of Bloomery, Wither Forge, Stone Collector, Refractory Collector [(#172)](https://github.com/codetaylor/pyrotech-1.12/issues/172)

---

**1.4.18**

  * **Fixed:**
    * Combining items doesn't make an outcome (worktable) [(#252)](https://github.com/codetaylor/pyrotech-1.12/issues/252)
    * Worktable deleting Silent's Gear items [(#262)](https://github.com/codetaylor/pyrotech-1.12/issues/262)

---

**1.4.17**

  * **Fixed:**
    * Normal custom recipes added via CrT not shown in JEI worktable category [(#142)](https://github.com/codetaylor/pyrotech-1.12/issues/142)

---

**1.4.16**

  * **Fixed:**
    * ToP error when viewing filled Mechanical Compactor [(#260)](https://github.com/codetaylor/pyrotech-1.12/issues/260)
    * Duplicate Ash item in creative tabs
    * Looking at pit ash doesn't display with Waila and has a broken name with ToP [(#259)](https://github.com/codetaylor/pyrotech-1.12/issues/259)

---

**1.4.15**

  * **Fixed:**
    * ToP error when viewing filled Bloomery [(#258)](https://github.com/codetaylor/pyrotech-1.12/issues/258)

---

**1.4.14**

  * **Fixed:**
    * Blacklisting Smelting Recipes for Campfire visually enables all non-blacklisted Furnace recipes in JEI [(#257)](https://github.com/codetaylor/pyrotech-1.12/issues/257)

---

**1.4.13**

  * **Fixed:**
    * Two-tall machine interactions don't work

---

**1.4.12**

  * **Fixed:**
    * Class cast exception when holding use button and moving between two different devices [(#246)](https://github.com/codetaylor/pyrotech-1.12/issues/246)

---

**1.4.11**

  * **Fixed:**
    * Class cast exception when hammering a bloom [(#242)](https://github.com/codetaylor/pyrotech-1.12/issues/242)
    
---

**1.4.10**

  * **Fixed:**
    * Silk touch on iron+ tier pickaxes should not drop cobbled versions of andesite, diorite, granite, and limestone [(#238)](https://github.com/codetaylor/pyrotech-1.12/issues/238)
    * Faucets can't be used with crucibles [(#234)](https://github.com/codetaylor/pyrotech-1.12/issues/234)
    
  * **Added:**
    * Config option to reduce block drops from explosions
        * `plugin.Dropt.cfg` -> `REDUCE_EXPLOSION_DROPS`
        * Blocks affected: dirt, grass, sand, red sand, gravel, limestone, stone, cobblestone, diorite, smooth diorite, cobbled diorite, andesite, smooth andesite, cobbled andesite, granite, smooth granite, and cobbled granite

---

**1.4.9**

  * **Fixed:**
    * Bloomery / Wither Forge slag exploit [(#237)](https://github.com/codetaylor/pyrotech-1.12/issues/237)
    
  * **Added:**
    * Config option to toggle lit Bloomery / Wither Forge dropping slag when broken
        * `module.tech.Bloomery.cfg` -> `BLOOMERY` -> `DROP_SLAG_WHEN_BROKEN`
        * `module.tech.Bloomery.cfg` -> `WITHER_FORGE` -> `DROP_SLAG_WHEN_BROKEN`
        
  * **Changed:**
    * Bloomery / Wither Forge will now drop slag items when broken after activation instead of dropping the input ore 
    
---

**1.4.8**

  * **Fixed:**
    * Campfire output stack size should not be limited to one [(#235)](https://github.com/codetaylor/pyrotech-1.12/issues/235)

---

**1.4.7**

  * **Fixed:**
    * Crash when a lit campfire burns the block below [(#231)](https://github.com/codetaylor/pyrotech-1.12/issues/231)

---

**1.4.6**

  * **Fixed:**
    * Mod does not replace lit furnaces [(#227)](https://github.com/codetaylor/pyrotech-1.12/issues/227)

---

**1.4.5**

  * **Fixed:**
    * Dependency load order with Waila and ToP
    * Mouse event handler shouldn't load on the server
    * Waila plugins should not load on the server

---

**1.4.4**

  * **Fixed:**
    * Lapis and redstone anvil recipes don't give correct output amount [(#217)](https://github.com/codetaylor/pyrotech-1.12/issues/217)

---

**1.4.3**

  * **Fixed:**
    * Fossil Ore -> Bone Shard silk touch dupe [(#212)](https://github.com/codetaylor/pyrotech-1.12/issues/212)
    * Grass -> Grass Clump silk touch dupe
    * Coal Ore -> Coal silk touch dupe

---

**1.4.2**

  * **Fixed:**
    * Pyrotechnic Esoterica doesn't open on server [(#211)](https://github.com/codetaylor/pyrotech-1.12/issues/211)

---

**1.4.1**

  * **Fixed:**
    * Rocks don't drop when broken [(#208)](https://github.com/codetaylor/pyrotech-1.12/issues/208)

---

# 1.4.0

  * **Translators:**
    * New lang keys:
        * gui.pyrotech.tooltip.durability.indestructible
        * gui.pyrotech.tooltip.fluid.transfer.rate
        * gui.pyrotech.tooltip.fluid.transfer.limit
        * tile.pyrotech.faucet_stone.name
        * tile.pyrotech.faucet_brick.name
    * New book entries:
        * entries/accelerate/refractory_faucet.json
        * entries/innovate/stone_faucet.json

  * **Added:**
    * Cooldown to thrown rocks / clumps [(#157)](https://github.com/codetaylor/pyrotech-1.12/issues/157)
        * Config value: `core.cfg` -> `ROCKS` -> `THROW_COOLDOWN_TICKS`
    * Config option to set Sawmill blades as indestructible [(#98)](https://github.com/codetaylor/pyrotech-1.12/issues/98)
        * Config value: `module.tech.Machine.cfg` -> `SAWMILL_BLADES` -> `INDESTRUCTIBLE_SAWBLADES`
    * Config option to set Cogs as indestructible [(#98)](https://github.com/codetaylor/pyrotech-1.12/issues/98)
        * Config value: `module.tech.Machine.cfg` -> `COGS` -> `INDESTRUCTIBLE_COGS`
    * Config option to set Chopping Block as indestructible [(#98)](https://github.com/codetaylor/pyrotech-1.12/issues/98)
        * Config value: `module.tech.Basic.cfg` -> `CHOPPING_BLOCK` -> `USES_DURABILITY`
    * Config option to set anvils as indestructible [(#98)](https://github.com/codetaylor/pyrotech-1.12/issues/98)
        * Config value: `module.tech.Basic.cfg` -> `GRANITE_ANVIL` -> `USES_DURABILITY`
        * Config value: `module.tech.Basic.cfg` -> `IRONCLAD_ANVIL` -> `USES_DURABILITY`
    * Pyrotech will now scan loot tables and replace `Iron Ingot` with `Iron Ore` [(#102)](https://github.com/codetaylor/pyrotech-1.12/issues/102)
        * Config value: `core.cfg` -> `TWEAKS` -> `REPLACE_IRON_INGOTS_WITH_IRON_ORE`
    * New Block: Stone / Refractory Faucet [(#132)](https://github.com/codetaylor/pyrotech-1.12/issues/132)
        * Transfers fluid from attached fluid handler to fluid handler below
        * Can break with hot fluids (optional)
        * Can shutoff after transfer limit reached (optional)
        * Configs: `module.Storage.cfg` -> `STONE_FAUCET`, `BRICK_FAUCET`
            * `I:HOT_TEMPERATURE`
            * `B:TRANSFERS_HOT_FLUIDS`
            * `I:TRANSFER_AMOUNT_PER_TICK`
            * `I:TRANSFER_LIMIT`
    * Cog Machines can now be disabled with a redstone signal [(#145)](https://github.com/codetaylor/pyrotech-1.12/issues/145)
    * New Item: Lump of Refractory Clay `<pyrotech:material:35>`
    * Terracotta and Glazed Terracotta recipes have been added to the Pit Kiln, Stone Kiln, and Refractory Kiln [(#134)](https://github.com/codetaylor/pyrotech-1.12/issues/134)
    * Config options to change the input capacity of the Bloomery and Wither Forge [(#79)](https://github.com/codetaylor/pyrotech-1.12/issues/79)
        * `module.tech.Bloomery.cfg` -> `BLOOMERY` -> `CAPACITY`
        * `module.tech.Bloomery.cfg` -> `WITHER_FORGE` -> `CAPACITY`
    * Drying Racks are now climbable when stacked vertically
        * Config values:
            * `module.tech.Basic.cfg` -> `DRYING_RACK` -> `CLIMB_SPEED`
            * `module.tech.Basic.cfg` -> `DRYING_RACK` -> `USE_AS_LADDER`

  * **Fixed:**
    * Pit Kiln only plays wood placement sound for the last log placed
    * Piles of wood chips yield unexpected quantities when broken [(#143)](https://github.com/codetaylor/pyrotech-1.12/issues/143)
    * Tongs should not take damage when a player is in creative mode
    * Can't set harvest level of Pyrotech tools with Tool Progression mod [(#164)](https://github.com/codetaylor/pyrotech-1.12/issues/164)

  * **Changed:**
    * Patchouli is now a required dependency [(#169)](https://github.com/codetaylor/pyrotech-1.12/issues/169)
    * Pit Kiln is now configured to take less time when it has fewer items [(#119)](https://github.com/codetaylor/pyrotech-1.12/issues/119)
        * Config value: `module.tech.Basic.cfg` -> `PIT_KILN` -> `VARIABLE_SPEED_MODIFIER`
    * ZS method for Campfire recipes now has an optional duration parameter [(#138)](https://github.com/codetaylor/pyrotech-1.12/issues/138)
        * If omitted, defaults to config value: `module.tech.Basic.cfg` -> `CAMPFIRE` -> `COOK_TIME_TICKS`
    * Redesigned and rebalanced the Sawmill and Wood Chips [(#140)](https://github.com/codetaylor/pyrotech-1.12/issues/140)
        * The sawmill will now process one item at a time
        * Recipe:
            * Recipe time value is now per item, not per batch
            * Recipe wood chips value is now per item, not per batch
        * Wood Chip production:
            * Wood chips are now produced on the ground each time an item completes
            * Stone Sawblade recipes will produce 4 wood chips per item processed
            * Flint / Bone Sawblade recipes will produce 2 wood chips per item processed
            * Iron / Obsidian / Diamond Sawblade recipes will produce 1 wood chip per item processed
        * Input / output:
            * Input items can't be inserted while the machine contains output items
            * Input items must be extracted by hand before output items can be extracted by hand
            * Output items can still be extracted by hopping the bottom at any time
        * Sound:
            * The Sawmill's recipe complete sounds now play after each item is processed
            * The Sawmill's recipe complete sounds have been shortened and varied
            * The original, longer recipe complete sound plays when the last item is processed
        * Burn time:
            * Reduced Pile of Wood Chips burn time from 100 to 50
            * Reduced Board burn time from 200 to 75
        * Pit Burn:
            * Wood Chips block in a Pit Burn will now produce 8 Charcoal Flakes instead of 4 Charcoal
            * Wood Chips block Pit Burn recipe duration increased
    * All wood chips now require a shovel to gather [(#137)](https://github.com/codetaylor/pyrotech-1.12/issues/137)
        * Config: `core.cfg` -> `TWEAKS` -> `REQUIRE_SHOVEL_TO_PICKUP_WOOD_CHIPS`
    * Refractory Brick cost changed to 2x Lump of Refractory Clay
    * With respect to [(#130)](https://github.com/codetaylor/pyrotech-1.12/issues/130):
        * Reduced default damage to Granite Anvil from hammering a bloom by half
        * Renamed config value `module.tech.Basic.cfg` -> `GRANITE_ANVIL` -> `BLOOM_DAMAGE_PER_HIT`:
            * New name: `BLOOM_EXTRA_DAMAGE_PER_HIT`
        * Renamed config value `module.tech.Basic.cfg` -> `IRONCLAD_ANVIL` -> `BLOOM_DAMAGE_PER_HIT`:
            * New name: `BLOOM_EXTRA_DAMAGE_PER_HIT`
        * Config option to control chance of extra anvil damage when hammering a bloom
            * Config value: `module.tech.Basic.cfg` -> `GRANITE_ANVIL` -> `BLOOM_EXTRA_DAMAGE_CHANCE`
            * Config value: `module.tech.Basic.cfg` -> `IRONCLAD_ANVIL` -> `BLOOM_EXTRA_DAMAGE_CHANCE`
    * When an anvil breaks with a bloom on it, the bloom will be placed in the world where the anvil was [(#129)](https://github.com/codetaylor/pyrotech-1.12/issues/129)
    * Worktable recipe whitelist / blacklist now accepts `*` as a valid path wildcard [(#179)](https://github.com/codetaylor/pyrotech-1.12/issues/179)
    * Drying Racks now connect visually when stacked vertically [(#109)](https://github.com/codetaylor/pyrotech-1.12/issues/109)
    * Campfire state changes are no longer only visual [(#123)](https://github.com/codetaylor/pyrotech-1.12/issues/123)
    * Removed all entry locking from the guidebook [(#75)](https://github.com/codetaylor/pyrotech-1.12/issues/75), [(#115)](https://github.com/codetaylor/pyrotech-1.12/issues/115), [(#128)](https://github.com/codetaylor/pyrotech-1.12/issues/128)

---

**1.3.13**

  * **Fixed:**
    * Crash when breaking a lit campfire with the bloomery module disabled [(#189)](https://github.com/codetaylor/pyrotech-1.12/issues/189)

  * **Changed:**
    * Updated `ru_ru.lang` [(#188, SSKirillSS)](https://github.com/codetaylor/pyrotech-1.12/pull/188)

---

**1.3.12**

  * **Fixed:**
    * Crash with SpongeForge plugin Grief Prevention [(#176)](https://github.com/codetaylor/pyrotech-1.12/issues/176)

  * **Changed:**
    * When an active pile in a pit burn fails, it will change to fire instead of air [(#176)](https://github.com/codetaylor/pyrotech-1.12/issues/176)

---

**1.3.11**

  * Added:
    * `ru_ru.lang` [(#178, SSKirillSS)](https://github.com/codetaylor/pyrotech-1.12/pull/178)

---

**1.3.10**

  * Fixed:
    * Snow accumulates on top of machines [(#172)](https://github.com/codetaylor/pyrotech-1.12/issues/172)
    * Duplicate line in TOP display for tanks [(#173)](https://github.com/codetaylor/pyrotech-1.12/issues/173)
    * Drains and Collectors missing TOP display

---

**1.3.9**

  * Fixed:
    * Startup crash caused by setting `DISABLE_YOUR_PATREON_EFFECTS` to `true`

---

**1.3.8**

  * Fixed:
    * Slag glass furnace recipe should be in the bloomery module and not the refractory module

---

**1.3.7**

  * Fixed:
    * No Cog sound for Mechanical Mulcher [(#162)](https://github.com/codetaylor/pyrotech-1.12/issues/162)
    * Worktable.blacklistAllVanillaRecipes() does not remove blacklisted recipes from JEI [(#165)](https://github.com/codetaylor/pyrotech-1.12/issues/165)

---

**1.3.6**

  * Fixed:
    * Wood chip pile doesn't work in a pit burn [(#161)](https://github.com/codetaylor/pyrotech-1.12/issues/161)

---

**1.3.5**

  * Fixed:
    * Block of iron and gold only give 1 ingot when broken on an anvil [(#158)](https://github.com/codetaylor/pyrotech-1.12/issues/158)

---

**1.3.4**

  * Fixed:
    * JEI plugin for Refractory module will fail to load under certain conditions [(#154)](https://github.com/codetaylor/pyrotech-1.12/issues/154)

---

**1.3.3**

  * Fixed:
    * Custom CrT drying recipes don't work [(#153)](https://github.com/codetaylor/pyrotech-1.12/issues/153)

---

**1.3.2**

  * Fixed:
    * Grass Path block should drop dirt and grass clumps [(#146)](https://github.com/codetaylor/pyrotech-1.12/issues/146)

---

**1.3.1**

  * Added:
    * `/ptlang` command will now copy the lang key to the clipboard

  * Fixed:
    * `/ptlang` command uses the wrong text component
    * Base duration modifier for Pit Kiln, Crude / Drying Rack, Soaking Pot, Pit / Refractory Burn not reflected in JEI [(#144)](https://github.com/codetaylor/pyrotech-1.12/issues/144)
    * Refractory Kiln uses Stone Kiln recipes instead of its own recipes [(#144)](https://github.com/codetaylor/pyrotech-1.12/issues/144)

---

# 1.3.0

  * Notes:
    * Refresh your `core.OreDict-Custom.json` file or copy the new entries from `core.OreDict-Generated.json`.
    * Rock bags in item form may lose their pre-existing contents and functionality: place in world and retrieve to restore function, but not pre-existing contents.
    * Recipes made with CraftTweaker are no longer automatically inherited. [(DOC)](inheritance) [(#110)](https://github.com/codetaylor/pyrotech-1.12/issues/110)

  * Docs:
    * Documentation for the alternate Refractory Machine textures [(DOC)](refractorymachines)
    * Documentation for recipe inheritance [(DOC)](inheritance)
    * Documentation for modules [(DOC)](modules)
    * Documentation for commands [(DOC)](commands)
    * Documentation for worktable QoL [(DOC)](worktables)
    * Documentation for drying rack speed modification [(DOC)](dryingracks)
    * Documentation for Dropt rules [(DOC)](droptrules)

  * Added:
    * GameStages support for worktable recipes [(#3)](https://github.com/codetaylor/pyrotech-1.12/issues/3) [(DOC)](zs/worktable) [(DOC)](zs/stages)
    * Exposed config values for both drying racks' speed calculations [(#92)](https://github.com/codetaylor/pyrotech-1.12/issues/92) [(DOC)](dryingracks)
    * CrT methods for the drying racks that allow overriding a biome's base speed [(#92)](https://github.com/codetaylor/pyrotech-1.12/issues/92) [(DOC)](dryingracks)
    * Vanilla smelting recipe for [(#82)](https://github.com/codetaylor/pyrotech-1.12/issues/82):
        * Slag -> Slag Glass (bloomery)
        * Unfired Clay Bucket -> Clay Bucket (bucket)
        * Unfired Refractory Brick -> Refractory Brick (core)
        * Crushed Limestone -> Quicklime (core)
        * Gravel -> Cobblestone (core)
        * Unfired Clay Shears -> Clay Shears (tool)
    * Client-side command `/ptlang` to display the unlocalized name of a held item [(#94)](https://github.com/codetaylor/pyrotech-1.12/issues/94) [(DOC)](commands)
    * Worktable QoL: Recipe Clear, Recipe Repeat [(#99)](https://github.com/codetaylor/pyrotech-1.12/issues/99) [(DOC)](worktables)
    * Progress particle indicators to [(#22)](https://github.com/codetaylor/pyrotech-1.12/issues/22):
        * Chopping Block
        * Drying Rack, Crude Drying Rack
        * Campfire
        * Soaking Pot
        * Combustion Machines
    * Sawmill audio feedback [(#22)](https://github.com/codetaylor/pyrotech-1.12/issues/22):
        * The sawmill will emit a whirring drone when the machine is lit and has a sawblade.
        * The sawmill will emit a distinct cutting noise when the machine completes a recipe.
        * Config: `module.tech.Machine.cfg`: `SAWMILL_SOUNDS`
    * Oredict entries [(#108)](https://github.com/codetaylor/pyrotech-1.12/issues/108):
        * Durable Twine -> `twine`
        * Coal Coke -> `fuelCoke`
        * Block of Coal Coke -> `blockFuelCoke`
        * Dense Nether Coal -> `oreNetherCoal`
    * Press shift to view contents of rock bags in tooltip when in item form [(#116)](https://github.com/codetaylor/pyrotech-1.12/issues/116)
    * Optional ZenScript method parameter for recipe inheritance [(DOC)](inheritance) [(#110)](https://github.com/codetaylor/pyrotech-1.12/issues/110)
    * Support for The One Probe [(#6)](https://github.com/codetaylor/pyrotech-1.12/issues/6)

  * Fixed:
    * Smelting recipes added by the mod were also being removed by the mod
    * Hammering the bloom sometimes destroys nearby water sources [(#113)](https://github.com/codetaylor/pyrotech-1.12/issues/113)
    * Can put Cooked Fish back into the Campfire to produce Cooked Fish [(#114)](https://github.com/codetaylor/pyrotech-1.12/issues/114)
    * Some recipes can't be removed [(#110)](https://github.com/codetaylor/pyrotech-1.12/issues/110)
    * Pit Burn remove method removing recipes added by CrT also [(#141)](https://github.com/codetaylor/pyrotech-1.12/issues/141)

  * Changed:
    * Combustion Machine smoke particles are now used to indicate that the machine is burning fuel instead of indicating that the machine is actively working on a recipe [(#22)](https://github.com/codetaylor/pyrotech-1.12/issues/22)
    * The Soaking Pot will now eject any extra input items that it does not have the fluid to process when the fluid level drops below the amount needed to process all input items
    * Mulch can now be placed on dry farmland as well as wet farmland [(#118)](https://github.com/codetaylor/pyrotech-1.12/issues/118)
        * See config `core.cfg` -> `MULCHED_FARMLAND` -> `RESTRICT_TO_MOISTURIZED_FARMLAND`
    * Rock bags now bypass the item capability system in Forge in an attempt to fix [(#117)](https://github.com/codetaylor/pyrotech-1.12/issues/117)
        * Item data is now written directly to the item's NBT

---

**1.2.9**

  * Fixed:
      * Crash when other mods throw an exception during a call to their block's `Block#getItem` method [(#139)](https://github.com/codetaylor/pyrotech-1.12/issues/139)

---

**1.2.8**

  * Notes:
      * CrT Bloomery recipes with an oredict as input may fail to deduce the lang key from the input if the oredict is empty during script execution. To solve this, simply supply a lang key with the recipe builder. This issue has been resolved in-dev as a part of the inheritance overhaul for `1.3.0`.

  * Added:
      * Chinese translation for guidebook! Thank you Snownee and Taskeren! [(#135 Snownee, Taskeren)](https://github.com/codetaylor/pyrotech-1.12/pull/135)

  * Fixed:
      * Crash on startup | ArrayIndexOutOfBoundsException [(#133)](https://github.com/codetaylor/pyrotech-1.12/issues/133)

---

**1.2.7**

  * Fixed:
      * Worktable whitelist / blacklist doesn't work [(#125)](https://github.com/codetaylor/pyrotech-1.12/issues/125)

---

**1.2.6**

  * Fixed:
      * ArrayIndexOutOfBoundsException when using a whitelisted non-axe tool with the chopping block [(#124)](https://github.com/codetaylor/pyrotech-1.12/issues/124)

---

**1.2.5**

  * Fixed:
      * ZenScript method to whitelist campfire fuel doesn't work [(#121)](https://github.com/codetaylor/pyrotech-1.12/issues/121)

---

**1.2.4**

  * Note:
      * Any Stone Igniter or Refractory Igniter currently in the world will be inert after this update. They will need to be broken and replaced in order to function.

  * Fixed:
      * Crash when using igniter blocks [(#107)](https://github.com/codetaylor/pyrotech-1.12/issues/107)

---

**1.2.3**

  * Fixed:
      * Unfired Clay Shears should not work as shears with 238 durability [(#100)](https://github.com/codetaylor/pyrotech-1.12/issues/100)

---

**1.2.2**

  * Note:
    * Remove the leading `.` from Pyrotech's config files
    * Thermal Expansion sawmill may be missing plank recipes, please read about solutions here: [https://pyrotech.readthedocs.io/en/latest/knownissues/](https://pyrotech.readthedocs.io/en/latest/knownissues/)

  * Fixed:
    * Config files prefixed with `.` are not correctly imported by the Twitch app (#96)
    * Removed vanilla crafting recipes still showing up in JEI (#97)

  * Changed:
    * All config files that were previously prefixed with `.` have had the `.` removed
    * Pyrotech once again removes recipes during post-init, pre-CrT

---

**1.2.1**

  * Fixed:
    * Missing config option to disable stick drops from leaves: `DROP_STICKS_FROM_LEAVES` in the `TWEAKS` section of `.core.cfg`

---

# 1.2.0

  * Note:
    * Bugs: A lot of code has been touched in this release - thank you for your continued bug reports!
    * The default oredict entries have changed, please refresh your `config/pyrotech/.core.OreDict-Custom.json` file
    * It is safe to delete the `B:leaves` entry from the `config/pyrotech/plugin.Dropt.cfg` file

  * API:
    * Added `IAirflowConsumerCapability`
    * Bumped version to 1

  * Added:
    * Config options to modify base recipe duration for (#70): Pit Kiln, Crude / Drying Rack, Soaking Pot, Pit / Refractory Burn
    * ZS methods to assign Bloomery and Wither Forge fuel modifiers (#56)
    * ZS methods to white / blacklist campfire fuels (#63)
    * Config option to disable using any `logWood` as campfire fuel (#63)
    * Pyrotech and Vanilla axes (sans wood) have been added to the oredict `toolAxe` with a wildcard damage value
    * ZS methods to restrict device interaction with gamestages for (#4): Worktable / Stone Worktable, Soaking Pot, Pit Kiln, Crude Drying Rack / Drying Rack, Compacting Bin, Chopping Block, Campfire, Granite Anvil / Ironclad Anvil, Bloom, Bloomery, Wither Forge, Stone / Refractory Machines, Mechanical Hopper, Mechanical Bellows, Mechanical Mulcher, Bellows, Stone / Brick Tank, Wood Rack, Simple / Durable Rock Bag, Crate / Durable Crate, Shelf / Durable Shelf, Stash / Durable Stash
    * Sticks will now attempt to drop from any block with an entry in the `treeLeaves` oredict (#69 giggity)

  * Changed:
    * The Chopping Block recipe will now accept any axe with a `toolAxe` oredict entry
    * The Chopping Block recipe will now damage the input axe instead of consuming the entire axe
    * The vanilla recipe removal has been delayed until the load complete event to allow time for other mods, such as TE, to generate recipes
    * Dropt is no longer in charge of the leaf / stick drops
    * The Stone / Refractory Crucible will now only accept a total number of input items for which it has the output capacity (#25)
    * The Soaking Pot will now only accept a total number of input items for which it has fluid to process (#25)

---

**1.1.7**

  * Fixed:
    * Mulched Farmland should not sound like stone (#90)
    * Templates of refractory machines showing wrong machine tooltip (#89)
    * Crash when using Tongs (#88)

  * Changed:
    * Updated zh_cn.lang (#87 Snownee)

---

**1.1.6**

  * Fixed:
    * Having an open rock bag suppresses pick-up noises of other items (#62)
    * Mycelium blocks should drop dirt clumps when broken (#83)
    * Custom CrT Worktable recipes improperly displayed in JEI

---

**1.1.5**

  * [!] Requires Athenaeum >= 1.17.2

  * Added:
    * Bare-bones worktable zen methods `addShaped` and `addShapeless`

  * Fixed:
    * Snow collects on and fences connect to drying racks (#76)
    * Farmland blocks should drop dirt clumps like dirt blocks
    * Mulched Farmland blocks should drop dirt clumps like dirt blocks

  * Changed:
    * Increased crude / drying rack base speed when raining in a high humidity biome from 0.0 to 0.25

---

**1.1.4**

  * Fixed:
    * Can't remove crude drying rack recipes (#73)
    * Contrary to the proclamations of popular literature, a stone bucket does not last longer than a stone bucket (#74)
    * Fluid rendering crash mod conflict
    * Light update issues when world is first loaded

---

**1.1.3**

  * Fixed:
    * CrT Burn method `addFailureItem` should take `IItemStack` not `ItemStack`

---

**1.1.2**

  * Note:
    * To fix a conflict with generated wood compat recipe names, the generated recipe names have been changed. They now include both the input and output and look something like this: `pyrotech:minecraft_planks_4_from_minecraft_log2_0`.

  * Fixed:
    * CrT Burn method `setFluidProduced` should take `ILiquidStack` not `FluidStack`
    * Wood compat generated recipe name conflicts (#67)

  * Changed:
    * Generated wood compat recipe names, see note

---

**1.1.1**

  * Notes:
    * The format of both `config/pyrotech/.core.compat.Wood` json files has changed, be sure to delete and refresh or manually edit those files.
    * Do you have duplicate iron and gold slag? Remove the iron and gold entries from the `module.tech.Bloomery.Slag-Custom.json` file.

  * Fixed:
    * Design oversight in the wood compat .json file (#67)
    * Mobs spinning on rocks (#68)

  * Changed:
    * Format of the `config/pyrotech/.core.compat.Wood` json files (#67)
    * All slag items and blocks generated by the `module.tech.Bloomery.Slag-Custom.json` config are now suffixed with `_custom` to avoid crash conflict with slag items and blocks generated by the ore compat system (#66)

---

# 1.1.0

  * Notes:
    * Load mod once to generate new ore and wood compat .json files in config folder:
      * `.core.compat.Ore-Custom.json`
      * `.core.compat.Ore-Generated.json`
      * `.core.compat.Wood-Custom.json`
      * `.core.compat.Wood-Generated.json`
    * Player will receive a message to restart if compat files are missing and subsequently generated
    * Reload mod for generated data to take effect
    * Each subsequent load will load generated data from the `Custom` .json files
    * `Generated` files will be overwritten with derived data on every load
    * `Custom` files will not be overwritten and will be generated if missing
    * The `Slag-Custom` and `Slag-Generated` are now only for explicitly generating a slag that isn't generated by the ore compat and are not used for the ore compat in any way

  * Added:
    * CrT builder for the worktable recipes (#1)
    * Support for non-hammer tools in the CrT worktable recipes (#1)
    * Bone meal particles to indicate recipe progress when banging on a worktable or anvil
    * Auto generated log -> plank and plank -> slab recipes from other mods (#5)
    * Auto generated ore compat for common ores (#5)
    * Config option to prevent buckets from placing source blocks when broken (#14)

  * Fixed:
    * Conflict with TE causing all wood recipes to output a Chopping Block (#17)
    * Refractory Sawmill recipe tab no longer shows in JEI (#60)

  * Changed:
    * Recipe for Chopping Block now requires a Crude Axe, prevents conflict with TE (#17)
    * Fluid `clay` has been renamed to `liquid_clay` to prevent conflict with TiC fluid `clay` (#57)

---

**1.0.9**

  * NOTE: Remember to refresh (delete and re-run the game) your `Custom` ore dict config file or add the changes manually, changes will only appear in the `Generated` file.

  * Added:
    * Information to the guidebook introduction to draw attention to Pyrotech's sneak + scroll inventory mechanics (#33)
    * `cobblestone` oredict entry for Cobbled Andesite, Cobbled Diorite, Cobbled Granite, Cobbled Limestone (#51)
    * `cobblestoneAndesite` oredict entry for Cobbled Andesite (#51)
    * `cobblestoneDiorite` oredict entry for Cobbled Diorite (#51)
    * `cobblestoneGranite` oredict entry for Cobbled Granite (#51)
    * `cobblestoneLimestone` oredict entry for Cobbled Limestone (#51)

  * Fixed:
    * Sawmill recipes that use a blade the machine is not configured to use should not be displayed in JEI
    * Advancement, Simply Slabs, does not check metadata (#58)

  * Changed:
    * Modified wording of the guidebook entry for Mulched Farmland to clearly state the effect is temporary (#32)
    * Improved list of factors affecting Drying Rack performance (#31)
    * Bloomery iron and gold ore recipes have been changed to use the oredict for input (#51)

---

**1.0.8**

  * Added:
    * Config option to disable milking cows with the buckets (#48)

  * Fixed:
    * Duplicate advancement title (#45)

  * Changed:
    * Update chinese translation (#47 Snownee)

---

**1.0.7**

  * Fixed:
    * Lapis block gives dandelion yellow in anvil (#35)
    * NPE when hammering a bloom from the creative tab (#38)
    * Chopping block should not sound like stone (#40)
    * Refractory glass should not sound like stone (#41)
    * Stash, crate, shelf should not sound like stone (#42)

  * Added:
    * zn_ch.lang (#34 Snownee)

  * Removed:
    * Bloom from creative tab, shouldn't have been in there to begin with (#38)

---

**1.0.6**

  * Added:
    * Limestone block to `stoneLimestone` oredict (#29) - NOTE: Remember to refresh (delete and re-run the game) your `Custom` ore dict config file or add the changes manually, changes will only appear in the `Generated` file.

  * Fixed:
    * Crash when pit burn is lit with door placed on top (door should be placed on the side anyway) (#28)

  * Changed:
    * Improved the guidebook information on excavating flint shards with a shovel

---

**1.0.5**

  * Fixed:
    * Recipe left in worktable doesn't work after logging out and back in
    * Duplicate crude axe recipe in guidebook, missing crude hoe
    * Worktable voids items when it breaks from running out of durability (#24)
    * Anvil recipe conflict for stone, removed stone -> cobblestone hammer recipe (#23)

  * Changed:
    * Split the guide entry for introduction into introduction and campfire entries making it easier to find the campfire instructions
    * Removed advancement restriction on guidebook entries for Flint and Tinder and Bone and Flint Shards; the player should now have all required information necessary to make the campfire and flint and tinder without having to unlock any guidebook entries via advancements

---

**1.0.4**

  * Fixed:
    * Removed conflicting bone meal anvil recipes (#18)
    * Hammer check should occur before pickaxe check (#19)
    * Dedicated server crash (#21)

---

**1.0.3**

  * Fixed:
    * Build filename missing MC version
    * Dedicated server crash (#15)
    * Advancements fail to load when Patchouli mod is not available (#9)
    * Campfire book recipe should not register when Patchouli mod is not available

  * Notes: Players will now receive the root Pyrotech advancement when they pick up any item from the mod or open the Patchouli book given at the start.

---

**1.0.2**

  * Fixed:
    * Error with Thermal Expansion (#8)

---

**1.0.1**

  * Fixed:
    * Repeated grammatical error in guidebook (#10)
    * Dedicated server crash (#11)

---

# 1.0.0

  * Initial beta release

---

0.0.0