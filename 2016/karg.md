---
layout: talk
active: bob2016
title: "Functional Programming and the Web: Frontend Development in PureScript"
speaker: Michael Karg, Jürgen Nicklisch-Franken
portrait: michael-karg.jpg
portrait2: juergen-nicklisch-franken.jpg
time: 14:15-15:00
type: Vortrag
slides-file: karg.pdf
youtube: EArV7Uy-TD0
language: english
head: 2016
---

PureScript is a strongly-typed functional programming language that
compiles to JavaScript. Its roots lie in the Haskell world, and the
(open source) PureScript compiler itself is implemented in Haskell.

It aims to be a general-purpose language for the Web; the code
produced by the compiler is standalone, and as such does not require
any additional runtime system library, and can be seamlessly
integrated with existing JavaScript libraries or frameworks.

While PureScript's syntax may be very close to Haskell's, there are
interesting conceptual differences between the two languages, such as
PureScript's strict evaluation, or the use of extensible effects in
PureScrips's type system.

At Symbolian GmbH, we use PureScript as a main tool in the development
of a WebGL-based 3D visualization library for big (and small)
data. Whilst this being a commercial closed-source product, we have
contributed to the PureScript ecosystem over the course of its
development: PureScript's bindings to WebGL as well as various utility
packages for matrix and vector datatypes have been released by
Symbolian.

In our talk, we want to give a short overview over PureScript and the
state of its ecosystem. Then, we want to share our experiences with
using this relatively young language for a production-grade software
with respect to some real-world challenges like e.g. performance
profiling, compiler optimization of the generated JavaScript code, or
interface stability.

### Michael Karg

During the studies for his master's degree in computer science and
general linguistics at Göttingen University (Germany), Michael came in
contact with lambda calculus and the Haskell programming
language. He kept on using it professionally and privately ever
since graduation.

His fascination with functional programming (and type systems) lies not
only in how directly the theoretical, academic discourse about it can
be applied to every-day code, but also in how reliably it improves
software quality in several regards. For a year now he has been working
on building production-grade software for the web in a cutting-edge
functional language at Symbolian GmbH.

### Jürgen Nicklisch-Franken

In the first period of his 30+ years of software development in industry
(mainly finance and transportation) he had to follow the object-oriented
paradigm professionally, but advocated functional programming with Lisp and
Scheme. He used OCaml as main backbone language in the first company he
founded 1998 (Persist AG) and switched to Haskell as preferred language
sometimes later. He started the development of Leksah (a Haskell IDE
written in Haskell) and worked his last year on generating and testing
safety critical real time software in Haskell.

He co-founded Symbolian a year ago, with the ultimate aim to marry the Web
with derivation and computation based on advanced type systems to make it
safe, reliable and powerful.
