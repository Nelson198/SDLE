# Enunciado - Trabalho Prático

## SDLE - Sistemas Distribuídos em Larga Escala

### *Decentralized Aggregation*

#### Evaluation

* Groups can have 1 to 3 participants;

* **Report deadline**: 31/05/2020 (to be sent to cbm@di.uminho.pt and vitorenesduarte@gmail.com):
    * Each group should submit a short report (up to 6 pages) on the main challenges and choices. The report should contain:
        * Brief description of the algorithm;
        * Why was the algorithm picked ?
        * Brief description of the simulator;
        * In which way did the simulator help (in case it did) ? Did it find any implementation bug during development ?
* **Presentation**: 01/06/2020 via Blackboard Collaborate Ultra:
    * On the presentation day, each group will be asked to do a 10 minute presentation to the class.

* Choice of technology is free.

---

#### Theme

This project will explore **distributed aggregation algorithms**. These algorithms can be used to compute functions like COUNT, SUM and AVERAGE.

A survey of these algorithms can be found in: https://arxiv.org/pdf/1110.0725.pdf.

Each group should pick one of the algorithms described in the survey and implement / test such algorithm in the simulator that has been developed during the semester. The testing will depend on the algorithm and system model: if the algorithm tolerates message faults, faults should be injected; if it adapts to input value change, then values should evolve as it runs.

At this point, the simulator supports:

1. Sending of messages between processes;
2. Scheduling of local events (e.g. scheduling of a single timeout or periodic actions);
3. Network fault-injection (e.g. 10% of messages should be lost);
4. Periodic view-change (e.g. every 10s, the set of neighbours changes).

Where the *1.* and *2.* are used to specify algorithms and *3.* and *4.* are used to test them. Depending on the algorithm picked, some of the above four features may not be necessary.
