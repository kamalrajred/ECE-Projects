# Requirements vs. Outcomes

[← Back to project README](../README.md)

Six requirements were defined up front to guide the prototype. Each one is evaluated below against what was actually built and measured.

| # | Requirement | Outcome |
| :-: | :-- | :-: |
| 1 | The prototype must float | **Met** |
| 2 | Electronics must be protected from splashing water | **Partially met** |
| 3 | The gimbal must track the sun through boat motion and the sun's daily movement | **Met** |
| 4 | All boat functions must be sustained by solar power | **Partially met / out of scope** |
| 5 | The tracker must shut down when light is too low | **Designed, not validated** |
| 6 | Tracking must outperform a fixed panel | **Met** (about 40% gain) |

---

## Requirement 1: The prototype must float: Met

**Design:** a thick raft of foam and pool noodles. A wide foam piece improves stability and keeps the boat from tipping due to panel movement or waves.

**Result:** The prototype floated. Even while the panel moved, it was never in any real danger of taking on water or capsizing.

## Requirement 2: Electronics protected from splashing water: Partially met

**Design:**
- A 3D-printed housing holds the electronics in place and shields them.
- The raft raises the electronics well above the water line.
- The photoresistors sit in water-protector housings (from the concept sketch).

**Result:** The foam and pool noodles were far more buoyant than needed, so the electronics sat high, which helped. However, nearly all electrical components were still **exposed from above**.

**What full waterproofing would need:** every connection soldered and thermally shielded, and waterproof servos.

## Requirement 3: Track the sun through boat and sun motion: Met

**Design:** four corner-mounted photosensors, read by the Arduino, which steers the two-axis panel toward the brightest direction ([Firmware](firmware.md)).

**Result:** The panel tracked the light source in all tests. It slews at about **60 degrees per second**, far faster than the sun moves. The team believes that is also enough for wave-induced boat motion, but **further testing is needed** to confirm that.

## Requirement 4: Everything sustained by solar power: Partially met / out of scope

**Original intent:** replicate the functions of existing autonomous boats, such as propulsion and active marine-life tracking.

**Result:** Propulsion and animal tracking were not feasible within the project's time and budget, so they were dropped. The solar panel **does** sustain the prototype's actual electronics: the Arduino, the Sunny Buddy, the photosensors, and the servos. Full-boat self-sufficiency was not demonstrated.

## Requirement 5: Shut down when light is too low: Designed, not validated

**Design:** when photosensor readings fall below a set minimum, the program stops the gimbal from searching, which saves power at night or when tracking would cost more than it earns.

**Result:** The report classes this as out of scope for testing. Validation would need a continuous test lasting days, which the project schedule did not allow. The report judges the implementation itself to be easy to achieve.

## Requirement 6: Tracking must beat a fixed panel: Met

This was the most important requirement. The measured gain was roughly **40% more energy** than a fixed panel, even after accounting for possible systematic error. That is significant, and the team believes it is well beyond the threshold needed to justify the tracker in a commercial product. Full method and data: [Testing and Results](testing_and_results.md).

---

## What this shows

- Requirements were written **before** building and checked **after** testing.
- Shortfalls are documented as such, with a reason and a plan to fix them, instead of being glossed over.
- Scope was managed. When time and budget ruled out propulsion and tracking, the team concentrated on the feature that mattered most, the tracking efficiency gain.
