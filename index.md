---
layout: page
show_excerpts: true
entries_layout: list
---

## About Me

I am a PhD candidate in Computer Science at the **University of Waterloo**, specializing in **mobile platform security** with a focus on **Android systems**. My research explores how static analysis, along with techniques like probabilistic inference, graph theory, and natural language processing can be applied to the Android framework to uncover **access control inconsistencies** that lead to critical security vulnerabilities.

Prior to my doctoral studies, I worked as an **Android developer** at **General Motors**, contributing to large-scale automotive software systems, and at **Stack Fintech**, a startup focused on financial technologies. I began my professional career at **Samsung Electronics** as an Android developer, where I gained hands-on experience with large-scale mobile platforms.

I hold a **Master’s degree in Computer Science from IIT Bombay**, where my research centered on **operating systems security using information flow control**. These experiences—spanning both academic research and industry development—have shaped my interest in building rigorous, scalable methods to strengthen mobile and automotive computing platforms.

You can find more about my work on my [**Google Scholar**](https://scholar.google.com/citations?user=61zFh8IAAAAJ&hl=en&oi=ao) and download my [**CV from here**](docs/images/Resume_Academic.pdf).

## Dissertation

Android’s flexibility has fueled its global success across phones, cars, TVs, and wearables — but this very openness also introduces serious security challenges. In particular, customizations made by device manufacturers often lead to inconsistent access control (AC) enforcement, leaving sensitive functionality exposed to malicious apps.

My dissertation develops new static analysis techniques that uncover these hidden vulnerabilities by leveraging Android-specific context. I present four contributions:

Bluebird infers AC requirements from app behavior, revealing 391 under-protected private APIs across stock and vendor ROMs.

Ariadne models AC dependencies in framework data holders, uncovering 30 novel inconsistencies missed by prior tools.

RepFinder identifies duplicated APIs (“Replicas”) introduced through vendor copy-paste code, showing that 37% are under-protected.

AutoAcRaptor analyzes Android Automotive OS, exposing security flaws in car-specific services, with several confirmed by vendors.

Together, these tools demonstrate that context-aware analysis can systematically reveal access control flaws across customized Android frameworks and emerging platforms like Automotive OS. This work advances our ability to secure billions of devices against overlooked vulnerabilities stemming from code duplication, OEM customizations, and domain-specific adaptations.
