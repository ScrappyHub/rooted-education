# ROOTED Education — Application Architecture

This vertical is a governed UI shell running on top of:

- ROOTED Core (providers, events, RFQs, bids, analytics)
- ROOTED Platform Governance (roles, tiers, Kids Mode law, vertical access contracts)

It is NOT a standalone platform.
It is a plug-in on top of the ROOTED operating system.

---

## 🧠 Inherited Architecture Layers

Education reuses all ROOTED subsystems:

### Identity & Governance
- Auth
- Role + tier enforcement
- Feature flags
- Admin control
- Kids Mode (OFF at launch)

### Marketplace & Procurement
- RFQs (institution → vendor)
- Bids (vendor → institution)
- Bulk (Premium+ only, optional)

### Discovery & Intelligence
- Providers
- Educational events
- Landmarks & learning sites
- Seasonal overlays
- Holiday cultural intelligence

### Safety & Consent
- Kids Mode restrictions
- Nonprofit & sanctuary limits
- Educational age-appropriateness

### Analytics
- Vendor analytics (tier-gated)
- Procurement analytics (Premium+)
- Discovery engagement analytics

---

## 🧬 Vertical Plug-In Doctrine

ROOTED Education:

- Does NOT define new schema
- Does NOT define new markets
- Does NOT alter Kids Mode
- Does NOT alter billing

It **adds UI only**:

- Educational categories
- Institution dashboard views
- RFQ creation + overview
- Vendor bid overview (tier-gated)
- Field trip / program discovery surfaces

---

## 🛑 Architectural Non-Negotiables

- RLS cannot be bypassed by any UI element  
- Kids Mode cannot surface RFQs or bids  
- Institutions ≠ Vendors; permissions differ  
- Premium+ vendors only can submit bids  
- Discovery caps (6–8 cards) cannot be overridden  
- GEO caps (50 miles, 25 markers) cannot be overridden  

Education must operate inside ROOTED’s safety ecosystem — especially for minors.

---

## 📡 Vertical API Dependencies

Education relies on the following core APIs:

- `providers_*` views  
- `rfqs_public_v1`, `bids_public_v1`  
- `events_public_v1` for educational experiences  
- `seasonal_featured_providers_v1`  
- `vertical_conditions_v1` (for seasonal overlays)  

No Education API may modify platform-wide governance.

---

## 🚧 Development Boundaries

Allowed:
- UI layouts
- Institution-facing dashboards
- Vendor bid review UI
- Kids-friendly education discovery

Forbidden:
- New marketplaces
- New billing states
- Changing RFQ or bid logic
- Overriding governance

---

END OF ARCHITECTURE
