# Changelog

## v0.5.0 — 2026-11-04

Selection behaviour (MINOR).

- Selecting a timeline entry now fades every unselected map element to a
  ghost (lines 0.07, points 0.10, labels 0.10, other timeline pins 0.13),
  leaving the selected pin and any related lines at full strength. A line
  counts as related when its period covers the entry's year and it passes
  near the entry's place.
- The camera follows the selection: it zooms to the pin, or fits out to
  show the related line(s) when one exists. Tapping the entry again, or
  closing the popup, restores the full map.

## v0.4.0 — 2026-11-04

Map/timeline integration and the disproof check (MINOR).

- **Tappable timeline**: all 66 timeline rows now carry coordinates. Tapping
  a row flies the map to its pin, rings it, and opens its entry; tapping a
  pin selects and scrolls to the row. On mobile a row tap expands the map.
- **Timeline pins**: one pin per entry, coloured by historical age with a
  high-contrast scale (before 1914 deep violet; 1914 deep red; 1915 burnt
  orange; 1916 dark gold; 1917 deep green; 1918+ deep blue), white-ringed,
  with the year legend in the layers panel.
- **Dates and labels on lines**: every line feature now carries its date and
  name along the line (symbol layer, haloed for contrast).
- **Layers & legend moved onto the map**: an expandable "Layers & legend"
  button at the map's top left holds the layer toggles, the timeline-pin
  toggle, the certainty note, and the year legend. The sidebar keeps the
  reading rules and the steps.
- **Disproof check**: a second reading rule, and annotations on the fire
  features and Hypothesis A: a fire explains a missing register only if it
  explains the survivors (Kotzman births 1902-1907 in Fond 1245-1/941;
  Czernowitz, Sadagora, and Wiznitz's Christian books; the partial court
  fire). New file research/disproof-check.md; steps log now 17 entries.

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
