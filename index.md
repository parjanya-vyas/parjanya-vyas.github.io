---
layout: page
show_excerpts: true
entries_layout: list
title: Dissertation
---

Android’s flexibility has fueled its global success across phones, cars, TVs, and wearables — but this very openness also introduces serious security challenges. In particular, customizations made by device manufacturers often lead to inconsistent access control (AC) enforcement, leaving sensitive functionality exposed to malicious apps.

My dissertation develops new static analysis techniques that uncover these hidden vulnerabilities by leveraging Android-specific context. I present four contributions:

Bluebird infers AC requirements from app behavior, revealing 391 under-protected private APIs across stock and vendor ROMs.

Ariadne models AC dependencies in framework data holders, uncovering 30 novel inconsistencies missed by prior tools.

RepFinder identifies duplicated APIs (“Replicas”) introduced through vendor copy-paste code, showing that 37% are under-protected.

AutoAcRaptor analyzes Android Automotive OS, exposing security flaws in car-specific services, with several confirmed by vendors.

Together, these tools demonstrate that context-aware analysis can systematically reveal access control flaws across customized Android frameworks and emerging platforms like Automotive OS. This work advances our ability to secure billions of devices against overlooked vulnerabilities stemming from code duplication, OEM customizations, and domain-specific adaptations.
