# Lab 1 — Requirements Engineering & UML Use-Case Modelling

**Name:** Krishitha Kankanala
**SRN:** PES2UG24CS234
**Class:** 5D

## Problem Statement

**#44 — Developer Tools & IT Operations: Database Query Performance Profiler**

A database observability tool that ingests slow query logs, parses SQL execution plans, identifies missing index candidates, and generates weekly performance optimization digests.

**Target Stakeholders / Actors:** Database Administrator, Backend Lead

## Repository Contents

| File | Description |
|---|---|
| `Lab1_Combined.docx` | Full submission — requirements table, UML use-case diagram, and use-case flow in one document |
| `DB_Query_Profiler_UseCase.drawio` | Editable source file for the UML use-case diagram (open at [app.diagrams.net](https://app.diagrams.net)) |
| `README.md` | This file |

## Deliverable Summary

### 1. Requirements Table
- **5 Functional Requirements** (FR-001–FR-005) covering EXPLAIN plan parsing, log ingestion, weekly digest generation, recommendation status tracking, and threshold-based alerting.
- **2 Non-Functional Requirements** (NFR-001–NFR-002) covering ingestion throughput/scale and data security (encryption at rest, role-based access control).
- Each requirement includes ID, Type, Description, Priority, measurable Acceptance Criteria, and Rationale.

### 2. UML Use-Case Diagram
- **Actors:** Database Administrator, Backend Lead, Scheduler (automated trigger)
- **Use Cases (UC-01–UC-07):** Ingest Slow Query Logs, Parse EXPLAIN Execution Plan, Recommend Missing Indexes, Generate Weekly Performance Digest, View Performance Dashboard, Manage Recommendation Status, Send Threshold Alert
- **«include»:** Recommend Missing Indexes includes Parse EXPLAIN Execution Plan; Generate Weekly Performance Digest includes Recommend Missing Indexes
- **«extend»:** Send Threshold Alert extends Ingest Slow Query Logs

### 3. Use-Case Flow
- **Use Case:** Recommend Missing Indexes
- **Actor:** Database Administrator (primary), Scheduler (secondary)
- 9-step Main Flow plus one Alternate Flow (no sequential scans found)

## Tools Used
- draw.io for UML use-case modelling
