---
title: Rebuild from bare metal
description:
  Week 10 studio, prove the setup is reproducible by building it again on a
  clean machine
week: 10
date: 2027-04-26
teachers:
  - idris-fenn
spec:
  - your setup bootstraps onto a fresh machine from your repository
  - you have timed the rebuild and logged every manual fix it needed
  - you can say where on the reproducibility spectrum your setup sits
---

The studio that tests the dream against a clean disk.

## Before the studio

Bring a bootstrap path for your setup, however rough, and a fresh virtual machine
to run it against.

## In the studio

Everyone rebuilds from bare metal at once. The clock runs, and every hand-fix you
have to make is a hole in your repository you did not know was there. We compare
where each setup sits on the spectrum, from copied folders to a declarative Nix
build, and what the next step up would cost.

## Afterwards

You leave with a setup that regenerates itself, or a precise list of why it does
not yet, which is nearly as valuable.
