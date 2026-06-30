# The Rail Automation Paradox
### *Why a robotaxi will drive you across a city while the train still needs a human*

**Author:** Jon (redfoxrun / PostMillennium Renaissance MTB)
**Published at:** [postmillenniumrenaissance.com](https://postmillenniumrenaissance.com)
**File:** `autonomy-paradox.html` — single self-contained HTML file, no build step, no dependencies beyond Google Fonts CDN
**Lines:** ~2,807

---

## What This Is

An interactive data visualization exploring the counterintuitive gap between autonomous car technology and rail automation in the United States — and why the "simpler" problem (trains on fixed rails) has fallen further behind than the "harder" one (cars in chaotic traffic).

Built for two audiences simultaneously:
- **Technical readers** (MTB engineering audience, Pinkbike) who will scrutinize the methodology and want honest confidence tiers
- **Municipal/civic stakeholders** (Castle Rock Town Council, transit advocates) who need accessible, persuasive arguments

The central thesis: the US gap is not a technology limitation. BART was built driverless-capable in 1972. The bottleneck is **Section 13(c)** of the Federal Transit Act — a labor protection clause that makes removing rail jobs from federally funded projects legally very difficult. Automation happens precisely where that clause doesn't apply.

---

## Tabs

### 01 · The Paradox
The core argument. Two verdict panels establish the inversion immediately: ~500k driverless car rides per week (Waymo) vs. ~0% of US trains running without a human. Includes:
- **Automation ladder** — six US train modes (automated guideway, light rail, subway, commuter, Amtrak, Class I freight) plotted on the GoA 0–4 scale with animated bars
- **Today vs. technically possible toggle** — striped "could reach" ghost bars extend each mode to its realistic ceiling, making the deployment gap visible at a glance. The subway bar extending to 100% GoA4 (tech has existed since 1972, barely deployed today) is the key visual argument
- **Expandable mode rows** — tap any mode for the real story: what automation it has, why the human is still there, and a color-coded tag (green = the exception, amber = technical limit, red = legal barrier)
- **Crew-dot tooltips** — hover/tap the ● markers for the specific reason the human's legally required at each point on the ladder
- **Why it's stuck** — Section 13(c) explainer, BART/DC Metro history, and why cars leapt ahead (no labor protection equivalent, no legacy workforce, deep capital)
- **Timeline strip** — 1972 (BART opens driverless-ready), 1985 (Vancouver SkyTrain), 2023 (Honolulu Skyline), 2025 (first crewless freight pilot)

### 02 · What Is GoA?
Plain-language explainer of the international Grades of Automation standard (IEC 62290-1 / UITP).

- **Interactive GoA selector** — buttons GoA 0–4 highlight the matching column in the responsibility matrix and scroll to the matching card below, dimming everything else. Lets a non-expert walk up the ladder and watch the human's jobs hand off to the system one at a time
- **Responsibility matrix** — five rows, five columns. Who owns: setting the train in motion, stopping it, closing doors, handling disruption — and the critical fifth row: *Can the system override a human mistake?* GoA 0 gets a dark crimson "No" (no ATP, nothing intervenes if the driver misses a signal). GoA 1–4 all get green "Yes" — this is the row that visually answers the "GoA 0 and GoA 1 look the same" question
- **Five plain-language cards** — color-graded red (GoA 0) to green (GoA 4), each with the operating mode name (STO / DTO / UTO), a plain description, and a US example

### 03 · USA vs. Canada vs. Switzerland
Three-country scorecard across six transport modes (automated metro/guideway, light rail/tram, urban subway, commuter/regional, intercity, freight).

- **Country selector** — clicking a country button (or the column header) highlights that country's column and dims the others to ~25% opacity
- **Canada as the perfect internal control** — Vancouver SkyTrain GoA4 since 1985 (80+ km, 427k daily rides) vs. Toronto TTC GoA1 throughout, because the Scarborough RT kept operators aboard by labor agreement in 1985. Same country, same decade, opposite outcomes. Clearest proof the constraint is institutional
- **Switzerland's whole-network approach** — SBB smartrail 4.0 targets GoA4 across the entire national network by 2027–2038, including mainline IC. No Section 13(c) equivalent, but facing the genuine engineering challenge of open mixed-traffic mainline track
- **Country deep-dive cards** — three cards with narrative text, flagged stats (80 km, 1985, 2031), and pull quotes

### 04 · By the Numbers
Three chart sections, all interactive.

**Section A — US transit operating cost donut**
Animated donut showing labor at 59% of US transit operating costs (APTA / FTA National Transit Database 2025). The largest slice dominates visually before a word is read. Callout: Paris cut costs 30% converting Metro Line 1 to GoA4; one study estimates 46% savings possible on US systems.

**Section B — Canada's internal divide**
Donut showing the 80/99 km split (SkyTrain GoA4 / TTC GoA1) across Canada's 179 km total rapid transit. The amber/red vs. green split makes the labor-agreement story immediate.

**Section C — 16-country urban metro comparison**
Stacked bar chart (and pie grid) comparing urban metro km by GoA across 16 countries. Urban metro only — no mainline, commuter, or freight — because that's the cleanest apples-to-apples comparison where the technology is proven and only deployment differs.

**View toggle:** ▬ Bars / ◉ Pies — switches between the stacked bar chart (best for seeing total network scale vs. GoA split) and a 16-card pie grid (best for at-a-glance pattern recognition). Both views respect all three sort modes.

**Sort buttons (work in both views):**
- `% GoA 4` — Saudi Arabia and UAE lead (100% GoA4 greenfield builds), USA and Switzerland near the bottom
- `Total km` — China leads at ~10,976 km with a barely-visible green sliver; shows deployment gap at scale
- `Country` — alphabetical for direct lookup

**The 16 countries:** Saudi Arabia, UAE, Qatar, Singapore, Denmark, Australia, Canada, France, Germany, Japan, UK, Spain, USA, Mexico, China, Switzerland

### 05 · US Metro Spotlight
Six expandable system cards showing automation grade and percentage across major US systems, with animated progress bars and three verified facts per system on expansion. Cards auto-collapse when another is opened.

| System | GoA Today | Key fact |
|--------|-----------|----------|
| NYC Subway | ~15% GoA2 (CBTC), ~85% GoA1 | Fixed-block signals from the same era as the 1904 opening still run 85% of the system |
| DC Metro (WMATA) | 100% GoA2 | Built for ATO in the 1970s; ran manual for 15 years after 2009 crash; ATO restored system-wide June 2025 |
| Chicago 'L' | 100% GoA1 | Largest US rapid transit with zero CBTC deployment; no program funded or contracted |
| BART (SF) | ~5% GoA2 live, ~95% GoA1 | Built ATO-capable 1972; $798M Hitachi CBTC contract underway; GoA2 full rollout targets 2030–32 |
| Boston MBTA | PTC 100% (GoA1), subway GoA1 | PTC complete across all 12 commuter rail lines January 2025; no CBTC program |
| PATCO Speedline ★ | 100% GoA2 | **First ATO line ever built in the USA, opened February 1969** — 57+ years of continuous ATO, predates BART by three years |

---

## Theme Switcher

Four named color themes, selectable via pill buttons at the top of every page. GoA chart colors (green/amber/red for GoA4/GoA2/GoA1) never change between themes — they carry semantic meaning that must remain consistent. Only UI chrome (tabs, headlines, active buttons, focus rings, borders) shifts with the theme.

| Theme | Background | Accent | Notes |
|-------|-----------|--------|-------|
| **St Mark's** | Dark steel (default) | Blue `#3a7bd5` | Keeps the "dispatch board" dark aesthetic |
| **St Phil's** | Maroon-tinted dark | Gold `#d4a843` | Warmest and most visually distinct |
| **St Bernard's** | White / light grey | Navy `#1d3a6e` | Full light theme; print-friendly |
| **St Thomas** | Warm off-white | Maroon `#7a1f2b` | Similar to St Bernard's, warmer tone |

Canvas charts (donuts, pie grid) redraw automatically on theme switch so donut holes and center labels match the active panel background color rather than showing as dark holes in a light theme.

---

## Confidence Tiers

Every data point is labeled honestly. This is non-negotiable for the engineering and civic audiences this tool targets.

| Tier | Label | Meaning |
|------|-------|---------|
| ✅ Verified | Green badge | Directly stated in a named, dated source |
| 🟡 Modeled | Amber badge | My characterization of a range, category-level claim, or figure summed from multiple sources — not a single published number |

The distinction matters most in Tab 04 Section C: GoA4 km for deployed systems like Riyadh, Vancouver, Copenhagen, and Sydney are Verified. National totals for countries with many systems (China, Japan, UK, USA) are Modeled from summed line-length data.

---

## Data Sources

### Tab 01 — The Paradox
- Waymo driverless rides/fleet size: thedriverlessdigest.com, cnbc.com (Dec 2025), carboncredits.com
- Honolulu Skyline GoA4: hitachi.com, railwayage.com, masstransitmag.com
- Section 13(c) analysis, BART/WMATA design history: ifp.org — "Close America's Transit Automation Gap"
- Parallel Systems crewless pilot (Georgia): railwayage.com, FRA

### Tab 02 — What Is GoA?
- IEC 62290-1 / UITP grade definitions: railjournal.com, questglobal.com (IEC 62290-1 function allocation), rail-kn.com
- STO/DTO/UTO operating mode names: Wikipedia, en.wikipedia.org/wiki/Automatic_train_operation
- 70+ GoA4 metro lines worldwide, 1920s driverless history: railwaynews.net

### Tab 03 — World Comparison
- SkyTrain (80 km, GoA4, 1985): Wikipedia
- Toronto TTC (99.4 km, GoA1, union opposition): Wikipedia, Toronto Star
- Ontario Line GoA4 (~2031): metrolinx.com, toronto.ca
- Waldenburgerbahn GoA2 (Jan 2026): urban-transport-magazine.com, railwaypro.com
- SBB smartrail 4.0 (GoA4 target 2027–2038): railtech.com
- SBB no plans for driverless mainline: railjournal.com

### Tab 04 — By the Numbers
- US transit labor = 59% of operating costs: APTA via IFP.org analysis of FTA National Transit Database 2025
- Riyadh Metro 176 km GoA4: Gulf News, Guinness World Records 2025
- Dubai Metro+Tram 101 km GoA4: Railway Technology
- Copenhagen Metro 43 km GoA4: Wikipedia
- Sydney Metro 52 km GoA4: Wikipedia, Sydney Metro official
- Singapore NEL/DTL/TEL GoA4, NSL/EWL/CCL GoA2: Wikipedia, SGTrains
- France Lines 1,4,14 GoA4: Paris Metro Wikipedia, railwaypro.com
- Qatar (Doha Metro 76 km GoA4): Wikipedia, Doha Metro official
- Spain (Barcelona L9/L10 GoA4, Madrid Line 6 GoA4 upgrade): Barcelona Metro Wikipedia, railwaypro.com
- Mexico (Lines 1 & 12 CBTC GoA2): railway-technology.com (Dec 2025)
- China (~900 km GoA4 estimate): Shanghai Metro Wikipedia, Railway Gazette China metro report (Mar 2025), Grokipedia urban rail China
- Germany Nuremberg GoA4: Wikipedia

### Tab 05 — US Metro Spotlight
- NYC CBTC status: MTA capital plan documentation, Railway Age
- DC Metro ATO restoration timeline: WMATA press releases Dec 2024 – Jun 2025
- Chicago L Red/Purple modernization: CTA press release Jul 2025
- BART CBTC contract ($798M, Hitachi): BART press release 2020, railwayage.com
- Boston MBTA PTC completion: MBTA press release Jan 2025
- PATCO first ATO line in USA (Jan 1969): DRPA/PATCO official history, Wikipedia

---

## Technical Notes

### Deployment
Single self-contained HTML file. No npm, no build step, no server-side code. All CSS and JavaScript is inline. Google Fonts loads via CDN (`@import` in the stylesheet). Drop the file anywhere — GitHub Pages, a local server, a Pinkbike `[IFRAME]` embed — and it works.

### Interactive features
- **5 tabs** with keyboard arrow navigation and ARIA roles
- **Expandable rows** (accordion) on the ladder and metro spotlight cards
- **Today/possible toggle** on the ladder — ghost bars animate to capability width
- **Crew-dot tooltips** on hover and tap (3.2s auto-dismiss on mobile)
- **GoA selector** on the reference tab (highlights matrix column + scrolls to card)
- **Country selector** on the world comparison tab
- **Sort buttons** (% GoA4 / Total km / Country) — work in both bar and pie view modes
- **Bar ↔ Pie view toggle** on the 16-country chart
- **Theme switcher** (4 named themes with live canvas redraws)
- `prefers-reduced-motion` respected throughout — all animations skip or reduce when the OS setting is active

### CSS architecture
Color system built on CSS custom properties (`--steel`, `--steel-2`, `--accent`, `--accent-dk`, etc.) defined on `:root` and overridden per theme via `html[data-theme="..."]`. Chart-semantic colors (`--green`, `--amber`, `--red` for GoA4/GoA2/GoA1) are intentionally separated from the `--accent` variable so they never change between themes.

### Canvas charts
The three donut pies and the 16-country pie grid draw to `<canvas>` elements using the 2D Canvas API (no charting library). At draw-time, each function reads live CSS custom properties via `getComputedStyle(document.documentElement)` so donut holes, gaps, and center labels always match the active theme's panel background color.

### Data model
The 16-country dataset lives in a plain JavaScript array (`COUNTRIES`) near the top of the script block, making it easy to update without touching the rendering logic:

```js
{flag:'🇨🇦', name:'Canada', g4:80, g23:0, g01:99,
 note:'SkyTrain GoA4; TTC GoA1'}
```

Each entry has `g4` (GoA4 km), `g23` (GoA2/3 km), `g01` (GoA0/1 km), and a `note` string that surfaces as a tooltip on hover.

---

## Scope Boundaries

**What this tool covers:**
- Urban rapid transit (closed, grade-separated metro systems) for international comparisons
- US national rail network for the paradox and mode ladder

**What is intentionally excluded:**
- Mainline rail, commuter rail, freight, and light-rail-in-mixed-traffic from the international comparisons (included in Tab 01 US ladder but not in the cross-country charts, because the comparison would be misleading without consistent scope)
- Airport people-movers excluded from country km totals (included in the US mode ladder as an example of GoA4, but too small and structurally different for cross-country comparison)
- Future/planned systems — the charts show deployed reality today, not announced targets (smartrail 4.0, Ontario Line, Madrid Line 6 upgrades are mentioned in text but not reflected in km figures)

---

## Known Confidence Limitations

**China's GoA4 total (~900 km)** is a 2025 estimate that moves quickly — China opens hundreds of km of new metro annually, some of it GoA4. The figure is grounded in confirmed systems (Shanghai's Lines 10/14/15/18/Pujiang = ~169 km confirmed) but the national total requires estimation across dozens of cities. Treat as directional.

**Japan's GoA breakdown** — Toei Oedo's GoA4 status is confirmed. The ~190 km GoA2 attribution to Tokyo Metro lines is based on ATO being present on all lines, though the GoA2 vs GoA1 classification of some lines is disputed in the literature. The total km are verified; the grade assignments are modeled.

**US GoA2 km (~60 km)** — covers confirmed CBTC lines in NYC (L, 7, Queens Blvd), DC Metro (full system ATO restored 2025), and BART (early CBTC section). Approximate; the DC ATO restoration alone increased this figure significantly in 2025.

**Mexico Lines 1 & 12** — CBTC deployment on Line 1 confirmed December 2025 (Siemens Mobility press release). Line 12 km is an estimate based on reported Alstom Urbalis contract scope.

---

## Changelog

| Version | Changes |
|---------|---------|
| v1.0 | Initial build: paradox tab, US ladder, today/possible toggle, expandable rows, crew-dot tooltips |
| v1.1 | Added GoA reference tab with interactive responsibility matrix and GoA selector |
| v1.2 | Added world comparison tab (USA / Canada / Switzerland) with country selector |
| v1.3 | Added "By the Numbers" tab (pie charts A & B) and US Metro Spotlight tab (6 system cards) |
| v1.4 | Added ATP protection row to responsibility matrix (GoA 0 vs GoA 1 distinction) |
| v1.5 | Added 16-country GoA chart (stacked bars + pie grid, 3 sort modes, bar/pie toggle) |
| v1.6 | Expanded to 16 countries: added Qatar, Spain, Mexico, China |
| v1.7 | Fixed sort-in-pie-mode bug (sort buttons now work in both bar and pie views) |
| v1.8 | Added 4-theme color switcher (St Mark's, St Phil's, St Bernard's, St Thomas) with full CSS variable architecture and live canvas redraws |

---

*Built by redfoxrun / PostMillennium Renaissance · Castle Rock, CO · 2026*
*"There are no solutions, only tradeoffs." — Thomas Sowell*
