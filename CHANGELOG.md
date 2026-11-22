# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- First release: 174,406 endpoints from 11,421 services, tested 14–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 162,487 endpoints from 10,738 services, 11,919 fewer endpoints than first published under this snapshot (174,406 from 11,421 services), tested 14–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 160k-environment-apis-for-agents (was 170k-environment-apis-for-agents; first published as environment-api-endpoints). The name follows the count, rounded down.
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
