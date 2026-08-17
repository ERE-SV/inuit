# Brainstorming: Neue Geschäftsidee — Jobbörse / zweiseitiger Marktplatz

> **Lebendes Dokument** — organisch gewachsen aus mehreren Gesprächen. Ziel: alle Gedanken an einem Ort bündeln, ohne Kontext zu verlieren.

---

## Inhaltsverzeichnis

1. [Kernidee](#1-kernidee)
2. [Marktstruktur](#2-marktstruktur)
3. [Problem & Pain](#3-problem--pain)
4. [Zielgruppe](#4-zielgruppe)
5. [Lösung & Produkt](#5-lösung--produkt)
6. [Markt & Wettbewerb](#6-markt--wettbewerb)
7. [Geschäftsmodell](#7-geschäftsmodell)
8. [Go-to-Market](#8-go-to-market)
9. [Team, Skills & Machbarkeit](#9-team-skills--machbarkeit)
10. [Risiken, Annahmen & offene Fragen](#10-risiken-annahmen--offene-fragen)
11. [Technische Architektur](#11-technische-architektur)
12. [Nächste Schritte](#12-nächste-schritte)
13. [Chronik](#13-chronik)

---

## 1. Kernidee

**Zweiseitiger Marktplatz**, auf dem **Stellensuchende** und **Unternehmen** zusammentreffen — beide mit **mehreren parallelen Opportunitäten**. Zentrales Element: ein **bidirektionales Matching**, das strukturierte Präferenzen und harte Fakten beider Seiten gegenüberstellt.

**Was die Plattform bietet:**

- **Bewerbende:** ein einziges, wiederverwendbares, strukturiertes Profil statt wiederkehrender Bewerbungsmappen; die Plattform übernimmt den administrativen Bewerbungsaufwand soweit möglich.
- **Unternehmen:** das ist phase 2 ein strukturiertes Anforderungsprofil pro Stelle statt kanalweise neu formulierter Inserate, zu beginn crawlen wir nur die career websieten der unternehmen); Das ist kernidee HR sieht deutlich weniger, aber deutlich bessere Kandidaten.
- **Matching-Ausgabe:** Top-X-Vorschläge beidseitig — als **Indikator** für Passung, nicht als Einstellungsgarantie.

**Note Das ist Phase 2: Ergänzender Mehrwert:** Aus den aggregierten Stellenanforderungen der Plattform lässt sich ein **Karriere-Gap-Modul** ableiten, das Nutzern zeigt, welche Qualifikationen für eine Zielrolle typischerweise noch fehlen. Das fördert **Retention** — Nutzer bleiben auch zwischen Bewerbungsphasen aktiv.

---

## 2. Marktstruktur


| Seite               | Charakteristik                                                                             |
| ------------------- | ------------------------------------------------------------------------------------------ |
| **Stellensuchende** | Haben **mehrere** Stellen gleichzeitig im Blick — nicht „eine Bewerbung, ein Arbeitgeber". |
| **Unternehmen**     | Haben **mehrere** Vakanzen parallel — nicht „ein Inserat, ein Kandidat".                   |


**Gemeinsames Muster:** Beide Seiten operieren **multi-opportunity**. Der Markt skaliert nur, wenn **Liquidität** (genug passende Treffer) und **Vertrauen** (fairer, nachvollziehbarer Prozess) stimmen.

---

## 3. Problem & Pain

### 3.1 Stellensuchende

- **Hoher Administrationsaufwand** durch viele parallele Bewerbungen.
- **Schwierige Identifikation** passender Unternehmen: Präferenzen wie Standort/Erreichbarkeit, Unternehmensgrösse, Vergütung, Arbeitsmodell oder Kultur müssen bei jedem Arbeitgeber einzeln abgefragt werden.
  - *Beispiel:* Arbeit in Zürich, Tram 6 ~10 Minuten, >50 Mitarbeitende, >80'000 CHF — solche kombinierten Constraints sind auf klassischen Portalen kaum filterbar.
- **Fehlende Gesamtübersicht** über alle laufenden Bewerbungen und Fortschritte.

### 3.2 Unternehmen / HR

**Inserate & Reichweite:**

- Das lösen wir erst in phase 2, da wir zu beginn nur die webseiten der unternehmen crawlen um jobinserate zu finden, Multi-Channel-Inserate auf jobs.ch, LinkedIn etc. — **hohe Gesamtkosten**, Doppelarbeit, Inkonsistenz-Risiko.
- Das lösen wir erst in phase 2, da wir zu beginn nur die webseiten der unternehmen crawlen um jobinserate zu findenAufwändige Erstellung und Pflege über mehrere Plattformen.

**Bewerbungsflut & Screening:**

- HR wird mit **zu vielen** Bewerbungen überflutet, davon ein Grossteil ohne passende Kriterien aus verschiedenen quellen.
- Selektionsprozess ist **arbeitsintensiv** und birgt Reputationsrisiko (Kununu, Glassdoor).
- Subjektive Faktoren oft stärker gewichtet als objektive Kompetenz.

**Organisatorische Last:**

- Weiterleitung an Fachabteilungen, Interview-Koordination, Phasen-Tracking, Absagen, Zusagen, Inserate-Pflege — alles bindet Kapazität, die für individuelle Bewerberbetreuung fehlt.

### 3.3 Markt / Branche (Meta)

- Klassische Jobportale: sehr hohe Preise.
- HR-Abteilungen teils überdimensioniert — bedingt durch Eingangsflut und manuelle Screening-Last, dieses screening ist lückenhaft, nicht strukturiert und rational.

### 3.4 Asymmetrische Präferenzen und Informationslücken

Bewerber- und Arbeitgeber-Präferenzen laufen **nicht** immer über dieselben Dimensionen:

- *Beispiel:* Der Bewerber will die maximale Pendelzeit kennen. Das Unternehmen hat kein „Pendel-Feld" — trotzdem braucht das System Arbeitsort + ÖV-Daten + Wohnort des Bewerbers für diese Prüfung.
- Sensible Arbeitgeberdaten (Kultur, Lohnbänder, Teamdetails) werden oft nicht oder nur teilweise publiziert — das Matching benötigt **Anreicherung** aus Drittquellen für die fakten.

### 3.5 Zwei parallele Informationsräume ohne systematischen Abgleich

- **Bewerbende** investieren in Lebensläufe, Zeugnisse, Motivationsschreiben.
- **Unternehmen** investieren in Employer Branding, Career-Webseiten, ausführliche Jobbeschreibungen.
- **Lücke:** Diese Informationsräume werden selten automatisiert und strukturiert gegeneinandergelegt — stattdessen übernimmt HR den Abgleich in mühseliger Handarbeit.

---

## 4. Zielgruppe

- **Status:** noch nicht abschliessend festgelegt. Branchen oder Jobfamilien dienen als Arbeitshypothesen bis zur Klärung.
- **Primär B2B2C / Marketplace:** Arbeitgebende (HR, Hiring Manager, SMB bis Enterprise) und aktiv suchende Fach- und Bürokräfte.
- **Käufer:** typischerweise Unternehmen (Budget für Recruiting); Stellensuchende oft ohne direkte Zahlung.
- **Erreichbarkeit:** noch offen (LinkedIn/XING, Fachcommunities, HR-Netzwerke, Hochschulen, Branchenverbände).

---

## 5. Lösung & Produkt

### 5.0 Scope-Abgrenzung

**Was die Plattform bewusst nicht ist:**

- Kein vollständiger ATS-Ersatz: keine Fachbereichs-Freigaben, kein Interview-Scheduling, kein internes Phasen-Tracking — das bleibt im bestehenden Stack (ATS, HRIS, Kalender, E-Mail).

**Kern Arbeitgeberseite:**
HR sieht **deutlich weniger** Bewerbungen, dafür **nur vorausqualifizierte** Kandidaten (Top-X, Matching-Schwellwerte).

**Kern Bewerberseite (bewusst breiter):**

- Ein einziges Profil + Suchkriterien; die Plattform übernimmt die administrative Organisation: Matching, Top-X-Stellen, Profilwiederverwendung, Übersicht, Benachrichtigungen.
- Terminvergabe, Zusagen und Fachbeurteilung bleiben beim Arbeitgeber.
- Eine kandidatenseitige Pipeline-Ansicht (eigene Bewerbungen / Status) gehört zur Vision; sie ist kein Arbeitgeber-ATS.

### 5.1 Kernmechanik: Bidirektionales Präferenz-Matching

Die Plattform speichert und strukturiert Präferenzen auf **beiden Seiten**:


| Seite                     | Beispiele                                                                                        |
| ------------------------- | ------------------------------------------------------------------------------------------------ |
| **Bewerbende**            | Maximale Pendelzeit, ÖV-Qualität, Firmengrösse, Gehaltsuntergrenze, Arbeitsmodell, Kulturwünsche |
| **Unternehmen / Stellen** | Qualifikationen, Erfahrungslevel, Sprachen, Ausbildungsniveau, Zertifikate                       |


**Asymmetrie im Modell:** Nicht jede Bewerber-Präferenz hat ein Gegenstück beim Arbeitgeber. Das Matching ist daher oft **Constraint-Erfüllung**:

- *„Erfüllt diese Stelle die Wünsche des Bewerbers?"* — unter Nutzung von Stellen-Fakten + Anreicherung.
- *„Erfüllt dieser Bewerber die Anforderungen der Stelle?"* — direkte Gegenüberstellung der Profile.

Wo Kategorien paarig sind (z. B. Sprachniveau, Remote-Anteil), kann echte **Überdeckung** modelliert werden. Hohe Kompatibilität ist ein **Indikator**, kein Einstellungsversprechen.

### 5.2 Datenquellen und Anreicherung

**Ziel:** Bewerber-Präferenzen möglichst gut abdecken, auch wenn Arbeitgeber nicht alles liefern — ohne Vertrauen und rechtliche Sauberkeit zu verlieren.

#### Quellen-Mix (je nach Machbarkeit)


| Thema                         | Mögliche Quellen                                                              | Vorsicht                                       |
| ----------------------------- | ----------------------------------------------------------------------------- | ---------------------------------------------- |
| **Arbeitsort / Standort**     | Arbeitgeber-Pflichtfelder, Google Maps (Geocoding), Handelsregister           | Genauigkeit bei Mehrstandorten                 |
| **Pendel / ÖV**               | Google Maps (Directions/Distance Matrix), CH-ÖV-Daten (opendata.swiss)        | Kosten pro Request; DSG                        |
| **Gehalt / Benchmarks**       | Kununu, Glassdoor, Indeed (Bandbreiten), BFS/Branchenlohnstudien              | Vertragspflicht; keine falschen Einzelgehälter |
| **Kultur / Arbeitgeberimage** | Kununu (nur über erlaubte Schnittstelle), ähnliche Portale                    | Aggregat vs. Einzelfall                        |
| **Stellenanforderungen**      | Jobbörsen-APIs/-Feeds (Phase 1), Erstpartei-Suchprofile Arbeitgeber (Phase 2) | Extraktionsunsicherheit aus Freitext           |


**Strategie — Quellen-Matrix:** Welche Bewerber-Frage → welche Daten → welche Quelle rechtlich nutzbar → Fallback wenn fehlend? Pareto: häufigste Constraints zuerst anbinden.

**Privacy:** Wohnort des Bewerbers nur so nutzen, wie DSG/nDSG und Consent erlauben; Matching läuft serverseitig — Arbeitgeber sieht nicht zwingend den Wohnort.

#### Phasenmodell


| Phase                                                | Datenbasis                                                         | Implikation                                                |
| ---------------------------------------------------- | ------------------------------------------------------------------ | ---------------------------------------------------------- |
| **Phase 1** — keine Erstpartei-Suchprofile vorhanden | Inferenz aus Jobbörsen-Feeds/APIs; LLM-Extraktion aus Inseratstext | Konfidenz tiefer; Quelle im UI transparent machen          |
| **Phase 2** — Unternehmen ongeboardet                | Primärdaten direkt auf der Plattform                               | Höhere Präzision; Phase-1-Daten als Backfill / Validierung |


#### Stellenmarkt-Daten: API-first (bevorzugter Pfad)

**Problem mit Crawling:** Einzelne Corporate-Career-Sites dauerhaft zu crawlen ist sehr aufwändig und engineering-intensiv.

**Strategie:** Anbindung an ~3 grosse Inserate-/Stellenanbieter über offizielle APIs oder lizenzierte Feeds. Fokus Engineering auf Normalisierung, Deduplizierung, Quota-Management — nicht auf n× fragile HTML-Parser.

*Zahl „3" ist Arbeitshypothese — welche Anbieter im CH-Markt realistisch, vertraglich zulässig und preislich tragbar sind, muss noch recherchiert werden.*

#### Career-Webseiten-Crawling — optional, nur als Lückenfüller

Nur ergänzend, wo APIs lückenhaft sind — gezielte Allowlist, kleine Fläche, nicht als Skalierungsstrategie. Rechtliche Risiken (AGB, robots.txt, Arbeitgeberbeziehung) vor Ausweitung prüfen.

#### Crawl-/Ingestion-Architektur und Betrieb

Als eigenes Subsystem geplant. Kernbausteine:

1. **Bestand & Discovery** — Arbeitgeber-Registry, Karriere-URLs, ATS-Templates (Workday, Greenhouse, Custom HTML).
2. **Planung & Frequenz** — Priorisierung (heiss/warm/cold), Change-Detection (ETags, Hash), SLAs pro Tier.
3. **Fetch-Schicht** — Polite Fetching, Rate Limits, Backoff, Captcha-Erkennung → Escalation.
4. **Extraktion & Normalisierung** — Versionierte Template-Adapter, Schema-Mapping; LLM-Nutzung mit Guardrails, Confidence, Human-in-the-loop.
5. **Datenhaltung & Lineage** — Canonical URL, fetchZeit, parserVersion, Rohhash; Retention-Regeln.
6. **Qualitätssicherung** — Extraktionsrate, Feld-Vollständigkeit, Drift-Monitoring, Regression bei Relaunch.
7. **Compliance-by-Design** — Allowlists, Opt-out-Flags, robots.txt, Staging→Review→Publish.
8. **Observability** — Dashboards (Crawl-Erfolg, Latenz, Queue, Fehlerklassen, Kosten), Runbooks.
9. **Organisation** — klare Ownership „Ingestion" vs. „Domain-Experts"; On-Call für Parser-Updates.

**Noch zu entscheiden:** Feed-/API-Anbieter (Priorität, Redundanz); Eigenbau vs. externe Hilfe; Cloud-Region CH/EU; Push-Feed vs. Polling.

### 5.3 Strukturiertes Profil, Filter-Stelle, Top-X

**Vision Bewerberseite:**

- Qualifikationen, Eigenschaften und Präferenzen werden **mühelos und strukturiert** erfasst (geführtes Onboarding, gezielte Felder, Nachweise nur wo nötig).
- **Ein Profil** für alle Arbeitgeber — keine wiederholten Unterlagenpakete, kein Motivationsschreiben pro Stelle.
- *(Akzeptanz in verschiedenen Branchen/Regionen validieren)*

**Vision Arbeitgeberseite:**

- Statt langer Marketingtexte: präzise **Filterkriterien / strukturiertes Anforderungsprofil**; Storytelling optional ergänzend.

**Matching-Ausgabe:**

- Top-X-Stellen für Bewerbende; Top-X-Kandidaten für Arbeitgeber — beidseitig mit Kurzbegründung (welche Kriterien trafen / fehlten).
- Ein Profil über viele Arbeitgeber; einmal Kriterien statt per-Portal neu formulierte Inserate.

### 5.4 Karriere-Gap-Analyse („Karriereberatung light") & Retention

**Grundidee:** Aus dem aggregierten Bestand an Stellenanforderungen entsteht ein **Marktbild**, welche Qualifikationen für bestimmte Zielrollen typischerweise gefragt werden. Nutzer können ihr Profil gegen eine Zielrolle vergleichen lassen.

**Nutzer-Story:** Junior Consultant → Senior Consultant. Das System vergleicht das Profil mit aggregierten Anforderungsprofilen der Zielrolle und liefert eine **Lückenliste**: z. B. Master Wirtschaftswissenschaften, +2 Jahre Erfahrung, Zertifikat X, Englisch Niveau C1 — mit Priorität (Must-have vs. häufig) und Quelle.

**Wert:**

- Karriere-Radar / Selbstcoaching ohne klassische Einzelberatung.
- **Retention nach Jobwechsel:** Nutzer kommen zurück, um sich für den nächsten Wechsel vorzubereiten.

**Vorsicht:**

- Kommunikation vorsichtig: „basierend auf X Stellen bei uns", nicht als absolute Marktwahrheit.
- Tipps primär als Kohorten-Norm (Mindest-Stichprobe, Anonymisierung), nicht firmenspezifisch für alle sichtbar.
- Kein Ersatz für individuelle Beratung; Disclaimer je nach Tiefe der Tipps.

### 5.5 0-Match-Diagnose & What-if-Vorschläge

**Problem:** Zu enge oder kombinierte Kriterien → 0 Treffer oder nur schwache Matches.

**Produktidee:** Das System analysiert die bindenden Filter und schlägt **minimal-invasive Anpassungen** vor — am Profil (qualifizierbar: Zertifikat, Sprache) oder an den Suchkriterien (Gehaltsuntergrenze, Radius, Remote, Branche).

**Erklärung für Nutzer:** „Wenn du Constraint A lockerst, gewinnst du Z zusätzliche passende Stellen."

**Beispiel:** >100'000 CHF und max. 15 km um Chur → kaum Stellen → Vorschläge: Gehaltsuntergrenze senken, Radius erweitern, oder Arbeitsmarkt wechseln (z. B. Zürich ist ein anderer Markt, nicht innerhalb 15 km von Chur — im UI klar trennen).

**UX / Ethik:** Vorschläge wie Umzug oder Lohnverzicht sensibel und neutral formulieren; Nutzerentscheid, keine Wertung.

---

## 6. Markt & Wettbewerb

**Direkte Konkurrenz:**

- CH-Kontext: jobs.ch (explizit), LinkedIn Jobs, StepStone, Indeed, regionale Börsen, Fachportale.

**Indirekte Konkurrenz:**

- Headhunter, interne Empfehlungen, Active Sourcing, Karrierecoaches, Weiterbildungsanbieter, Skill-Assessment-Plattformen.

**Relevante Trends:**

- Arbeitnehmerbewertungen (Kununu, Glassdoor), DSGVO/nDSG, Gleichstellungsdiskussion bei Auswahlverfahren, KI in Recruiting (Chancen + Regulierung / Bias-Risiko).

**USP-Richtung (Entwurf):**
Strukturierter Abgleich statt zwei unvernetzter Informationsräume; Matching trotz asymmetrischer Kategorien mit Stellen-Fakten + kontrollierter Datenanreicherung; bidirektionale Kompatibilität und Top-X-Vorschläge; ein Profil, viele Arbeitgeber; Karriere-Radar aus Marktanforderungen; What-if-Vorschläge bei leerem Ergebnis. — *Exakte Differenzierung gegenüber jobs.ch, LinkedIn etc. noch ausarbeiten.*

---

## 7. Geschäftsmodell

- **Ausgangspunkt:** Kritik an hohen Preisen bestehender Anbieter → eigene Logik muss nachvollziehbar günstiger oder wertbezogener sein (z. B. Erfolgsfee, Pay-per-qualified-lead, Abo mit Caps).
- **Offen:** Zahlen nur Arbeitgeber, oder auch Premium für Kandidaten? Freemium-Modell?
- **Kostenblöcke:** Matching-Qualität, Support, Compliance, Marketing für zweiseitige Liquidität; API-/Feed-Gebühren, Volumen-Limits, Integrationspflege.
- **Retention / LTV:** Karriere-Gap und Profil-Pflege zwischen Jobs senken Reakquise-Kosten und erhöhen Datenqualität. Optional: Premium für tiefe Pfad-Analysen, Kursempfehlungen (Partner).

---

## 8. Go-to-Market

*(Noch nicht im Detail besprochen.)*

- Typische Hebel: Nische (Branche/Region/Rolle) zuerst, Liquidität in einem Segment aufbauen, dann erweitern.
- Content: Transparenz, „weniger Noise", faire Prozesse — vorsichtig formulieren, damit es nicht wie unbelegtes HR-Bashing wirkt.

---

## 9. Team, Skills & Machbarkeit

*(Noch offen.)*

Benötigte Kompetenzfelder: Tech (Backend, ML/Matching, Voice/AI), HR-Domain-Know-how, Legal/Compliance, Sales/BD.

Bei Daten-Ingestion zusätzlich: API-/Feed-Integration, Vertrags- und Quota-Management, Web-Compliance, NLP-/Parser-Qualität, DevOps.

---

## 10. Risiken, Annahmen & offene Fragen

### Kernrisiken


| Annahme / Risiko                                               | Wie testen / absichern?                                       |
| -------------------------------------------------------------- | ------------------------------------------------------------- |
| Arbeitgeber zahlen, wenn Kandidaten kostenlos parallel suchen  | Pricing-Interviews, Pilot mit messbarem Zeitgewinn            |
| „Weniger, aber bessere Bewerbungen" erfordert starkes Matching | Metriken: Qualification-Rate, Time-to-hire, Offer-Accept-Rate |
| Fairness / Bias durch Algorithmen oder Kriterien               | Legal Review, Erklärbarkeit, ggf. Human-in-the-loop           |
| Chicken-and-Egg: ohne Jobs keine Kandidaten und umgekehrt      | Start mit klarer Nische oder einem „Anker"-Partner            |
| Match-Score wird als Garantie missverstanden                   | UX-Copy, Erklärbarkeit, menschliche Bestätigung vor Kontakt   |


### Daten & Matching


| Risiko                                                                        | Massnahme                                                                       |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Standort/ÖV-Daten unvollständig oder veraltet                                 | Routing-APIs, Arbeitgeber-Verifikation, konservative Schätzungen                |
| Gehalt/Firmengrösse als Filter: rechtliche oder wahrgenommene Diskriminierung | Legal-Review CH; freiwillige Angaben; keine verbotenen Kriterien automatisieren |
| Anreicherung aus Drittquellen falsch oder veraltet                            | Quellenangabe im UI, Feedback-Loop, Arbeitgeber-Korrekturworkflow               |
| Arbeitgeber fühlen sich durch inferierte Signale „gestellt"                   | Opt-in, nur aggregierte/neutrale Signale, keine behaupteten Einzelgehälter      |
| Phase-1-Inferenz wirkt wie garantierte HR-Wahrheit                            | UI: „aus Inserat abgeleitet"; Übergewicht auf Primärdaten nach Onboarding       |
| API-/Feed-Anbieter: Preiserhöhung, Limit-Kürzung                              | Mehrquellen-Strategie, Exit-Plan, Budget-Puffer                                 |
| Parser-Rot (Relaunch der Website) bricht Extraktion still                     | Monitoring + Regression, Canary-Crawls, schnelle Hotfix-Ownership               |
| Arbeitgeber fühlen sich durch Crawl ausspioniert                              | Opt-out/Claim-Flow, Mehrwert kommunizieren                                      |


### Produkt & UX


| Risiko                                                                    | Massnahme                                                                       |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Struktur ersetzt Freitext — Verlust von Nuancen und Motivation            | Optionale Kurztexte; erklärbare Scores; später ggf. KI-Entwurf aus Profil       |
| Erwartung Motivationsschreiben / klassischer Bewerbungsprozess (CH)       | Pilotsegment wählen; Arbeitgeber-Settings „Freitext erforderlich ja/nein"       |
| Top-X schliesst gute Kandidaten aus oder begünstigt Gaming des Scores     | Transparenzregeln, Bandbreite zeigen, Human Override                            |
| Karriere-Tipps wirken wie Zusage trotz lückenhafter Daten                 | Stichprobe anzeigen, Unsicherheit kommunizieren                                 |
| What-if-Vorschläge (Umzug, Lohnverzicht) wirken paternalistisch           | Nutzerführung: freundlich, optional, „du entscheidest"                          |
| HR erwartet nach dem Match weiterhin ATS-/Kalender-Features               | Klar kommunizieren: Pre-ATS-Filter; schlanke Exporte                            |
| Bonitäts-/Kredit-Daten im Matching                                        | Nur mit Legal und klarer Zweckbindung; sonst weglassen                          |
| Reverse Engineering von Hiring Bars durch zu detaillierte Firmen-Insights | Nur Kohorten-/Marktansicht; firmenspezifisch nur im legitimen Bewerbungskontext |
| Karriere-Beratungs-Haftung / regulierte Berufe                            | Klare Disclaimer, Tiefe des Rats abgrenzen, ggf. Kooperation mit Coaches        |


### Offene Produktfragen

- **Erster Beachhead:** welche Branche, Region, Jobfamilie?
- **Regulatorik:** Schweiz/DACH — arbeitsrechtliche Aspekte von Auswahl und Dokumentation?
- **Commute-Modellierung:** Tiefe (Tramlinie vs. Minuten-Isochrone)? Welche Datenquellen (OpenData vs. kommerziell)?
- **Weiche Präferenzen** (Kultur, Teamgrösse): modellierbar oder bewusst ausserhalb der Automatik?
- **Drittquellen:** welche sind rechtlich und wirtschaftlich lizenzierbar? Wer haftet bei fehlerhaften Matches?
- **Unsicherheitskommunikation:** „geschätzt" / „Selbstauskunft" / „Marktbenchmark" im UI ohne Überforderung?
- **Profil-Sichtbarkeit:** Einwilligung pro Arbeitgeber, Sichtbarkeitsstufen, Zeugnisse nur auf Anforderung?
- **Gap-Analyse:** Mindest-N pro Kohorte, Zielrollen-Taxonomie (eigene Tags vs. ESCO/O*NET), welche Aggregation (offen vs. inkl. archivierte Stellen)?
- **What-if / Relaxation:** welche Constraints dürfen gelockert werden, wie viele Szenarien gleichzeitig?
- **Geo-What-if:** alternative Ballungsräume namentlich oder nur abstrakt vorschlagen?
- **Top-X & Ranking:** Was ist X (fix, adaptiv)? Erklärbarkeit, Gleichstand, Fairness?
- **Feed-/API-Anbieter:** welche 1–3 Anbieter für CH realistisch (Vertrag, Kosten, Felder, Aktualität)? Dedupe zwischen Quellen?
- **Crawling-Restfläche:** für welche Lücken, mit welcher Maximalfläche, wie Rechtsfreigabe dokumentieren?
- **ATS-Integration:** reicht Export (PDF/CSV/API) der Top-X-Profile in bestehende ATS — welche Integrationen für Beachhead nötig?

---

## 11. Technische Architektur

### 11.1 Zwei Rollen und ihre Datenobjekte


| Rolle           | Aufgabe auf der Plattform                                                                                                                | Datenobjekte                                                                                |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| **Unternehmen** | Stellen bekannt machen und als **strukturiertes Anforderungsprofil** definieren — nicht nur als Marketingtext, sondern als Match-Filter. | **Suchprofil(e)** pro Stelle oder Talent-Pipeline                                           |
| **Bewerbende**  | **Einmalig** Profil und Suchkriterien mitteilen, damit das System gegen Unternehmens-Suchprofile matchen kann.                           | **Bewerberprofil** (Qualifikationen, Nachweise) + **Suchprofil** (Präferenzen, Constraints) |


**Naming-Logik:** „Suchprofil" passt auf beiden Seiten — Unternehmen sucht Personen, Bewerbende suchen Opportunitäten.

**Matching:** Bewerber-Suchprofil ↔ Stellen-Anforderungen + Arbeitgeber-Suchprofil ↔ Bewerberprofil. Constraint-Erfüllung + Überdeckung wo Kategorien paarig sind.

### 11.2 Problem: Viele Felder, wenig Lust auf Formulare

Bewerbende sollen reichhaltige Angaben machen — Berufserfahrung, Skills, Sprachen, Verfügbarkeit, Gehaltsvorstellung, Mobilität, Weiterbildung, weiche Präferenzen. Ein reines Vollformular skaliert schlecht in Akzeptanz und Vollständigkeit (Abbruch, spätere Korrekturen).

**Produkthypothese:** Ergänzend zu geführten UI-Wizards eine **gesprächsbasierte** Erfassung, die sich für den Nutzer wie ein natürliches Interview anfühlt — intern aber schema-getrieben ist, damit Antworten maschinenlesbar werden.

### 11.3 Idee: KI-Agenten + Voice API (ausgehende Anrufe)

**Konzept:** KI-gestützte Agenten rufen Bewerbende via **Voice-/Telefonie-API** an und führen einen dialogischen Ablauf durch. Antworten werden erfasst (Audio → Transkript), anschliessend strukturiert, validiert und zusammengefasst — als Grundlage für Bewerberprofil und Suchprofil.

**Mögliche Vorteile:**

- Niedrige Einstiegshürde — lieber sprechen als tippen, besonders unterwegs.
- Natürliche Nachfragen im Fluss statt starrer Dropdown-Ketten.
- Progressives Profil: Kerndaten zuerst, Vertiefung bei Bedarf per Follow-up-Call.

**Risiken und Designpflichten:**


| Thema                       | Anforderung                                                                                                                               |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| **Vertrauen & Transparenz** | Klar kommunizieren, dass ein Assistent/Bot anruft; Zweck und Speicherdauer offenlegen; Opt-in pro Kanal                                   |
| **Qualitätssicherung**      | Bestätigungsschritt im UI nach dem Call; Confidence-basierte Nachfrage bei unsicheren Extrakten; kein blindes Schreiben ins Matching      |
| **Barrierefreiheit**        | Voice optional halten; gleiche Infos immer auch per Text/UI erreichbar                                                                    |
| **Regulatorik CH/DACH**     | Telefon-/Recording-Einwilligung, Hinweis auf Aufzeichnung, Datenminimierung, Zugriff/Löschung; Biometrie (Voiceprint) explizit ausgrenzen |
| **Technik**                 | Latenz, Dialekte, Sprachwechsel (DE/FR/IT/EN), EU/CH-Region-Compliance der Voice-Provider, Kosten pro Minute                              |
| **Sicherheit**              | Scope der Fragen definieren — keine sensiblen Daten (Gesundheit, Bank) per ungesichertem Kanal                                            |


### 11.4 Architektur-Bausteine Voice-Erfassung (Skizze, nicht final)

1. **Orchestrierung** — Agent führt Zustandsgraph (Themenblöcke, Reihenfolge, Abhängigkeiten).
2. **Voice Layer** — Outbound-Call, STT (Speech-to-Text), optional TTS; Anbieterwahl nach DSG und Region.
3. **Dialog-Kern** — regelbasiert für kritische Felder + LLM für Nachfragen/Zusammenfassung; Guardrails (keine Rechtsberatung, keine Job-Zusagen).
4. **Strukturierung** — Mapping Gesprächsinhalte → internes Schema (Profilfelder, Konfidenz); Human-in-the-loop wo nötig.
5. **Persistenz & Versionierung** — Roh-Transkript vs. abgeleitete Daten; Audit-Spur für den Nutzer.
6. **Anbindung ans Matching** — erst nach Nutzer-Freigabe oder Timeout-Follow-up; UI-Korrekturen sauber mergen.

**Offene Entscheide:** Cloud Voice vs. lokale Nummern; Echtzeit vs. Callback planen; ein Agent pro Themenblock vs. ein langer Flow; Mehrsprachigkeit pro Nutzerprofil.

### 11.5 Einordnung im Gesamtprodukt

- Ergänzt §5.3 (geführtes Onboarding) um einen kanalübergreifenden Erfassungsweg — nicht als Ersatz, sondern als Akzeptanz- und Vollständigkeitshebel.
- Arbeitgeber-Suchprofile primär UI-/API-basiert (Voice-Onboarding für SMB optional, nicht aktueller Fokus).
- Voice-MVP kann **nach** erstem formularbasiertem Kern validiert werden (Completion-Rate, Datenqualität, Kosten/Nutzen).

---

## 12. Nächste Schritte

1. **Positionierung in einem Satz** für eine Ziel-Nische formulieren (nicht „alle Jobs weltweit").
2. **10–15 Interviews:** 5 HR-Leads, 5 aktive Suchende — Pain quantifizieren (Zeit, Kosten, Tools).
3. **Wettbewerbsmatrix:** Preismodell + Features der 3–5 wichtigsten Alternativen.
4. **Paper-Prototyp / User Journey** (Bewerber + Unternehmen) mit Screens, die Übersicht und Status zeigen.
5. **Geschäftsmodell-Skizze** mit 2 Varianten und Break-even-Annahmen.
6. **API-/Feed-Due-Diligence:** Anbieter kurzlisten, Sandbox-Zugänge, Feld-Mapping ins interne Modell, Kostenrechner.
7. **Rechts- und Risiko-Review** für Feeds und ggf. Rest-Crawl (CH): Vertragsbedingungen, AGB/robots.txt, Opt-out/Arbeitgeberkommunikation — vor flächigem Rollout.
8. **Architektur-Spike** (1–2 Wochen): End-to-End Ingestion (Feed oder kleiner Crawl-Pfad) → Normalisierung → Store → Metrik + Runbook-Entwurf.

---

## 13. Chronik

*(Chronologische Zusammenfassung der wichtigsten Gedanken aus den Gesprächen)*

- **Grundidee:** Jobbörse als zweiseitiger Markt — viele Opportunitäten parallel auf beiden Seiten.
- **Pain Jobsuchende:** Administration, Übersicht, viele Arbeitgeber einzeln bedienen.
- **Pain Unternehmen:** Inserate, Gebühren, Massenbewerbungen, Screening, Interview-Last, Fairness/Kununu, Subjektivität vs. Profil, Intransparenz, Ineffizienz; HR-Überlast inkl. Weiterleitung, Interview-Koordination, Phasen-Management, Absagen/Zusagen, Inserate-Pflege — wenig Zeit für individuelle Bewerberbetreuung.
- **Multi-Posting:** Parallel auf jobs.ch, LinkedIn etc. — hohe Gesamtkosten + Aufwand. Vision: künftig ein zentraler Einstieg.
- **Präferenz-Matching:** Bewerber (Zürich, Tram 6 ~10 Min, >50 MA, >80k CHF) und Arbeitgeber (Qualifikation, Erfahrung, Sprachen …) — Plattform kennt beide Seiten → Überdeckung als Indikator.
- **Asymmetrie:** Nicht alle Dimensionen paarig (Pendel-Constraint nur kandidatenseitig; Firma braucht kein Wohnort-Feld, aber Arbeitsort + Routing). Viele Bewerber-Infos arbeitgeberseitig sensibel → mehrere Datenquellen / Anreicherung nötig.
- **Parallele Informationsräume:** Bewerbungsmappen vs. Career-Seiten — heute wenig systematischer Abgleich, viel HR-Handarbeit. Vision: strukturierte Profile, Top-X-Matches, ein Profil für viele Unternehmen.
- **Karriere-Gap / Coaching light:** aus aggregierten Anforderungen Lücken zum aktuellen Profil ableiten → Retention nach erfolgreicher Einstellung.
- **0-Match-What-if:** bei keinen Treffern Vorschläge zur Kriterien-Anpassung; Beispiel >100k + 15 km Chur — Zürich als anderer Markt, nicht innerhalb 15 km.
- **Scope Arbeitgeber:** kein vollständiges Prozessmanagement; Kern = HR sieht weniger, dafür vorausqualifizierte Bewerber.
- **Scope Bewerber:** eine Profil- + Suchkriterien-Basis; Plattform übernimmt administrative Organisation.
- **Daten:** API-first mit wenigen grossen Inserate-Anbietern (~3 als Hypothese); Career-Sites nicht flächendeckend crawlen; Branchenfilter bis Zielgruppe definiert.
- **Phasen:** Phase 1 = Inferenz aus Börsen; Phase 2 = Erstpartei-Suchprofile ongeboardeter Arbeitgeber.
- **Technische Architektur / Rollen:** Zwei Rollen — Unternehmen (eigene Suchprofile) und Bewerbende (Profil + Suchkriterien). Natürliche Datenerfassung via KI-Agenten + Voice API (ausgehende Anrufe), Dialog statt Formularflut, anschliessend Strukturierung und Zusammenfassung — mit Compliance-Anforderungen und optionaler UI-Bestätigung.

---

*Nächste sinnvolle Runden: Nische/Beachhead festlegen, erste User Journey skizzieren, MVP-Scope schärfen.*