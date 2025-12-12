# ROOTED Education — Vertical Application

This repository powers the **Education vertical** for ROOTED.

It is **not** a standalone platform.  
It is a governed surface layer built on top of:

- `rooted-core` (backend, schema, RLS, RPCs)
- `rooted-platform` (governance, law, safety, access)

---

## 🎓 What ROOTED Education Is

ROOTED Education exists to:

- Connect **schools, youth programs, and institutions** with vetted experiences
- Coordinate **field trips, learning programs, and educational visits**
- Provide a **safe discovery layer** for parents, educators, and institutions
- Reuse ROOTED’s core:
  - Providers
  - RFQs & quotes
  - Events & experiences
  - Landmarks & seasonal intelligence

Education is:

- ✅ Non-political
- ✅ Safety-first
- ✅ Institution-supervised
- ✅ Fully governed by ROOTED’s Kids and Sanctuary laws

---

## 🔒 Governance Boundaries

This repository:

- ❌ Does **NOT** define roles, tiers, or global access law  
- ❌ Does **NOT** modify database schema or RLS  
- ❌ Does **NOT** redefine Kids Mode rules  
- ❌ Does **NOT** change sanctuary/nonprofit protections  
- ❌ Does **NOT** introduce new markets outside the procurement grid

ALL of that lives in:

- `rooted-platform/governance/`
- `rooted-core/docs/`

This app must obey:

- `ROOTED_PLATFORM_CONSTITUTION.md`
- `ROOTED_KIDS_MODE_GOVERNANCE.md`
- `ROOTED_SANCTUARY_NONPROFIT_LAW.md`
- `ROOTED_VERTICAL_ACCESS_CONTRACT.md`
- `BILLING_ARCHITECTURE.md`
- `DISCOVERY_RULES.md` + `GEO_RULES.md`

UI is **never** a source of authority.  
It only reflects law — it does not create it.

---

## 🧭 Vertical Scope

Education vertical focuses on:

- School & youth **institution dashboards**
- **Field trip** discovery + planning
- **Program** discovery (camps, classes, clinics)
- **RFQ / quote requests** from institutions to vetted providers
- Trip **conditions** (weather, access, safety) via `vertical_conditions_v1`

Education **does not**:

- Turn Kids UI into a marketplace
- Allow children to trigger bookings or payments
- Create independent roles or tiers outside `user_tiers`

---

## ✅ Allowed Work Here

- Education-specific UI and flows
- Institution dashboards and trip planners
- Program & trip discovery layouts
- Adult-facing quote/payment UI wiring (to existing core APIs)
- Accessibility, performance, and mobile layout improvements
- Visual integration with seasons / holidays (respecting consent law)

## ❌ Forbidden Work Here

- Defining or changing Kids Mode behavior
- Weakening sanctuary / nonprofit protections
- Creating new RFQ/bid/bulk schemas
- Changing tier → feature entitlement rules
- Overriding GEO (50-mile) or discovery (6–8 card) laws

---

## 🔗 Source of Authority

This vertical must read from:

- `rooted-core` for:
  - Education-related views, RPCs, and conditions
- `rooted-platform/governance` for:
  - Roles, tiers, Kids rules, sanctuary rules, abuse & debug guides

If Education UI and governance conflict →  
**governance wins**.
