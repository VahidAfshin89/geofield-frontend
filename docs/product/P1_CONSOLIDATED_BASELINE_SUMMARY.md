# GeoField — P1 Consolidated Baseline Summary

This document is the compact transfer/continuation summary for P1. It does not replace the canonical detailed document; it provides the fastest reliable context for a new chat/session.

## Status

```text
P1.1 Product Vision & Boundaries       ✅
P1.2 User Roles & Personas             ✅
P1.3 User Jobs & Pain Points           ✅
P1.4 Mobile vs Web Responsibility      ✅
P1.5 Core Operational Workflows        ✅
P1.6 Field Conditions & Offline        ✅
P1.7 GIS / Spatial Workflows           ✅
P1.8 Feature Prioritization            ✅
P1.9 Consolidation & Decision Gate     ✅

P1 = CLOSED / PASS
Next = P2 — Information Architecture
```

## Product
GeoField = GIS-centric Field Intelligence Platform combining field operations, spatial context, offline-first collection, monitoring, operational workflow, analysis and action.

## Identity
```text
International / Country-Neutral
Persian RTL-first
Localization-ready
Brand-flexible
```

## Primary Personas
```text
Field Officer
Operational Supervisor
GIS Specialist
```

## Platform
```text
Mobile = Field Action Center
Web    = Spatial + Operational Command Center
```

```text
Mobile ≠ Mini Web
Web ≠ Enlarged Mobile
Persona ≠ RBAC Role
```

## North Star
```text
FIELD → SYNC → UNDERSTAND → ACT → VERIFY
```

## Core Workflow
```text
CAPTURE → SAVE → SYNC → REVIEW → ANALYZE → DECIDE → ACT → VERIFY
```

## Offline
```text
Offline = Operating Mode
Target = Up to 72 hours for essential workflows
Saved Locally ≠ Uploaded ≠ Verified
```

## Core UX Principles
- Context Over Complexity
- Map Is a Core Interaction Surface
- Save Must Mean Safe
- Never Lose Context
- Record Continuity
- Data → Action
- Attention Before Information
- Errors should be recoverable

## GIS
Map is a primary work surface. Field uses it for locate/identify/navigate/capture; supervisors for operational monitoring; GIS specialists for explore/filter/query/measure/compare/analyze.

## MVP
P0 covers authentication, projects, field visit, GNSS, dynamic forms, offline/local persistence/sync, attachments, basic map, incident, actions, verification, list↔map, feature inspector, basic layers/filtering and supervisor dashboard.

P1 includes reporting, patrol, fire, grazing, violation, restoration, monitoring and map+timeline. P2/P3 contain advanced GIS, advanced 3D and future AI/ML.

## Technology Status
```text
Flutter = provisional
React + Next.js + TypeScript = provisional
Rive = optional
Three.js + React Three Fiber = optional
Map Engine = NOT FROZEN
```

## Backend Alignment
```text
Stage 90 = Operational Reporting
Stage 91 = GIS Production API
Stage 92 = API Consumer Contract
```

## Governance
```text
UX Requirement ≠ Schema Delta
```
No migration/backend mutation was made by P1.

## Next
```text
P2 — Information Architecture
```
