# Skills Demonstrated

[← Back to project README](../README.md)

Each skill below is tied to specific evidence in this project, so it can be checked.

## Embedded systems and firmware

| Skill | Evidence |
| :-- | :-- |
| Arduino programming (C/C++) | A light-tracking control loop that drives two servos ([Firmware](firmware.md)) |
| Analog sensor reading (ADC) | Four photoresistors read through analog inputs |
| Closed-loop control | Differential comparison of opposite sensor pairs with a dead-band threshold and incremental servo stepping |
| Sensor calibration | A software offset to compensate for sensor-to-sensor mismatch |
| Debugging | Serial-monitor output of raw readings |
| Servo actuation | A two-axis pan/tilt gimbal, tracking at about 60 degrees per second |

## Electrical and power systems

| Skill | Evidence |
| :-- | :-- |
| Breadboard prototyping and wiring | Full electronics assembly, using components planned in CAD |
| Solar charging systems | Solar panel, Sunny Buddy charge circuit, and onboard battery |
| Power budgeting | Checked that the solar panel supports the Arduino, Sunny Buddy, photosensors, and servos |
| Net-power measurement | Measured power into the battery, including the tracker's own overhead |

## Mechanical design and fabrication

| Skill | Evidence |
| :-- | :-- |
| 3D CAD modeling | Electronics mount with walled compartments and mounting holes ([Design and Build](design_and_build.md)) |
| 3D printing | The printed enclosure |
| Design for assembly | Component layout planned in CAD before wiring |
| Buoyancy and stability design | Foam and pool-noodle raft sized for panel motion and waves |
| Materials selection | Choosing lab-available foam for buoyancy |

## Test, validation, and data analysis

| Skill | Evidence |
| :-- | :-- |
| Experiment design | Controlled A/B test, gimbal vs. fixed panel ([Testing and Results](testing_and_results.md)) |
| Test calibration | Lamp calibrated to about 300 W/m² and angled to match Ann Arbor's sun geometry |
| Data aggregation and visualization | Raw-power graphs aggregated into energy graphs |
| Stating assumptions and limits | Explicit assumptions and a limitations list |
| Quantified results | About 40% more energy and about 60 deg/s tracking speed |

## Engineering process

| Skill | Evidence |
| :-- | :-- |
| Requirements engineering | Six requirements, each evaluated against results ([Requirements vs. Outcomes](requirements_and_outcomes.md)) |
| Scope management | Dropped propulsion and tracking to protect the key goal |
| Design iteration planning | Second-design-cycle plan ([Lessons and Next Steps](lessons_and_next_steps.md)) |
| Honest self-assessment | Partially-met requirements documented with reasons |

## Professional skills

| Skill | Evidence |
| :-- | :-- |
| Technical writing | A formal 20-page team report ([PDF](../report/Ohmericans_Final_Report.pdf)) |
| Cost and stakeholder analysis | [Business and Cost Analysis](business_and_cost_analysis.md) |
| Teamwork | Four-person engineering team with a shared deliverable |
| Research | Cited sources on marine tracking, legal limits, solar trackers, and marine components |

## Tools and technologies

Arduino, C/C++, servo motors, photoresistors, solar panel, Sunny Buddy charge circuit, onboard battery, breadboard prototyping, 3D CAD, 3D printing, serial debugging, lab test equipment (lamp, water tank), and data graphing and analysis.
