# Software Process Models: From Waterfall to Agile

This presentation introduces software processes and compares common development
approaches, then considers how process choices fit two different products:
Netflix's streaming service and Riot Games' League of Legends.

## Author

- **Name:** Truong Phat Tu
- **Course/section:** BLA SWE 1 2026
- **Program:** Master of Computer Science
- **Institution:** Concordia University Chicago

## Overview

A software process is an organized set of activities for developing and
maintaining a software system. The presentation covers the four fundamental
activities:

- **Specification** — define what the system should do.
- **Design and implementation** — shape the solution and build the software.
- **Validation** — check that the system meets its specification and user needs.
- **Evolution** — update the system as defects, environments, and requirements change.

It also explains how these activities appear in QA automation: requirements are
turned into test cases, application and test code are developed, tests validate
the system, and regression tests help protect existing behavior as the system
changes.

## Topics

1. **Software process fundamentals** — activities, roles, products, and
   preconditions and postconditions.
2. **Process models** — plan-driven and agile approaches, and why real projects
   often combine elements of both.
3. **Waterfall** — sequential phases, upfront planning, documentation, and
   phase reviews; suited to stable requirements and environments where formal
   coordination matters.
4. **Incremental development** — deliver usable functionality in stages and
   use customer feedback to guide later increments.
5. **Integration and configuration** — assemble and adapt existing software,
   frameworks, or services instead of building every component from scratch.
6. **Software evolution** — corrective maintenance for faults, adaptive
   maintenance for environmental changes, and perfective maintenance to improve
   functionality or performance.
7. **Coping with change** — use prototyping to explore requirements and designs,
   and incremental delivery to get feedback early and manage changes in smaller
   pieces.
8. **Industry examples** — compare streaming-service requirements with
   multiplayer-game requirements and release practices.

## Netflix and Riot Games comparison

The presentation contrasts the needs of a cloud-based streaming service with
those of a competitive, real-time multiplayer game:

| Area | Streaming service | Multiplayer game |
|---|---|---|
| Core concerns | Video encoding, content delivery, recommendations, and adaptive streaming | Game-client rendering, authoritative game servers, low-latency networking, and matchmaking |
| Typical change and feedback | Continuous deployment, telemetry, experiments, and short feedback loops | Gameplay balance, community feedback, scheduled patches, and urgent hotfixes |
| Process emphasis | Cloud-native services, automation, and frequent incremental delivery | Structured release increments, extensive testing, and predictable patch cadence |
| Main challenge | Coordinating distributed services while maintaining availability and performance | Balancing rapid gameplay changes with stability, synchronization, and competitive integrity |

These examples illustrate that process selection should reflect the product's
architecture and risks rather than follow a single universal template.

## Main takeaways

- No one software process is right for every project.
- Stable requirements and formal constraints can favor plan-driven practices;
  changing requirements and the need for early feedback can favor incremental
  and agile practices.
- Teams can combine approaches—for example, retaining formal planning where
  needed while delivering and validating functionality incrementally.
- Evaluate a process against the software type, team, customer expectations,
  regulation and safety needs, cost, risk, and release frequency.
- Changes have costs beyond implementation: they can affect schedules, require
  regression testing, and make documentation outdated.

## Source

This README summarizes the presentation transcript in [`swe_2_mp3.srt`](./swe_2_mp3.srt).

## Links

- YouTube: URL to be added
- LinkedIn: URL to be added

## References

1. Royce, W. W. (1970). Managing the development of large software systems.
   *Proceedings of IEEE WESCON, 26*, 328–338.
2. Sommerville, I. (2015). *Software Engineering* (10th ed.). Pearson.
3. Mokhtar, R., & Khayyat, M. (2022). A comparative case study of waterfall
   and agile management. *SAR Journal - Science and Research*, 52–62.
   https://doi.org/10.18421/SAR51-07
4. Sommerville, I. (2015). *Software Engineering* (10th ed.). Pearson.
   Foundational reference for Waterfall phases, incremental development,
   interleaving specification and development, and plan-driven versus agile
   methodologies.
5. F5 NGINX Developer Blog. (2015). *Adopting microservices at Netflix:
   Lessons for architectural design*. F5 Networks. Reference for Netflix's
   microservices architecture, cloud deployment strategies, and independent
   build and deployment processes.
6. Riot Games Engineering. (2016–2021). *The Riot Games API: Deep Dive* and
   *Keeping Legacy Software Alive: A Case Study*. Riot Games official news and
   technology articles. References for live-service patch cadences,
   client-server synchronization, and multi-region infrastructure.