# GeoField — Frontend Bootstrap & Product Charter Reference

این سند خلاصه مرجع دو سند اولیه ارائه‌شده برای Frontend Track است:
1. Frontend & Product Design Continuation Charter
2. Frontend & Product Design Master Charter

برای وضعیت اجرایی P1، سند Canonical برابر `P1_PRODUCT_UX_DISCOVERY.md` است.

## Backend Baseline
- Backend baseline: end of Stage 89
- Latest migration at that baseline: `8912_restoration_planting`
- Latest full regression stated in the charter: `820 passed / 1 skipped / 2 warnings`

## Product Direction
```text
Modern
+
Professional
+
GIS-oriented
+
Field-oriented
+
Fast
+
Clear
+
Offline-aware
+
Visually distinctive
```

## Core Philosophy
GeoField باید از Backend قدرتمند به یک Product Experience واقعی برای عملیات میدانی و تصمیم‌گیری مکانی تبدیل شود.

```text
Understand
→ Design
→ Prototype
→ Contract
→ Implement
→ Integrate
→ Verify
→ Field Validate
```

## Mobile
```text
Flutter = provisional
Rive = optional
```

هدف Mobile: Android/iOS، field-first، action-first، location-first، offline-first.

## Web
```text
React + Next.js + TypeScript = provisional
```

هدف Web: dashboard، GIS workspace، operational command، analysis، reporting.

## Web 3D
```text
Three.js + React Three Fiber = optional
```

3D و Animation باید purposeful باشند.

## Design
```text
Figma
Blender / Spline as needed
```

## Map
Map Engine عمداً تا زمان بررسی Offline، tiles، licensing، self-hosting، 3D، performance، CRS، PostGIS و ایده اختصاصی Map کاربر Freeze نشده است.

## Product Benchmarks
- ArcGIS Field Maps — field/GIS/offline/location/forms
- ArcGIS Dashboards — operational/map-driven analytics
- KoboToolbox/KoboCollect — forms/offline/GPS/drafts
- Fulcrum — field/GPS/tracking

اصل:
```text
Reference ≠ Copy
```

## Learning Policy
برای کاربر مبتدی:
```text
Explain → Install → Verify → Practice → Build
```

فناوری‌ها فقط هنگام نیاز معرفی و سپس نصب/Verified می‌شوند.

## Product Roadmap Baseline
```text
P1 Product UX Discovery       ✅ CLOSED
P2 Information Architecture  → NEXT
P3 UX Wireframes
P4 Design System
P5 Visual Prototype
...
```

## Backend Alignment
```text
Stage 90 — Operational Reporting
Stage 91 — GIS Production API
Stage 92 — API Consumer Contract
```

## Governance
- Do not redesign Backend without regression evidence.
- Do not turn every UX requirement into an MVP feature.
- Do not hard-code Dynamic Forms.
- Do not treat Offline as an error screen.
- Do not equate local save, upload and verification.
- Do not turn Mobile into mini desktop GIS.
- Do not reduce Web to KPI-only BI.
- Do not Freeze Map Engine before requirements are reviewed.
- Do not hard-code country-specific branding.
- Do not invent Frontend states without Backend Contract.
- Do not create migration without real schema delta + explicit design + review.
