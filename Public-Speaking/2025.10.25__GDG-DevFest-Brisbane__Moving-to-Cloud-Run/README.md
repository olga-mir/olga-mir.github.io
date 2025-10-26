# GDG DevFest Brisbane 2025

I presented at GDG DevFest Brisbane 2025 on October 25th, exploring the critical mindset shift needed when transitioning from Google Kubernetes Engine (GKE) to Cloud Run.

When moving from GKE to Cloud Run, engineers and security teams often bring their Kubernetes "luggage" with them—trying to replicate familiar concepts like network policies and perimeter-based security in a fundamentally different world. But what if this is the wrong approach? Instead of forcing old patterns, let's first step back to understand the new serverless paradigm and build security from there. "Where we going we don't need roads". We need identity.

This session explores the common traps you can fall into by applying Kubernetes recipes to Cloud Run. We'll focus on the native Cloud Run ecosystem and show how network security should be reimagined for a serverless architecture. In GKE, we carefully craft network policies and segment clusters to prevent lateral movement. In Cloud Run, you need a different mindset and a new set of tools.

A technical deep-dive demo walks through practical patterns for securing production Cloud Run applications, covering ingress control, egress management, and service-to-service communication in ways that work with Cloud Run's design, not against it. You'll leave ready to confidently set aside old habits and embrace the powerful, identity-first security model that Cloud Run offers.

[Session Details](https://devfest-brisbane-2025.sessionize.com/session/1023109)

## Slides

- [Download PDF](./moving-to-cloud-run.pdf)
