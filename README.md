Purpose / Problem
 Design a real-time embedded system capable of monitoring multiple temperature sensors, detecting threshold violations, and logging alert events using deterministic, low-level firmware suitable for resource-constrained environments.
My Role
 Individually designed and implemented the complete system in ARM Thumb-2 assembly, including interrupt handling, memory management, and system verification.
Technical Details
Implemented a 1 ms SysTick interrupt-driven architecture for periodic sensor sampling and processing


Designed a per-sensor finite state machine to detect high/low threshold violations, manage alert persistence, and handle alert clearance


Developed a custom xorshift pseudo-random number generator to simulate realistic temperature drift across multiple sensors


Enforced safe value clamping to maintain valid sensor ranges and prevent overflow conditions


Created a memory-resident, timestamped event logging system using compact data structures optimized for RAM usage


Manually managed stack, heap, vector table, and exception handlers in accordance with AAPCS and Cortex-M4 architectural requirements


Verified system behavior using the Keil µVision simulator by inspecting live RAM contents and interrupt execution without external hardware or I/O interfaces
