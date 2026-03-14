# Case Study: Recruiting & Onboarding Automation System

**Context:** TekSynap | Department of the Interior federal contract | 70-person hiring operation  
**Stack:** Microsoft Power Apps, Power Automate, SharePoint Lists, Microsoft Teams, Outlook  

## What Was Broken

A 70-person federal contract with 15 concurrent job openings and 100+ candidates in the pipeline simultaneously. Every step ran through email and memory: resume routing, interview scheduling, feedback collection, offer assembly, and security handoff. The process consumed 15+ hours per week and had zero real-time visibility for recruiters.

## What I Designed

A two-component system: a Power App for candidate intake and a Power Automate workflow with six conditional branches — each triggered by a specific action inside the app.

The six branches: resume routing to the correct technical lead, candidate availability requests, automated Teams interview creation, feedback packaging to recruiters, offer parameter assembly, and EOD security handoff with pre-formatted candidate packages.

A central SharePoint List provided live status tracking across all candidates — eliminating recruiter interruptions for status updates entirely.

## What I Built

- Power App UI for single-form candidate intake with resume attachment upload
- Power Automate workflow with six conditional branches, SharePoint read/write, dynamic Teams meeting creation, and Outlook email generation
- SharePoint List as the operational database — structured for multi-recruiter, multi-task-order filtering
- Automated EOD package assembly that sent pre-formatted security intake emails with zero manual data entry

## What Changed

- Recruiting coordination time dropped from 15+ hours/week to under 7 hours — despite increasing candidate volume
- 150+ candidates processed with consistent tracking and zero dropped handoffs
- Recruiter status update interruptions eliminated completely
- EOD security handoff fully automated — previously required manual assembly and email composition for every accepted offer
- System scaled across 15 concurrent positions with different technical leads, pay structures, and clearance requirements

---

*The n8n proof project in this repo rebuilds the core intake and routing pattern in an open-source stack with an AI classification layer added. The production system described above ran on a live federal contract.*
