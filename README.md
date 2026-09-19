# Admin dashboard analytics

## Overview
Add a live overview as the first screen inside the existing PIN-protected Admin Portal. It will use the current Railway Hall visual system and real records already stored in Lovable Cloud.

## What will be built
- Add a **Dashboard** tab before the existing Students tab and open it by default after admin access is granted.
- Show summary figures for:
  - total students
  - residents and non-residents
  - upcoming/published events
  - marketplace listings and orders
- Add responsive charts for:
  - student growth over recent months
  - resident versus non-resident distribution
  - events by month
  - marketplace listing and order activity over recent months
- Add compact operational summaries for upcoming events and marketplace status so the charts connect to actionable records.
- Include loading, empty, and retry/error states without sample or fabricated data.
- Keep all existing admin tabs and PIN protection unchanged.

## Technical details
- Create a focused admin dashboard component using the installed Recharts package.
- Read `profiles`, `events`, `marketplace_listings`, and `marketplace_orders` through the existing signed-in client and current admin access policies.
- Aggregate chart series in the browser from the returned timestamps and statuses; no schema migration is needed.
- Use existing semantic colors, cards, typography, and responsive layout patterns.
- Update the roadmap and verify the dashboard on phone and desktop, including empty-data rendering and app health.

