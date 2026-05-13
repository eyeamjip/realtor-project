# Outlaw Realty (Prototype)

Single-file HTML prototype of a CRM for Patty Outlaw-Troutman (Outlaw Realty). No build step — Tailwind / Lucide / Google Fonts via CDN.

**Live preview:** https://eyeamjip.github.io/realtor-project/

## Views

| View | Pattern |
|---|---|
| Overview | KPI tiles + Active Clients table + side rail (Today's Showings · New Leads · Recent Activity) |
| Leads & Clients | 6-column Kanban: New Inquiry → Qualified → Showing → Offer Made → Under Contract → Closed |
| Listings | Sortable property list with status pills + DOM + agent-side column |
| Property Detail | Banner header + tabbed workspace (Overview, Showings, Offers, Documents, Notes) |
| Calendar | Sun-first week grid (8 AM–6 PM) with "now" indicator + side rail (Legend, Tasks, Key Dates); mobile agenda view below 1024px |
| Commission Forecast | KPI strip + SVG bar chart (actual vs projected) + per-deal commission breakdown |
| Activity Log | Day-grouped feed with action-type pills + entity links |

## Brand tokens

- **Primary:** `#1B3A6B` (deep navy)
- **Accent:** `#C9972C` (warm gold)
- **Display font:** Playfair Display
- **Body font:** Inter

## Architecture

- Tailwind CSS via Play CDN
- Lucide icons via CDN
- Vanilla JS hash router + sidebar collapse + tab switching (~80 lines total)
- Mobile breakpoint: `< 1024px` switches to bottom tab bar + calendar agenda view
- Desktop content max-width: `2800px` (workspace standard — fills 1080p/1440p edge-to-edge, ~78% on 4K)
