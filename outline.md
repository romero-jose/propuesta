# Compilation Framework for Gradually Typed Languages

## Introduction

Programming languages are usually statically typed or dynamically typed, each of these typing paradigms having its advantages and disadvantages. Gradual typing aims to allow static typing and dynamic typing to coexist in the same programming language. Getting the advantage of the guarantees provided by static typing and the flexibility of dynamic typing. Also, allowing a dynamically typed program to evolve into a statically typed version by adding type annotations.

Many gradual type disciplines have been developed, such as subtyping, inference, information flow security, references, etc. However, most of these developments have been ad-hoc to the specific typing discipline.

Abstracting Gradual Typing (AGT) introduces a systematic approach for designing gradual typing disciplines from a static typing discipline. Given a source language and a designer-selected interpretation for gradual types, AGT yields static and dynamic semantics for the gradual language grounded in the type discipline of the static language.

One of the challenges of gradual typing disciplines is that language implementations require runtime type checking in addition to static type checking. This imposes a runtime performance penalty that can dissuade users from enabling runtime checks.

Compilers for gradually typed languages have been developed to mitigate these performance issues, but there are few implementations. One of these is Grift, a compiler developed by Kuhlenschmidt et al. (2019), that attempts to obtain good performance by using a close-to-the-metal implementation of casts. Other implementations such as Typed Racket are based on existing mechanisms that are not specific to gradual typing (e.g. contracts). Additionally, these implementations focus on standard typing and do not support other gradual typing disciplines.

The space of compilation techniques for gradual typing in general is underexplored. We believe we can build upon the general AGT approach to devise a general compilation framework for gradual typing disciplines. This would be more flexible than existing compilers, while potentially being more performant than the existing interpreters for these typing disciplines.

## State of the Art

* Gradual Typing

* Abstracting Gradual Typing (AGT)

* Micro-Policies Formally Verified, Tag-Based Security Monitors

* Efficient Gradual Typing

* Toward Efficient Gradual Typing
for Structural Types via Coercions (grift)

* Abstracting Gradual References

* Gradual System F

* A Gradual Interpretation of Union Types

## Problem

* Gradual typing has advantages

* Several gradual typing disciplines exist in the literature

* AGT introduces a systematic approach for designing gradual typing disciplines based on a static typing discipline

* The dynamic semantics resulting from AGT are based on evidence

* The execution of gradually typed languages presents a performance challenge

* There are compilers that try to mitigate these performance issues, but they are few and the focus on standard typing and do not support other gradual typing disciplines

## Hypothesis

* We can build upon the AGT approach to devise a general compilation framework for gradual typing disciplines

* This approach could offer better performance than existing interpreters for gradual typing disciplines, while being more flexible than existing compilers

* The general approach used in Micro-Policies could be applied to the evidence-based semantics of gradual typing disciplines derived from AGT

* Compact memory representations can be found for the evidence used in multiple gradual typing disciplines derived from AGT

* Using a compact memory representation of evidence and the general approach from Micro-Policies this approach would yield compilers with reasonable performance

## Objectives

Develop a flexible approach for building compilers for gradual typing disciplines derived from AGT

* Develop compact memory representations for the evidence used in multiple typing disciplines derived from AGT

* Develop an approach for compiling evidence-based semantics to machine code inspired by Micro Policies

* Compare the resulting compiler to existing interpreters and compilers for similar typing disciplines

## Methodology

1. Study the state of the art in gradual typing disciplines, the compilation of gradually typed programming languages, and applicable compilation techniques

2. Implement a simple compiler for a gradual typing discipline derived from AGT using an approach similar to Micro Policies 

3. Develop a compact memory representation for the evidence used in multiple gradual typing disciplines derived from AGT

4. Implement a compiler that can be used for multiple gradual typing disciplines derived from AGT, by parametrizing the parts that are different for each typing discipline

5. Study the performance overhead of runtime checks

6. Compare to existing implementations, specifically, Grift and the existing AGT abstract machines developed in Scala.

## Expected Contributions

* An approach for building compilers for typing disciplines derived from AGT

* A compact memory representation for the evidence used in gradual typing disciplines derived from AGT

* A better understanding of how this approach compares to existing compilers and interpreters for gradual typing
