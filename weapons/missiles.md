![Battlespace Banner 3](../assets/battlespace-banner.png)

[:back: Back](../readme.md)

---

# Missiles

Missiles are self-propelled weapons launched from dedicated Missile Launchers.

Each missile class has its own launcher, magazine, range, damage, and Movement Point allocation.

Missiles remain in play after launch and may be intercepted by Point Defense.

---

## Missile Characteristics

| Characteristic              | Meaning                                                    |
| --------------------------- | ---------------------------------------------------------- |
| **Launcher Mass**           | Mass of the launcher itself                                |
| **Launcher Superstructure** | Mass required to mount and support the launcher            |
| **Launcher Total Mass**     | Launcher Mass + Launcher Superstructure                    |
| **Launch Power**            | Reactor Power required to launch one missile               |
| **Magazine Mass**           | Mass of the magazine itself                                |
| **Magazine Superstructure** | Mass required to mount and support the magazine            |
| **Magazine Total Mass**     | Magazine Mass + Magazine Superstructure                    |
| **Missiles Stored**         | Number of missiles carried in one magazine                 |
| **Range**                   | Maximum range at which the missile may be launched         |
| **MP**                      | Movement Points available to the missile each Action Phase |
| **Damage**                  | Damage caused by a successful hit                          |

---

## Missile Launchers

Missile Launchers are purchased individually.

| Launcher                | Component Mass | Superstructure | Total Mass | Launch Power | Arc  |
| ----------------------- | -------------: | -------------: | ---------: | -----------: | ---- |
| Light Missile Launcher  |              2 |              1 |          3 |            1 | 360° |
| Medium Missile Launcher |              3 |              2 |          5 |            1 | 360° |
| Heavy Missile Launcher  |              6 |              3 |          9 |            2 | 360° |

```text
Launcher Total Mass =
Component Mass + Superstructure
```

Each launch requires the listed Power.

Launcher size determines which missile class it may fire.

```text
Light Missile Launcher  → Light Missile
Medium Missile Launcher → Medium Missile
Heavy Missile Launcher  → Heavy Missile
```

A Missile Launcher cannot fire without a compatible missile aboard the ship.

---

## Missile Performance

Each missile class has its own Range, Movement Points, and Damage.

| Missile        | Range | MP | Damage | Compatible Launcher     |
| -------------- | ----: | -: | -----: | ----------------------- |
| Light Missile  |     5 |  6 |      4 | Light Missile Launcher  |
| Medium Missile |     6 |  4 |      6 | Medium Missile Launcher |
| Heavy Missile  |     7 |  3 |      9 | Heavy Missile Launcher  |

### Range

Range is the maximum range at which the missile may be launched at a target.

### Movement Points

MP is the number of Movement Points the missile receives during each Action Phase after launch.

```text
Light Missile  = 6 MP
Medium Missile = 4 MP
Heavy Missile  = 3 MP
```

Missile MP does not require additional Power from the launching ship after launch.

Missiles use MP according to the missile movement rules.

### Damage

Damage is inflicted if the missile successfully hits its target.

```text
Light Missile  = 4 Damage
Medium Missile = 6 Damage
Heavy Missile  = 9 Damage
```

---

## Missile Magazines

Missile Magazines store missile ammunition.

There are three magazine types:

* Light Missile Magazine
* Medium Missile Magazine
* Heavy Missile Magazine

Each Magazine may only store missiles of its own class.

| Magazine                | Missiles Stored | Component Mass | Superstructure | Total Mass |
| ----------------------- | --------------: | -------------: | -------------: | ---------: |
| Light Missile Magazine  |              12 |              2 |              1 |          3 |
| Medium Missile Magazine |               6 |              2 |              1 |          3 |
| Heavy Missile Magazine  |               3 |              2 |              1 |          3 |

The three Magazine types have the same Mass and Superstructure requirement.

Larger missiles consume more internal volume, so heavier missile classes store fewer rounds.

```text
Light Missile Magazine  = 12 Light Missiles
Medium Missile Magazine = 6 Medium Missiles
Heavy Missile Magazine  = 3 Heavy Missiles
```

A ship may install more than one Missile Magazine of any type.

Each additional Magazine adds its full ammunition capacity and its full Mass and Superstructure cost.

Example:

```text
2 Light Missile Magazines

Missiles Stored = 24
Component Mass  = 4
Superstructure  = 2
Total Mass      = 6
```

Multiple compatible Missile Launchers may draw ammunition from the same Magazine.

---

## Missile Expenditure

Each Missile Launcher expends one compatible missile when it fires.

```text
1 Missile Launch =
1 Missile expended
```

A launcher cannot fire if no compatible missiles remain.

Example:

```text
3 Light Missile Launchers fire
= 3 Light Missiles expended
```

A single Light Missile Magazine begins with 12 missiles and can therefore support four full three-launcher salvos.

---

## Missile Summary

| Missile Class | Launcher Total Mass | Launch Power | Magazine Total Mass | Missiles per Magazine | Range | MP | Damage |
| ------------- | ------------------: | -----------: | ------------------: | --------------------: | ----: | -: | -----: |
| Light         |                   3 |            1 |                   3 |                    12 |     5 |  6 |      4 |
| Medium        |                   5 |            1 |                   3 |                     6 |     6 |  4 |      6 |
| Heavy         |                   9 |            2 |                   3 |                     3 |     7 |  3 |      9 |

Light missiles provide the highest speed and ammunition endurance.

Medium missiles trade speed and magazine capacity for greater range and damage.

Heavy missiles provide the greatest individual damage and longest range, but require the largest launcher, move the slowest, and provide the fewest shots per Magazine.