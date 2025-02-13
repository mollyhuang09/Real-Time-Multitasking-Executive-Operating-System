# Real-Time-Multitasking-Executive-Operating-System

Implemented a real-time executive (RTX) system on the ARM Cortex M4 microprocessor. The specific chip used is the STM32F401RE, which has 96KB of RAM and 512KB of on-chip flash memory. The chip also contains an on-chip UART, JTAG debug interface accessed via the STLink utility, and several on-chip timers. The RTX provides a basic multi-programming environment that supports priority (via deadlines), pre-emption, and dynamic memory management. 

Implemented an API that does the following: 
- Dynamic Task Management. The RTX supports a fixed number of tasks, specified at compile-time. The RTX supports task creation and termination during runtime. It also supports multiple concurrent tasks and allows constant switching between tasks, saving the information of all running tasks. 
- Dynamic Memory Management. The RTX supports dynamic memory allocation on the RAM using the First Fit allocation scheme and a freelist structure.
- Real-Time Scheduling. The RTX supports pre-emptive scheduling using the Earliest Deadline First scheduler, timer-based interruption (using SysTick) and priority.
