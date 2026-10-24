---
title: Try It Yourself - Catching a Cheating Drone
date: 2026-10-17 10:30:00 +0100
categories: [Machine Learning, Security]
tags: [federated-learning, security, demo]
description: An interactive, step-by-step demo of how a group can spot and ignore one cheating member.
published: true
---

In the [previous post](/mzblog/posts/spotting-bad-drones/), we saw how a group can spot a cheater. Now try it yourself.

The demo below uses a study group of eight students. Three of them cheat by writing the opposite answer. Work through the five steps and see what happens.

<iframe src="/mzblog/assets/demo/fl_poisoning_demo_v5.html" width="100%" height="950" style="border:0; border-radius:12px;" loading="lazy" title="Interactive demo: catching a cheating drone"></iframe>

Can't see the demo? [Open it in a new tab](/mzblog/assets/demo/fl_poisoning_demo_v5.html).

## How to use it

1. **Meet the group.** Each student is an arrow. The study guide is their average.
2. **Find the typical answer.** Tap a student to see their score against the median.
3. **Set the trust line.** Move the slider. Students below the line are blocked.
4. **Compare the guides.** See which guide points at the star, with and without blocking.
5. **Check yourself.** Answer two quick questions. Feedback appears under each one.

## What to notice

- Cheaters send arrows pointing the opposite way, so their scores fall.
- The median stays with the honest students, even when a few cheat.
- Blocking the cheaters keeps the guide on target.

## What the demo simplifies

- Each student is a two-dimensional arrow. Real models have thousands of numbers.
- The answers are fixed, not produced by real training.
- The trust line is a simple setting. Choosing it well is part of the research.

The idea is the same, though: check each answer against the group, and ignore the ones that disagree.
