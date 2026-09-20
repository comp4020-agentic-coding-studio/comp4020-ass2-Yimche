---
title: The Dotfiles Repository
description:
  The setup as engineering, a repository graded on whether a stranger can
  rebuild your desktop, not on how it looks
week: 12
due: 2027-05-28T12:00:00+10:00
weight: 20
marking:
  mode: weighted
  criteria:
    - name: Reproducibility
      weight: 40
    - name: Structure and legibility
      weight: 25
    - name: Documentation
      weight: 20
    - name: History and hygiene
      weight: 15
spec:
  - submitted as a public git repository with a README that explains how to use it
  - it bootstraps a bare machine to your desktop with the fewest manual steps
  - forked, borrowed, and AI-assisted parts are credited in a form a marker can follow
related:
  - the-rice
---

Here the desktop is judged as software. Beauty earns nothing on this page; the
beauty is marked under The Rice. What is marked here is whether the thing can be
rebuilt.

## The brief

> Deliver the repository that turns a bare machine into your desktop, and make it
> good enough that a stranger could.

The reason this is separate from The Rice is that the two virtues genuinely
diverge. A stunning desktop that exists only as undocumented, hand-mutated config
on one laptop fails here exactly as it should. A plain setup that clones cleanly
and rebuilds itself without fuss scores well. Reproducibility is the actual
discipline of the craft, and this component exists to reward it on its own.

## What you submit

A public git repository. It should bootstrap a fresh machine with as little
manual intervention as you can manage, read clearly enough that a marker can find
where any setting lives, carry a history that shows how the setup was built rather
than a single dumped commit, and credit every source it grew from.

The criteria below are weighted. Reproducibility carries the most because it is
the point.
