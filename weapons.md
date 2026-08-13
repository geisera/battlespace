![Battlespace Banner 3](assets/battlespace-banner.png)

[:back: Back](readme.md)

---

# Weapons

Weapons are installed during ship construction.

Each weapon has a fixed **Component Mass**, **Superstructure requirement**, **Total Mass**, **Power Requirement**, **Damage**, and **Range**.

Weapons are purchased individually. They do not use the 1–6 component Rating table unless a weapon rule specifically says otherwise.

---

## Weapon Characteristics

| Characteristic | Meaning |
| --- | --- |
| **Component Mass** | Mass of the weapon itself |
| **Superstructure** | Mass required to mount and support the weapon |
| **Total Mass** | Component Mass + Superstructure |
| **Power** | Reactor Power required to fire the weapon once |
| **Damage** | Damage caused by a successful hit |
| **Range** | Maximum range band at which the weapon may attack |
| **Arc** | Facings from which the weapon may fire |
| **Special** | Additional rules that apply to the weapon |

```text
Total Weapon Mass =
Component Mass + Superstructure
```

### Missile Launchers

| Weapon | Component Mass | Superstructure | Total Mass | Power | Damage | Range | Arc | Special |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | --- | --- |
| Light Missile Launcher | 2 | 1 | 3 | 1 | 4 | 5 | 360° | Missile |
| Medium Missile Launcher | 3 | 2 | 5 | 1 | 6 | 6 | 360° | Missile |
| Heavy Missile Launcher | 6 | 3 | 9 | 2 | 9 | 7 | 360° | Missile |

Missile Launchers fire self-propelled weapons.

Each launch requires the listed Power.

Missiles may remain in play after launch and may be intercepted by Point Defense.

Ammunition is not tracked in this version of the rules.

### Missile Magazines

Missile Magazines store missile ammunition.

Each Magazine has a **Capacity**. Different missile sizes consume different amounts of that Capacity.

| Missile Type | Capacity per Missile |
| --- | ---: |
| Light Missile | 1 |
| Medium Missile | 2 |
| Heavy Missile | 4 |

Missile Magazines are purchased at Rating 1–6.

| Rating | Magazine Capacity | Light Missiles | Medium Missiles | Heavy Missiles | Component Mass | Superstructure | Total Mass |
| ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| 1 | 8 | 8 | 4 | 2 | 1 | 1 | 2 |
| 2 | 16 | 16 | 8 | 4 | 3 | 2 | 5 |
| 3 | 24 | 24 | 12 | 6 | 6 | 3 | 9 |
| 4 | 32 | 32 | 16 | 8 | 10 | 5 | 15 |
| 5 | 40 | 40 | 20 | 10 | 15 | 8 | 23 |
| 6 | 48 | 48 | 24 | 12 | 21 | 11 | 32 |

A Magazine may contain any mix of compatible missiles.

The total Capacity used may not exceed the Magazine's Capacity.

```text
Capacity Used =
Light Missiles
+ (Medium Missiles × 2)
+ (Heavy Missiles × 4)