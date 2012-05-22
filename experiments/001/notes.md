# Notes

## Overview

### Stance

* Surprised combatants have no stance. They do not allocate their prowess until
the surprise round is over.
* During the first round of combat, after everyone rolls initiative, the
combatant with the *lowest* initiative declares his stance first, then the
second lowest, and so on until the character with the *highest* inititative
declares his stance. That character then takes his turn, and combat progresses
as normal.
* During any round of combat other than the first, characters declare their
stance at the beginning of their turn.


### Maneuvers

* If you are surprised, you get no maneuvers.
* During the first

How many

### Resistance

Resistance is the damage threshold an attacker must exceed in order to cause
damage to an opponent. Under experiment 1 -- Ftr5 vs Bbn5 -- it was broken
as shit. We used this calculation:

> [health] + [CON+] + [clvl] + [warmor] + [narmor] + [hp]/10 (round down)

* _CON+_: Your Constitution bonus
* _health_: The number of health boxes you have when unwounded
* _clvl_: Your character level. Do not include template levels
* _warmor_: The armor bonus from your worn armor
* _narmor_: Your natural armor bonus
* _hp_: Your current hitpoints


The reason it was broken was that it was rare that combatants could damage one
another. Exceeding resistance required an explosion of the damage dice
(12.5% chance on a d8). The system unneccessarily over-favored burst damage,
further over-empowering spellcasters.

Our solution during the experiment was to add the excess of the hit roll to
damage. While this yielded some success, I would like to discard this result
for a few reasons:

1. It nerfs power attack.
2. It makes critical hits less special.
3. It adds an additional calculation to the already-heavy new combat system.

There are two ways to fix the problem of "no one ever gets damaged":

1. Increase weapon damage.
2. Decrease resistance.

I believe that the latter is a better solution. Whatever system we institute,
it should exhibit the following characteristics:

1. It should be fair to existing characters. If you have 100 hp right now, it's
  not fair if your resistance calcluates to 3.
1. It should scale approximately linearly with character level. A level 5
  fighter should have a higher resistance than a level 1 fighter.
1. It should be easy to calculate. The DM will have to convert a lot of monsters,
  and there will undoubtedly, every session, be a confused player who asks,
  "Wait... how do I calculate that again?"
1. It should serve as a complete system and a full replacement for the hit-point
  system. (I don't like that the current calculation includes "hit points.")
1. It should not require a rewrite of weapon damage. A shortsword cannot
  suddenly do 3d6 damage.


I propose we change the resistance calculation to:

> 1 + [clvl] + [CON+] + [armor] + [bonus]

* _CON+_: Your Constitution bonus
* _clvl_: Your character level or Hit Dice. Do not include template levels
* _armor_: The armor bonus from your worn and natural armors
* _bonus_: The number of bonus hit points you are granted per level based on
  effects like Toughness or other magical items

The downside is that this completely nerfs Barbarian, whose only class features
are "hits hard," "moves fast" and "can get hit hard." (Also: "Can't read" and
"gets pretty tuckered out somtimes.") So, I propose that when raging, a
barbarian adds half of his barbarian levels to his resistance.


Ran some calculations, and this means...

<table>
  <tr>
    <td>Class/Monster</td>
    <td>Level/CR</td>
    <td>Typical Damage</td>
    <td>Typical Resistance</td>
  </tr>

  <tr>
    <td>Goblin</td>
    <td>1/3</td>
    <td>4, 10(17%)</td>
    <td>3</td>
  </tr>
  <tr>
    <td>Orc</td>
    <td>1/2</td>
    <td>9, 13(45%)</td>
    <td>6</td>
  </tr>

  <tr>
    <td>Fighter</td>
    <td>1</td>
    <td>7, 15(12%)</td>
    <td>10-12</td>
  </tr>
  <tr>
    <td>Barbarian</td>
    <td>1</td>
    <td>10, 20(10%)</td>
    <td>9-11 (11-13 when raging)</td>
  </tr>
  <tr>
    <td>Rogue</td>
    <td>1</td>
    <td>4, 8(sneak), 10(30%), 14(sneak, 30%)</td>
    <td>6-8</td>
  </tr>
  <tr>
    <td>Wizard</td>
    <td>1</td>
    <td>3, 7(25%) (magic missile)</td>
    <td>3-4</td>
  </tr>


  <tr>
    <td>Fighter</td>
    <td>5</td>
    <td>10, 18(12%)</td>
    <td>17+</td>
  </tr>
  <tr>
    <td>Barbarian</td>
    <td>5</td>
    <td>11, 21(10%)</td>
    <td>13-14 (17-18 when raging)</td>
  </tr>
  <tr>
    <td>Rogue</td>
    <td>5</td>
    <td>4, 15(sneak), 21(sneak, 49%)</td>
    <td>10-12</td>
  </tr>
  <tr>
    <td>Wizard</td>
    <td>5</td>
    <td>17, 23(60%)(fireball)</td>
    <td>7-8</td>
  </tr>

  <tr>
    <td>Young Adult Black Dragon</td>
    <td>9</td>
    <td>30(breath), 11(bite), 17(bite, 30%)</td>
    <td>20</td>
  </tr>

  <tr>
    <td>Great Wyrm Red Dragon</td>
    <td>26</td>
    <td>79(breath), 48(bite), 56(bite, 41%)</td>
    <td>51</td>
  </tr>
</table>

I like the look of this. Let's experiment.


### Miscellaneous

* Can power attack become a maneuver? Should it be more powerful?
* What is a fair number of maneuvers? More than 4 seems outrageous for anyone.
* Swarm maneuver? Something to lower enemy's resistance?
* Weapon focus increases explosion range of weapon?
