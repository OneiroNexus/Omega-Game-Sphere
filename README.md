# Sensor timing for the Omega Game Sphere AR engine

**Aaron Michael Weis** · OneiroNexus · Version 0.1.0 · [ORCID 0009-0002-1906-148X](https://orcid.org/0009-0002-1906-148X)

## Why the engine needs sensor timing research

I’m developing the Omega Game Sphere as the device and game engine for a OneiroNexus augmented reality experience people can play by moving through physical space. The hardware and the engine have a shared problem. The hardware captures a movement or an interaction at a particular instant, and the engine has to decide when that measurement belongs in the game. The usefulness of the measurement depends on when it was taken, how soon it arrives, and whether it can be aligned with other observations. That makes sensor timing an engine requirement. [OneiroNexus community hub](https://oneironexus.com) · [The game](https://oneironexus.com/game)

Consider a player turning toward a virtual object. A measurement that arrives late or carries the wrong time can put the engine a step behind the player. In a shared scene, measurements with inconsistent timestamps can make two participants disagree about which event happened first. Those are examples of behavior the sensor and engine teams can test. The aim is to find out how much timing error changes what the game does and what a player sees.

## Why propose COQI

The Colorado Quantum Incubator publicly describes its open-access Quantum Timing Testbed as a third-party environment for testing timing technologies. I propose the COQI Quantum Timing Testbed as the site for evaluating the timing side of the Omega Game Sphere sensor design. The OneiroNexus work would define the engine’s requirements and build the candidate sensor interface. A timing testbed could supply an independent reference and controlled conditions to measure how sensor observations line up before the engine uses them. Access, equipment fit, and an agreed test plan would determine what can be measured there. [Colorado Quantum Incubator Quantum Timing Testbed](https://quantumincubator.org/quantum-testbed/)

The public experiment would start with a conventional timing baseline. It would measure clock offset and drift, compare the variation in capture-to-engine delay, and count late or out-of-order events. Replay of the same event stream would show whether those timing differences change event ordering or the engine’s response. If the conventional baseline meets the proposed engine requirements, that is a useful result. A candidate timing approach earns further work only if it improves a stated metric under a repeatable comparison.

## What the public record should establish

This brief records my project rationale and proposed evaluation. A later results release can identify the tested setup, publish the cleared measurements and their units, describe the baseline, and report where the results do and do not support a design change. This version describes the proposed evaluation. Work at COQI would require access, equipment fit, and an agreed test plan.

The motivation is straightforward. I want a physical action in OneiroNexus to produce a predictable event in the AR engine. Sensor timing is one part of that requirement, and a timing testbed gives us a way to measure it.
