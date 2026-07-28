# Starship Tactical Combat Rules

## 1. Core Concepts

Each combat round represents approximately 20 seconds.

The game uses:

* A hex map
* Six ship facings
* Alternating ship activations
* Two six-sided dice
* Power allocation
* Command Points
* Facing-based armor
* Individual ship systems
* Progressive damage and critical effects

Whenever a rule calls for a test, roll:

**2d6 + relevant rating + modifiers**

A result of **8 or higher** succeeds unless another target number is specified.

### Margin of Success

* Success by 0–3: normal success
* Success by 4 or more: strong success
* Failure by 4 or more: severe failure

---

# 2. Ship Characteristics

Each ship has the following primary characteristics.

## Size Class

Size Class normally ranges from 1 to 5.

| Size | Example                 |
| ---: | ----------------------- |
|    1 | Fighter or shuttle      |
|    2 | Corvette or patrol ship |
|    3 | Frigate or dropship     |
|    4 | Cruiser                 |
|    5 | Battleship or carrier   |

Size affects detection, maneuverability, collision damage, and weapon accuracy.

## Hull

Hull represents exterior plating, compartments, and general damage tolerance.

When Hull reaches 0, further Hull damage is applied to Structure.

## Structure

Structure represents the ship’s frame and pressure vessel.

When Structure reaches 0, the ship is crippled and must make a Catastrophic Damage Test.

## Thrust

Thrust determines acceleration and maximum maneuver expenditure.

## Rotation

Rotation determines how many facing changes the ship may make during movement.

## Reactor Output

Reactor Output determines how much power the ship may allocate each round.

## Heat Maximum

Heat Maximum determines how much heat the ship can tolerate before suffering penalties.

## Base Signature

Base Signature determines how easy the ship is to detect.

## Command Rating

Command Rating measures the effectiveness of the bridge crew, command systems, and tactical organization.

Command Rating determines:

* Command Point generation
* Command Point reserve
* Some initiative modifiers
* Resistance to command disruption

Typical Command Ratings range from 1 to 5.

---

# 3. Crew Departments

Ships have crew departments rated from 1 to 5.

Recommended departments are:

* Command
* Engineering
* Gunnery
* Sensors
* Damage Control

A department’s rating is its Skill.

Fatigue, casualties, morale, and damage may reduce Effective Skill.

```text
Effective Skill =
Skill
- Fatigue penalties
- Casualty penalties
- Morale penalties
```

A department cannot normally have an Effective Skill below 0.

---

# 4. Command Points

Command Points represent the ship’s capacity to respond to changing circumstances.

At the start of each round:

```text
CP Generated =
Command Rating
- Command Disruption
```

```text
Current CP =
Current CP + CP Generated
```

Current CP cannot exceed:

```text
CP Reserve = Command Rating + 2
```

## Standard Command Point Uses

### Change an Order — 1 CP

Change the ship’s stance, primary order, target priority, or crew assignment outside the normal declaration step.

### Reroute Power — 1 CP

Move 1 Power from one allocation category to another.

### Focus a Department — 1 CP

Gain +1 on one test made by a crew department.

### Additional Reaction — 1 CP

Perform one additional reaction after the ship has used its normal reaction.

### Initiative Boost — 1 CP per +1

Spend CP before initiative is rolled.

### Minor Interrupt — 2 CP

Perform a Minor Action immediately before or after another ship’s action.

### Emergency Action — 2 CP

Temporarily operate a disabled system, perform emergency thrust, immediately seal a breach, or take another exceptional action permitted by the referee.

An Emergency Action usually generates 1 Heat or risks system damage.

Command Points purchase flexibility. They do not replace Power, ammunition, functioning systems, or required crew.

---

# 5. Power

At the start of each round, a ship generates Power equal to the current output of its reactor.

Power may be allocated to:

* Propulsion
* Weapons
* Sensors
* Damage Control
* Life Support
* Electronic Warfare
* Shields, if used
* Reserve

The total allocated Power cannot exceed Reactor Output.

## Minimum Power

Life Support normally requires 1 Power.

A system that does not receive its required Power cannot operate normally.

## Reserve Power

Power placed in Reserve may be spent during the round through reactions or Command Point abilities.

One point of Reserve Power may be moved without CP if a rule specifically permits it.

## Reactor Damage

A degraded reactor produces 75% of normal output, rounded down.

An impaired reactor produces 50% of normal output, rounded down.

A disabled reactor produces no Power.

---

# 6. Heat

Ships gain Heat from:

* Weapon fire
* Hard burns
* Active sensors
* Reactor overloads
* Emergency actions
* Damaged systems

At the end of each round, reduce Heat by the ship’s cooling rate. The default cooling rate is 2.

## Heat Effects

| Heat level                     | Effect     |
| ------------------------------ | ---------- |
| Below half maximum             | No effect  |
| Half maximum or more           | Hot        |
| Three-quarters maximum or more | Overheated |
| Heat Maximum or more           | Critical   |

### Hot

No automatic penalty, but the ship gains +1 Signature.

### Overheated

* −1 to Engineering and Gunnery tests
* +1 Signature
* Hard Burn costs 1 additional Heat

### Critical

Immediately make an Overheat Test:

```text
2d6 + Engineering Skill
```

Target number: 8.

On failure, one randomly selected powered system becomes degraded.

Heat cannot normally exceed Heat Maximum by more than 3. At that point, the reactor automatically shuts down.

---

# 7. Armor and Facing

Ships have four armor facings:

* Fore
* Aft
* Port
* Starboard

Each facing has:

* Current Armor
* Maximum Armor

Armor absorbs incoming damage before Hull.

The facing struck is determined by the attacker’s position relative to the target.

Dorsal and ventral attacks use the nearest logical facing unless the scenario uses three-dimensional movement.

---

# 8. Systems

Systems have:

* Condition
* Maximum Condition
* Operational State
* Power requirement
* Location

Operational states are:

| State       | Condition | Effect                           |
| ----------- | --------: | -------------------------------- |
| Operational |   76–100% | Full effect                      |
| Degraded    |    51–75% | 75% effect                       |
| Impaired    |     1–50% | 50% effect                       |
| Disabled    |         0 | Cannot operate                   |
| Destroyed   |   Special | Cannot be repaired during battle |

Condition percentages are rounded normally.

A system at 0 Condition becomes Disabled unless a critical effect destroys it.

---

# 9. Round Sequence

Each round follows this sequence:

1. Command Phase
2. Detection Phase
3. Power Phase
4. Initiative Phase
5. Maneuver Phase
6. Action Phase
7. Ordnance Phase
8. Damage Control Phase
9. End Phase

---

# 10. Command Phase

Each ship performs the following:

1. Resolve command disruption.
2. Generate Command Points.
3. Select a stance.
4. Declare a primary order.
5. Assign crew departments where required.

## Stances

### Balanced

No modifier.

### Aggressive

* +1 Gunnery
* −1 Evasion
* Cannot use Silent sensor mode

### Defensive

* +1 to defensive reactions
* −1 Gunnery

### Evasive

* +1 Evasion
* −1 Gunnery
* Heavy weapons cannot use Aimed Fire

### Pursuit

* +1 Thrust when moving toward the designated target
* −1 Rotation when turning away from it

### Damage Control

* +1 Damage Control
* −1 Thrust
* −1 Gunnery

### Silent

* −2 Signature
* Cannot use active sensors
* Cannot coordinate fire with other ships

A ship may change stance during the round for 1 CP.

---

# 11. Detection Phase

Each ship maintains its own contact level for each enemy.

## Sensor Modes

Each ship chooses one mode.

### Silent

* Cannot make detection rolls
* −2 Signature
* Existing contacts against the ship may degrade

### Passive

* May make normal detection rolls
* No Signature modifier

### Active

* +2 to detection rolls
* +2 Signature
* Automatically becomes Detected by enemies with functioning sensors in range

## Detection Roll

A ship may test once against each enemy within sensor range.

```text
2d6
+ Sensor Rating
+ Sensors Crew Skill
+ Target Signature
- Range Penalty
```

A result of 8 or higher improves contact by one level.

Success by 4 or more improves contact by two levels.

## Contact Levels

| Level | State    | Effect                                  |
| ----: | -------- | --------------------------------------- |
|     0 | Unknown  | No usable contact                       |
|     1 | Detected | Approximate location                    |
|     2 | Tracked  | Exact position, speed, and facing       |
|     3 | Locked   | Guided and precision weapons may engage |

## Range Modifiers

| Range   | Modifier |
| ------- | -------: |
| Close   |       +1 |
| Short   |        0 |
| Medium  |       −1 |
| Long    |       −2 |
| Extreme |       −4 |

## Losing Contact

A contact drops one level when:

* The target leaves sensor range
* The target enters significant cover
* The target uses Silent mode
* The observer’s sensors become impaired or disabled
* A successful electronic-warfare action breaks contact

A contact reduced below Detected is removed.

## Weapon Requirements

* Direct-fire weapons require Tracked
* Guided weapons require Locked
* Point-defense weapons require Detected
* Area attacks may target a Detected contact but suffer −2 accuracy

---

# 12. Initiative Phase

Each ship rolls:

```text
2d6
+ Command Rating
+ Command Crew Skill
+ initiative modifiers
```

Players may spend CP before rolling. Each CP adds +1.

Record each ship’s Initiative Score.

### Movement

Ships move from lowest Initiative to highest.

### Actions

Ships act from highest Initiative to lowest.

When multiple ships have the same Initiative, the ship with the higher Command Rating acts first. Remaining ties are rerolled.

---

# 13. Maneuver Phase

Each ship receives a movement activation.

Movement occurs in this order:

1. Drift
2. Apply thrust
3. Change facing
4. Perform a maneuver
5. Check collisions and hazards

## Speed

Speed is measured in hexes.

During Drift, move the ship forward a number of hexes equal to its Speed.

A ship may spend Propulsion Power to alter Speed.

Each Power allocated to Propulsion permits one of the following:

* Increase Speed by 1
* Decrease Speed by 1
* Cancel one hex of Drift
* Gain one maneuver point

Speed cannot be reduced below 0.

## Turning

A ship may change facing a number of times equal to its effective Rotation.

A normal facing change is one hex-side, or 60 degrees.

A ship must normally move at least one hex between facing changes.

## Maneuvers

### Accelerate

Increase Speed by up to available Thrust.

### Decelerate

Reduce Speed by up to available Thrust.

### Hard Turn

Spend 1 additional Propulsion Power to make one extra facing change.

Gain 1 Heat.

### Evasive Pattern

Spend 1 Propulsion Power.

Gain +1 Evasion until the ship’s next activation.

All weapon attacks made by the ship suffer −1.

### Hard Burn

Spend 2 Propulsion Power.

Increase Speed by 2 beyond normal acceleration.

Gain 2 Heat and +2 Signature.

### Pivot

Only available at Speed 0 or 1.

Change facing by up to two hex-sides without forward movement.

### Silent Drift

Requires Silent sensor mode.

The ship may not accelerate, fire weapons, or actively scan.

It retains current Speed and gains an additional −1 Signature.

---

# 14. Action Phase

Ships activate from highest Initiative to lowest.

When a ship activates, it may perform:

* One Major Action
* One Minor Action
* Any permitted Free Actions

## Major Actions

* Fire one weapon group
* Launch missiles
* Conduct an electronic-warfare attack
* Perform an active scan
* Make a major repair
* Vent heat
* Launch or recover small craft
* Attempt boarding
* Recharge shields, if used

## Minor Actions

* Rotate a weapon mount
* Shift one point of Power using 1 CP
* Improve one contact
* Activate countermeasures
* Brace a section
* Prepare a weapon
* Change crew assignment
* Clear a weapon jam
* Reload a weapon

## Free Actions

* Communicate
* Drop a target lock
* Shut down a system
* Release cargo
* Cancel a prepared action

---

# 15. Reactions

Each ship receives one Reaction per round.

A Reaction resolves immediately after its trigger.

Common reactions include:

### Evasive Thrust

Trigger: The ship is targeted by a direct-fire attack.

Spend 1 Propulsion Power.

Gain +1 Evasion against that attack.

### Brace for Impact

Trigger: The ship is hit.

Reduce Hull damage by 1.

The braced section’s crew suffers +1 Fatigue.

### Point Defense

Trigger: A missile or boarding pod enters range.

Fire an eligible point-defense weapon.

### Countermeasures

Trigger: A guided weapon attacks.

Reduce the attacker’s lock or attack roll by 1.

### Emergency Shield Reinforcement

If shields are used, move shield strength to the threatened facing.

A ship may spend 1 CP to perform one additional Reaction.

---

# 16. Weapon Attacks

Resolve attacks in this order:

1. Declare weapon and target.
2. Confirm range, firing arc, contact level, ammunition, and Power.
3. Choose firing mode.
4. Defender declares reactions.
5. Roll attack.
6. Apply damage.
7. Check for critical effects.
8. Apply Heat and ammunition costs.

## Attack Roll

```text
2d6
+ Weapon Accuracy
+ Gunnery Skill
+ contact modifier
+ firing mode modifier
- Range Penalty
- Target Evasion
- damage penalties
```

The attack hits on 8 or higher.

## Target Evasion

```text
Evasion =
base handling
+ Evasive stance
+ Evasive Pattern
+ reaction modifiers
- size modifier
```

Suggested Size modifiers:

| Target Size | Attack modifier |
| ----------: | --------------: |
|           1 |              −2 |
|           2 |              −1 |
|           3 |               0 |
|           4 |              +1 |
|           5 |              +2 |

## Contact Modifiers

| Contact  | Attack modifier |
| -------- | --------------: |
| Detected |              −2 |
| Tracked  |               0 |
| Locked   |              +1 |

Weapons must still meet their minimum contact requirement.

## Firing Modes

### Snap Fire

* −1 accuracy
* May be used as a prepared or interrupt action

### Standard Fire

No modifier.

### Aimed Fire

* +1 accuracy
* Requires Locked contact
* Cannot be used after a Hard Burn or Hard Turn

### Overcharge

* +2 damage
* Gain 2 additional Heat
* On an attack roll of 2–4, the weapon loses 1 Condition

### Salvo

Fire multiple identical weapons as one attack.

Gain +1 accuracy or +2 damage, chosen before rolling.

All weapons expend ammunition and generate Heat.

---

# 17. Damage

Weapons have a Damage value and may have Penetration.

Resolve damage in this order:

1. Shields, if present
2. Armor
3. Hull
4. Systems
5. Structure
6. Critical effects

## Armor

Subtract the struck facing’s Current Armor from incoming damage, to a minimum of 0.

After resolving the attack, reduce that facing’s Current Armor by 1 if any damage penetrated.

A weapon with Penetration ignores Armor equal to its Penetration value.

Example:

```text
Incoming Damage: 8
Armor: 5
Penetration: 2

Effective Armor: 3
Damage after Armor: 5
```

## Hull Damage

Apply remaining damage to Hull.

For every full 5 Hull damage inflicted by one attack, make one System Hit.

## System Hit

Determine the struck section from the attack facing.

Select or randomly determine one system in that section.

The system loses Condition equal to:

```text
1 + weapon System Damage modifier
```

If no valid system exists, apply 1 additional Structure damage.

## Structure Damage

Damage reaches Structure when:

* Hull is already 0
* A weapon has the Structural trait
* A critical effect applies Structure damage

When Structure is reduced below half maximum:

* −1 Rotation
* −1 Command Point generation
* All repair tests suffer −1

When Structure reaches 0, make a Catastrophic Damage Test.

---

# 18. Critical Effects

A critical effect occurs when:

* An attack succeeds by 4 or more
* One attack inflicts at least 5 Hull damage
* A weapon has the Critical trait
* A system becomes Disabled
* A rule specifically requires one

Roll 1d6:

| Roll | Critical effect      |
| ---: | -------------------- |
|    1 | Power failure        |
|    2 | Fire                 |
|    3 | Hull breach          |
|    4 | Crew casualties      |
|    5 | System malfunction   |
|    6 | Severe system damage |

## Power Failure

One powered system immediately shuts down.

It may be restarted during Damage Control.

## Fire

Place a Fire effect in the struck section.

During each Damage Control Phase, an uncontrolled fire inflicts 1 Hull damage and 1 Condition damage to a system in that section.

## Hull Breach

The section becomes breached.

Crew actions in that section suffer −1 until sealed.

## Crew Casualties

The relevant department loses effectiveness.

Apply −1 Skill until treated or reinforced.

## System Malfunction

The affected system becomes Degraded, or loses 1 additional Condition if already Degraded.

## Severe System Damage

The affected system becomes Disabled.

If already Disabled, it is Destroyed.

---

# 19. Missiles and Ordnance

Missiles are placed on the map when launched.

A missile salvo has:

* Speed
* Endurance
* Attack value
* Damage
* Armor or durability
* Target lock

## Missile Movement

During the Ordnance Phase, missiles move their Speed toward the target.

They may turn freely unless otherwise specified.

## Missile Attack

When a missile enters the target’s hex or attack range:

```text
2d6
+ Missile Attack
+ Lock bonus
- Target Evasion
- Countermeasures
```

A missile hits on 8 or higher.

## Point Defense

Point-defense weapons attack missiles before impact.

Each successful point-defense hit destroys one missile or reduces the salvo’s Damage by a defined amount.

If the missile loses Locked contact, it suffers −2 to attack.

If it loses all contact, it continues toward the target’s last known position and then expires.

---

# 20. Electronic Warfare

A ship with an electronic-warfare system may take one EW Major Action.

Make an opposed test:

```text
Attacker:
2d6 + EW Rating + Sensors Skill

Defender:
8 + EW Rating or Sensor Rating
```

## Jam

On success, the target suffers −1 to detection and attack rolls until the next Detection Phase.

Strong success imposes −2.

## Break Lock

On success, one Locked contact held by the target drops to Tracked.

## Mask

On success, reduce the ship’s Signature by 2 until the next Detection Phase.

Masking ends if the ship uses Active sensors or Hard Burn.

## Spoof

On success, create a false Detected contact within two hexes of the ship.

The false contact disappears when an enemy successfully detects it again.

---

# 21. Damage Control Phase

Resolve the following:

1. Ongoing fires
2. Hull breaches
3. Reactor instability
4. Crew casualties
5. Repair attempts
6. Boarding actions

Each eligible Damage Control department may attempt one action.

## Repair Test

```text
2d6
+ Damage Control Skill
+ Engineering support
- repair difficulty
```

A result of 8 or higher succeeds.

## Repair Actions

### Extinguish Fire

Success removes one Fire effect.

### Seal Breach

Success removes one Hull Breach effect.

### Restore Disabled System

Success restores a Disabled system to 1 Condition and Impaired state.

Destroyed systems cannot be restored during combat.

### Repair Condition

Success restores 1 Condition.

Strong success restores 2 Condition.

A system cannot normally be restored above Degraded during combat unless a special repair system permits it.

### Stabilize Reactor

Success removes one Reactor Instability effect.

### Treat Casualties

Success removes one temporary crew Skill penalty.

---

# 22. End Phase

Each ship performs the following:

1. Dissipate Heat.
2. Reduce cooldowns by 1.
3. Regenerate shields, if applicable.
4. Remove expired status effects.
5. Check morale.
6. Check catastrophic damage.
7. Score objectives.
8. Advance the round counter.

## Morale Test

Make a Morale Test when:

* Structure falls below half
* The bridge is disabled
* The captain is incapacitated
* Half the allied ships are destroyed
* The ship suffers catastrophic damage

```text
2d6 + Command Skill + Morale
```

Target number: 8.

On failure, the ship becomes Shaken:

* −1 Initiative
* First CP ability used next round costs +1 CP

A second failure while Shaken may force withdrawal or surrender.

---

# 23. Catastrophic Damage

When Structure reaches 0, roll:

```text
2d6 + Engineering Skill - active critical effects
```

|    Result | Outcome                    |
| --------: | -------------------------- |
|       10+ | Stable wreck               |
|       8–9 | Disabled ship              |
|       6–7 | Reactor shutdown; evacuate |
|       4–5 | Breakup in 1d3 rounds      |
| 3 or less | Catastrophic explosion     |

## Stable Wreck

The ship cannot move or attack but remains habitable.

## Disabled Ship

The ship loses Power and cannot act except for Damage Control.

## Reactor Shutdown

The crew must evacuate or restore emergency power.

## Breakup

The ship is destroyed after the indicated number of rounds unless stabilized.

## Catastrophic Explosion

The ship is immediately destroyed. Nearby ships may suffer damage based on Size Class.

---

# 24. Example Ship Activation

The *Archibald Henderson* has:

* Speed 4
* Thrust 5
* Rotation 2
* 12 Reactor Output
* 3 Command Rating
* 2 current CP
* Degraded main engine

During the Power Phase, the player allocates:

* Propulsion 4
* Weapons 3
* Sensors 2
* Damage Control 1
* Life Support 1
* Reserve 1

During movement, the ship drifts four hexes. Its degraded engine reduces effective Thrust from 5 to 4. It spends 1 Propulsion Power to turn, 1 to reduce Speed, and retains the rest for an Evasive Thrust reaction.

During its action, it fires the medium coilgun at a Tracked target.

The attack roll is:

```text
2d6
+ Weapon Accuracy
+ Gunnery Skill
- Range Penalty
- Target Evasion
```

The attack hits and inflicts 7 Damage against 4 effective Armor. Three Damage reaches Hull. Because the attack did not inflict 5 Hull damage, it does not automatically cause a System Hit.

Later in the round, an enemy missile attacks. The ship uses its normal Reaction and spends 1 Propulsion Power for Evasive Thrust, increasing its Evasion by 1 against the missile attack.

During Damage Control, the Engineering department attempts to correct the existing engine-misalignment critical effect.

---

# 25. Recommended Starting Scale

For an initial version of the game, use:

* One to three ships per player
* Ship ratings from 1 to 5
* Hull between 15 and 50
* Structure between 5 and 15
* Reactor Output between 6 and 18
* Weapon Damage between 3 and 10
* Armor between 2 and 10
* Command Points between 1 and 7
* Sensor range no greater than Extreme range

A typical engagement should last six to ten rounds.

The rules should create a steady progression:

```text
Detection
→ Positioning
→ Weapon engagement
→ Armor loss
→ System damage
→ Command disruption
→ Withdrawal, surrender, or destruction
```

The central tactical choices are how to allocate Power, when to spend Command Points, which facing to expose, whether to pursue or disengage, and whether to use actions offensively or preserve them for survival.
