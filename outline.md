# Compilation Framework for Gradually Typed Languages

## Introduction

Programming languages are usually statically typed or dynamically typed, each of these typing paradigms having its advantages and disadvantages. Gradual typing aims to allow static typing and dynamic typing to coexist in the same programming language. Getting the advantage of the guarantees provided by static typing and the flexibility of dynamic typing. Also, allowing a program with no type annotations to evolve into a statically typed version by adding type annotations.

Many gradual type disciplines have been developed, such as subtyping, inference, information flow security, references, etc. However, most of these developments have been ad-hoc to the specific typing discipline.

Abstracting Gradual Typing (AGT) introduces a systematic approach for designing gradual typing disciplines from a static typing discipline. Given a source language and a designer-selected interpretation for gradual types, AGT yields static and dynamic semantics grounded in the type discipline of the source language.

One of the challenges of gradual typing disciplines is that language implementations require runtime type checking in addition to static type checking. This imposes a runtime performance penalty that can dissuade users from enabling runtime checks.

Compilers for gradually typed languages have been developed to mitigate these performance issues, but they have been designed ad-hoc to the specific language.

A flexible approach for building compilers for gradual typing disciplines derived from AGT could be developed. This would be more flexible than existing compilers, while potentially being more performant than the existing interpreters for these typing disciplines.

## State of the Art

* Gradual Typing

* Abstracting Gradual Typing (AGT)

* Micro-Policies Formally Verified, Tag-Based Security Monitors

* Efficient Gradual Typing

## Problem

* Gradual typing has advantages

* Several gradual typing disciplines exist in the literature

* AGT introduces a systematic approach for designing gradual typing disciplines based on a static typing discipline

* The dynamic semantics resulting from AGT are based on evidence

* The execution of gradually typed languages presents a performance challenge

* A compiler that allows for the efficient execution of languages derived from AGT would be useful

* Current approaches for compiling gradually typed languages are designed in an ad-hoc way for a specific typing discipline, thus a compiler for languages derived from AGT would be more flexible

* In order to design a compiler of efficient programs, tags could be used to represent evidence, similarly to Tag-based Policy Enforcement

## Hypothesis

* There exists a compact memory representation for the evidence used in gradual typing disciplines derived from AGT

* The general approach used in Tag Based Machines could be applied to the evidence-based semantics of gradual typing disciplines derived from AGT

* A flexible approach for building compilers for gradual typing disciplines derived from AGT can be developed

* This approach could offer better performance than existing interpreters for gradual typing disciplines, while being more flexible than existing compilers

## Objectives

Develop a flexible approach for building compilers for gradual typing disciplines derived from AGT

* Develop a compact memory representation for the evidence used in typing disciplines derived from AGT

* Develop an approach for compiling evidence-based semantics to machine code inspired by Tag Based Machines

* Compare the resulting compiler to existing interpreters and compilers for similar typing disciplines

## Methodology

1. Study the state of the art in gradual typing disciplines, the compilation of gradually typed programming languages, and applicable compilation techniques

2. Implement a simple compiler for a gradual typing discipline derived from AGT using an approach similar to Tag Based Machines 

3. Develop a compact memory representation for the evidence used in multiple gradual typing disciplines derived from AGT

4. Implement a compiler that can be used for multiple gradual typing disciplines derived from AGT, by parametrizing the parts that are different for each typing disciplines

5. Study the performance overhead of runtime checks

6. Compare to existing compilers

## Expected Contributions

* An approach for building compilers for typing disciplines derived from AGT

* Compilers for some typing disciplines derived from AGT

* A memory representation for the evidence used in typing disciplines derived from AGT

* A better understanding of how this approach compares to existing compilers and interpreters for gradual typing
