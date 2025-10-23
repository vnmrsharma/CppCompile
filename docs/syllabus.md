---
layout: default
title: Detailed Syllabus - CppCompile Course
---

# 📅 Detailed Syllabus

<div class="course-header">
  <h2>Complete 12-Week Curriculum</h2>
  <p>Intensive 26-hour per week learning sprint focused on modern C++ and compiler development</p>
</div>

<table class="syllabus-table">
  <thead>
    <tr>
      <th>Week</th>
      <th>Day & Time Block</th>
      <th>Topic/Task</th>
      <th>Focus & Deliverable (Goal)</th>
      <th>Resource Reference</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Week 1</strong> (Oct 27–Nov 2)</td>
      <td>Mon (3h): 2–5 PM</td>
      <td>Environment Setup, Basic Syntax (Variables, I/O)</td>
      <td>Get the compiler running (VS Code/CMake). Compile/Run "Hello World" and a simple I/O program.</td>
      <td>LearnCpp.com (Ch 0–4)</td>
    </tr>
    <tr>
      <td></td>
      <td>Tue (3h): 2–5 PM</td>
      <td>Control Flow (If/Loops), Functions</td>
      <td>Master for loops, create multi-file project with headers.</td>
      <td>LearnCpp.com (Ch 8–10)</td>
    </tr>
    <tr>
      <td></td>
      <td>Wed (3h): 2–5 PM</td>
      <td>Debugging: GDB/LLDB</td>
      <td>Learn to set breakpoints, inspect variables, step into/over.</td>
      <td>GDB/LLDB Official Docs (Basic Tutorial)</td>
    </tr>
    <tr>
      <td></td>
      <td>Thu (3h): 2–5 PM</td>
      <td>Classes, Structs, Access Modifiers</td>
      <td>Define a Point or Vector class with private data.</td>
      <td>LearnCpp.com (Ch 17.1–17.8)</td>
    </tr>
    <tr>
      <td></td>
      <td>Fri (3h): 2–5 PM</td>
      <td>Constructors, Destructors, const</td>
      <td>Master initialisation lists; understand resource cleanup.</td>
      <td>LearnCpp.com (Ch 17.9–17.16)</td>
    </tr>
    <tr>
      <td></td>
      <td>Sat (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Project 1: Simple Class Utility</td>
      <td>Build a class that manages a resource (e.g., a simple custom logger).</td>
      <td>Hands-on Coding</td>
    </tr>
    <tr>
      <td></td>
      <td>Sun (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Tool Mastery: CMake</td>
      <td>Complete a basic tutorial: create a CMakeLists.txt for a multi-file project and build it.</td>
      <td>Official CMake Tutorial</td>
    </tr>
    <tr>
      <td><strong>Week 4</strong> (Nov 17–23)</td>
      <td>Mon (3h): 2–5 PM</td>
      <td>std::unique_ptr (Ownership)</td>
      <td><div class="critical"><strong>CRITICAL</strong>: Understand how it guarantees single ownership.</div></td>
      <td>LearnCpp.com (Ch 18.5); cppreference.com</td>
    </tr>
    <tr>
      <td></td>
      <td>Tue (3h): 2–5 PM</td>
      <td>std::vector Deep Dive</td>
      <td>Size vs Capacity, Reserve, Iterators, and Performance Implications.</td>
      <td>cppreference.com</td>
    </tr>
    <tr>
      <td></td>
      <td>Wed (3h): 2–5 PM</td>
      <td>std::map vs std::unordered_map</td>
      <td>Understand hash-table vs tree implementation, and complexity (O(1) vs O(logn)).</td>
      <td>cppreference.com</td>
    </tr>
    <tr>
      <td></td>
      <td>Thu (3h): 2–5 PM</td>
      <td>Move Semantics 1: R-value References</td>
      <td>The && syntax and the concept of "stealing" data.</td>
      <td>LearnCpp.com (Ch 23.3)</td>
    </tr>
    <tr>
      <td></td>
      <td>Fri (3h): 2–5 PM</td>
      <td>Move Semantics 2: Move Constructor/Assignment</td>
      <td>Implement the move special members to avoid expensive deep copies.</td>
      <td>LearnCpp.com (Ch 23.4–23.6)</td>
    </tr>
    <tr>
      <td></td>
      <td>Sat (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Project 2: Refactoring for Ownership</td>
      <td>Take Project 1 (or any class with raw pointers) and refactor it entirely to use std::unique_ptr and move semantics.</td>
      <td>Hands-on Coding</td>
    </tr>
    <tr>
      <td></td>
      <td>Sun (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Advanced Bitwise Operations</td>
      <td>Bit flags, masking, and simple data packing/unpacking.</td>
      <td>LearnCpp.com (Ch O)</td>
    </tr>
    <tr>
      <td><strong>Week 5</strong> (Nov 24–30)</td>
      <td>Mon (3h): 2–5 PM</td>
      <td>Inheritance & Polymorphism</td>
      <td>Base/Derived classes, Public/Private inheritance.</td>
      <td>LearnCpp.com (Ch 21)</td>
    </tr>
    <tr>
      <td></td>
      <td>Tue (3h): 2–5 PM</td>
      <td>Virtual Functions & Abstract Classes</td>
      <td><div class="critical"><strong>CRITICAL</strong>: The mechanism for runtime type dispatch (used heavily in LLVM).</div></td>
      <td>LearnCpp.com (Ch 22)</td>
    </tr>
    <tr>
      <td></td>
      <td>Wed (3h): 2–5 PM</td>
      <td>The Visitor Pattern (Theory)</td>
      <td>Understand how it enables operation separation (Crucial for AST traversal).</td>
      <td>Refactoring Guru: Visitor</td>
    </tr>
    <tr>
      <td></td>
      <td>Thu (3h): 2–5 PM</td>
      <td>The Visitor Pattern (Implementation)</td>
      <td>Implement the Visitor pattern on a simple custom class hierarchy.</td>
      <td>Hands-on Coding</td>
    </tr>
    <tr>
      <td></td>
      <td>Fri (3h): 2–5 PM</td>
      <td>Exception Handling (Basics)</td>
      <td>try/catch, std::exception hierarchy. Focus on RAII safety.</td>
      <td>LearnCpp.com (Ch 24)</td>
    </tr>
    <tr>
      <td></td>
      <td>Sat (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Project 3: Expression Tree</td>
      <td>Build a simple class hierarchy (Literal, BinaryOp, UnaryOp) and implement the Visitor to print the expression.</td>
      <td>Hands-on Coding</td>
    </tr>
    <tr>
      <td></td>
      <td>Sun (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>static_cast vs dynamic_cast</td>
      <td>When and why to use each, and the runtime cost of dynamic_cast.</td>
      <td>LearnCpp.com (Ch 12.11)</td>
    </tr>
    <tr>
      <td><strong>Week 8</strong> (Dec 15–21)</td>
      <td>Mon (3h): 2–5 PM</td>
      <td>Function Templates</td>
      <td>Writing generic functions (e.g., a generic max() function).</td>
      <td>LearnCpp.com (Ch 25.1)</td>
    </tr>
    <tr>
      <td></td>
      <td>Tue (3h): 2–5 PM</td>
      <td>Class Templates & Specialization</td>
      <td>Creating generic data structures (e.g., a simple Maybe<T>).</td>
      <td>LearnCpp.com (Ch 25.2–25.4)</td>
    </tr>
    <tr>
      <td></td>
      <td>Wed (3h): 2–5 PM</td>
      <td>const vs constexpr</td>
      <td>Understanding compile-time constants and functions for optimisation.</td>
      <td>cppreference.com</td>
    </tr>
    <tr>
      <td></td>
      <td>Thu (3h): 2–5 PM</td>
      <td>Tool: clang-tidy / clang-format</td>
      <td>Set up coding standard enforcement for professional C++ development.</td>
      <td>Clang Documentation</td>
    </tr>
    <tr>
      <td></td>
      <td>Fri (3h): 2–5 PM</td>
      <td>Concurrency Basics</td>
      <td>std::thread, std::mutex, std::lock_guard (Focus on safe parallel operations).</td>
      <td>C++ Concurrency in Action (Ch 2)</td>
    </tr>
    <tr>
      <td></td>
      <td>Sat (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Project Refactor: Templates</td>
      <td>Refactor Project 3 (Expression Tree) to be template-based where possible.</td>
      <td>Hands-on Coding</td>
    </tr>
    <tr>
      <td></td>
      <td>Sun (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Review & Catch-up</td>
      <td>Solidify weaker topics from the first 8 weeks.</td>
      <td>All Resources</td>
    </tr>
    <tr>
      <td><strong>Week 9</strong> (Dec 22–28)</td>
      <td>Mon (3h): 2–5 PM</td>
      <td>Compiler Theory: Lexing & Tokens</td>
      <td>Read theory on tokenization. Define your AI language tokens (e.g., tok_matrix, tok_relu).</td>
      <td>Crafting Interpreters (Ch 2–4)</td>
    </tr>
    <tr>
      <td></td>
      <td>Tue (3h): 2–5 PM</td>
      <td>LLVM Kaleidoscope Ch 1: The Lexer</td>
      <td>Implement the Lexer for the toy language. <strong>CODE</strong>.</td>
      <td>LLVM Kaleidoscope Tutorial</td>
    </tr>
    <tr>
      <td></td>
      <td>Wed (3h): 2–5 PM</td>
      <td>Compiler Theory: Parsing & AST</td>
      <td>Read theory on Recursive Descent Parsing and Operator Precedence.</td>
      <td>Crafting Interpreters (Ch 5–7)</td>
    </tr>
    <tr>
      <td></td>
      <td>Thu (3h): 2–5 PM</td>
      <td>LLVM Kaleidoscope Ch 2: The Parser & AST</td>
      <td>Implement the Parser and the Expression AST nodes. <strong>CODE</strong>.</td>
      <td>LLVM Kaleidoscope Tutorial</td>
    </tr>
    <tr>
      <td></td>
      <td>Fri (3h): 2–5 PM</td>
      <td>LLVM Style RTTI: isa<>, cast<>, dyn_cast<></td>
      <td><div class="critical"><strong>CRITICAL</strong>: Understand this custom type casting used throughout LLVM.</div></td>
      <td>LLVM Documentation: Style RTTI</td>
    </tr>
    <tr>
      <td></td>
      <td>Sat (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Project 4: Complete Lexer/Parser</td>
      <td>Extend the Kaleidoscope code to handle a custom keyword relevant to AI (e.g., tensor or dot).</td>
      <td>Hands-on Coding</td>
    </tr>
    <tr>
      <td></td>
      <td>Sun (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>LLVM IR Generation Theory</td>
      <td>Read about Static Single Assignment (SSA) and the structure of LLVM IR.</td>
      <td>LLVM Tutorial (Ch 3 Overview)</td>
    </tr>
    <tr>
      <td><strong>Week 12</strong> (Jan 12–18)</td>
      <td>Mon (3h): 2–5 PM</td>
      <td>LLVM Kaleidoscope Ch 3: Code Generation</td>
      <td>Implement LLVM IR code generation for basic arithmetic. <strong>CODE</strong>.</td>
      <td>LLVM Kaleidoscope Tutorial</td>
    </tr>
    <tr>
      <td></td>
      <td>Tue (3h): 2–5 PM</td>
      <td>LLVM Kaleidoscope Ch 4: JIT & Optimiser</td>
      <td>Integrate the Just-In-Time (JIT) compiler and a basic optimization pass. <strong>CODE</strong>.</td>
      <td>LLVM Kaleidoscope Tutorial</td>
    </tr>
    <tr>
      <td></td>
      <td>Wed (3h): 2–5 PM</td>
      <td>MLIR Core Concepts</td>
      <td>Read: Context, Dialects, Operations, Attributes, Types.</td>
      <td>MLIR Documentation (Getting Started)</td>
    </tr>
    <tr>
      <td></td>
      <td>Thu (3h): 2–5 PM</td>
      <td>MLIR: Defining a Custom Dialect</td>
      <td>Start defining your first MLIR Dialect for AI Operations (e.g., a simple linalg or tensor op).</td>
      <td>MLIR Custom Dialects Guide</td>
    </tr>
    <tr>
      <td></td>
      <td>Fri (3h): 2–5 PM</td>
      <td>Tool: Address Sanitizer / Valgrind</td>
      <td>Learn to detect memory errors (use on a deliberately faulty code snippet).</td>
      <td>Valgrind/ASan Official Docs</td>
    </tr>
    <tr>
      <td></td>
      <td>Sat (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>Final Project Prototype</td>
      <td>Define a simple MLIR Operation and write a C++ function that creates and returns it.</td>
      <td>Hands-on Coding</td>
    </tr>
    <tr>
      <td></td>
      <td>Sun (5.5h): 1–5 PM, 8:30–10 PM</td>
      <td>System Review & Planning</td>
      <td>Review the full 12 weeks. Plan your next 3 months on extending the MLIR Dialect and implementing compiler passes.</td>
      <td>Self-Directed</td>
    </tr>
  </tbody>
</table>

## 🎯 Key Learning Milestones

<div class="course-phase">
  <h3>Phase 1: C++ Fundamentals (Weeks 1-4)</h3>
  <p>Master the basics of modern C++, memory management, and development tools.</p>
</div>

<div class="course-phase">
  <h3>Phase 2: Advanced C++ & Design Patterns (Weeks 5-8)</h3>
  <p>Learn advanced concepts like polymorphism, templates, and concurrent programming.</p>
</div>

<div class="course-phase">
  <h3>Phase 3: Compiler Foundations (Weeks 9-12)</h3>
  <p>Build your first compiler with LLVM and explore MLIR for advanced compiler development.</p>
</div>

---

<a href="index.html" class="btn">Back to Home</a>
<a href="navigation.html" class="btn btn-secondary">Course Navigation</a>