# CppCompile: 12-Week Accelerated C++ Compiler Developer Guide

## 🎯 Goal

To gain the foundational C++ systems knowledge, modern design patterns, and initial LLVM/MLIR exposure required to contribute to or build a sophisticated compiler or high-performance toolchain.

## 📖 Overview

This repository documents an intensive **12-week, 26-hour-per-week** learning sprint focused on:

- **Modern C++** (C++17/20)
- **Low-level memory management**
- **Compiler infrastructure** (Lexer, Parser, AST, and early MLIR concepts)

This resource aims to be the go-to guide for anyone transitioning from basic programming to systems-level C++ development.

## 📚 Syllabus Overview

This accelerated timeline is divided into three focused phases:

| Phase | Focus Area | Duration |
|-------|------------|----------|
| **Phase 1** | C++ Fundamentals & System Core | Weeks 1-4 |
| **Phase 2** | Advanced C++ & Design Patterns | Weeks 5-8 |
| **Phase 3** | Compiler Foundations & Project Jumpstart | Weeks 9-12 |

### 📅 Detailed Syllabus

| Week | Day & Time Block | Topic/Task | Focus & Deliverable (Goal) | Resource Reference |
|------|------------------|------------|----------------------------|-------------------|
| **Week 1** (Oct 27–Nov 2) | Mon (3h): 2–5 PM | Environment Setup, Basic Syntax (Variables, I/O) | Get the compiler running (VS Code/CMake). Compile/Run "Hello World" and a simple I/O program. | LearnCpp.com (Ch 0–4) |
| | Tue (3h): 2–5 PM | Control Flow (If/Loops), Functions | Master for loops, create multi-file project with headers. | LearnCpp.com (Ch 8–10) |
| | Wed (3h): 2–5 PM | Debugging: GDB/LLDB | Learn to set breakpoints, inspect variables, step into/over. | GDB/LLDB Official Docs (Basic Tutorial) |
| | Thu (3h): 2–5 PM | Classes, Structs, Access Modifiers | Define a Point or Vector class with private data. | LearnCpp.com (Ch 17.1–17.8) |
| | Fri (3h): 2–5 PM | Constructors, Destructors, const | Master initialisation lists; understand resource cleanup. | LearnCpp.com (Ch 17.9–17.16) |
| | Sat (5.5h): 1–5 PM, 8:30–10 PM | Project 1: Simple Class Utility | Build a class that manages a resource (e.g., a simple custom logger). | Hands-on Coding |
| | Sun (5.5h): 1–5 PM, 8:30–10 PM | Tool Mastery: CMake | Complete a basic tutorial: create a CMakeLists.txt for a multi-file project and build it. | Official CMake Tutorial |
| **Week 4** (Nov 17–23) | Mon (3h): 2–5 PM | std::unique_ptr (Ownership) | **CRITICAL**: Understand how it guarantees single ownership. | LearnCpp.com (Ch 18.5); cppreference.com |
| | Tue (3h): 2–5 PM | std::vector Deep Dive | Size vs Capacity, Reserve, Iterators, and Performance Implications. | cppreference.com |
| | Wed (3h): 2–5 PM | std::map vs std::unordered_map | Understand hash-table vs tree implementation, and complexity (O(1) vs O(logn)). | cppreference.com |
| | Thu (3h): 2–5 PM | Move Semantics 1: R-value References | The && syntax and the concept of "stealing" data. | LearnCpp.com (Ch 23.3) |
| | Fri (3h): 2–5 PM | Move Semantics 2: Move Constructor/Assignment | Implement the move special members to avoid expensive deep copies. | LearnCpp.com (Ch 23.4–23.6) |
| | Sat (5.5h): 1–5 PM, 8:30–10 PM | Project 2: Refactoring for Ownership | Take Project 1 (or any class with raw pointers) and refactor it entirely to use std::unique_ptr and move semantics. | Hands-on Coding |
| | Sun (5.5h): 1–5 PM, 8:30–10 PM | Advanced Bitwise Operations | Bit flags, masking, and simple data packing/unpacking. | LearnCpp.com (Ch O) |
| **Week 5** (Nov 24–30) | Mon (3h): 2–5 PM | Inheritance & Polymorphism | Base/Derived classes, Public/Private inheritance. | LearnCpp.com (Ch 21) |
| | Tue (3h): 2–5 PM | Virtual Functions & Abstract Classes | **CRITICAL**: The mechanism for runtime type dispatch (used heavily in LLVM). | LearnCpp.com (Ch 22) |
| | Wed (3h): 2–5 PM | The Visitor Pattern (Theory) | Understand how it enables operation separation (Crucial for AST traversal). | Refactoring Guru: Visitor |
| | Thu (3h): 2–5 PM | The Visitor Pattern (Implementation) | Implement the Visitor pattern on a simple custom class hierarchy. | Hands-on Coding |
| | Fri (3h): 2–5 PM | Exception Handling (Basics) | try/catch, std::exception hierarchy. Focus on RAII safety. | LearnCpp.com (Ch 24) |
| | Sat (5.5h): 1–5 PM, 8:30–10 PM | Project 3: Expression Tree | Build a simple class hierarchy (Literal, BinaryOp, UnaryOp) and implement the Visitor to print the expression. | Hands-on Coding |
| | Sun (5.5h): 1–5 PM, 8:30–10 PM | static_cast vs dynamic_cast | When and why to use each, and the runtime cost of dynamic_cast. | LearnCpp.com (Ch 12.11) |
| **Week 8** (Dec 15–21) | Mon (3h): 2–5 PM | Function Templates | Writing generic functions (e.g., a generic max() function). | LearnCpp.com (Ch 25.1) |
| | Tue (3h): 2–5 PM | Class Templates & Specialization | Creating generic data structures (e.g., a simple Maybe<T>). | LearnCpp.com (Ch 25.2–25.4) |
| | Wed (3h): 2–5 PM | const vs constexpr | Understanding compile-time constants and functions for optimisation. | cppreference.com |
| | Thu (3h): 2–5 PM | Tool: clang-tidy / clang-format | Set up coding standard enforcement for professional C++ development. | Clang Documentation |
| | Fri (3h): 2–5 PM | Concurrency Basics | std::thread, std::mutex, std::lock_guard (Focus on safe parallel operations). | C++ Concurrency in Action (Ch 2) |
| | Sat (5.5h): 1–5 PM, 8:30–10 PM | Project Refactor: Templates | Refactor Project 3 (Expression Tree) to be template-based where possible. | Hands-on Coding |
| | Sun (5.5h): 1–5 PM, 8:30–10 PM | Review & Catch-up | Solidify weaker topics from the first 8 weeks. | All Resources |
| **Week 9** (Dec 22–28) | Mon (3h): 2–5 PM | Compiler Theory: Lexing & Tokens | Read theory on tokenization. Define your AI language tokens (e.g., tok_matrix, tok_relu). | Crafting Interpreters (Ch 2–4) |
| | Tue (3h): 2–5 PM | LLVM Kaleidoscope Ch 1: The Lexer | Implement the Lexer for the toy language. **CODE**. | LLVM Kaleidoscope Tutorial |
| | Wed (3h): 2–5 PM | Compiler Theory: Parsing & AST | Read theory on Recursive Descent Parsing and Operator Precedence. | Crafting Interpreters (Ch 5–7) |
| | Thu (3h): 2–5 PM | LLVM Kaleidoscope Ch 2: The Parser & AST | Implement the Parser and the Expression AST nodes. **CODE**. | LLVM Kaleidoscope Tutorial |
| | Fri (3h): 2–5 PM | LLVM Style RTTI: isa<>, cast<>, dyn_cast<> | **CRITICAL**: Understand this custom type casting used throughout LLVM. | LLVM Documentation: Style RTTI |
| | Sat (5.5h): 1–5 PM, 8:30–10 PM | Project 4: Complete Lexer/Parser | Extend the Kaleidoscope code to handle a custom keyword relevant to AI (e.g., tensor or dot). | Hands-on Coding |
| | Sun (5.5h): 1–5 PM, 8:30–10 PM | LLVM IR Generation Theory | Read about Static Single Assignment (SSA) and the structure of LLVM IR. | LLVM Tutorial (Ch 3 Overview) |
| **Week 12** (Jan 12–18) | Mon (3h): 2–5 PM | LLVM Kaleidoscope Ch 3: Code Generation | Implement LLVM IR code generation for basic arithmetic. **CODE**. | LLVM Kaleidoscope Tutorial |
| | Tue (3h): 2–5 PM | LLVM Kaleidoscope Ch 4: JIT & Optimiser | Integrate the Just-In-Time (JIT) compiler and a basic optimization pass. **CODE**. | LLVM Kaleidoscope Tutorial |
| | Wed (3h): 2–5 PM | MLIR Core Concepts | Read: Context, Dialects, Operations, Attributes, Types. | MLIR Documentation (Getting Started) |
| | Thu (3h): 2–5 PM | MLIR: Defining a Custom Dialect | Start defining your first MLIR Dialect for AI Operations (e.g., a simple linalg or tensor op). | MLIR Custom Dialects Guide |
| | Fri (3h): 2–5 PM | Tool: Address Sanitizer / Valgrind | Learn to detect memory errors (use on a deliberately faulty code snippet). | Valgrind/ASan Official Docs |
| | Sat (5.5h): 1–5 PM, 8:30–10 PM | Final Project Prototype | Define a simple MLIR Operation and write a C++ function that creates and returns it. | Hands-on Coding |
| | Sun (5.5h): 1–5 PM, 8:30–10 PM | System Review & Planning | Review the full 12 weeks. Plan your next 3 months on extending the MLIR Dialect and implementing compiler passes. | Self-Directed |


## 📁 Repository Structure

The files are organized to separate notes, runnable code examples, and videos for optimal learning experience:

| Directory | Description |
|-----------|-------------|
| **`/Code`** | Contains all runnable C++ examples, organized by week and day (e.g., `w1_d1`, `w12_project`). Each folder includes a `CMakeLists.txt` |
| **`/Notes`** | Contains detailed notes, concepts, diagrams, and summaries of complex topics like RAII or the Visitor Pattern |
| **`/Projects`** | Contains larger, multi-file assignments (e.g., the final Lexer/Parser) |
| **`/Videos`** | Short, self-recorded clips explaining a concept or troubleshooting a specific bug—a quick reference for future learners organised in a weekly manner |
| **`README.md`** | This file |


## 🤝 Community & Contribution

This guide is meant to be a collaborative effort.

### 📝 Feedback Welcome
- Found an error in the notes? 
- Know a more modern way to achieve a goal? 
- **Open an issue!**

### 📚 Resources
If you know of an exceptional article, book, or video for a specific topic, please suggest it via a **Pull Request**.

---

## 🚀 Let's Build a Compiler!

Thank you for following along! Ready to dive into the world of C++ compiler development? Start with Week 1 and begin your journey to becoming a systems-level C++ developer.