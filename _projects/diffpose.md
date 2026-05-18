---
layout: page
title: DiffPose
description: Differentiable projection matching for fast pose inference in cryo-EM
img: assets/img/diffpose.png
importance: 1
category: methods
related_publications: false
---

**DiffPose** is a differentiable framework for pose inference in cryo-electron microscopy. By replacing exhaustive projection matching with gradient-based optimization, DiffPose enables fast, accurate orientation refinement on large single-particle datasets.

**Key ideas**

- Differentiable projection operator that backpropagates pose gradients through the imaging model.
- GPU-efficient implementation suitable for hundreds of thousands of particles.
- Compatible with downstream 3D reconstruction pipelines.

**Status:** preprint available; software release in preparation.
