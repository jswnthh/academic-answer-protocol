# Operating Systems — CIA I Subject Rubric

**Source:** Uploaded *CIA I Operating Systems Answer Key*, TY/BCA Semester V, subject code 320C5A, 2026–27. Prescribed reference: Silberschatz, Galvin & Gagne, *Operating System Concepts*, 9th ed. The source lists topic keywords and a general evaluation rubric, **not** fully worked answers for every question.

## Evaluation matrix (as supplied)

| Evaluation component | 2 marks | 5 marks | 10 marks |
|---|---:|---:|---:|
| Definition / core concept | 1 | 1 | 2 |
| Key points / components | 1 | 2 | 3 |
| Diagram / Gantt chart / process representation | — | 1 | 2 |
| Algorithm / working / calculation / synchronization logic | — | 1 | 2 |
| Result / example / interpretation | — | — | 1 |
| **Total** | **2** | **5** | **10** |

Marks are awarded proportionately for correct core concepts, OS terminology, logical explanation, appropriate diagrams/Gantt charts/algorithms and accurate calculations. Accept technically correct equivalents and valid alternative methods. When a component is not applicable, proportionately redistribute its marks among relevant components.

## Topic coverage and essential keywords

| Topic | Expected terminology |
|---|---|
| Operating system | System software; hardware/resource management; execution environment; intermediary; kernel |
| System calls and modes | System call; kernel service; trap/software interrupt; user/kernel mode; mode bit; privileged instructions; handler; parameters; return |
| Process states | New; ready; running; waiting/blocked; terminated; admission; dispatch; preemption; I/O completion; exit |
| PCB | Process state; program counter; CPU registers; scheduling; memory-management; accounting; I/O status |
| CPU scheduling | Ready queue; short-term scheduler; dispatcher; context switch; dispatch latency; save/restore state |
| Synchronization | Critical section; mutual exclusion; progress; bounded waiting; semaphores; atomic wait(P)/signal(V) |
| Producer-consumer | Bounded buffer; producer/consumer; mutex=1; empty=n; full=0; wait; signal |
| Deadlocks | Blocked processes; resources; circular dependency; necessary conditions; resource ordering; preemption |
| Busy waiting | Repeated testing/spinning; CPU cycles wasted; no blocking; reduced utilization |

## Calculation requirements
- **5-mark priority-scheduling question:** all processes arrive at 0; **smaller** priority number means higher priority; ties use FCFS. Process (burst, priority): P1(2,1), P2(8,4), P3(4,2), P4(5,2), P5(1,3). Show execution order/Gantt chart, completion, turnaround and waiting times.
- **10-mark scheduling comparison:** P1(2,2), P2(1,1), P3(8,4), P4(4,2), P5(5,3); all arrive at 0 in listed order. Compare FCFS, SJF, non-preemptive priority (**larger** number means higher priority), and RR (quantum=2). Show all four Gantt charts, each process's turnaround and waiting times, average waiting times, and identify the minimum. **The priority convention differs between the two questions; never assume one universal convention.**
- Formulas: Turnaround time = completion time − arrival time; waiting time = turnaround time − burst time. Check scheduling assumptions before calculation.

## Diagram and algorithm policy
- For conceptual process-state, PCB, semaphore and similar diagrams, provide a **textbook diagram reference/description only**; do not draw ASCII diagrams. Cite a chapter/figure number only if verified.
- For scheduling problems, **do show** the requested Gantt chart, preferably as a compact labeled table or ordered time intervals, because it is part of the numerical solution.
- For semaphore solutions, show correct pseudocode and explain mutual exclusion; reference a diagram if requested.

## Reference areas
Operating-System Structures; Processes; Process Synchronization; CPU Scheduling; Deadlocks. Do not invent exact page or figure numbers.
