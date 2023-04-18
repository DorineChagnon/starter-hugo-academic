---
summary: Announcement of the poster about Path Validation for RESSI 2023 conference.
slides:
  theme: white
  highlight_style: dracula
authors: []
title: "RESSI 2023 : Network Path Validation for Packets Delivery"
date: 2023-04-18T07:20:48.457Z
tags:
  - network security
  - path validation
  - cryptography
image:
  filename: addition.png
categories: []
---
# Network Path Validation for Packets Deliver

### Dorine CHAGNON

Université Clermont Auvergne, CNRS, Mines Saint-Etienne, LIMOS, France\
dorine.chagnon@doctorant.uca.fr\
May 10-12, RESSI 2023

- - -

## Context for Path Validation

* Skipping attack

![Skipping attack: A malicious router redirects the packet and skips at least one router on the path. Hence, some router along the intended path does not forward the packet.](skipping.png "Skipping Attack")

* Out-of-order attack

![Out-of-order attack : One or many routers on the intended path are not traversed in the right order, but they are all visited.](outoforder.png "Out-Of-Order Attack")

* ﻿Addition attack

![Addition attack : Packets are forwarded to some additional routers that are not on the intended path and eventually return to the expected path. Packets visit one or more routers that are not expected.](addition.png "Addition Attack")

* ﻿Detour attack

![Detour attack : Packets are deviated from some of the routers before arriving to the destination. Not all routers are visited.](detour.png "Detour Attack")

- - -

## Steps of Path Validation

![Path validation consists of the following steps: Path dissemination, Key exchange, Proof initialization, Prood verification, Proof update](validationsteps.png "Steps of Path Validation")

- - -

## State-of-the-art

* ICING (2011)
* OPT (2014)
* OSV (2016)
* PPV (2018)
* Atomos (2019)
* PrivNPV (2020)
* EPIC (2020)

### Go see my poster to know more about\
Path Validation.

Dorine CHAGNON\
dorine.chagnon@doctorant.uca.fr\
May 10–12, RESSI 202