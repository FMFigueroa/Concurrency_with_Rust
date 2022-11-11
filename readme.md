# Concurrency with Rust

## Chapter 1 - Machine Architecture and Getting Started with Rust

- Discusses modern CPU architectures, focusing specifically on x86 and ARM. These two architectures will be the focus of the book. The reader is assumed to be familiar with Rust, but we will also discuss verifying that your installation works as expected.

## Chapter 2 - Sequential Rust Performance and Testing

- Introduces inspecting the performance of a Rust program. The details of the underlying computer hardware are especially important in this: cache interactions, memory layout, and exploiting the nature of the problem domain are key to writing fast programs.
However, fast doesn't matter if the results are inaccurate. This chapter also focuses on testing in Rust.

## Chapter 3 - The Rust Memory Model – Ownership, References and Manipulation

- Discusses the memory model of Rust, focusing specifically on what makes Rust memory safe, how the language is constrained to achieve such safety and how
these constraints influence the fundamental types' implementations. The reader will understand the borrow checker and its ways at the close of this chapter.

## Chapter 4 - Sync and Send – the Foundation of Rust Concurrency

- Is the first in which notions of concurrency make their appearance. The chapter discusses the Sync and Send traits, both why they exist and their implications. The chapter closes with a concrete demonstration of a multithreaded Rust program. Not the last, either.

## [Chapter 5 - Locks – Mutex, Condvar, Barriers and RWLock](https://github.com/FMFigueroa/Concurrency_with_Rust/tree/main/src/Chapter_05)

- Introduces the coarse synchronization methods available to the Rust programmer. Each is examined in turn and demonstrated in context of an industrial Rust project, hopper. The
coarse synchronization methods are elaborated on in more detail in a series of smaller projects and data structures.

## Chapter 6 - Atomics – the Primitives of Synchronization

- Introduces fine synchronization in terms of atomic primitives available on all modern CPUs. This is an exceedingly difficult topic, and a deep investigation into atomic programming and its methods is carried out. The chapter lock-free, atomic data structures, and production-grade codebases.

## Chapter 7 - Atomics – Safely Reclaiming Memory

- Discusses at length one of the key difficulties of atomic programming in any language—safely deallocating memory. The main three methods—reference counting, hazard pointers, epoch-based reclamation—are each discussed in great detail, and production-worthy codebases are investigated. Crossbeam, especially, is discussed in great detail.

## Chapter 8 - High-Level Parallelism – Threadpools Parallel Iterators and Processes

- Motivates and explains the implementation of thread pooling. Having this knowledge in hand, the Rayon project is investigated and subsequently used in a complex project that benefits greatly from simple data parallelism.

## Chapter 9 - FFI and Embedding – Combining Rust and Other Languages

- Extends the final project of Chapter 8, High-Level Parallelism – Threadpools, Parallel Iterators, and Processes by embedding C code into it. The rlua project, a convenient
library to extend Rust programs with lua programs, is discussed. The chapter closes by compiling Rust for embedding into C, Python, and Erlang projects.

## Chapter 10 - Futurism – Near-Term Rust

Closes with a discussion of the near-term changes to the language that are
apropos to parallel programmers, as well as a few miscellaneous remarks.



