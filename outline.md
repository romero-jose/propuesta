# Compilation Framework for Gradually Typed Languages

## Introduction

Programming languages are usually statically typed or dynamically typed, each of these typing paradigms having their advantages and disadvantages. Gradually typed languages aim to allow static typing and dynamic typing to coexist in the same programming languages, thus getting the advantages of both typing disciplines. Furthermore, different aspects of a type system can be gradualized, such as security types, structural types, etc.

One of the challenges of gradual typing disciplines is that implementations of these languages require runtime type checking to enforce the type guarantees that can't be statically checked. This imposes a performance penalty that can dissuade users from enabling the runtime checks.

Compilers for gradually typed languages have been developed to mitigate these performance issues, but they have been designed ad-hoc to the specific language.

AGT introduces a systematic approach for designing gradually typed languages. Given a source language and a designer-selected interpretation for gradual types, AGT yields static and dynamic semantics grounded in the type discipline of the source language.

Using AGT a compilation framework for gradually typed languages could be developed that is not designed ad-hoc to the specific language, but can be applied to several gradually-typed languages.

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

