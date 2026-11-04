# Vizhnitz in World War I — Records, Front, and Movements

An interactive research site on what happened to the Jewish community of Wiznitz
(Vyzhnytsia, Bukovina) during World War I, and what happened to its records.

The project exists because of one concrete gap: the Jewish birth register of
Wiznitz for 1897 (and every pre-1918 Wiznitz Jewish register) does not survive
in the catalogues. The surviving books are DAChO (Chernivtsi) Fond 1245-1/933-940,
1918–1930 only. This site organises the research into *why* — front movement,
community fate, leaders' policies, other denominations' preservation, movement
of people and of documents — with every claim dated, cited, and graded.

## The map

Mapbox GL map with toggleable layers:

- War movements of armies (advances, battles, the 30 Jul 1917 Cheremosh front line)
- Recorded events
- Jewish movements (flights, expulsions, hostages, the court in exile, returns)
- Document movements — known (solid) and hypothetical (dashed)
- Document loss — proven loss (red) and hypothetical mechanisms (hollow)
- Records that survived (green counter-examples)

The sidebar on the same page lists every step taken, in order, with its result.

## Reading rule

**Loss is not destruction.** A missing or re-created register proves loss.
“Destroyed” needs its own source (a fire, a unit, a date, an eyewitness, an
inventory). A source that asserts destruction without mechanism evidence is
labelled an assertion. Hypothetical routes and mechanisms are drawn dashed or
hollow, never solid. Inventory labels may misstate contents, so catalogue
absence is not shelf absence.

## Versioning

Tagged semantic releases, same policy as the Lehmann map project:

- PATCH: corrections, wording, small data fixes
- MINOR: new layers, new research tracks folded in, new timeline entries
- MAJOR: breaking data or URL changes

Each release bumps `SITE_VERSION` in `index.html`, updates `CHANGELOG.md` and
`steps.js`, commits, and is tagged `vX.Y.Z`. The site is served by GitHub Pages
from the `main` branch root.

## Layout

- `index.html` — the page (sidebar + map)
- `data.js` — all map layers as GeoJSON, with date, certainty, note, and source per feature
- `steps.js` — the steps-taken log shown in the sidebar
- `research/` — the full research files the map is built from
- `CHANGELOG.md` — release notes per tag

## Mapbox token

The site uses the project owner's existing public Mapbox token, which is
URL-restricted to `mosheberman.github.io`. Public `pk.` tokens are designed to
be embedded in frontend code; the restriction is what protects it.
