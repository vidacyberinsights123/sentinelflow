# SentinelFlow

Splunk detection-as-code and SOC automation lab on Kali Linux.

## Goal
Build a small, realistic SOC workflow on a single low-resource laptop: collect logs, detect attacks with version-controlled Splunk searches, and automate triage and reporting with Python.

## Why I'm building this
Splunk is built for large organisations and is expensive. This project shows how to practise SIEM work on a free license with limited hardware (8 GB RAM), and to document it the way a SOC analyst would.

## Planned architecture
- Splunk Enterprise running in Docker (memory-capped)
- Kali Linux authentication and system logs as the log source
- Simulated attacks against my own machine only (e.g. SSH brute force)
- Detections written as SPL searches and mapped to MITRE ATT&CK
- Python automation: alert polling, IP enrichment, severity scoring, incident report generation

## Repository layout
| Folder | Purpose |
|---|---|
| `lab/` | Docker and Splunk setup files |
| `detections/` | SPL detection rules with MITRE mapping |
| `automation/` | Python triage and reporting scripts |
| `reports/` | Incident reports from simulated attacks |
| `docs/` | Documentation and screenshots |

## Status
Week 1: project setup. Nothing is working yet; progress is committed as I go.

## Disclaimer
This is a home lab for learning. All attack simulations run only against systems I own. It is not production experience.

## Author
David Ndolo, aspiring SOC analyst. Thika, Kenya.
