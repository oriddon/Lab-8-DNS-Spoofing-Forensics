# SBT-DF203 Lab 8 – DNS Spoofing Forensics

## Student Information

- **Student Name:** Athanasius Alekwe
- **Student ID:** 2025/FWSD/11230
- **Course:** SBT-DF203 – Basic Networking Skills for Digital Forensics
- **Lab:** Lab 8 – DNS Spoofing Forensics
- **Instructor:** Aminu Idris
- **Submission Date:** 24 September 2026

---

## Overview

This repository contains my practical work for **SBT-DF203 Lab 8 – DNS Spoofing Forensics**.

The purpose of the practical was to investigate a controlled DNS spoofing event inside an authorized virtual lab environment. I established a normal network baseline, reviewed the supplied ARP and DNS spoofing scripts, captured the controlled spoofing activity, analysed the DNS and ARP evidence, correlated the spoofed DNS response with the victim's later HTTP connection, and finally restored the lab environment.

The exercise was carried out using a Kali Linux analyst VM and a Metasploitable victim VM.

---

## Lab Objectives

The practical focused on:

- Recording normal DNS, ARP and network information before the simulation.
- Creating and hashing a harmless training web page.
- Reviewing the instructor-provided ARP and DNS spoofing scripts.
- Performing the controlled simulation in an isolated lab environment.
- Capturing DNS, ARP and HTTP traffic.
- Identifying DNS query and response anomalies.
- Correlating DNS activity with ARP manipulation.
- Verifying the victim's connection to the spoofed destination.
- Preserving evidence using SHA-256 hashes.
- Cleaning up and restoring the network environment after the test.

---

## Lab Environment

The practical used two main virtual machines:

### Kali Linux Analyst VM

The Kali machine was used for:

- Packet capture and analysis
- Hosting the harmless ICDFA training page
- Reviewing the supplied scripts
- Running the authorized ARP and DNS spoofing simulation
- Analysing DNS, ARP and HTTP evidence

During the final NAT-based controlled test, the Kali analyst machine used:

```text
192.168.45.130
