![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

## Ship Construction

A ship is the sum of its components. You choose the parts. The parts determine the mass. The mass determines the class — and how much power it takes to move it.

Build a ship in four steps:

1. Buy components.
2. Buy Superstructure to secure them.
3. Total the Mass.
4. Derive the ship's characteristics.

A completed ship must be capable of movement. If its reactor cannot generate enough Power to purchase at least **1 Movement Point**, the design is invalid.

---

### 1. Buy Components

Every component except the reactor is bought at a **Rating** from 1 to 6. Rating measures capacity. A Rating 3 component has three times the capacity of a Rating 1 component.

Capacity rises in a straight line. Mass does not. Every step up costs more than the last.

| Rating | Capacity | Mass | Superstructure Cost |
| -----: | -------: | ---: | ------------------: |
|      1 |       ×1 |    1 |                   1 |
|      2 |       ×2 |    3 |                   2 |
|      3 |       ×3 |    6 |                   3 |
|      4 |       ×4 |   10 |                   5 |
|      5 |       ×5 |   15 |                   8 |
|      6 |       ×6 |   21 |                  11 |

**What each point of Rating buys:**

| Component        | Per point of Rating                                     |
| ---------------- | ------------------------------------------------------- |
| Engine           | +1 Engine Rating                                        |
| Sensor Array     | +1 detection range band. Rating also caps Sensor Power. |
| Cargo / Drop Bay | 2 bay units                                             |

**Weapons** are bought individually. Each weapon lists its own Mass and Superstructure Cost. See [Weapons](weapons.md).

#### Engines

A ship must carry at least one engine. It may carry more than one.

Add the Ratings of all installed engines to determine **Total Engine Rating**.

```text
Total Engine Rating = Sum of all Engine Ratings
```

Example:

```text
Rating 4 Engine
Rating 3 Engine
Rating 2 Engine

Total Engine Rating = 9
```

Individual engines remain limited to Rating 1–6. Total Engine Rating has no fixed maximum.

Multiple engines allow large ships to generate enough propulsion without requiring components above Rating 6. They also carry the normal Mass and Superstructure costs of each installed engine.

Movement Power Cost is derived after Total Mass is known.

```text
Movement Power Cost =
Mass Factor ÷ Total Engine Rating,
rounded up
```

Movement Power Cost can never be less than 1.

```text
Movement Power Cost =
maximum of 1 or
Mass Factor ÷ Total Engine Rating,
rounded up
```

See [Maneuver](maneuver.md).

#### Reactors

Reactors are chosen for their desired **Output** — the Power the ship generates each round.

Mass and Superstructure follow from the output you demand:

| Output | Mass | Superstructure Cost |
| -----: | ---: | ------------------: |
|      4 |    1 |                   1 |
|      8 |    3 |                   2 |
|     12 |    6 |                   3 |
|     16 |   10 |                   5 |
|     20 |   15 |                   8 |
|     24 |   21 |                  11 |

Doubling output from 12 to 24 more than triples the reactor's mass. The yard always takes its cut.

A ship may carry only one reactor.

**Every ship must carry:**

* one reactor;
* at least one engine;
* one sensor array.

---

### 2. Buy Superstructure

Superstructure is the frame: keel, trusses, and mounting hardware.

Three rules apply:

1. Every component requires Superstructure equal to its Superstructure Cost.
2. Every point of Superstructure adds 1 Mass.
3. You may buy extra Superstructure to reinforce the frame. It raises Structure and adds Mass like any other point.

Every engine is a separate component. A ship with multiple engines must pay the Mass and Superstructure Cost of each engine.

---

### 3. Total the Mass

```text
Total Mass = Component Mass + Superstructure + Armor Mass
```

**Armor** is bought by the point and distributed across the four facings. No facing may be 0.

* Every 4 points of Armor = 1 Mass.
* Every 4 Mass of Armor requires 1 Superstructure.

After all components, armor, and Superstructure are installed, calculate Total Mass.

---

### 4. Derive Characteristics

Nothing is assigned. Everything is computed.

```text
Mass Factor = Total Mass ÷ 10, rounded up
```

| Characteristic      | Formula                                                                                          |
| ------------------- | ------------------------------------------------------------------------------------------------ |
| Size Class          | By Total Mass: 1–15 → Size 1 · 16–35 → Size 2 · 36–70 → Size 3 · 71–120 → Size 4 · 121+ → Size 5 |
| Base Signature      | Mass Factor                                                                                      |
| Structure           | Superstructure ÷ 2, rounded up                                                                   |
| Hull                | Component Mass + Armor Mass                                                                      |
| Reactor Output      | As purchased                                                                                     |
| Total Engine Rating | Sum of installed Engine Ratings                                                                  |
| Movement Power Cost | Mass Factor ÷ Total Engine Rating, rounded up; minimum 1                                         |

#### Minimum Mobility

Every completed ship must be capable of purchasing at least **1 Movement Point** using its Reactor Output.

```text
Reactor Output ≥ Movement Power Cost
```

If this condition is not met, the ship is an invalid design.

The designer must:

* install additional engines;
* install higher-rated engines;
* install a larger reactor;
* reduce the ship's mass; or
* use some combination of these changes.

A ship is not required to be fast. A heavily loaded freighter may spend most of its reactor output to crawl across the battlespace. It must only be capable of moving under its own power.

---

### Worked Example

**SDC-468 *Archibald Henderson*, Valkyrie-class dropship**

| Component           | Rating | Capacity |   Mass | Superstructure | Total Mass |
| ------------------- | -----: | -------- | -----: | -------------: | ---------: |
| Reactor             |      — | 12 Power |      6 |              3 |          9 |
| Engine              |      3 | —        |      6 |              3 |          9 |
| Sensor Array        |      2 | —        |      3 |              2 |          5 |
| Medium Coilgun      |      — | —        |      3 |              2 |          5 |
| Point Defense Laser |      — | —        |      1 |              1 |          2 |
| Drop Bay            |      2 | 4 units  |      3 |              2 |          5 |
| Armor (32 points)   |      — | —        |      8 |              2 |         10 |
| **Totals**          |        |          | **30** |         **15** |     **45** |

```text
Total Mass          = 30 + 15 = 45
Mass Factor         = 45 ÷ 10 = 5
Size Class          = 3
Base Signature      = 5
Structure           = 15 ÷ 2 = 8
Hull                = 30
Reactor Output      = 12
Total Engine Rating = 3
```

Movement Power Cost:

```text
5 ÷ 3 = 1.67
Round up = 2 Power per Movement Point
```

The design passes the Minimum Mobility requirement:

```text
Reactor Output      = 12
Movement Power Cost = 2

12 ≥ 2
```

At maximum burn — 6 Power allocated to Propulsion — *Archibald Henderson* buys **3 Movement Points**.

```text
6 Power ÷ 2 Power per MP = 3 MP
```

That is enough to advance two hexes and swing one hex-side, with 6 Power left for sensors, shields, weapons, and other systems.

Strip the drop bays and armor and movement gets cheaper. Load her for an assault and every hex costs.

The manifest decides.

---

### Multiple-Engine Example

A larger warship has:

```text
Total Mass = 138
Mass Factor = 14
Reactor Output = 20
```

A single Rating 6 engine gives:

```text
Total Engine Rating = 6

14 ÷ 6 = 2.33
Movement Power Cost = 3
```

The ship can move, but propulsion is expensive.

The designer adds a Rating 4 engine.

```text
Total Engine Rating = 6 + 4 = 10
```

After accounting for the additional engine and its Superstructure, assume the ship's Mass Factor rises to 15.

Its new Movement Power Cost is:

```text
15 ÷ 10 = 1.5
Movement Power Cost = 2
```

The additional propulsion made the ship heavier, but reduced the Power required for each Movement Point.

Large ships therefore tend to demand larger propulsion plants. More engines add thrust, but they also add mass and require more structure.

There is no free tonnage.
