---
title: The Dotfile as Autobiography
description:
  Week 4, configuration as prose, version control as memory, and the
  reproducibility problem at the centre of the craft
week: 4
date: 2027-03-15
teachers:
  - shelly-powell
slides: /decks/week-04/
related:
  - sessions/04-dotfiles
  - assessments/dotfiles-repository
---

A dotfile is a record of every decision you made and then forgot you had made.
Read someone's config carefully and you can reconstruct their habits, their
irritations, the tutorial they followed at 2am, and the exact keybinding that
once cost them an afternoon. Configuration is prose. It has an author, a voice,
and passages that were clearly written by a different, more optimistic person.

This lecture turns that observation into a working practice. If a dotfile is
autobiography, version control is memory, and a setup with no git history is a
life with no diary: you cannot say when a choice was made or why, only that it
now exists. From here we name the problem the rest of the course circles, the
one the Dotfiles Repository is marked on. A setup that lives only on your machine
is not reproducible, and a rice that cannot be rebuilt is a photograph of a
place that no longer exists.

## In this lecture

- config as authored text: reading a stranger's setup like a letter
- version control as the memory a setup otherwise lacks
- the reproducibility problem, stated plainly
- what separates a dotfiles repository from a folder of backups

## Before next week

Put your config under git if it is not already. Write the first commit message
as though a stranger will read it, because one will.
