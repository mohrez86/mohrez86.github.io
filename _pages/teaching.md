---
layout: page
permalink: /teaching/
title: teaching
# description: Materials for courses you taught. Replace this text with your description.
nav: true
nav_order: 30
---

# Teaching

My teaching experience, both as a teaching assistant and as a lecturer:

<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->

- [University of Passau, Passau, Germany](#university-of-passau-passau-germany)
   * [Co-Lecturer, Compiler Construction Lab](#compiler-construction-lab)
- [USI, Lugano, Switzerland](#usi-lugano-switzerland)
   * [TA, Programming Fundamentals 1 (five times)](#programming-fundamentals-1)
   * [TA, Software Atelier 4: Software Engineering Project (twice)](#software-atelier-4-software-engineering-project)
   * [TA, Compiler Construction](#compiler-construction)

<!-- TOC end -->

---

## University of Passau, Passau, Germany

I was one of the lecturers for the following course at the [University of Passau](https://www.uni-passau.de), along with Professor Christian Hammer.

### Compiler Construction Lab  
- [Winter 2024/2025](https://www.fim.uni-passau.de/software-engineering-i/lehrstuhlteam/personendetails?config_id=232ee5ad516ac92bf590f99ac8c2baa8&module=TemplateLecturedetails&range_id=d33789fe6848842635609cb3c3a3ff66&seminar_id=55f222b1ddb736dbee2ec627faf45279&cHash=f4c6375dd28bbc0be140eccbb4abe7f4)

In our Compiler Construction Lab, students implement a compiler in Java for the ChocoPy programming language.
ChocoPy is a simplified, statically typed dialect of Python, specifically designed for compiler construction courses. It supports many interesting features from Python, such as classes, inheritance, nested functions, and lists.
For more information about this programming language, visit [ChocoPy.org](https://ChocoPy.org).

The course primarily consists of three extensive programming assignments that build upon each other to implement a full-fledged compiler:

- **Programming Assignment 1 (PA1):** Lexing and Parsing  
- **Programming Assignment 2 (PA2):** Semantic Analysis and Type Checking  
- **Programming Assignment 3 (PA3):** Assembly Code Generation  

In PA1, students build the front end of their compiler, consisting of a lexer and a parser. The goal of PA1 is to take a ChocoPy program as input and construct an Abstract Syntax Tree (AST). This front end is also expected to report errors, including their locations and explanations, in case the input ChocoPy program contains syntactic errors.

In PA2, students develop a semantic analyzer and type checker for their compiler. The goal of PA2 is to take the AST generated by the front end (implemented in PA1) and return the same AST with additional type information.
Similar to PA1, the semantic analyzer is also expected to support error reporting (semantic errors).

Finally, in PA3, students implement the last phase of their compiler, which takes a typed AST generated by the semantic analyzer (implemented in PA2) and produces the corresponding RISC-V assembly code.

For each of the three programming assignments, students are provided with an extensive set of sample ChocoPy programs, each testing a specific feature of the language to ensure their compilers behave as expected.

---

## USI, Lugano, Switzerland

During my PhD studies at [USI Università della Svizzera italiana](https://www.usi.ch), I was a teaching assistant for three different courses over eight semesters.

### Programming Fundamentals 1
- [Fall 2023/2024](https://search.usi.ch/en/courses/35268178/programming-fundamentals-1)
- [Fall 2022/2023](https://search.usi.ch/en/courses/35265698/programming-fundamentals-1)
- [Fall 2021/2022](https://search.usi.ch/en/courses/35263600/programming-fundamentals-1)
- [Fall 2020/2021](https://search.usi.ch/en/courses/35262255/programming-fundamentals-1)
- [Fall 2019/2020](https://search.usi.ch/en/courses/35260902/programming-fundamentals-1)

Programming Fundamentals 1 (PF1) is a course designed for first-year bachelor's students.
The programming language of the course is Racket.
However, learning Racket is not the main focus.
The primary goal of this course is to teach students how to write programs well, regardless of the programming language.
This course teaches students how to start from a problem and end with an implementation, step by step, in a principled manner.

For more information about Racket and this course, visit [racket-lang.org](https://racket-lang.org/).
You can also see some of PF1's final projects implemented by our students in [this video](https://www.youtube.com/watch?v=DhnO80Oj5_8).

### Software Atelier 4: Software Engineering Project
- [Spring 2021/2022](https://search.usi.ch/en/courses/35263656/software-atelier-4-software-engineering-project)
- [Spring 2020/2021](https://search.usi.ch/en/courses/35262270/software-atelier-4-software-engineering-project)

Software Atelier 4 (SA4) prepares students not only to be good programmers but also to be effective team players.
SA4 teaches students how to work in large teams and develop large, complex software systems.
The course consists of several theoretical and hands-on lectures, as well as a project.

During the project, students form teams of 10 people, acting as *software development teams*; instructors play the role of *customers*; and teaching assistants act as *project managers*.
SA4's project involves continuous interactions between these different roles throughout the course.

### Compiler Construction
- [Spring 2019/2020](https://search.usi.ch/en/courses/35260839/compiler-construction)

Compiler Construction covers a wide variety of topics in the areas of programming languages, compilers, and interpreters. This course teaches students about the different tasks performed by compilers and exposes them to the tools and techniques required to construct them.
