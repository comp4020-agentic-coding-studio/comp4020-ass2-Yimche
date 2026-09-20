---
title: The Dream of the Perfect Setup
description:
  Week 10, dotfile managers, Nix, and the fantasy of a machine you will never
  have to configure again
week: 10
date: 2027-04-26
teachers:
  - idris-fenn
related:
  - sessions/10-reproducibility
  - assessments/dotfiles-repository
---

Every ricer nurses the same dream: the setup so perfectly captured that a new
machine becomes the old one in a single command, and configuration is over
forever. This lecture is about the tools built to chase that dream and about why
the dream keeps receding. Dotfile managers, bare git repositories, symlink
farms, and at the far end Nix and home-manager, which promise not just your files
but the entire environment, declared once and rebuilt identically anywhere.

We take these seriously as engineering, because the Dotfiles Repository is marked
as engineering. Reproducibility is a spectrum, from a folder you copy and pray
over, to a bootstrap script, to a fully declarative system that treats your
desktop as a build artefact. Each step up the spectrum buys real guarantees and
charges real complexity, and Nix in particular asks you to learn a language and a
worldview to escape the chore of setup. The dream is worth wanting. It is also
worth asking what you would do with all the time it promised to save.

## In this lecture

- the reproducibility spectrum, from copied folders to declarative systems
- dotfile managers and bare git repositories: the pragmatic middle
- Nix and home-manager: the desktop as a build artefact
- the cost of the guarantee, and the receding horizon of "done"

## Before next week

Make your setup bootstrap on a fresh machine, real or virtual. Time how long it
takes and write down everything you had to fix by hand.
