---
title: The Stack Beneath the Skin
description:
  Week 2, X11 versus Wayland, the role of the compositor, and what you are
  actually theming when you theme a desktop
week: 2
date: 2027-03-01
teachers:
  - idris-fenn
slides: /decks/week-02/
related:
  - sessions/02-the-stack
---

Before you can theme a desktop you have to know what a desktop is made of. Most
of what a beginner calls "the desktop" is in fact several programs that have
agreed to cooperate: a display server, a compositor, a window manager, a bar, a
launcher, a terminal, and the applications on top. Change one and the others may
stop cooperating. This lecture takes the stack apart so that later, when a
tutorial says "just add this line", you know which program you are talking to.

The central split is X11 against Wayland. X11 is old, permissive, and endlessly
scriptable, which is why so much ricing tooling assumes it. Wayland is newer,
stricter, and folds the compositor and display server together, which changes
what is even possible to theme. Neither is a moral choice, whatever the forums
tell you. They are different contracts, and the rest of your setup lives inside
whichever one you sign.

## In this lecture

- display server, compositor, and window manager: who does what
- X11 and Wayland as two different contracts, not two teams
- what "theming" actually reaches: which layer owns your borders, gaps, shadows
- why a screenshot cannot tell you which stack produced it

## Before next week

Identify the stack on the machine you brought last week. Name every layer, and
find the one program you will spend the most time fighting.
