# Cybersecurity GRC and Incident Response Case Studies

This repo contains two simulated case studies built to practice the defensive and governance side of cybersecurity: incident response reporting and risk assessment. Both were completed as part of the Datacom Cyber Security Operations Job Simulation on Forage, then extended into full standalone reports.

**These are simulated exercises for fictional companies. They are not real client engagements or real incidents.**

## Background

My main focus has been offensive security through bug bounty work on HackerOne. These case studies were a deliberate exercise in thinking from the other side, the team that has to investigate, contain, and report on an incident after it happens, and the team that has to identify and prioritise risk before anything happens at all.

## What's in this repo

### 1. Incident Response Report — Orion Health Services (Ransomware Attack)

A full incident response report for a simulated ransomware attack against a healthcare technology provider. Covers:

- Executive summary
- Incident timeline reconstructed from indicators of compromise (phishing email, Mimikatz credential harvesting, lateral movement, ransomware deployment)
- Impact assessment across data, systems, business operations, and regulatory exposure (NDB scheme, Privacy Act 2020)
- Root cause analysis mapping each technical gap to what let the attack escalate
- Prioritised recommendations (immediate, short-term, long-term)

`/incident-response-report/`

### 2. Cybersecurity Risk Assessment Report — RetailNova Pty Ltd

A complete risk assessment for a simulated retail company, built around a threat and vulnerability inventory and a full risk register. Covers:

- Threat and vulnerability identification across 8 key assets (customer data, e-commerce platform, POS systems, CRM/ERP, cloud hosting, endpoints, third-party vendors, internal comms)
- Three fully worked risks, each grounded in a real historical incident from the case study (phishing, ransomware, third-party vendor data leak)
- Inherent vs residual risk ratings using a 5x5 risk matrix (likelihood x consequence)
- A risk escalation email for the one risk that stayed HIGH after existing controls were considered
- Reference risk prioritisation matrix and ratings criteria

`/risk-assessment-report/`

## A finding worth highlighting

In the RetailNova assessment, the third-party vendor data leak risk kept a HIGH residual rating even after accounting for existing controls. That's not an error, it's the point. RetailNova had no vendor risk management program in place, so nothing actually reduced that risk. A risk assessment is only useful if it's willing to show you where the gap still is, rather than assuming a generic control fixes everything.

## Methodology

Both reports follow structured frameworks rather than ad hoc analysis:

- **Incident response** follows the NIST/SANS IR lifecycle: identification, containment, eradication, recovery, lessons learned.
- **Risk assessment** follows a standard 5x5 risk matrix (Likelihood 1-5 x Consequence 1-5), with separate inherent and residual ratings so the effect of existing controls is visible rather than assumed.

## Acknowledgements

Built following the Datacom Cyber Security Operations Job Simulation, hosted on Forage.

## Disclaimer

All company names, incidents, and data referenced in these reports are fictional and used for training purposes only. No real organisation, individual, or incident is represented.
