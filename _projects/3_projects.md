---
layout: page
title: FSI Interface Tracking
description: An interface tracking algorithm for FSI time-step initialization
img: assets/img/fsi_interface.png
importance: 3
category: work
---

***This page is currently a `WORK IN PROGRESS`. Here I will be posting my results for a novel interface tracking stratgey aimed at drastically enhancing the convergence rate of moderately challenging FSI simulations. This scheme (for the time-being) is restricted to applications in which the interface of the multiphysical problem will adopt a state (maybe many states) of oscillatory motion (distributed or otherwise). Though ideas involving more general reduce order model (ROM) supported schemes are also being simultaneously pursued. Regardless, this "trick" may prove itself incredibly useful as a reasonably simple means to significantly reduce the costs of high-fidelity mixing simulations (for example) where the deformable structure will adopt SOME type of steady or slowly evolving periodic coupled motion which cannot be defined exactly a priori. In these types of problems; where we are more interested in the unknown physical/chemical processes (mixing efficiency, heat transfer, reaction physics) of a big/bigger/massive fluid domain that is continually perturbed by an embedded or surrounding dynamic elastic structure(s); by making a priori general assumptions on the `class` of motion the structure(s) will (eventually) adopt we can considerably imporve our prelimniary estimate of its spatial configuration (which initializes each time step) and thus reduce the number of fixed point iterations required for FSI solution convergence. The resultant effect of this, as such, is that studying FSI probelms involving bigger (/more complex) fluid domains that have a deformable structural component (maybe many) somewhere becomes more computationally feasible.***

---
