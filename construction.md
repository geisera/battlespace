![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

## Ship Construction

A ship is the sum of its components. You choose the parts. The parts determine the mass. The mass determines the class — and how much power it takes to move it. Size is a result, not a choice.

Build a ship in four steps:

1. Buy components.
2. Buy Superstructure to secure them.
3. Total the Mass.
4. Derive the ship's characteristics.

---

### 1. Buy Components

Every component except the reactor is bought at a **Rating** from 1 to 6. Rating measures capacity. A Rating 3 engine is three times the engine of a Rating 1.

Capacity rises in a straight line. Mass does not. Every step up costs more than the last.

| Rating | Capacity | Mass | Superstructure Cost |
| ---: | ---: | ---: | ---: |
| 1 | ×1 | 1 | 1 |
| 2 | ×2 | 3 | 2 |
| 3 | ×3 | 6 | 3 |
| 4 | ×4 | 10 | 5 |
| 5 | ×5 | 15 | 8 |
| 6 | ×6 | 21 | 11 |

**What each point of Rating buys:**

| Component | Per point of Rating |
| --- | --- |
| Engine | Reduces the Power cost of Movement Points (see [Maneuver](maneuver.md)) |
| Sensor Array | +1 detection range band. Rating also caps Sensor Power. |
| Cargo / Drop Bay | 2 bay units |

**Weapons** are bought individually. Each weapon lists its own Mass and Superstructure Cost (see [Weapons](weapons.md)).

#### Reactors

Reactors are chosen for their desired **Output** — the Power the ship generates each round. Mass and Superstructure follow from the output you demand:

| Output | Mass | Superstructure Cost |
| ---: | ---: | ---: |
| 4 | 1 | 1 |
| 8 | 3 | 2 |
| 12 | 6 | 3 |
| 16 | 10 | 5 |
| 20 | 15 | 8 |
| 24 | 21 | 11 |

Doubling output from 12 to 24 more than triples the reactor's mass. The yard always takes its cut.

**Every ship must carry:** one reactor, one engine, and one sensor array.

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
| Reactor Output | As purchased |

---

### Worked Example

**SDC-468 *Archibald Henderson*, Valkyrie-class dropship**

| Component | Rating | Capacity | Mass | Superstructure | Total Mass |
| --- | ---: | --- | ---: | ---: | ---: |
| Reactor | — | 12 Power | 6 | 3 | 9 |
| Engine | 3 | — | 6 | 3 | 9 |
| Sensor Array | 2 | — | 3 | 2 | 5 |
| Medium Coilgun | — | — | 3 | 2 | 5 |
| Point Defense Laser | — | — | 1 | 1 | 2 |
| Drop Bay | 2 | 4 units | 3 | 2 | 5 |
| Armor (32 points) | — | — | 8 | 2 | 10 |
| **Totals** | | | **30** | **15** | **45** |

```text
Total Mass     = 30 + 15 = 45
Mass Factor    = 45 ÷ 10 = 5
Size Class     = 3          (36–70 band)
Base Signature = 5
Structure      = 15 ÷ 2 = 8
Hull           = 30
Reactor Output = 12
```

Her Movement Points cost 5 ÷ 3 = **2 Power each**. At maximum burn — 6 Power to Propulsion — she buys **3 Movement Points**: enough to advance two hexes and swing one hex-side, with 6 Power left for everything else. Not enough to run it all. Strip the drop bays and armor and her movement gets cheap. Load her for an assault and every hex costs. The manifest decides.

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
