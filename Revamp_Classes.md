These idea are not final. If you have feedback or ideas, please share them on our [Discord](https://discord.gg/KXf9zen).

Ability Slots:
* Tier 2 classes have 2 ability slots
* Tier 3 classes retain their tier 2 abilities and have 2 additional slots for a total of 4
* Each class will have at least 2 abilities
* In some cases, a slot may be used for 2 abilities by holding Shift (key can be changed) while pressing the hotkey to active the alternative ability instead.
  * Tier 2 classes can therefore have up to 4 abilities
  * Tier 3 classes can therefore have up to 8 abilities


Abilities should do one or more of the following:
* Have a risk/reward element
* Require skill or timing to use
* Create a new playstyle
* Provide utility or convenience


Abilities should NOT:
* Be "press and forget"
* Grant free damage with no downside


Definition of Channelling:
* Dramatically reduces movement speed
* Cannot attack or use items
* Cannot use most abilities
* Interrupted by taking damage or dying
* Interrupted by frozen, stoned, and silenced
* May require an upkeep cost (mana or resource)


### Tier 1: Novice
* No abilities. Low, balanced stats. Power scales all damage types.

# Close Range (not just melee)
### Tier 2: Warrior
* Damage Scaling:
  * melee with a close-range bonus
  * any close-range non-melee damage (i.e., other damage types when the hit occurs at close range)
* Resource: Poise
  * Regenerates slowly (faster out of combat)
  * Consumed when Guard prevents damage and gradually while holding Guard
  * Scales with Vitality and level
* Ability 1: Guard
  * Channelling ability
  * Reduces 50% of incoming damage from hits (if you have enough Poise)
  * Reduction is increased to 100% for the first 0.5 seconds to reward good timing
  * Maximum damage prevented is equal to defense
* Ability 2: Endure
  * very short duration buff
  * grants immunity to knockback
  * later grants a medium duration defense boost to self and nearby allies

### Tier 3: Blood Knight
* _Has a Bloodforce mechanic that regenerates life when high, degenerates life when low, and gradually returns to a midpoint. Abilities drain the resource for powerful effects while simultaneously pushing towards degeneration. Bloodforce can be quickly filled at the cost of life. At any moment, the Blood Knight can focus on building up Bloodforce to sustain (and offset the life cost) or risk death to deal massive damage._
* Resource: Bloodforce
  * Capacity is 100
  * 50 is the base level. Every second, it increases/decreases by 1 towards 50.
  * When <40, life degenerates
  * When >60, life regenerates
  * Generated when hitting an enemy at close range
* Ability 1: Sacrifice
  * Consume life to generate Bloodforce
* Ability 1 Alternate: Blood Rage
  * Toggles a status that drains Bloodforce to increase Damage and attack speed, but decreases defense
* Ability 2 and 2 Alternate: ???
  * consume Bloodforce for powerful effects:
    * These effects should be powerful enough to be worth the risk of spending life and/or incurring degeneration
    * Maybe a skill to massively boost the damage of the next hit
    * Maybe a wave that inflicts a strong bleed

### Tier 3: Guardian (WIP)
* Tank class
* Passive to reduce/remove the slow from channelling (for Guard)
* Ability Ideas:
  * Barrier in front of player (moves with player) that pushes enemies and stops projectiles
  * Hook on to one or more enemies. Pulls them in until they're within a certain distance. Reduce damage from hooked enemies.
    * Does not pull bosses or knockback-immune enemies, but still reduces damage from them
  * Link to allies to take half of their damage for them
  * Reflect incoming damage
  * Force all nearby enemies to switch to target you

### Tier 3: Berserker? (WIP)
* Attack speed class?
* Rage mechanic?
  * Gain Rage with each close-range hit
  * Increases melee attack speed proportional to Range
  * Ability to consume rage and grant super rage buff

# Projectile (not just ranged)
### Tier 2: Name?
* Damage Scaling:
  * ranged, magic, and throwing
  * Projectiles from melee weapons
* Resource: Preparation
    * this resource is consumed instead of ammo items (1:1) and throwing items (1:5)
    * also consumed to reduce the mana cost of weapon attacks
    * slowly refills when you have not used the resource recently
* Ability 1: Trap
  * launch a floating trap towards the cursor
    * the maximum distance increases with level
  * enemies that touch the trap are damaged and briefly held in placed
    * bosses and enemies that are immune to knockback are slowed instead
  * traps last a set duration
* Ability 2: Rapid Fire
  * gain a brief boost to ranged/throwing/magic attack speed followed by a brief "Reload" debuff that prevents attacking

### Tier 3: Artillery
* High damage, critical-focused, burst damage class that rewards good aim
* Tier 2 Ability Notes:
  * Trap now causes the enemy to take triple damage from the next hit by this player
  * Rapid Fire increases charge-up rate of Charged Shot
* Resource: Precision
    * Hits with Charged Shot generate 1 Precision (once per shot, not per target hit)
    * Missing with Charged Shot reduces Precision by half
    * Each Precision increases the base critical chance of Charged Shot and Mega Shot by 5% up to 10 stacks (50% base crit)
    * Stacking precision can virtually guarantee a critical hit
* Ability 1: Charged Shot
  * Channelling ability
  * Works with any weapon that has a projectile (that isn't a minion)
  * Press and hold the key to charge, release to shoot an empowered attack
  * Damage and critical chance are increased based on the charge amount
    * At max charge, the critical rate bonus is equivalent to rolling the critical check twice and taking the better roll (i.e., 2 chances to crit). Rather than reroll on a failed crit, the crit chance is just multiplied as follows before rolling:
      * new_crit = 1 - (1-crit)^2
        * _this is the probability of not failing to crit twice_
      * Examples:
        * 5%  => 9.75%
        * 20% => 36%
        * 50% => 75%
        * 75% => 93.75%
  * Charge-up rate is based on weapon's use speed
  * An indicator is shown when charge reaches maximum
  * No cooldown and low mana cost. This is the core ability of the Sniper so it can be used repeatedly as an alternative to holding down the fire button.
    * weapon's mana cost is added to the ability cost
  * Average speed of charging to max should take a few seconds, but the multiplier should feel rewarding (worth the time not attacking) even when released earlier
* Ability 1 Alternate: Toggle Charged Shot
  * Toggles switching regular attacks with the mouse to be Charged Shots (press and hold mouse, then release)
* Ability 2: Mega Shot
  * Shoots a single massively empowered projectile from the held weapon
    * Scale with base use time so that faster weapons aren't that much worse
  * Prevents the use of any weapon (including abilities) for 3 seconds
    * 30 seconds for the weapon type used (i.e., affects all weapons of the same type - e.g., all Minishark)

### Tier 3: Tinkerer
* Projectile/minion hybrid class
* Partially scales minion damage in addition to projectiles
* Tier 2 Ability Notes:
  * Rapid Fire affects Gizmo as well
  * Ammo resource is used for Gizmo resources
* Ability 1: _customizable_ Gizmos
  * Created by holding a weapon and using the ability. The Gizmo will copy the weapon (projectile, rate of attack, damage). Each Gizmo must use a different weapon. The weapons used by Gizmos cannot be used by the player. This includes all copies of that weapon.
    * Example: Only one Gizmo can be created from a Minishark and doing so will prevent the player from using any Minishark while that Gizmo is deployed.
    * Any weapon with a projectile (that isn't a minion) will work
  * Gizmos consume ammo from the player's inventory
    * If a mana-consuming weapon is used, then the player's mana is consumed but the cost is reduced
  * Up to 4 Gizmos can be deployed at once, but each requires a minion slot
  * Each deployed Gizmo decreases the player's final damage by 20% (80% reduction if the max number of Gizmos are deployed)
  * Gizmos follow the player closely and attack the nearest target that they have line-of-sight to
  * Gizmo damage is scaled by the type of the weapon in addition to minion bonuses
  * Gizmos stop attacking while the player is dead, but are not destroyed. You'll need to recreate them every time you enter a world but not every time you die.
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

### Tier 3: Chrono
* *A time-based combo class that triggers bonus attacks by attacking at precise moments and can even jump back in time. This class is meant to be somewhat challenging to play, but has high potential.*
* Mechanic: Combo Mechanic
  * Shortly after each attack, you will be prompted to attack again. If you attack at the right time, your combo will increase by 1. If not, the combo breaks.
  * At each multiple of 5 combo points, a flurry of bonus projectiles are unleashed
    * Higher combo counts produce more projectiles
  * Weapon use time (including the bonus from rapid fire) scales:
    1. the time between attacking and being prompted to attack again (the delay should be fairly short and slightly random)
    1. the time window during which attacking results in a combo
* Resource: Memories
  * Every 3 seconds, the player's location and combo count is recorded in a memory
  * Up to 5 memories can be stored (15 seconds)
  * Gaining a memory while at capacity erases the oldest memory
  * The location of the most recent memory is marked
* Ability 1: Time Jump
  * Jumps back to the most recent memory (consumes that memory)
    * The player is teleported to the location
    * The combo count is set to the value it had been at that time
  * Can be used multiple times in a row to jump back in sequence, but the memories are consumes so you can run out of memories to jump to
* Ability 2: Redo
  * Similar as Time Jump except half of the life lost is restored
    * Also, it jumps back to the memory with the highest life and consumes the more-recent memories along the way
    * Makes it worthwhile to keep an old memory in the queue, but doing so requires frequent jumps - makes it difficult to build combo
  * 5 minute cooldown
  * Example:
    * The memory has 200 life and the player current has 20 life
    * They have lost 180 life so they will gain 90
    * The player's new life amount will be 110

# Trickery
### Tier 2: Rogue
  * Damage Scaling:
    * all damage types with a bonus for close-range hits
  * Mechanic: Attacks of Opportunity
    * Additional damage when hitting an enemy from behind
    * Additional damage when hitting an enemy that is not targeting you
  * Mechanic: Sneak Attack
    * Hitting a target while in stealth deals massive damage (removes stealth)
    * The damage is increased relative to how close the target is to the player (closer = more damage)
  * Ability 1: Stealth
    * Toggle ability
    * Drains mana while active
    * Reduces movement speed (no reduction at later levels - might even gain a movement speed bonus)
    * You cannot enter stealth if an enemy is nearby
    * Reduces aggro, making enemies unlikely to target you
    * Removed by taking or dealing damage
  * Ability 2: Dodge
    * Gain a burst of speed in the direction of the cursor
    * Cannot be hit during the dodge

### Tier 3: Shadow
  * The Shadow can weave in an out of melee-range to easily re-stealth and trigger a sneak attack. They also have the utility of attacking from two locations at once.
  * Tier 2 Notes:
    * Stealth no longer has a mana cost
  * Ability 1: Shadow
    * Creates a shadow at the current location
    * Cast again to switch places with the shadow and gain Stealth
      * also restores the Shadow's life
    * The Shadow can be targeted and destroyed by enemies
    * You must be in Stealth to create a shadow
    * Shadow vanishes if you move too far away
      * Show a projectile return to the player to make it obvious that this has happened
    * Draw an indicator with the direction of the shadow to make it more intuitive
  * Ability 1 Alternate: Shadow Attack
    * Toggles a status that causes your Shadow to duplicate your attacks
    * Reduces damage to 60% each
  * Ability 2: Shadow Trap
    * Consume the shadow to inflict a status on nearby targets that holds them in place and reduces their defense
      * Bosses and knockback-immune targets are slowed instead of held

### Tier 3: Assassin
  * *The Assassin tries to get as much out of one Stealth as possible. They can whittle down their opponents with Covert Attacks from stealth and then finally break the Stealth with a massive Sneak Attack that inflicts a powerful poison. Assassins have both burst damage and damage-over-time. They specialize in getting into close-range and doing massive damage.*
  * Tier 2 Notes:
    * Sneak Attacks are now deal double damage and are always a critical hit
  * Passive: Poison
    * Critical hits inflict a damage-over-time poison based on the damage dealt
    * A target can have several poisons at once
      * The actual limit is 255
  * Ability 1: Covert Attack
    * An close-range attack that can only be used while in Stealth
    * Does not break Stealth
    * When hitting from behind, damage is doubled and critical is guaranteed
    * Several seconds cooldown
  * Ability 1 Alternate: Ambush
    * Instantly move to the enemy nearest the cursor
  * Ability 2: Poison Shroud
    * Create a cloud of poison that inflicts poison on enemies at set intervals
    * While in the shroud, you can enter Stealth even if enemies are nearby and Stealth has no mana cost
  * Ability 2 Alternate: Instant Poison
    * End all poisons on nearby enemies to deal half of the remaining damage-over-time instantly

# Minion (pure minion stuff)
### Tier 2: Summoner
* *Summoner provides an early-game source of minion damage and a bunch of minion utility.*
* Passive: Floating Sentry
  * Allow all sentries to be placed in the air
* Ability 1: Name?
  * Creates time-limited minions that scale with level/attributes
  * Does not consume minion cap, but the max number of these is limited by cap (1/minion cap and 2/sentry cap)
    * Example: If you have 3 minion slots and 1 sentry slot then you can have 5 of these
  * Requires a short channel time (move slowly, but not attack or use items during this)
  * Start off grounded and become flying at later level
  * Maintaining several of these will consume a considerable amount of mana and require you to spend a lot of time channeling, which puts the player in danger
  * The goal is for this to be a core ability early on, and act as filler for when you have a safe moment in later game
* Ability 1 Alternate: Sentry Mode
  * A cycling toggle ability to convert minion slots into sentry slots at a 2:1 ratio (use multiple times to select number of slots to convert)
  * This will allow players to build around sentries while wearing the standard minion armor if they so choose
* Ability 2: Command
  * commands all minions to switch to the target nearest the cursor (some mod minion's AIs might not work with this)
* Ability 2 Alternate: Recall
  * teleports all minions (including sentries) to the player

### Tier 3: Soul Binder
* *Soul Binders have relatively few minions, but they are much stronger than normal. Their minions are also targetable/destroyable and the player takes damage if a minion dies. Soul Binders transfer life between themselves and their minions, and they can even consume a minion for a damage boost.*
* Mechanic: Condense
  * Reduce minion cap to increase minion damage
  * Overall, damage is increased and less spread out
* Mechanic: Minion Souls
  * Minions become targetable and can be destroyed, but deal 25% more damaged
  * When a slot-requiring minion dies, the Soul Binder takes damage based on how much health the minion had
  * Minion health is based on:
    * Level
    * Spirit attribute
    * Number of slots that the minion uses
    * Condense
  * Minions must be summoned again if they die
  * Sentries are included
  * Minion life regenerates slowly while out of combat
* Ability 1: Share Life
  * Consume some player life to heal the most injured minion
* Ability 1 Alternate: Siphon life
  * Consume some life from the least injured minion to heal the player
* Ability 2: Consume Soul
  * Consume your most injured minion (hurts player) to boost damage for a short time
* Ability 2 Alternate: Vampiric Soul
  * Marks the enemy for a short times
  * Minion hits against the target heal the most injured minion
  * Long cooldown
  * This ability will help the Soul Binder to sustain minions in difficult boss fights

### Tier 3: Placeholder Class
* This will be replaced with an actual class later
* In the meantime, this is a tier 3 class with access to the Summoner skills that does not make your minions destructible

# Utility (all damage types)
### Tier 2: Traveler
* Damage Scaling:
  * all
* Passive: Return to the Scene of the Crime
  * On respawn, the Traveler has the ability to return to their place of death by pressing the teleporter activation key while at the respawn point
* Ability 1: Teleport
  * teleport towards the cursor
  * at higher level, does not require line-of-sight
  * longer cooldown in combat
* Ability 1 Alternate: Long-Range Teleport
  * teleports to a position in the direction of the cursor that is 10x the distance from the player to the cursor
    * if that location is invalid, teleport to a nearby location
  * longer cooldown than basic teleport
  * longer cooldown in combat
* Ability 2: Place Teleporter A
  * places a teleporter
  * while out of combat, any player can freely move between the teleporters by pressing an activation hotkey
  * teleporters cannot be placed directly on the respawn point
* Ability 2: Place Teleporter B
  * places the second teleporter

### Tier 3: Controller
* Ability 1: Black Hole - Projectiles
  * Creates a black hole which pulls nearby projectiles towards it
  * Affects both friendly and hostile projectiles
  * The pull is stronger towards the center
  * Not strong enough to trap projectiles unless they are very slow or pass near the center
  * The number is limited only by cooldown
* Ability 1 Alternate: Force Field - Projectiles
  * Creates a force field which pushes away nearby projectiles
  * Affects both friendly and hostile projectiles
  * The push is stronger towards the center
  * May completely deflect slow projectiles and those that pass near the center
  * The number is limited only by cooldown
* Ability 2: Black Hole - Enemies
  * Same as "Black Hole - Projectiles" but affects enemies instead
    * Weaker pull
    * Limited to 1 at a time
* Ability 2: Force Field - Enemies
  * Same as "Force Field - Projectiles" but affects enemies instead
    * Weaker push
    * Limited to 1 at a time
* These abilities do no push/pull minions, but can push/pull their projectile attacks

# Support (WIP)
* Mostly unchanged from pre-revamp cleric. See [here](./Temporary_Rework_User_Documentation.md)
* Will have a toggle ability that converts damage bonuses of any weapon type into healing power to allow flexible itemization. This ability cannot be used with the hybrid ability that makes equipment affect all damage types.
* Remove Sanctuary teleport (moved to anther class)
* Potential changes:
   * Remove paragon abilities for something more interesting
   * Rework heal
* Might split into two final classes: heal-focused and buff-focused
* Maybe add a debuff/degen class?
* Maybe a support/minion class that has a healing minion

# Hybrid (use multiple damage types together) (WIP)
### Hybrid (tier 2) and Hybrid Prime (tier 3)
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

# Non-Combat Class
### Tier 2: Explorer
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

# Other/Old ideas
### Elementalist
* Damage magic class
* Elemental attunement mini-game. Use the ability to start rotating through 4 elements (fire/water/earth/air). Use the ability again to select the current element. Each element grants a different buff for a duration.
* Selecting opposite elements consecutively (fire+water or earth+air) causes the buff to fail, the history to reset, and might consume life/mana.
* Once you have used all 4 elements at lease once without failing, you will trigger all 4 buffs together for an extended duration.
* Alternatively, the element system could instead store charges rather than trigger buffs. A second ability could be used to release the charges. Releasing charges could trigger large spell effects (meteors, etc). Still, there would be a max of 4 charges and opposite element charges could not be added consecutively. A unique effect would be triggered if you have all 4 elements. Duplicates of the same element would empower that elements effect (e.g., 2 fire + 2 earth = empowered fire and earth effects).
* A tornado ability that pulls monsters in (more suction the closer they are) and deals damage. An upgrade could add lightning. If the charge version of attunement is used then this could be the wind spell.
* Overall, this class offers primarily damage-focused effects at the cost of mana and attention.
* Attunement could be something that you prepare before a difficult fight. During boss fights, it might be challenging to get the attunement that you want with everything else going on.

### Elementalist 2 (from Discord suggestion)
Elementalist could have 4 abilities (fire,wind,water,earth) the more he use one element, the more attune he is to that element, giving specific buff and debuff depending on the element: Fire attunement could increase damage by a lot but will cut health regen and reduce defence, Earth would bolster your defense and your health regen but slow you down, Water could increase all the mana variables at the cost of spell power , wind would greatly increase your movements but reduce your defence and, at once point, remove knockback immunity is any and increase knockback when hit

### Sage/Seer
* Utility and/or buff and/or debuff class?
* Has a certain number of orbs. An ability is used to fire an orb to the targeted location. Using the ability when all orbs are already out launches the farthest away orb to the cursor location. An alternate ability recalls all orbs. When orbs are moving, they deal damage to anything they pass through.
* Other abilities would trigger on each fielded orb (e.g., create a debuff aura around each orb)
* Maybe a player-cented aura that boosts attributes of nearby allies? The abillity itself could be recast to cycle between the attributes so you could pick what kind of effect to grant? (this could be given to another class if not this one)

### Minion Master (weak idea - need something better for making minions interactive) (WIP)
* Gains more control over minions
* An ability to teleport minions to the cursor
* An toggle ability that keeps minions near the player. This can be used to allow grounded ranged minions to be used in the air (e.g., tiki) or to keep minions together when moving.
* An ability that actively commands minions... possibly by throwing them at your enemies. This ability would have a per-minion cooldown. Perhaps the ability would select the minion nearest the cursor and then throw them in the direction that you move the mouse? The goal of the ability would be to have more control over which enemies are being dealt damage and to offer a new way of dealing minion damage. While a minion is being thrown, it would not be attacking normally. Minions with collision damage would lose this while being thrown to prevent dealing both hits. Distance travelled could increase the damage.
* If possible, these abilities will affect sentries

### Sentry Class
* Passive (or toggle) to allow sentries to be placed in the air
* Ability that spawns several sentries in a vertical line that attack for a few seconds before disappearing. The sentry placed could be from whichever sentry weapon you held most recently.

### Maybe a spirit/necromancer class?
