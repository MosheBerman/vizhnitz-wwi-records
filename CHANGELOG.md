# Changelog

## v0.3.0 — 2026-11-04

Two interface additions (MINOR).

- **Timeline tab**: the sidebar now has two tabs, "Map & steps" and
  "Timeline · 66". The Timeline tab renders the full 66-entry table from
  research/timeline.md (generated into timeline.js, same source document),
  with a live text filter. Date conflicts stay flagged in the entries.
- **Mobile map expand/collapse**: in the mobile split view, an "Expand map"
  button (bottom right) expands the map to full screen and collapses back
  to the split ("Show panel"). Desktop layout unchanged.

## v0.2.0 — 2026-11-04

Deep research folded in (MINOR).

- Two new recorded events on the map: the December 1914 evacuation of Wiznitz
  (Judisches Archiv No. 1, May 1915, contemporary primary, text-verified) and
  the destruction by fire of the Wiznitz rabbi's court building in the second
  occupation (Schmelzer, Gold vol. I), with R. Mendele's chair documented as
  transported to Grosswardein.
- Steps log updated: deep-research synthesis, primary-source downloads, and
  the granular timeline are complete; the DRACS step shows the identified
  offices and the shelf-check consequence.
- research/ gains timeline.md (66 entries), deep-research-report.md, and
  primary-sources-index.md.

## v0.1.0 — 2026-11-04

Initial public site.

- Mapbox map centred on Bukovina/the Cheremosh with seven toggleable layers:
  army movements, recorded events, Jewish movements, document movements
  (known and hypothetical), document loss (proven loss and hypothetical
  mechanisms), and records that survived.
- Sidebar with the full steps-taken log (16 steps: five completed research
  tracks, two corrections, work in progress, and the open targets).
- Research files under `research/`: comparative towns, military leaders,
  movement records, cross-denomination preservation, Oradea, and the
  Vyzhnytsia vital-statistics access report.
- Reading rule encoded in the data model: recorded / loss-proven / asserted /
  hypothetical are distinct certainty values, rendered distinctly.
