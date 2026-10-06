# Solar Homes in Africa — prototype website

This is a dependency-free static site intended to be easy to host on Dock80_70/OpenWrt later.

## Local Windows location
Copy this whole folder to:

`C:\dl\micromite\_picomite\_claco\chat\SolarHomeInAfrica`

Open `index.html` directly in a browser for a quick preview, or run a local web server from that directory:

```powershell
python -m http.server 8000
```

Then visit `http://localhost:8000/`.

## Future Dock80_70 deployment
No framework or build step is required. Copy `index.html`, `styles.css`, `script.js`, and `assets/` into the chosen web root on Dock80_70. The exact deployment command should be decided after the COM4 serial connection is attached and the existing web-server layout is inspected.

## Codex continuation prompt
Use this when Codex has access to the Windows project directory:

> Work only in `C:\dl\micromite\_picomite\_claco\chat\SolarHomeInAfrica`.
> This is an early-stage static website for the Solar Homes in Africa household-solar project. Preserve its dependency-free static architecture: plain HTML, CSS, minimal JavaScript, and local images. It will eventually be hosted on a small OpenWrt Dockstar, so do not add Node, React, build systems, CDNs, web fonts, analytics, trackers, databases, or server-side dependencies unless explicitly requested.
>
> Before making changes, read `README.md`, `index.html`, `styles.css`, and `script.js`. Preserve the current visual language unless asked to redesign it. Keep the site responsive and accessible. Treat prices, rollout numbers, PAYGo terms, hardware cost and performance as working project targets, not established commercial claims. The site must continue to state clearly that it documents prototype development and is not presently a product offer, investment solicitation or donation campaign.
>
> When new prototype photos or test results are supplied, add them to `assets/img/` with concise filenames, optimize large images for the web without destroying schematic readability, and update the corresponding status text. Do not invent test results.
>
> If asked to deploy to Dock80_70 later, first inspect the actual OpenWrt web root and current server configuration over the user's provided serial/SSH connection. Do not overwrite existing unrelated files. Make a backup before replacing any existing site files.

## First-pass content choices
The current page contains:
- project concept and engineering principles;
- long-range 200M / 50M / 12.5M household objectives;
- USB prototype and phone-charging result;
- solar-emulator PCB, schematic, and measured cloud profiles;
- working PAYGo idea: US$10 down + US$3/month for 24 months;
- possible household add-ons;
- explicit separation between demonstrated results and open questions.

This is deliberately an early public notebook-style site. Expect many iterations.


## v1.1
Added an inline explanation of the World Bank/ESMAP electricity-access tiers, with the project's Tier 2 / Tier 3 / Tier 5 shorthand benchmarks and a source link.

## v1.2
Added the Solar Distributor V1 3D rendering and prototype-fabrication status. Added a sourced note on the 2019 GOGLA/Altai Consulting East Africa follow-up study: 28% of households reported additional income after about 15 months, averaging US$46/month among those reporting added income.


## v1.3
Added top and bottom bare-board fabrication views of Solar Distributor V1 beneath the assembled 3D rendering.


## v1.4 update
Added a sliced appliance-example gallery to the Add-ons section using the supplied reference collage.


## v1.5 update
Sharpened the GOGLA income-evidence section to distinguish early-adopter phone-charging income from effects that can persist as access becomes widespread. Added `cubaverter.html` and `lagosverter.html` as same-style design-study documentation pages, plus links from the main page.


## v1.6 update
Removed the Related system studies section and all CubaVerter/LagosVerter links from the main project page. The two standalone documentation pages remain in the package and retain their cross-links for direct use.

## v1.7 update
Kept “48 V” together on one line in the CubaVerter title at responsive widths.

## v1.8 update
Clarified the main project's physical charging-hub model: no fixed house wiring is required, one PV lead-in feeds a central distributor above a simple charging shelf, and portable rechargeable appliances move around the home. Added a compact system-flow diagram, documented the intended nominal-12 V ~100 W panel source, described replaceable connector-saver pigtails as a field-use concept, strengthened the emulator explanation around cloud-induced voltage collapse and recovery, and reorganized add-ons into portable-storage and daytime-direct loads. Continuous output ratings remain explicitly subject to prototype testing.

## v1.9–v1.10 updates
Added low-key reference-table pages and links near the bottom of the main page. Broadened the appliance gallery's phone/accessory card to show a phone, portable power bank and 12 V immersion heater together.

## v1.11 update
Added project-context upgrade studies for Tier 3 and Tier 5. The main page links to them immediately above the smaller Reference tables line. Tier 3 documents an additive 400–800 W+ PV step with roughly 1.3–2.6 kWh of optional shared storage; Tier 5 distinguishes the bare 2 kW threshold from a more practical ~2.4 kWp starting array and uses the project's 48 V, 5/10/15 kWh storage ladder. Existing CubaVerter and LagosVerter pages remain unlinked from the main project page.


## v1.12 update
Reframed the working additive upgrade path around a 150 W entry-panel target: Stage 1 is 150 W with no central battery; Stage 2 adds a second identical 150 W panel in parallel (1S2P) for a 300 W batteryless system; Stage 3 rewires the same pair in series (2S1P), adds a low-cost 24 V solar charger and a 25.6 V / 50 Ah LiFePO4 battery, and introduces efficient DC refrigeration as a major next service after lighting and air movement. The main page now highlights this path and the Tier-3 study has been rewritten around it. Current ~100 W-class hardware remains useful for prototype qualification while the deployment target is evaluated.
