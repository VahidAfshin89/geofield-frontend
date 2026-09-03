# GeoField — P1 Product UX Discovery
## Canonical Product UX Baseline — P1.1 to P1.9

**Project:** GeoField  
**Track:** Frontend / Product / UX  
**Repository:** `VahidAfshin89/geofield-frontend`  
**Phase:** P1 — Product UX Discovery  
**Status:** CLOSED / PASS  
**Language:** Persian RTL-first  
**Product Identity:** International / Country-Neutral

## 1. Product Definition
GeoField یک پلتفرم عملیات میدانی و تحلیل مکانی است که داده‌های میدانی، موقعیت مکانی، رخدادها، پایش، اقدامات و شواهد را از میدان تا داشبورد به یک جریان عملیاتی متصل می‌کند؛ با تجربه Field-first و Offline-first در Mobile و تجربه GIS-centric و Operational در Web.

GeoField نباید به Generic CRUD Panel، Generic Survey App، BI-only Dashboard، GPS App یا Generic GIS تقلیل یابد.

## 2. Product Identity & Language
- International / Country-Neutral
- Persian RTL-first
- Localization-ready
- Brand-flexible
- Country-specific behavior via configuration/data/localization
- هیچ کشور، سازمان یا ساختار اداری نباید در Core Product Identity hard-code شود.

هدف زبانی:
```text
fa
 en
 ...
```

## 3. Visual Direction
**Professional GIS + Modern Spatial**

اصول:
- Professional
- Clean
- Modern
- Spatial
- Operational
- Distinctive

3D:
```text
Purposeful 3D
```
نه Decorative 3D Everywhere.

Animation باید معنا داشته باشد: Sync، Upload، GPS، Loading، Success، Failure، Navigation و State Transition.

## 4. North Star
```text
FIELD
→ SYNC
→ UNDERSTAND
→ ACT
→ VERIFY
```

مدل کامل‌تر:
```text
OBSERVE
→ CAPTURE
→ SAVE
→ SYNC
→ REVIEW
→ ANALYZE
→ DECIDE
→ ACT
→ VERIFY
```

## 5. Personas
### Primary
1. Field Officer — Android-first
2. Operational Supervisor — Web-first, Android secondary
3. GIS Specialist — Web-first, Android secondary

### Secondary
4. Domain Expert
5. Manager / Decision Maker
6. Organization Admin
7. System Administrator

قاعده:
```text
Persona ≠ RBAC Role
```

## 6. Core Jobs
### Field Officer
```text
Locate → Observe → Capture → Save → Sync
```
نیازها: GNSS، Map context، Dynamic Forms، Photos، Attachments، Offline، Draft recovery، Sync status، Retry، حداقل تایپ.

### Operational Supervisor
```text
Monitor → Prioritize → Review → Assign → Follow-up
```
اصل: **Attention Before Information**.

### GIS Specialist
```text
Explore → Filter → Analyze → Compare → Interpret → Act / Report
```
تجربه هدف: **Spatial Workbench**.

## 7. Platform Strategy
### Mobile — Field Action Center
هدف: **Do the Work**
- Field-first
- Action-first
- Location-first
- Offline-first
- Fast
- Touch-friendly
- Low-typing

### Web — Spatial + Operational Command Center
هدف: **Understand and Manage the Work**
- Dashboard-first
- Analysis-first
- Map-first
- Information-dense where necessary
- Multi-panel
- Desktop-oriented

قاعده:
```text
Mobile ≠ Mini Web
Web ≠ Enlarged Mobile
```

## 8. Mobile / Web Responsibilities
### Mobile Core
Field Visit execution، GNSS، Capture، Dynamic Forms، Photos، Attachments، Offline، Drafts، Sync، Incident capture، Patrol execution، Fire/Grazing/Restoration/Monitoring capture.

### Web Core
Operational Dashboard، GIS Workspace، Spatial Analysis، Layer Management، Feature Inspection، Historical/Temporal Analysis، Reporting، Administration، Supervisor/Management workflows.

### Shared
Authentication، Projects، Dynamic Form Runtime، Domain Records، Map Context، Incident Review، Action State، Sync Awareness.

## 9. Core UX Principles
1. Context Over Complexity
2. Map Is a Core Interaction Surface
3. Save Must Mean Safe
4. Offline Is an Operating Mode
5. See → Act
6. Never Lose Context
7. Record Continuity
8. Data → Action
9. Attention Before Information
10. Errors should be recoverable
11. Persona ≠ RBAC
12. Shared Domain / Different Contexts

## 10. Core Operational Workflows
### Field Operation
```text
LOGIN
→ SELECT PROJECT
→ CHECK READINESS
→ START FIELD VISIT
→ GNSS
→ MAP
→ OBSERVATION
→ DYNAMIC FORM
→ PHOTO / ATTACHMENT
→ LOCAL SAVE
→ SYNC / QUEUE
→ COMPLETE VISIT
→ SERVER VERIFICATION
```

### Incident → Action → Verification
```text
CAPTURE
→ SYNC
→ REVIEW
→ SPATIAL CONTEXT
→ DECISION
→ ACTION
→ ASSIGNMENT
→ EXECUTION
→ EVIDENCE
→ VERIFICATION
→ FOLLOW-UP
```

### GIS Investigation → Analysis → Decision
```text
SELECT PROJECT
→ SELECT AREA / TIME
→ LOAD LAYERS
→ FILTER
→ SPATIAL QUERY
→ FEATURE INSPECTION
→ TIMELINE
→ ANALYSIS
→ INTERPRETATION
→ DECISION
→ ACTION / REPORT
```

## 11. Record Continuity
Record should preserve, as applicable:
```text
Record
├── Location
├── Time
├── User
├── Project
├── Parent Visit
├── Attachments
├── Actions
└── History
```

## 12. Save / Sync / Verification
```text
Saved Locally
≠
Uploaded
≠
Verified
```

Attachment lifecycle:
```text
Captured
→ Local
→ Waiting Sync
→ Uploading
→ Uploaded
→ Verified
```
Failure:
```text
Upload Failed → Retry
```

## 13. Field Conditions & Offline
Mobile باید برای Bright Sun، One-hand use، Gloves، Movement، Weak GPS، GPS loss، Weak/intermittent network، No network، Long sessions، Battery، Storage، Large attachments، App interruption/termination و Device restart طراحی شود.

Offline:
```text
Operating Mode
```
نه Error State.

Target:
```text
Up to 72 hours
```
برای Essential Field Workflows.

Essential Offline:
- Field Visit
- Forms
- Drafts
- GNSS
- Photos
- Attachments
- Incident
- Patrol
- Fire
- Grazing
- Restoration
- Monitoring

Technical requirements identified:
- Durable local persistence
- Offline form runtime
- Attachment persistence
- Retry strategy
- Controlled/background sync
- Idempotency
- Conflict strategy
- Storage management
- Recoverable app state
- GNSS accuracy handling
- Data freshness metadata

## 14. GIS / Spatial Model
Map یک Primary Interaction Surface است، نه decoration.

### Field
```text
Locate → Identify → Navigate → Capture
```

### Supervisor
```text
Monitor → Prioritize → Inspect → Act
```

### GIS Specialist
```text
Explore → Filter → Query → Measure → Compare → Analyze
```

الگوهای کلیدی:
- List ↔ Map
- Feature Inspector
- Layer Management
- Spatial Filter
- Temporal Filter
- Map + Timeline
- Spatial Query
- Spatial-to-Action
- Cross-filtering (candidate)

GIS capability levels:
```text
Level 1 Field: Locate / Navigate / Identify / Capture
Level 2 Operations: Filter / Monitor / Inspect / Prioritize
Level 3 GIS: Query / Measure / Compare / Analyze / Correlate
```

## 15. MVP Prioritization
### P0 — MVP Critical
- Authentication
- Projects
- Field Visit
- GNSS
- Dynamic Forms
- Offline
- Local Persistence
- Sync
- Attachments
- Basic Map
- Incident
- Actions
- Verification
- List ↔ Map
- Feature Inspector
- Basic Layers
- Basic Search/Filter
- Supervisor Dashboard

### P1 — MVP Important / Early Expansion
- Reporting
- Patrol
- Fire
- Grazing
- Violation
- Restoration
- Monitoring
- Map + Timeline

### P2 — Post-MVP
- Advanced Spatial Queries
- Advanced GIS Analysis
- Heatmaps
- Advanced Temporal Analytics
- Advanced Layer Styling
- Full Offline Map Packages
- Advanced 3D

### P3 — Future
- Advanced Spatial Statistics
- Advanced 3D Analysis
- Sophisticated AI/ML
- Predictive Capabilities

اصل:
```text
Core Workflow before Feature Volume
Reliability before AI
```

## 16. Dashboard Concept
Dashboard به سمت **Spatial + Operational Command Center** می‌رود.

Operational Command:
- Current status
- Alerts
- Open Actions
- Recent Incidents
- Patrol Status
- Fire/Grazing
- Field Activity
- Map

GIS / Analysis Workbench:
- Layers
- Filters
- Spatial Analysis
- Feature Selection
- Charts
- Time
- Queries
- Map
- Results

Dashboard نباید KPI-only یا Data Dump باشد.

## 17. Dynamic Forms
```text
Backend Form Definition
→ Schema / Runtime Contract
→ Frontend Form Renderer
```

هر Form نباید به‌صورت جداگانه hard-code شود.

## 18. 3D / AI Policy
3D:
```text
3D = Differentiation Opportunity
3D ≠ MVP Dependency
```

AI/ML:
```text
Not MVP Core
```
ترتیب مطلوب:
```text
Reliable Data
→ Spatial Context
→ Operational History
→ Analytics
→ AI/ML
```

## 19. Technical Status
Provisional:
```text
Mobile: Flutter
Web: React + Next.js + TypeScript
Animation: Rive
Web 3D: Three.js + React Three Fiber
Design: Figma
3D Authoring: Blender / Spline
```

نسخه‌ها در زمان implementation با مستندات رسمی بررسی و Freeze می‌شوند.

## 20. Map Engine
**NOT FROZEN**

تصمیم باید بر اساس Offline، Vector/Raster Tiles، Licensing، Tile Source، Self-hosting، 3D، Performance، Global availability، CRS و PostGIS integration باشد.

ایده اختصاصی کاربر برای Map باید پیش از Freeze وارد ارزیابی شود.

## 21. Backend Alignment
- Stage 90 — Operational Reporting
- Stage 91 — GIS Production API
- Stage 92 — API Consumer Contract

Stage 92 باید موضوعاتی مانند Authentication، Token Refresh، Errors، Pagination، GeoJSON، Attachments، Forms، Versioning، Offline Sync، Idempotency و Conflict semantics را formalize کند.

## 22. Migration Governance
```text
UX Requirement ≠ Schema Delta
```

P1 هیچ Backend/Database/Migration mutation ایجاد نکرده است.
Migration فقط با:
```text
Real Schema Delta
+
Explicit Design
+
Review
```
مجاز است.

## 23. P1 Decision
```text
P1.1 ✅
P1.2 ✅
P1.3 ✅
P1.4 ✅
P1.5 ✅
P1.6 ✅
P1.7 ✅
P1.8 ✅
P1.9 ✅

P1 STATUS = CLOSED
P1 RESULT = PASS
```

### Canonical Continuation State
```text
Repository: VahidAfshin89/geofield-frontend
Current Phase: P1 CLOSED
Next: P2 — Information Architecture
Primary: Field Officer / Operational Supervisor / GIS Specialist
Mobile: Field-first / Action-first / Location-first / Offline-first
Web: Dashboard-first / Spatial / Operational / Analytical
Visual: Professional GIS + Modern Spatial
Offline: 72-hour target for essential workflows
North Star: FIELD → SYNC → UNDERSTAND → ACT → VERIFY
Map: Primary interaction surface; engine NOT FROZEN
Technical Stack: Provisional
Backend Alignment: 90 / 91 / 92
Migration: NONE in P1
```
