These idea are not final. If you have feedback or ideas, please share them on our [Discord](https://discord.gg/KXf9zen).


Abilities should do one or more of the following:
* Have a risk/reward element
* Require skill or timing to use
* Create a new playstyle


Abilities should NOT:
* Be "press and forget"
* Grant free damage with no downside


# Novice
* No abilities. Low, balanced stats. Power scales all damage types.

# Melee
* Scale melee damage only
* Base ability could be a toggle to increase damage at the cost of defense or vice versa.
* Maybe rework these classes to work for other damage types so long as the hits occur within close-range?

### Blood Knight (concept nearly complete)
* _Has a Bloodforce mechanic that regenerates life when high, degenerates life when low, and gradually returns to a midpoint. Abilities drain the resource for powerful effects while simultaneously pushing towards degeneration. Bloodforce can be quickly filled at the cost of life. At any moment, the Blood Knight can focus on building up Bloodforce to sustain (and offset the life cost) or risk death to deal massive damage._
* Resource: Bloodforce
  * Capacity is 100
  * 50 is the base level. Every second, it increases/decreases by 1 towards 50.
  * When <40, life degenerates
  * When >60, life regenerates
* Ability 1: Sacrifice
  * Consume life to create Bloodforce
* Ability 1 Alternate: Blood Rage
  * Toggles a status that drains Bloodforce to increase Damage
* Ability 2 and 2 Alternate: ???
  * consume Bloodforce for a powerful effect:
    * These effects should be powerful enough to be worth the risk of spending life and/or incurring degeneration
    * Maybe a skill to massively boost the damage of the next hit
    * Maybe a wave that inflicts a strong bleed

### Guardian
* Tank class
* Abilities could include blocking, generating threat, perhaps reflecting damage, etc.
* blocking just before receiving an attack should have a bonus
* Might have an ability that hooks on to a target and pulls them in. Could receive less damage from hooked enemies. At high level, could hook all nearby targets that you have sight of. This skill would not pull targets that are immune to knockback. In boss fights it could reduce incoming damage from the boss and help group up the adds.

### Maybe a Rune Knight or Magic Knight?
* something to add range or projectiles to pure melee weapons?

# Ranged (non-magic projectile) (concept complete)
* Scales ranged and throwing damage
* Ability 1: Trap
  * launches a floating trap towards the cursor
    * the maximum distance increases with level
  * enemies that touch the trap are briefly held in placed
    * bosses and enemies that are immune to knockback are slowed instead
  * traps last a set duration
* Ability 2: Rapid Fire
  * gain a brief boost to ranged/throwing attack speed followed by a brief "Reload" debuff that prevents attacking
* Resource: Ammo
  * this resource is consumed instead of ammo items (1:1) and throwing items (1:5)
  * slowly refills when you have not used the resource recently

### Sniper (concept nearly complete)
* High damage, critical-focused, burst damage class that rewards good timing and aim
* Tier 2 Abilities:
  * Trap inflicts a status that causes the next hit to deal triple damage
  * Rapid Fire increases charge-up rate of Charged Shot
* Ability 1: Charged Shot
  * Press and hold the key to charge, release to shoot an empowered attack in the direction of the cursor
    * Cannot attack, use items, or use abilities while channeling. Getting hit interrupts channeling.
  * Damage and critical chance are increased based on the charge amount
    * At max charge, the critical rate bonus is equivalent to rolling the critical check twice and taking the better roll (i.e., 2 chances to crit). Rather than reroll on a failed crit, the crit chance is just multiplied as follows before rolling:
      * new_crit = 1 - (1-crit)^2
        * _this is the probability of not failing to crit twice_
      * Examples:
        * 5%  => 9.75%
        * 20% => 36%
        * 50% => 75%
        * 75% => 93.75%
  * Works with any projectile weapon
  * Charge-up rate is based on attack speed and weapon's use speed
  * An indicator is shown when charge reaches maximum
  * No cooldown and low mana cost. This is the core ability of the Sniper so it can be used repeatedly as an alternative to holding down the fire button.
  * Average speed of charging to max should take a few seconds, but the multiplier should feel rewarding (worth the time not attacking) even when released earlier
* Resource: Precision
  * Hits with Charged Shot generate 1 Precision (once per shot, not per target hit)
  * Missing with Charged Shot reduces Precision by half
  * Each Precision increases Charged Shot's base critical chance by 5% up to 10 stacks
* Ability 2: ???
  * I'm open to suggestions on discord

### Engineer (concept complete)
* Projectile minion class
* Scales ranged and throwing damage + minion damage too
* Tier 2 Abilities:
  * Trap activation creates a gravity well that pulls enemies in (does not affect bosses or knockback-immune)
  * Rapid Fire affects Gizmo as well
  * Ammo resource is used for Gizmo resources
* Ability 1: _customizable_ Gizmos
  * Created by holding a weapon and using the ability. The Gizmo will copy the weapon (projectile, rate of attack, damage). Each Gizmo must use a different weapon. The weapons used by Gizmos cannot be used by the player. This includes all copies of that weapon.
    * Example: Only one Gizmo can be created from a Minishark and doing so will prevent the player from using any Minishark while that Gizmo is deployed.
    * Any weapon with a projectile (that isn't a minion) will work
  * Gizmos consume ammo from the player's inventory
  * Up to 4 Gizmos can be deployed at once, but each requires a minion slot
  * Each deployed Gizmo decreases the player's final damage by 20% (80% reduction if the max number of Gizmos are deployed)
  * Gizmos follow the player closely and attack the nearest target that they have line-of-sight to
  * Gizmo damage is scaled by the type of the weapon in addition to minion bonuses
* Ability 1 Alternate: Destroy Gizmos
  * Destroy all active Gizmos
* Ability 2 : Command
  * commands one Gizmo to fly to the targeted location (requires line-of-sight) and attack from there
  * The Gizmo will stay there until the player is too far away or until commanded again
  * Using the ability multiple times commands other Gizmos that are still following the player
  * If all Gizmos have valid locations, then using the ability will command the least-recently-commanded Gizmo
* Ability 2 Alternate: Recall
  * recalls all Gizmos to the player at once (they fly back to the player - not teleport)
* The penalties to offset the high damage are:
  * Uses minion slots
  * Greatly reduces player damage
  * Requires several decent weapons
  * Requires micro-managing of Gizmo placement when having them follow the player is not ideal

# Magic
* Base ability might be a resource that fills by spending mana and can be expended for a buff that increases damage, but stops mana regen.
* Maybe a toggled mana-barrier? (half damage taken from mana first)
* Maybe a teleport?

### Elementalist
* Damage magic class
* Elemental attunement mini-game. Use the ability to start rotating through 4 elements (fire/water/earth/air). Use the ability again to select the current element. Each element grants a different buff for a duration.
* Selecting opposite elements consecutively (fire+water or earth+air) causes the buff to fail, the history to reset, and might consume life/mana.
* Once you have used all 4 elements at lease once without failing, you will trigger all 4 buffs together for an extended duration.
* Alternatively, the element system could instead store charges rather than trigger buffs. A second ability could be used to release the charges. Releasing charges could trigger large spell effects (meteors, etc). Still, there would be a max of 4 charges and opposite element charges could not be added consecutively. A unique effect would be triggered if you have all 4 elements. Duplicates of the same element would empower that elements effect (e.g., 2 fire + 2 earth = empowered fire and earth effects).
* A tornado ability that pulls monsters in (more suction the closer they are) and deals damage. An upgrade could add lightning. If the charge version of attunement is used then this could be the wind spell.
* Overall, this class offers primarily damage-focused effects at the cost of mana and attention.
* Attunement could be something that you prepare before a difficult fight. During boss fights, it might be challenging to get the attunement that you want with everything else going on.

### Sage/Seer
* Utility and/or buff and/or debuff class?
* Has a certain number of orbs. An ability is used to fire an orb to the targeted location. Using the ability when all orbs are already out launches the farthest away orb to the cursor location. An alternate ability recalls all orbs. When orbs are moving, they deal damage to anything they pass through.
* Other abilities would trigger on each fielded orb (e.g., create a debuff aura around each orb)
* Maybe a player-cented aura that boosts attributes of nearby allies? The abillity itself could be recast to cycle between the attributes so you could pick what kind of effect to grant? (this could be given to another class if not this one)

# Rogue
* These classes work well with throwing, but scale most damage types.
* Base abilities could be stealth, a burst of speed, dodge, etc.

### Assassin (work in progress)
* Scales all damage types EXCEPT minion (because the core mechanic does not work with minions)
* Specializes in stealth attacks and one-on-one
* Attacks from stealth to deal bonus damage
* Might gain bonus damage for hitting from behind
* The stealth attack would deal more damage the closer you are to the target (but does work with projectiles)
* Maybe an ability to mark a target (more damage to this target but less to others), use again to remove mark
* Maybe a shadow step ability to warp beside the enemy nearest the cursor (require line of sight)

### Shadow (concept nearly complete)
* Scales all damage types (including minion)
* Specializes in escaping danger while trapping enemies
* Ability 1: Shadow
  * Creates a shadow at the current location
  * Shadow vanishes if you get too far away - show a projectile return to the player to make it obvious that this has happened
  * Draw an indicator with the direction of the shadow to make it more intuitive
  * Cast again to switch places with the shadow
  * Shadow can be destroyed by enemies
  * While you have a Shadow, it duplicates any attacks but you and the Shadow deal only 60% damage
* Ability 2: Shadow Trap
  * Consume the shadow to inflict a status on nearby targets that holds them in place and reduces their defense
    * Might instead slow bosses and knockback-immune targets
* Might need something more - maybe enhancements to the tier 2 abilities

### Chrono (concept nearly complete) *might be switched to ranged or mage class*
* A class that triggers bonus attacks (or spells) by attacking at precise moments
* Scales all damage types except minion
* The goal would be to consistently combo, trigger the combo burst, and then use Time Jump to restore the combo count and keep going.
* This class is meant to be challenging to play, but has very high potential. You would need to keep track of the combo bar, the location of your latest memory (so you don't jump into danger), how close you are to a combo burst, how soon the next memory will form, etc.
* Combo Mechanic:
  * A bar above the character cycles between filling and emptying
    * higher attack speed and weapon use speed increases the rate of filling/emptying so that there is less waiting
  * Attacking when the bar is above a marked point increases combo and triggers a bonus attack
  * Attacking when the bar is too low breaks the combo (back to 0)
  * Reaching a certain combo count triggers a burst of attacks and resets the combo
    * This is a significant burst of damage
* Ability 1: Time Jump
  * Every 3 seconds, the player's location and combo count is recorded tracking up to 5 memories (15 seconds)
  * Using this ability jumps the player back to the most recent memory (and destroys that memory)
    * The player is teleported to their prior locations
    * The combo count is set to the value it had been at that time
  * The location of the most recent memory is marked
  * The number of memories held is shown in a resource bar
  * Can be used multiple times in a row to jump back several times, but the memories are destroyed so this can't be done often
* Ability 2: ???
  * I'm open to suggestions on discord

### Maybe a poison/bleed class?
* Portion of damage inflicted as damage-over-time instead?

# Minion (concept complete)
* First Ability: temporary minions
  * A minion attack that is available right at unlock to give players something to use early on
  * Creates time-limited minions that scale with level/attributes
  * Does not consume minion cap, but the max number of these is limited by cap (1/minion cap and 2/sentry cap)
    * Example: If you have 3 minion slots and 1 sentry slot then you can have 5 of these
  * Requires a short channel time (move slowly, but not attack or use items during this)
  * Start off grounded and become flying at later level
  * Maintaining several of these will consume a considerable amount of mana and require you to spend a lot of time channeling, which puts the player in danger
    * The goal is for this to be a core ability early on, and act as filler for when you have a safe moment in later game
* First Ability Alternate (not related to first ability but each class has only 2 ability slots)
  * A cycling toggle ability to convert minion slots into sentry slots at a 2:1 ratio (use multiple times to select number of slots to convert)
* Second Ability: Command
  * commands all minions to switch to the target nearest the cursor (some mod minion's AIs might not obey this)
* Second Ability Alternate: Recall
  * teleports all minions back to the player
  * sentries are teleported to nearest valid location if there is one

### Soul Binder
* Focuses on having a few very strong minions
* Can sacrifice minion capacity for minion damage. Use the skill repeatedly to cycle through the amount of slots to sacrificed. The overall damage is increased. For example, giving up 1 of 3 minion slots would increase minion damage by >50%.
* Can toggle on soul binding. This further increases minion damage, but gives each minion a life bar. Minions take damage from projectiles. When the player is hit, the nearest minion also takes damage. When a minion dies, the player takes a decent chunk of damage. Reducing minion cap with the above ability increases minion life. Minion life will regenerate slowly.
* Will have an ability to heal minions using the player's own life.
* The two toggle abilities can only be used when no minions are currently summoned
* If possible, soul binding will affect sentries

### Minion Master
* Gains more control over minions
* An ability to teleport minions to the cursor
* An toggle ability that keeps minions near the player. This can be used to allow grounded ranged minions to be used in the air (e.g., tiki) or to keep minions together when moving.
* An ability that actively commands minions... possibly by throwing them at your enemies. This ability would have a per-minion cooldown. Perhaps the ability would select the minion nearest the cursor and then throw them in the direction that you move the mouse? The goal of the ability would be to have more control over which enemies are being dealt damage and to offer a new way of dealing minion damage. While a minion is being thrown, it would not be attacking normally. Minions with collision damage would lose this while being thrown to prevent dealing both hits. Distance travelled could increase the damage.
* If possible, these abilities will affect sentries

### Sentry Class?? (might not be made)
* Passive (or toggle) to allow sentries to be places in the air
* Ability that spawns several sentries in a vertical line that attack for a few seconds before disappearing. The sentry placed could be from whichever sentry weapon you held most recently.

# Support
* Mostly unchanged. See [here](./Temporary_Rework_User_Documentation.md)
* Will have a toggle ability that converts damage bonuses of any weapon type into healing power to allow flexible itemization. This ability cannot be used with the hybrid ability that makes equipment affect all damage types.
* Potential changes:
   * Remove paragon abilities for something more interesting
   * Rework heal
* Might split into two final classes: heal-focused and buff-focused
* Maybe add a debuff/degen class?

### Maybe a support/minion class that creates healing minions?
* Maybe have a skill to attach them to players/recall them back?

# Hybrid (tier 2) and Hybrid Prime (tier 3)
* Scales all damage types equally
* Toggle ability to allow damage bonuses from equipment to apply to all damage types (perhaps at 80% value?)
* Has a resource bar for each damage type except minion
* Using a weapon while you have its resource offers a large damage boost
* Using a weapon while its resource is depleted incurs a large damage penalty
* Every time that you use a weapon, its resource will deplete for a few seconds (not based on attack speed or damage dealt)
* When any 2 of the 4 resources are emptied, all 4 resources refill
* The desired effect is that players are rewarded for using multiple damage types (any combination of melee/ranged/magic/thowing) and penalized for using just one
* Trigger a buff on switching held item/weapon. The buff would only affect the new weapon and it would have a weapon-specific cooldown that is longer than the duration. This would reward players for switching weapons frequently while also preventing players from switching right back to the same weapon immediately. Overall, this would offer a way to keep damage up in the short term while you work on emptying the resources in the longer term.
* Some ideas for enhancing this through passives:
   * When 1 resource is emptied, the other damage types gain a larger bonus
   * Bonus defense while wielding a melee weapon when the melee resource is not empty
   * Bonus mana regen when the magic resource is empty (replenish mana after you've used magic to empty the resource)
* Note re minions:
   * Most minion weapons use a snapshot of the minion damage so including it here would be very overpowered (minions would keep the bonus after the resource is emptied)
   * The class will still scale minion damage so you can use minions fairly well alongside the other damage types

# Explorer
* A tier 2 class with a max level of 100 (same as tier 3s)
* Power attribute scales fishing power
* Dexterity attribute scales tool use time (pickaxe/axe/hammer/etc)
* Will eventually gain bonuses such as spelunker effect
* Eventually, you'll be able to gain non-combat xp, but in the meantime you can funnel your orbs into this class (it has fairly low xp requirements)
* Maybe a resource-harvesting drone???
  * When it has line-of-sight to a tree, it'll fly over and whittle away at it
  * When minerals are nearby, it'll dig its way through the terrain to get to the mineral and then mine it
  * Use chopping/mining power equal to best in inventory
  * Collect resources for the player (maybe even have a capacity and fly back to owner when full to deposit)
