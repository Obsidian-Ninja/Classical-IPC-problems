IPC Problems in C++
This repository contains classic Inter-Process Communication (IPC) problems implemented in C++. The implementations cover the Reader-Writer, Producer-Consumer, and Dining Philosophers problems, demonstrating essential synchronization concepts for process coordination and efficient resource sharing.

Table of Contents
Description
Problems
Reader-Writer
Producer-Consumer
Dining Philosophers
Setup and Compilation
Usage
License
Description
This project implements three of the most well-known IPC synchronization problems, frequently encountered in operating systems and concurrency control:

Reader-Writer Problem: Managing access to a shared resource for multiple readers and writers.
Producer-Consumer Problem: Coordinating processes that produce and consume items in a shared buffer.
Dining Philosophers Problem: Simulating resource sharing for multiple processes (philosophers) needing access to limited resources.
Each problem is solved using mutexes, semaphores, and condition variables in C++.

Problems
Reader-Writer
The Reader-Writer Problem deals with synchronizing access to a shared resource where multiple readers can read concurrently, but writing must be exclusive. The solution ensures data consistency and avoids race conditions.

Key Features:
Prioritizes either readers or writers depending on the implementation.
Solves reader-preference, writer-preference, or no-preference versions of the problem.
Producer-Consumer
In the Producer-Consumer Problem, two types of processes interact with a shared buffer: producers add items, and consumers remove them. This implementation ensures proper coordination so that:

Producers wait if the buffer is full.
Consumers wait if the buffer is empty.
Key Features:
Bounded buffer implementation.
Efficient use of semaphores for empty and full buffer tracking.
Dining Philosophers
The Dining Philosophers Problem models five philosophers sitting at a table with a limited number of resources (forks) shared among them. It prevents deadlock and starvation using various synchronization techniques.

Key Features:
Demonstrates different solutions to avoid deadlocks and starvation.
Uses mutexes to lock and unlock resources.
