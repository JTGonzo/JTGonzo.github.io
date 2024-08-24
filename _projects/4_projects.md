---
layout: page
title: Interface gradient approximation
description: A ROM for predicitng the motion of FSI interfaces
img: assets/img/taylor_expans.jpg
importance: 4
category: work
---

***This page is currently a `WORK IN PROGRESS`. Here I will be posting incremental results as I progress my work developing a Reduced Order Method (ROM) that approximates the spatio-temporal gradient of an FSI problem’s interface. In smoothly evolving FSI problems, such as those involving elastic structures submerged in a laminar flow, the power spectrum of individually examined nodal trajectories (when sampled over a single period of oscillation for example) is shown to be extremely bi-modal with very low variance around the spectrum's dominant frequencies. As such, by using only a handful of strategically selected Fourier modes we can obtain (on a rolling basis) a continuous function that describes each node's local behavior reasonably well. With this array of continuous functions in hand we can then compute both the approximate location of each of the interface's nodes at the forward time step as well as the reduced order Jacobian matrix that describes the spatially dependent local rate of change. While not sufficient on its own to ensure problem convergence for any particular set of FSI problems; other than those that may already be implicitly convergent in which case we will likely see an acceleration in convergence rate; this technique may prove itself particularly valuable at imrpoving the performance of traditional quasi-Newton coupling techniques. Where those methods require at a minimum 2 fixed point iterations to generate the first secant pair used to appriximate the interfacial Jacobian, my newly proposed technique provides an approximate interfacial gradient immeidately. As such, this RO jacobian can be used in the first 2 iterations to stabilize the coupling procedure (minimize the degree of solution divergence) and thereby provide a better conditioned solution for traditional techniques to then progress more efficiently.***

---
