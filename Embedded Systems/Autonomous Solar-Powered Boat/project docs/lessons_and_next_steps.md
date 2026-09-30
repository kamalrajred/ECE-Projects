# Lessons and Next Steps

[← Back to project README](../README.md)

## Lessons learned

| Lesson | Detail |
| :-- | :-- |
| **Plan the layout in CAD first.** | Because component placement was worked out in the enclosure model, the physical assembly was straightforward. The only real task left was wiring correctly. |
| **Design for the power budget.** | With a small panel under weak light, the tracker's own draw (servos and sensors) matters. Measuring *net* power, not just panel output, is what made the comparison honest. |
| **More buoyancy is not automatically better.** | The raft was far more buoyant than necessary. That made the boat very stable, but it left the components exposed from above and did not solve waterproofing. |
| **Scope needs ruthless prioritizing.** | Propulsion and active marine-life tracking were dropped for time and budget reasons so the team could prove the most important claim: that tracking beats a fixed panel. |
| **Some requirements need long tests.** | Night shutdown could not be validated without a multi-day continuous test, which is a good reminder to plan test duration when writing requirements. |

## Known limitations

- Electronics were not fully waterproofed.
- Testing was in a tank with a lamp at about 300 W/m², not in real sun or waves.
- Low-light shutdown was not tested.
- Propulsion and autonomous navigation were not built.

## If there were a second design cycle

The team would put **less effort into the tracking mechanism** itself, since the first prototype proved it, and **more effort into real-world conditions**:

1. **Test in a lake or pond**, to get harsher conditions than the controlled tank and produce concrete evidence of viability.
2. **Implement and test night shutdown**, so the device stops tracking when tracking no longer pays for itself.
3. **Improve waterproofing**: soldered and thermally shielded connections, and waterproof servos.
4. **Add a gyroscope** to help counteract boat motion.
5. **Improve power efficiency at night.**
6. **Add the boat's tracking functionality**, to prepare for a real marine-life tracking test.
7. **Then design for the open ocean.**

## Skills the next cycle would exercise

- Soldered, sealed connections in place of breadboard wiring
- Gyroscope integration alongside the light sensors
- Power-efficiency and night-mode behavior
- Field testing in open water
