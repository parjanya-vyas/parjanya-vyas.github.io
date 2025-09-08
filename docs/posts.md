---
title: Dissertation
layout: page
permalink: /dissertation/
show_excerpts: true
---

Android’s open-source design and extensive customization have fueled its dominance across smartphones, automotive systems, wearables, and other domains. This flexibility, however, introduces serious security challenges, particularly in the enforcement of access control (AC). Prior research has investigated version-level, framework-level, and cross-layer inconsistencies, yet important gaps remain—especially in detecting OEM-introduced data-driven customizations, replicated APIs, and domain-specific adaptations (e.g., automotive) that are difficult to capture with existing techniques.

This dissertation investigates how Android-specific contextual features can be systematically leveraged to uncover AC vulnerabilities that evade prior analyses. I present four main contributions:

Bluebird — a probabilistic inference framework that derives AC requirements from application-side sensitivity indicators (UI cues and app-side AC). By fusing NLP-driven signals with static analysis, Bluebird identifies APIs whose protections do not match implied sensitivity. Applied to 14 ROMs, Bluebird flagged 391 likely-underprotected private APIs and supported 11 proof-of-concept exploits.

Ariadne — a static-analysis technique built around a novel AC dependency graph abstraction that models explicit and inferred AC relationships among framework data holders. Ariadne detects inconsistencies introduced by data-driven vendor customizations that traditional tools miss. Evaluated on AOSP and vendor ROMs, it discovered 30 unique inconsistencies and enabled 13 proof-of-concept exploits.

RepFinder — a large-scale measurement pipeline that identifies duplicated or “Replica” APIs created via copy-paste editing and evaluates their AC enforcement. Analyzing 342 ROMs from 10 vendors, RepFinder found replication to be widespread (≈141 Replicas/ROM on average) and that a significant fraction (~37% on average) of Replicas are under-protected.

AutoAcRaptor — a domain-specific static analysis framework for Android Automotive OS (AAOS) that identifies automotive entry points and evaluates both AC and feature-check enforcement. Applied to 10 AAOS ROMs, AutoAcRaptor reported an average of 23 auto feature and AC anomalies per ROM; several vendor-acknowledged issues demonstrate practical impact.

Collectively, these contributions show that Android-specific contextual features — from app-side sensitivity indicators to framework data holders and domain-specific service registrations — can be systematically harnessed to reveal overlooked AC vulnerabilities. They also demonstrate that techniques for identifying framework customization-induced vulnerabilities can be adapted to emerging Android-based domains such as AAOS by accounting for platform-specific differences.

# Publications

## Ariadne - Navigating through the Labyrinth of Data-Driven Customization Inconsistencies in Android

**Authors:** P Vyas, HUR Faheem, Y Aafer, N Asokan\
**Date Of Publication:** 11th August, 2025\
**Conference:** 34th USENIX Security Symposium (USENIX Security 25), 2025\
[Paper Link](https://www.usenix.org/system/files/usenixsecurity25-vyas.pdf), [BibTeX](../docs/images/ariadneBibTeX.txt)

## Red Light for Security - Uncovering Auto FeatureCheck and Access Control Gaps in AAOS

**Authors:** Jumana, P Vyas, Y Aafer\
**Date Of Publication:** 10th July, 2025\
**Conference:** International Conference on Detection of Intrusions and Malware, and Vulnerability Assessment\
[Paper Link](https://link.springer.com/chapter/10.1007/978-3-031-97623-0_9), [BibTeX](../docs/images/redlightBibTeX.txt)

## A Longitudinal Analysis Of Replicas in the Wild Wild Android

**Authors:** SMA Zaidi, S Khan, P Vyas, Y Aafer\
**Date Of Publication:** 24th October, 2024\
**Conference:** ASE '24 Proceedings of the 39th IEEE/ACM International Conference on Automated Software Engineering\
[Paper Link](https://dl.acm.org/doi/abs/10.1145/3691620.3695546), [BibTeX](../docs/images/wildAndroidBibTeX.txt)

## Auditing Framework APIs via Inferred App-side Security Specifications

**Authors:** P Vyas, A Waheed, Y Aafer, N Asokan\
**Date Of Publication:** 09th August, 2023\
**Conference:** 32nd USENIX Security Symposium (USENIX Security 23), 2023\
[Paper Link](https://www.usenix.org/system/files/usenixsecurity23-vyas.pdf), [BibTeX](../docs/images/auditingBibTeX.txt)
