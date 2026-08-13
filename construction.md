![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

# Ship Construction

Every ship begins with a mass.

Choose how large a ship you intend to build. That choice determines its Size Class, basic signature, propulsion requirements, and the amount of machinery and protection the hull can carry.

You then spend that mass on engines, reactor, weapons, sensors, armor, bays, and Superstructure.

A ship cannot exceed its chosen **Design Mass**.

Build a ship in five steps:

1. Choose Design Mass.
2. Derive Mass Factor and Size Class.
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

Choosing a larger ship gives you more Mass for equipment, armor, weapons, and structure. Larger ships also require more propulsion and have a greater Base Signature.

---

## 2. Derive Mass Characteristics

Calculate **Mass Factor** from Design Mass.

```text
Mass Factor = Design Mass ÷ 10, rounded up
```

Mass Factor is a simplified measure of the ship's overall mass for game purposes.

It is used to determine:

* Movement Power Cost;
* Base Signature;
* other rules that explicitly use ship mass.

### Base Signature

```text
Base Signature = Mass Factor
```

Larger ships are inherently easier to detect.

Other effects may modify Signature during play.

---

## 3. Install Components

Components consume part of the ship's Design Mass.

Every component except the reactor is purchased at a **Rating** from 1 to 6.

| Rating | Capacity | Mass | Superstructure Cost |
| -----: | -------: | ---: | ------------------: |
|      1 |       ×1 |    1 |                   1 |
|      2 |       ×2 |    3 |                   2 |
|      3 |       ×3 |    6 |                   3 |
|      4 |       ×4 |   10 |                   5 |
|      5 |       ×5 |   15 |                   8 |
|      6 |       ×6 |   21 |                  11 |

### Component Effects

| Component        | Effect                                                       |
| ---------------- | ------------------------------------------------------------ |
| Engine           | Contributes to Total Engine Rating                           |
| Sensor Array     | +1 detection range band per Rating; Rating caps Sensor Power |
| Cargo / Drop Bay | 2 bay units per Rating                                       |

Weapons are purchased individually. Each weapon lists its own Mass and Superstructure Cost.

See [Weapons](weapons.md).

Every ship must contain:

* one Reactor;
* at least one Engine;
* one Sensor Array.

---

## Engines

Engines determine how efficiently Reactor Power generates Movement Points.

A ship may carry any number of Engines.

Add their Ratings together.

```text
Total Engine Rating =
sum of all installed Engine Ratings
```

Example:

```text
Rating 4 Engine
Rating 3 Engine
Rating 2 Engine

Total Engine Rating = 9
```

Individual Engines are limited to Rating 1–6.

Total Engine Rating has no inherent maximum.

### Movement Power Cost

Once the engines are selected, calculate the Power required to generate one Movement Point.

```text
Movement Power Cost =
Mass Factor ÷ Total Engine Rating,
rounded up
```

Movement Power Cost can never be less than 1.

```text
Minimum Movement Power Cost = 1
```

A higher Total Engine Rating makes movement more Power-efficient.

It does not directly grant Movement Points.

---

## Reactors

The Reactor generates the ship's Power each round.

Choose the desired Reactor Output.

| Output | Mass | Superstructure Cost |
| -----: | ---: | ------------------: |
|      4 |    1 |                   1 |
|      8 |    3 |                   2 |
|     12 |    6 |                   3 |
|     16 |   10 |                   5 |
|     20 |   15 |                   8 |
|     24 |   21 |                  11 |

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

The designer must increase Engine Rating, increase Reactor Output, or choose a lower Design Mass.

---

## 4. Install Superstructure and Armor

### Superstructure

Superstructure represents the ship's keel, trusses, component mounts, and load-bearing frame.

Every component requires Superstructure equal to its listed Superstructure Cost.

```text
Required Superstructure =
sum of all Component Superstructure Costs
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

| Characteristic      | Formula                                                  |
| ------------------- | -------------------------------------------------------- |
| Design Mass         | Chosen during Step 1                                     |
| Mass Factor         | Design Mass ÷ 10, rounded up                             |
| Size Class          | Determined by Design Mass                                |
| Base Signature      | Mass Factor                                              |
| Total Engine Rating | Sum of all Engine Ratings                                |
| Movement Power Cost | Mass Factor ÷ Total Engine Rating, rounded up; minimum 1 |
| Reactor Output      | As purchased                                             |
| Structure           | Superstructure ÷ 2, rounded up                           |
| Hull Mass           | Design Mass − Used Mass                                  |

---

# Movement Points

Movement Points are not purchased during construction.

They are generated during play by allocating Reactor Power to propulsion.

```text
MP Generated =
Propulsion Power ÷ Movement Power Cost,
rounded down
```

Example:

A ship has:

```text
Mass Factor = 5
Total Engine Rating = 3
```

Its Movement Power Cost is:

```text
5 ÷ 3 = 1.67

Movement Power Cost = 2
```

If the captain allocates 6 Power to propulsion:

```text
6 ÷ 2 = 3 MP
```

The ship receives **3 Movement Points** for that Action Phase.

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

A Design Mass of 45 places the ship in **Size Class 3**.

```text
Size Class = 3
Base Signature = 5
```

### Step 3: Components

| Component           | Rating | Capacity |   Mass | Superstructure |
| ------------------- | -----: | -------- | -----: | -------------: |
| Reactor             |      — | 12 Power |      6 |              3 |
| Engine              |      3 | —        |      6 |              3 |
| Sensor Array        |      2 | —        |      3 |              2 |
| Medium Coilgun      |      — | —        |      3 |              2 |
| Point Defense Laser |      — | —        |      1 |              1 |
| Drop Bay            |      2 | 4 units  |      3 |              2 |
| **Components**      |        |          | **22** |         **13** |

Required Superstructure adds another 13 Mass.

```text
Component Mass = 22
Superstructure = 13

Used Mass = 35
```

The designer therefore has:

```text
45 - 35 = 10 Mass
```

remaining for Armor and Hull Mass.

If 8 Mass is used for Armor:

```text
Armor = 32 points
Armor Mass = 8
```

The armor requires 2 additional Superstructure.

```text
Used Mass =
22 Component
+ 15 Superstructure
+ 8 Armor
= 45
```

The ship completely fills its Design Mass.

```text
Hull Mass = 0
```

If the designer instead installs only 16 Armor Points:

```text
Armor Mass = 4
Armor Superstructure = 1

Used Mass =
22 + 14 + 4
= 40
```

The remaining 5 Mass becomes Hull Mass.

```text
Hull Mass = 5
```

The player has made a construction choice:

**more directional protection, or more general hull durability.**

### Propulsion

The ship has one Rating 3 Engine.

```text
Total Engine Rating = 3
Mass Factor = 5

Movement Power Cost =
5 ÷ 3
= 2 Power
```

With 6 Power allocated to propulsion:

```text
6 ÷ 2 = 3 MP
```

*Archibald Henderson* generates **3 Movement Points**.

---

# Design Principle

Design Mass is the constraint.

Everything installed aboard the ship competes for that Mass.

More engines improve movement efficiency but consume Mass.

A larger Reactor provides more Power but consumes Mass.

More armor improves protection but consumes Mass.

More Superstructure improves structural integrity but consumes Mass.

More weapons increase firepower but consume Mass.

Anything left over becomes Hull.

The player chooses the size of the ship first.

Everything after that is compromise.
