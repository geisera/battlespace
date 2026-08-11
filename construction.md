![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

## Ship Construction

Nothing about a ship is chosen from a chart. A ship is the sum of what you bolt into it. Pick components, pay their mass, pay the superstructure that holds them together — and the hull that results tells you what class of ship you built. Size is a consequence, not a decision.

Ships are built in five steps:

1. Select components by Rating
2. Pay Superstructure
3. Total Mass
4. Derive ship characteristics
5. Assign crew and command

---

### 1. Components and Ratings

Every component — reactor, engine, sensors, weapons, tankage, bays — is purchased at a **Rating** from 1 to 6.

Rating buys capacity linearly. Mass grows faster than capacity. This is the law of the yard: every step up costs more than the last one did.

| Rating | Capacity Multiplier | Mass | Superstructure Cost |
| ---: | ---: | ---: | ---: |
| 1 | ×1 | 1 | 1 |
| 2 | ×2 | 3 | 2 |
| 3 | ×3 | 6 | 3 |
| 4 | ×4 | 10 | 5 |
| 5 | ×5 | 15 | 8 |
| 6 | ×6 | 21 | 11 |

A Rating 4 reactor produces four times the power of a Rating 1 reactor — and weighs ten times as much before you've braced it to the frame.

**Component capacities per point of Rating:**

| Component | Capacity per Rating |
| --- | --- |
| Reactor | 4 Power output |
| Engine | See Movement, below |
| Sensor Array | +1 detection range band; Rating is max Sensor Power usable |
| Cargo / Drop Bay | 2 bay units |
| Life Support | Crew for one department per Rating |
| Weapon Mount | By weapon class; a mount's Rating must equal or exceed the weapon's class |

Ships require at minimum: one reactor, one engine, one sensor array, and life support.

---

### 2. Superstructure

Superstructure is the frame — the keel, trusses, and hard mounting that hold the ship together under thrust.

* Every component must be secured with Superstructure equal to its Superstructure Cost.
* Each point of Superstructure adds **1 Mass** to the ship.
* Additional Superstructure beyond the required minimum may be purchased to reinforce the frame (see Structure, below), at 1 Mass per point.

---

### 3. Mass

```text
Total Mass =
sum of all component Mass
+ total Superstructure
+ Armor Mass
```

**Armor** is plate bolted to the frame: every 4 points of armor = 1 Mass, and every 4 Mass of armor requires 1 Superstructure. Armor is distributed across the four facings; no facing may be 0.

---

### 4. Derived Characteristics

All ship characteristics fall out of Total Mass and installed components. Nothing is assigned.

```text
Mass Factor = Total Mass ÷ 10, rounded up
```

| Characteristic | Derivation |
| --- | --- |
| **Size Class** | Total Mass ≤ 15: Size 1 · 16–35: Size 2 · 36–70: Size 3 · 71–120: Size 4 · 121+: Size 5 |
| **Base Signature** | Mass Factor |
| **Structure** | Total Superstructure ÷ 2, rounded up |
| **Hull** | Total component Mass + Armor Mass (Superstructure excluded) |
| **Reactor Output** | 4 × Reactor Rating |
| **Rotation** | Engine Rating − Size Class + 2, minimum 1 |

Bigger ships are easier to see, harder to turn, and hungrier — not because a chart says so, but because you built them that way.

---

### 5. Movement

Movement Points are earned each round, not owned:

```text
Movement Points =
(Engine Rating × Power allocated to Propulsion)
÷ Mass Factor, rounded down
```

Maximum Power allocated to Propulsion in one round = 2 × Engine Rating.

The same engine that flings a corvette across the map barely nudges a battleship. Mass punishes everything: a heavier ship needs a higher-rated engine to reach the same speed, which adds mass, which demands more reactor, which adds mass, which demands more superstructure — which adds mass. At every step the yard takes its cut. Somewhere in that spiral is the ship you can actually afford to move.

---

### 6. Crew and Command

Assign the five crew departments (Command, Engineering, Gunnery, Sensors, Damage Control) skill ratings from 1 to 5. Total department skill points available = **10 + (2 × Size Class)**.

Command Rating may not exceed the Command department's skill.

**Minimum operating load**: Life Support requires 1 Power per point of its Rating. A reactor unable to meet minimum operating load plus 1 Power of Propulsion is not spaceworthy.

---

### Worked Example

**SDC-468 *Archibald Henderson*, Valkyrie-class dropship**

| Component | Rating | Capacity | Mass | Superstructure |
| --- | ---: | --- | ---: | ---: |
| Reactor | 3 | 12 Power | 6 | 3 |
| Engine | 3 | — | 6 | 3 |
| Sensor Array | 2 | — | 3 | 2 |
| Medium Coilgun | 2 | — | 3 | 2 |
| Point Defense Laser | 1 | — | 1 | 1 |
| Drop Bay | 2 | 4 units | 3 | 2 |
| Life Support | 2 | 2 departments+ | 3 | 2 |
| Armor (32 points) | — | — | 8 | 2 |
| **Totals** | | | **33** | **17** |

```text
Total Mass       = 33 + 17 = 50
Mass Factor      = 50 ÷ 10 = 5
Size Class       = 3 (36–70)
Base Signature   = 5
Structure        = 17 ÷ 2 = 9
Hull             = 33
Reactor Output   = 12
Rotation         = 3 − 3 + 2 = 2
```

At 6 Power to Propulsion (her engine's maximum): (3 × 6) ÷ 5 = **3 Movement Points** — and 4 Power left for everything else after life support. Strip the drop bays and armor and the *Henderson* is a Size 2 ship that runs like one. Load her for an assault and she's a frigate that fights like a barge. Nobody chose that. The manifest did.

---

## Table of Contents

* [Sequence of Play](sequence-of-play.md)
* [Initiative](initiative.md)
* [Maneuver](maneuver.md)
* [Combat](combat.md)
* [Damge](battle-damage.md)
* [Minor Actions](minor-actions.md)
* [Ship Construction](construction.md)
* [Weapons](weapons.md)
* [Auxiliary Equipment](equipment.md)

--- 
