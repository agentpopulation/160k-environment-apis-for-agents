## Environment API endpoints, snapshot 15 Nov 2026

- 162,487 endpoints passed a keyless data call, tested 14–15 Nov 2026 (IST)
- 10,738 services · 251 country codes · 105,803 keyless JSON rows

### Download

- `Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 162,487 rows, 7.7 MB gzipped (50.1 MB as CSV), SHA-256 `8e264ff317dd7f00c30c708b97f323464443db4188cbe17128626e9b249752a5`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 29,986 · Wrap one URL pattern as a get_species_records tool: pass a country code and a group, return species names, dates and coordinates; page with offset for more.
- 📱 App features: 4,532 · Draw protected areas, habitats, tree cover, noise zones, contaminated sites or waste points as a map layer, and show the nearest one on a card.
- 🧠 Grounding and data pipelines: 13,026 · Load emissions, waste, forest and radiation series on a schedule into your own store, so answers about the environment cite a dated source.
- 🧪 Evals and testing: 162,487 · Run your environment tool against a fixed set of URLs across formats; check that species, pollutant, value, unit and date parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 174,406 endpoints from 11,421 services, tested 14–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 162,487 endpoints from 10,738 services, 11,919 fewer endpoints than first published under this snapshot (174,406 from 11,421 services), tested 14–15 Nov 2026 (IST).
- Left out: 962 rows whose URL carried a credential-looking parameter or a login.
- Left out: 8 rows with an email-like address.
- Left out: 2,498 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 21 ArcGIS proxy layers (utility.arcgis.com/usrsvcs and portal /sharing/servers/ addresses) that can call a service with a stored login.
- Left out: 24 layers marked editable in the title (they can hold entries that people added).
- Left out: 338 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 2 rows that passed a data call only from a network location in India.
- Left out: 6 rows whose address or title held a token-like string, a private address or a similar string.
- Left out: 891 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 154 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 38 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 2 rows that are another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 170 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 2,746 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 544 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 7,987 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 196 rows that repeat an address already in the pack.
- Overlap: 12,567 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 502 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 4,630 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 1,432 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 568 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 195 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 2 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 4,185 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 1 of these URLs is also in 22k-maritime-apis-for-agents.
- Overlap: 11,535 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 231 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 105,430 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 5 of these URLs are also in 84k-health-apis-for-agents.
- Overlap: 8 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 5 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 40 of these URLs are also in 4.9k-wildfire-apis-for-agents.
- Overlap: 9 of these URLs are also in 67k-energy-apis-for-agents.
- Overlap: 13 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 2 of these URLs are also in 10k-parking-apis-for-agents.
- Overlap: 37 of these URLs are also in 7.8k-earthquake-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 14–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Environment API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
