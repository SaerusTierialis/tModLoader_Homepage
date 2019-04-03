These idea are not final. If you have feedback or ideas, please share them on our [Discord](https://discord.gg/KXf9zen).


Abilities should do one or more of the following:
* Have a risk/reward element
* Require skill or timing to use
* Create a new playstyle


Abilities should NOT:
* Be "press and forget"
* Grant free damage with no downside


1. Novice
    * No abilities. Low, balanced stats. Power scales all damage types.

1. Melee
    * Scale melee damage only
    * Base ability could be a toggle to increase damage at the cost of defense or vice versa.

    1. Blood Knight
        * _Has a Bloodforce mechanic that regenerates life when high, degenerates life when low, and gradually returns to a midpoint. Abilities drain the resource for powerful effects while simultaneously pushing towards degeneration. Bloodforce can be quickly filled at the cost of life. At any moment, the Blood Knight can focus on building up Bloodforce to sustain (and offset the life cost) or risk death to deal massive damage._
        * Has a Bloodforce resource with a capacity of 100
            * 50 is the base level. Every second, it increases/decreases by 1 towards 50.
            * When <40, life degens
            * When >60, life regens
        * The first ability consumes life to produce Bloodforce
        * Other ablities consume Bloodforce for powerful effects:
            * These effects should be powerful enough to be worth the risk of spending life and/or incurring degen
            * Maybe a toggle that drains Bloodforce to increase Damage
            * Maybe a skill to massively boost the damage of the next hit
            * Maybe a wave that inflicts a strong bleed

    1. Berserker
        * Attack speed class with a rage mechanic of some kind
        * maybe shouts/warcrys?

    1. Guardian
        * Tank class
        * abilities focusing on blocking, generating threat, and perhaps reflecting damage
        * blocking just before receiving an attack should have a bonus

1. Ranged (non-magic projectile classes)
    * Scales ranged and throwing damage
    * Base ability might be a gravity trap that is enhanced by the subclasses

    1. Sniper
        * High damage, crit-focused
        * Snipe ability locks the player in place (even in the air) and prevents the normal use of weapons. The player can then shoot off a few very powerful attacks. Each shot will be more powerful than the last to reward being immobile for longer. The player will be able to end the ability early.
        * Snipe deals bonus damage to enemies caught in the trap
        * Needs more work...

    1. Engineer
        * Scales ranged and throwing damage + minion damage too
        * Projectile minion class
        * Creates a _customizable_ floating Gizmo
             * first, use an active ability to select a weapon that has a projectile, the Gizmo will then use that weapon to attack but the player will be unable to use the weapon (applies to all copies of that weapon)
             * consumes a resource when Gizmo attacks (standardized resource consumption for attack speed of weapon)
             * resource regenerates while out of combat and when the Gizmo is not deployed (i.e., because it broke)
             * Gizmo breaks if resource is depleted
             * Gizmo automatically redeploys once above some resource threshold
             * Gizmo can be hit, which reduces the resource further
             * enemies may target the Gizmo
             * Gizmo damage is based on the weapon and then scaled by the damage type of the projectile AND by minion scaling, the Gizmo will be the player's primary damage
             * To balance the high damage of the Gizmo, player's  damage is massively reduced when resource is low
        * The Engineer should have good sustained damage while the Gizmo is deployed, and should deal massive bursts damage when resource level is high (because player damage will also be high)
        * The rate of resource degen/regen will be fairly quick to keep up the pace, but slow enough to ensure that a low resource level is punishing. The Engineer must protect the Gizmo.
        * Summary of penalties to offset massive Gizmo damage:
             * Gizmo must be kept alive
             * Gizmo cannot attack indefinitely
             * Locks out selected weapon so you can't just make 2 of the best available weapon
             * Player damage is massively reduced by low resource
        * Decision that still need to be made:
             * does Gizmo attack on its own or are its attacks triggered by player attacks? does it attack players most recent target? does it aim at the cursor?
             * is Gizmo stationary? does it follow the player? does it chase down enemies? maybe it is commanded to move to targeted location with an ability?
             * should melee projectiles and magic projectiles be allowed?
             * should have some kind of interaction with the tier 2 trap skill
             * maybe add some more utility? maybe defense mode where it stops attacking but taunts everything around and gains defense?
             * maybe add a skill to recover resource?
             * maybe add a crafted consumable to recover resource (with cooldown)

1. Magic
   * Base ability might be a resource that fills by spending mana and can be expended for a buff that increases damage, but stops mana regen.

    1. Elementalist
        * Damage magic class
        * Elemental attunement mini-game. Use the ability to start rotating through 4 elements (fire/water/earth/air). Use the ability again to select the current element. Each element grants a different buff for a duration.
        * Selecting opposite elements consecutively (fire+water or earth+air) causes the buff to fail, the history to reset, and might consume life/mana.
        * Once you have used all 4 elements at lease once without failing, you will trigger all 4 buffs together for an extended duration.
        * Overall, this class offers primarily damage-focused buffs at the cost of mana and attention.

     1. Sage/Seer/Mystic
         * Utility class
         * No good ideas yet

1. Rogue
   * These classes work well with throwing, but scale most damage types. The base class and Shadow scale minion, but the other classes do not.
   * Base ability could be stealth, a burst of speed, etc.

   1. Assassin
         * Scales all damage types EXCEPT minion (because the core mechanic does not work with minions)
         * Specializes in stealth attacks and one-on-one
         * Attacks from stealth to deal bonus damage
         * Can use any weapons except minion
         * Might gain bonus damage for hitting from behind
         * The stealth attack would deal more damage the closer you are to the target
         * Maybe an ability to mark a target (more damage to this target but less to others), use again to remove mark

   1. Shadow
         * Scales ALL damage types (including minion), but throwing gains added utility. Specializes in escaping danger while trapping enemies.
         * First ability: create a shadow at current locations
              * Shadow vanishes if you get too far away - show a projectile return to the player to make it obvious that this has happened
              * Draw an indicator with the direction of the shadow to make it more intuitive
              * Cast again to switch places with the shadow
         * First ability alternate key toggles a status that causes throwing attacks to _instead_ launch from the shadow's location if a shadow is active
              * might change this to launch throwing weapons from both the player and the shadow at 60% effectiveness each (a damage boost if both hit so long as target doesn't have extremely high defense)
         * Second ability: consume the shadow to inflict shadow trap status on nearby targets, holds targets in place, greatly reduced duration on bosses

   1. Trigger
         * Scales all damage types EXCEPT minion (because the core mechanic does not work with minions)
         * A class that triggers bonus attacks (or spells) by attacking at precise moments
         * Attacking that the right times increases combo and triggers a bonus attack. Attacking at the wrong time breaks combo. Reaching a certain combo count triggers a burst of attacks and resets the combo.
         * The idea is to deal damage through good timing and reacting instead of holding down the attack button as usual. The desired effect is burst damage and minimal resource consumption (bullets/mana/etc.). This may be the most skill-based class.

1. Minion
      * A level 1 ability will summon time-limited minions that do not consume minion cap. The goal of this ability is to give summoners something to use early on that isn't completely useless at high level. These minions will scale with attribute investment, but should fall off in late game.
        * The ability should have a moderate mana cost and short cooldown.
        * These minions should start off grounded and become flying at mid level.
        * Might add an immobile cast time to keep it from being too good in later game.
      * A second ability can recall minions to your location.

      1. Soul Binder
         * Focuses on having a few very strong minions
         * Can sacrifice minion capacity for minion damage. Use the skill repeatedly to cycle through the amount of slots to sacrificed. The overall damage is increased. For example, giving up 1 of 3 minion slots would increase minion damage by >50%.
         * Can toggle on soul binding. This further increases minion damage, but gives each minion a life bar. Minions take damage from projectiles. When the player is hit, the nearest minion also takes damage. When a minion dies, the player takes a decent chunk of damage. Reducing minion cap with the above ability increases minion life. Minion life will regenerate slowly.
         * Will have an ability to heal minions using the player's own life.
         * The two toggle abilities can only be used when no minions are currently summoned
         * If possible, soul binding will affect sentries

      1. Minion Master
         * Gains more control over minions
         * An ability to teleport minions to the cursor
         * An toggle ability that keeps minions near the player. This can be used to allow grounded ranged minions to be used in the air (e.g., tiki) or to keep minions together when moving.
         * An ability that actively commands minions... possibly by throwing them at your enemies. This ability would have a per-minion cooldown. Perhaps the ability would select the minion nearest the cursor and then throw them in the direction that you move the mouse? The goal of the ability would be to have more control over which enemies are being dealt damage and to offer a new way of dealing minion damage. While a minion is being thrown, it would not be attacking normally. Minions with collision damage would lose this while being thrown to prevent dealing both hits. Distance travelled could increase the damage.
         * If possible, these abilities will affect sentries

      1. No Sentry Class
         * The way that sentries are implemented is very messy and hard to work with. Most sentries don't even use sentry capacity and instead just have a hard limit of one per sentry type. No sentry-focused class is planned at this time, but I might revisit this once the other classes are complete. I personally enjoy sentries so I would eventually like to find a way to make it work.

1. Support
      * Mostly unchanged. See [here](./Temporary_Rework_User_Documentation.md)
      * Will have a toggle ability that converts damage bonuses of any weapon type into healing power to allow flexible itemization. This ability cannot be used with the hybrid ability that makes equipment affect all damage types.
      * Might split into two final classes: heal-focused and buff-focused

1. Hybrid (tier 2) and Hybrid Prime (tier 3)
      * Scales all damage types equally
      * Toggle ability to allow damage bonuses from equipment to apply to all damage types (perhaps at 80% value?)
      * Has a resource bar for each damage type except minion
      * Using a weapon while you have its resource offers a large damage boost
      * Using a weapon while its resource is depleted incurs a large damage penalty
      * Every time that you use a weapon, its resource will deplete for a few seconds (not based on attack speed or damage dealt)
      * When any 2 of the 4 resources are emptied, all 4 resources refill
      * The desired effect is that players are rewarded for using multiple damage types (any combination of melee/ranged/magic/throwing) and penalized for using just one
      * Some ideas for enhancing this through passives:
         * When 1 resource is emptied, the other damage types gain a larger bonus
         * Bonus defense while wielding a melee weapon when the melee resource is not empty
         * Bonus mana regen when the magic resource is empty (replenish mana after you've used magic to empty the resource)
      * Note re minions:
         * Most minion weapons use a snapshot of the minion damage so including it here would be very overpowered (minions would keep the bonus after the resource is emptied)
         * The class will still scale minion damage so you can use minions fairly well alongside the other damage types
