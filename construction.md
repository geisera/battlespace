![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

# Ship Construction

Every ship begins with a mass.

Choose how large a ship you intend to build. That choice determines its Size Class, basic signature, minimum propulsion requirement, baseline movement cost, and the amount of machinery and protection the hull can carry.

You then spend that mass on engines, reactor, weapons, sensors, armor, and Superstructure.

A ship cannot exceed its chosen **Design Mass**.

Build a ship in five steps:

1. Choose Design Mass.
2. Derive Mass Factor, Size Class, Minimum Engine Rating, and Base MPC.
3. Install components.
4. Install Superstructure and armor.
5. Derive the final characteristics.

---

## 1. Choose Design Mass

Choose the ship's **Design Mass**.

Design Mass is the maximum Mass of the completed ship.

```text
Completed Mass ≤ Design Mass
```

Design Mass may be any whole number of Mass points.

| Design Mass | Size Class |
| ----------: | ---------: |
|        1–15 |     Size 1 |
|       16–35 |     Size 2 |
|       36–70 |     Size 3 |
|      71–120 |     Size 4 |
|        121+ |     Size 5 |

Choosing a larger ship gives you more Mass for equipment, armor, weapons, and structure.

Larger ships also require larger engines, more Power to move, and have a greater Base Signature.

---

## 2. Derive Mass Characteristics

Calculate the ship's **Mass Factor**.

```text
Mass Factor =
Design Mass ÷ 10,
rounded up
```

Mass Factor is a simplified measure of the ship's overall mass for game purposes.

It is used to determine:

* Minimum Engine Rating;
* Base Movement Power Cost;
* Base Signature;
* other rules that explicitly use ship mass.

### Size Class

Size Class is determined directly from Design Mass.

| Design Mass | Size Class |
| ----------: | ---------: |
|        1–15 |          1 |
|       16–35 |          2 |
|       36–70 |          3 |
|      71–120 |          4 |
|        121+ |          5 |

### Base Signature

```text
Base Signature = Mass Factor
```

Larger ships are easier to detect.

Other effects may modify Signature during play.

---

## Minimum Engine Rating

Every ship must install enough propulsion for its Design Mass.

```text
Minimum Engine Rating =
Mass Factor ÷ 2,
rounded up
```

The ship's **Total Engine Rating** must equal or exceed this value.

### Base Movement Power Cost

Design Mass also determines the ship's baseline cost to generate Movement Points.

```text
Base MPC =
Mass Factor × 0.75,
rounded up
```

**MPC** means **Movement Power Cost**.

Base MPC is the Power required to generate 1 MP before any benefit from engines above the minimum requirement.

| Design Mass | Mass Factor | Minimum Engine Rating | Base MPC |
| ----------: | ----------: | --------------------: | -------: |
|        1–10 |           1 |                     1 |        1 |
|       11–20 |           2 |                     1 |        2 |
|       21–30 |           3 |                     2 |        3 |
|       31–40 |           4 |                     2 |        3 |
|       41–50 |           5 |                     3 |        4 |
|       51–60 |           6 |                     3 |        5 |
|       61–70 |           7 |                     4 |        6 |
|       71–80 |           8 |                     4 |        6 |
|       81–90 |           9 |                     5 |        7 |
|      91–100 |          10 |                     5 |        8 |
|     101–110 |          11 |                     6 |        9 |
|     111–120 |          12 |                     6 |        9 |
|     121–130 |          13 |                     7 |       10 |
|     131–140 |          14 |                     7 |       11 |
|     141–150 |          15 |                     8 |       12 |
|     151–160 |          16 |                     8 |       12 |
|     161–170 |          17 |                     9 |       13 |
|     171–180 |          18 |                     9 |       14 |
|     181–190 |          19 |                    10 |       15 |
|     191–200 |          20 |                    10 |       15 |

For ships above Design Mass 200, continue the same progression.

Both Minimum Engine Rating and Base MPC increase as Design Mass increases.

---

## 3. Install Components

Components consume part of the ship's Design Mass.

Every rated component is purchased at a **Rating** from 1 to 6.

| Rating | Capacity | Component Mass | Superstructure | Total Mass |
| -----: | -------: | -------------: | -------------: | ---------: |
|      1 |       ×1 |              1 |              1 |          2 |
|      2 |       ×2 |              3 |              2 |          5 |
|      3 |       ×3 |              6 |              3 |          9 |
|      4 |       ×4 |             10 |              5 |         15 |
|      5 |       ×5 |             15 |              8 |         23 |
|      6 |       ×6 |             21 |             11 |         32 |

**Total Mass** includes both the component and the Superstructure required to mount it.

### Component Effects

| Component    | Effect                                                       |
| ------------ | ------------------------------------------------------------ |
| Engine       | Contributes to Total Engine Rating and may reduce MPC        |
| Sensor Array | +1 detection range band per Rating; Rating caps Sensor Power |

Weapons are purchased individually.

Each weapon lists its Component Mass, Superstructure requirement, and Total Mass.

See [Weapons](weapons.md).

Every ship must contain:

* one Reactor;
* at least one Engine;
* one Sensor Array.

---

## Engines

Engines determine how efficiently the ship converts Power into Movement Points.

A ship may carry more than one Engine.

Add the Ratings of all installed Engines together.

```text
Total Engine Rating =
sum of all installed Engine Ratings
```

Example:

```text
Rating 4 Engine
Rating 3 Engine

Total Engine Rating = 7
```

Individual Engines are limited to Rating 1–6.

Total Engine Rating has no inherent maximum.

The ship's Total Engine Rating must equal or exceed its Minimum Engine Rating.

```text
Total Engine Rating ≥ Minimum Engine Rating
```

### Engine Bonus

Engine Rating above the minimum improves movement efficiency.

```text
Engine Bonus =
Total Engine Rating - Minimum Engine Rating
```

If Total Engine Rating equals Minimum Engine Rating, Engine Bonus is 0.

### Final Movement Power Cost

Subtract Engine Bonus from Base MPC.

```text
Movement Power Cost =
Base MPC - Engine Bonus
```

Movement Power Cost can never be less than 1.

```text
Minimum MPC = 1
```

Each point of Engine Rating above the minimum therefore reduces MPC by 1, until MPC reaches 1.

Example:

A Design Mass 100 ship has:

```text
Mass Factor = 10
Minimum Engine Rating = 5
Base MPC = 8
```

With Total Engine Rating 5:

```text
Engine Bonus = 0
MPC = 8
```

With Total Engine Rating 6:

```text
Engine Bonus = 1
MPC = 7
```

With Total Engine Rating 8:

```text
Engine Bonus = 3
MPC = 5
```

With Total Engine Rating 10:

```text
Engine Bonus = 5
MPC = 3
```

Additional engines therefore consume Mass but reduce the Power required to maneuver.

---

## Reactors

The Reactor generates the ship's Power each round.

Choose the desired Reactor Output.

| Output | Component Mass | Superstructure | Total Mass |
| -----: | -------------: | -------------: | ---------: |
|      4 |              1 |              1 |          2 |
|      8 |              3 |              2 |          5 |
|     12 |              6 |              3 |          9 |
|     16 |             10 |              5 |         15 |
|     20 |             15 |              8 |         23 |
|     24 |             21 |             11 |         32 |

A ship carries one Reactor.

Reactor Output is divided among systems during play.

Typical uses include:

* propulsion;
* shields;
* sensors;
* weapons;
* special systems.

### Minimum Propulsion Requirement

Every completed ship must be capable of generating at least **1 Movement Point**.

Therefore:

```text
Reactor Output ≥ Movement Power Cost
```

A design that cannot satisfy this requirement is invalid.

The designer must:

* increase Total Engine Rating;
* install a larger Reactor;
* choose a lower Design Mass;
* or use some combination of these changes.

Because Base MPC increases with Design Mass, larger ships require progressively more Power unless the designer invests additional Mass in propulsion.

---

## 4. Install Superstructure and Armor

### Superstructure

Superstructure represents the ship's keel, trusses, component mounts, and load-bearing frame.

Every component requires Superstructure equal to its listed Superstructure requirement.

```text
Required Superstructure =
sum of all Component Superstructure requirements
```

Every point of Superstructure consumes 1 Mass.

Additional Superstructure may be installed to reinforce the ship.

```text
1 Superstructure = 1 Mass
```

Extra Superstructure increases Structure but reduces the Mass available for other systems.

### Armor

Armor is purchased by the point and assigned to the ship's four facings.

No facing may have 0 Armor.

```text
4 Armor Points = 1 Mass
```

Every 4 Mass of Armor requires 1 additional Superstructure.

Armor Mass and its supporting Superstructure both count against Design Mass.

---

## Mass Budget

All installed equipment must fit within the Design Mass.

```text
Used Mass =
Component Mass
+ Superstructure
+ Armor Mass
```

The design is legal only if:

```text
Used Mass ≤ Design Mass
```

Any unused Design Mass becomes **Hull Mass**.

```text
Hull Mass =
Design Mass - Used Mass
```

Hull Mass represents compartments, bulkheads, crew spaces, tanks, conduits, damage-control spaces, and other general hull volume not represented by a specific component.

Unused Mass is therefore not wasted.

It makes the ship tougher.

---

## 5. Derive Final Characteristics

After all components are installed, calculate the ship's final characteristics.

| Characteristic        | Formula                                     |
| --------------------- | ------------------------------------------- |
| Design Mass           | Chosen during Step 1                        |
| Mass Factor           | Design Mass ÷ 10, rounded up                |
| Size Class            | Determined by Design Mass                   |
| Base Signature        | Mass Factor                                 |
| Minimum Engine Rating | Mass Factor ÷ 2, rounded up                 |
| Total Engine Rating   | Sum of all Engine Ratings                   |
| Base MPC              | Mass Factor × 0.75, rounded up              |
| Engine Bonus          | Total Engine Rating − Minimum Engine Rating |
| Movement Power Cost   | Base MPC − Engine Bonus; minimum 1          |
| Reactor Output        | As purchased                                |
| Structure             | Superstructure ÷ 2, rounded up              |
| Hull Mass             | Design Mass − Used Mass                     |

---

# Movement Points

Movement Points are not purchased during construction.

They are generated during play by allocating Reactor Power to propulsion.

```text
MP Generated =
Propulsion Power ÷ Movement Power Cost,
rounded down
```

A ship cannot generate MP unless it allocates at least enough Power to meet its MPC.

Example:

```text
Movement Power Cost = 4
Propulsion Power = 12
```

Therefore:

```text
12 ÷ 4 = 3 MP
```

The ship generates **3 Movement Points**.

Movement Points may be spent to change the ship's position or facing.

See [Maneuver](maneuver.md).

---

# Worked Example

## SDC-468 *Archibald Henderson*

The player decides first that *Archibald Henderson* will be a **45 Mass** ship.

### Step 1: Design Mass

```text
Design Mass = 45
```

### Step 2: Mass Characteristics

```text
Mass Factor =
45 ÷ 10
= 5
```

A Design Mass of 45 places the ship in Size Class 3.

```text
Size Class = 3
Base Signature = 5
```

Minimum Engine Rating:

```text
5 ÷ 2 = 2.5
rounded up = 3
```

Base MPC:

```text
5 × 0.75 = 3.75
rounded up = 4
```

Therefore:

```text
Minimum Engine Rating = 3
Base MPC = 4
```

### Step 3: Components

| Component           | Rating | Capacity | Component Mass | Superstructure | Total Mass |
| ------------------- | -----: | -------- | -------------: | -------------: | ---------: |
| Reactor             |      — | 12 Power |              6 |              3 |          9 |
| Engine              |      3 | —        |              6 |              3 |          9 |
| Sensor Array        |      2 | —        |              3 |              2 |          5 |
| Medium Coilgun      |      — | —        |              3 |              2 |          5 |
| Point Defense Laser |      — | —        |              1 |              1 |          2 |
| **Totals**          |        |          |         **19** |         **11** |     **30** |

The Rating 3 Engine exactly meets the ship's Minimum Engine Rating.

```text
Total Engine Rating = 3
Minimum Engine Rating = 3
```

Therefore:

```text
Engine Bonus = 0
Movement Power Cost = 4
```

The ship has:

```text
45 - 30 = 15 Mass
```

remaining for Armor, additional Superstructure, and Hull Mass.

If the designer installs 32 Armor Points:

```text
Armor Mass = 8
Armor Superstructure = 2
```

The finished allocation becomes:

```text
Components           = 19
Component Structure  = 11
Armor                 = 8
Armor Structure       = 2

Used Mass             = 40
Hull Mass             = 5
```

### Propulsion

The ship has:

```text
Base MPC = 4
Engine Bonus = 0
Movement Power Cost = 4
```

If the captain allocates 8 Power to propulsion:

```text
8 ÷ 4 = 2 MP
```

*Archibald Henderson* generates **2 Movement Points**.

If the designer instead installs one additional Rating 1 Engine, Total Engine Rating becomes 4.

```text
Engine Bonus =
4 - 3
= 1
```

New MPC:

```text
4 - 1 = 3
```

With the same 8 Power allocated to propulsion:

```text
8 ÷ 3 = 2 MP
```

With 12 Power:

```text
12 ÷ 3 = 4 MP
```

The additional Engine consumes Mass but improves propulsion efficiency.

---

# Design Principle

Design Mass is the primary constraint.

As Design Mass increases:

* Minimum Engine Rating increases.
* Base MPC increases.
* Base Signature increases.
* More Mass becomes available for weapons, armor, systems, and structure.

Engines above the minimum reduce MPC, but they consume Mass.

A larger Reactor provides more Power, but it consumes Mass.

More armor improves protection, but it consumes Mass.

More Superstructure improves structural integrity, but it consumes Mass.

More weapons increase firepower, but they consume Mass.

Anything left over becomes Hull.

The player chooses the ship's size first.

Everything after that is compromise.
