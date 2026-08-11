![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

## Ship Construction

A ship is the sum of its components. You choose the parts. The parts determine the mass. The mass determines the class. Size is a result, not a choice.

Build a ship in five steps:

1. Buy components.
2. Buy Superstructure to secure them.
3. Total the Mass.
4. Derive the ship's characteristics.
5. Assign crew.

---

### 1. Buy Components

Every component is bought at a **Rating** from 1 to 6. Rating measures capacity. A Rating 3 reactor produces three times the power of a Rating 1 reactor.

Capacity rises in a straight line. Mass does not.

| Rating | Capacity | Mass | Superstructure Cost |
| ---: | ---: | ---: | ---: |
| 1 | ×1 | 1 | 1 |
| 2 | ×2 | 3 | 2 |
| 3 | ×3 | 6 | 3 |
| 4 | ×4 | 10 | 5 |
| 5 | ×5 | 15 | 8 |
| 6 | ×6 | 21 | 11 |

Read the table this way: a Rating 4 reactor makes four times the power of a Rating 1 — and weighs ten times as much.

**What each point of Rating buys:**

| Component | Per point of Rating |
| --- | --- |
| Reactor | 4 Power |
| Engine | Drives Movement Points (Section 5) |
| Sensor Array | +1 detection range band. Rating also caps Sensor Power. |
| Cargo / Drop Bay | 2 bay units |
| Life Support | Supports 1 crew department |
| Weapon Mount | Mount Rating must equal or exceed the weapon's class |

**Every ship must carry:** one reactor, one engine, one sensor array, and life support.

---

### 2. Buy Superstructure

Superstructure is the frame: keel, trusses, and mounting hardware.

Three rules:

1. Every component requires Superstructure equal to its Superstructure Cost.
2. Every point of Superstructure adds 1 Mass.
3. You may buy extra Superstructure to reinforce the frame. It raises Structure (Section 4) and adds Mass like any other point.

---

### 3. Total the Mass

```text
Total Mass = Component Mass + Superstructure + Armor Mass
```

**Armor** is bought by the point and distributed across the four facings. No facing may be 0.

* Every 4 points of armor = 1 Mass.
* Every 4 Mass of armor requires 1 Superstructure.

---

### 4. Derive Characteristics

Nothing is assigned. Everything is computed.

```text
Mass Factor = Total Mass ÷ 10, rounded up
```

| Characteristic | Formula |
| --- | --- |
| Size Class | By Total Mass: 1–15 → Size 1 · 16–35 → Size 2 · 36–70 → Size 3 · 71–120 → Size 4 · 121+ → Size 5 |
| Base Signature | Mass Factor |
| Structure | Superstructure ÷ 2, rounded up |
| Hull | Component Mass + Armor Mass |
| Reactor Output | 4 × Reactor Rating |
| Rotation | Engine Rating − Size Class + 2, minimum 1 |

---

### 5. Movement

Movement Points are computed fresh each round:

```text
Movement Points = (Engine Rating × Propulsion Power) ÷ Mass Factor, rounded down
```

Maximum Propulsion Power per round = 2 × Engine Rating.

The chain that governs every design: more mass needs a bigger engine, a bigger engine needs a bigger reactor, and both need more Superstructure — all of which is more mass. Every hull is a truce with that spiral.

---

### 6. Assign Crew

Rate the five departments — Command, Engineering, Gunnery, Sensors, Damage Control — from 1 to 5.

* Skill points available: **10 + (2 × Size Class)**.
* Command Rating may not exceed the Command department's skill.
* Life Support requires 1 Power per point of its Rating each round. A ship that cannot power life support plus 1 Propulsion is not spaceworthy.

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
| Life Support | 2 | 2 departments | 3 | 2 |
| Armor (32 points) | — | — | 8 | 2 |
| **Totals** | | | **33** | **17** |

```text
Total Mass     = 33 + 17 = 50
Mass Factor    = 50 ÷ 10 = 5
Size Class     = 3          (36–70 band)
Base Signature = 5
Structure      = 17 ÷ 2 = 9
Hull           = 33 
Reactor Output = 12
Rotation       = 3 − 3 + 2 = 2
```

At maximum burn — 6 Power to Propulsion — she makes (3 × 6) ÷ 5 = **3 Movement Points**, with 4 Power left after life support. Not enough to run everything. Strip the drop bays and armor and she is a Size 2 ship that moves like one. Load her for an assault and she moves like a barge. The manifest decides.

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
