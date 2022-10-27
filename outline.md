# Compilation Framework for Gradually Typed Languages

## Introduction

Programming languages are usually statically typed or dynamically typed, each of these typing paradigms having its advantages and disadvantages. Gradual typing aims to allow static typing and dynamic typing to coexist in the same programming language. Getting the advantage of the guarantees provided by static typing and the flexibility of dynamic typing. Also, allowing a program with no type annotations to evolve into a statically typed version by adding type annotations.

Many gradual type disciplines have been developed, such as subtyping, inference, information flow security, references, etc. However, most of these developments have been ad-hoc to the specific typing discipline.

Abstracting Gradual Typing (AGT) introduces a systematic approach for designing gradual typing disciplines from a static typing discipline. Given a source language and a designer-selected interpretation for gradual types, AGT yields static and dynamic semantics grounded in the type discipline of the source language.

One of the challenges of gradual typing disciplines is that language implementations require runtime type checking in addition to static type checking. This imposes a runtime performance penalty that can dissuade users from enabling runtime checks.

Compilers for gradually typed languages have been developed to mitigate these performance issues, but they have been designed ad-hoc to the specific language.

Using AGT a compilation framework for gradually typed languages could be developed that is not designed ad-hoc to the specific language, but can be applied to several gradual typing disciplines. This would be more flexible than the existing approaches that rely on the specific typing discipline. Additionally, this approach could be applied to all the gradual typing disciplines developed using AGT.

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

* A compiler that allows for efficient execution of languages derived from AGT would be useful

* Current approaches for compiling gradually typed languages are designed in an ad-hoc way to a specific typing discipline, thus a compiler for languages derived from AGT would be more flexible

* In order to design a compiler of efficient programs, tags could be used to represent evidence, similarly to Tag-based Policy Enforcement

## Hypothesis

* A systematic approach for building compilers for programming languages designed with AGT can be developed that allows for efficient execution of evidence-based dynamic semantics

## Objectives

* Develop a systematic approach for building compilers for programming languages designed with AGT that allows for efficient execution of evidence-based dynamic semantics

  * Develop a systematic approach for building compilers for programming languages designed with AGT

  * Develop an approach for compiling evidence-based semantics to efficient machine code

  * Evaluate the performance of the programs compiled with this compiler and compare it with the performance of programs compiled with existing compilers for gradual typing disciplines

## Methodology

## Expected Results

## Contributions

