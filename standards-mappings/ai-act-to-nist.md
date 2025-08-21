---
title: Mapping EU AI Act ↔ NIST AI RMF 1.0
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, NIST AI RMF, Standards Mapping, Cybersecurity]
---

# Mapping EU AI Act ↔ NIST AI RMF 1.0

Dieses Dokument ordnet zentrale Anforderungen des **EU AI Act (2024/1689)** den Kernfunktionen des **NIST AI Risk Management Framework (AI RMF 1.0)** zu: **Govern, Map, Measure, Manage**.  
Ziel ist eine praxisnahe Brücke zwischen regulatorischen Pflichten und risikobasierten Managementpraktiken.

---

## Legende
- **GOV** = Govern  
- **MAP** = Map  
- **MEAS** = Measure  
- **MAN** = Manage  

---

## Mapping-Tabelle

| EU AI Act Artikel | Kurzinhalt / Pflicht | NIST AI RMF Zuordnung (Funktion → Kategorie/Beispiel) | Bemerkung |
|---|---|---|---|
| Art. 9 Risikomanagementsystem | Systematische Identifikation, Bewertung, Minderung von Risiken | **GOV** → Policies, Roles; **MAP** → Context, Intended Use; **MAN** → Risk Response, Change Management | Fundament für risikobasiertes AI-Management |
| Art. 10 Daten- und Daten-Governance | Datenqualität, Repräsentativität, Bias-Kontrolle, Integrität | **GOV** → Data Management; **MAP** → Data Characteristics; **MEAS** → Data Quality, Bias Measures; **MAN** → Data Lifecycle Controls | Stützt Fairness, Robustheit und Nachweisführung |
| Art. 13 Transparenz & Nutzerinformation | Dokumentation, Nutzungsinformationen, Nachvollziehbarkeit | **GOV** → Documentation; **MAP** → Use Context Disclosure; **MAN** → Communication, Stakeholder Engagement | Unterstützt erklärbare, überprüfbare KI |
| Art. 14 Menschliche Aufsicht | Human-in-the-loop, Eingriffsmöglichkeiten, Grenzen | **GOV** → Accountability; **MAP** → Human Factors; **MAN** → Operational Controls, Override/Shutdown | Design- und Betriebsanforderung |
| Art. 15 Robustheit, Sicherheit und Genauigkeit | Resistenz gegen Angriffe/Fehler, Genauigkeitsmetriken, Fail-safe | **MEAS** → Performance & Robustness Evaluation; **MAN** → Monitoring, Incident Response; **GOV** → Security Policies | Drehscheibe für Security- und Testpflichten |
| Art. 16 Pflichten der Anbieter | QM, Doku, Konformität, Updates, Logbuchführung | **GOV** → Risk Governance, Supply Chain; **MAN** → Lifecycle Management, Change & Patch | Verbindet Governance mit Betrieb |
| Art. 21 Post-Market-Monitoring | Betriebsüberwachung, Vorfallsanalyse, Meldungen | **MAN** → Monitoring, Incident Management; **MEAS** → Drift/Degradation Measurement | Kontinuierliche Verbesserung im Betrieb |
| Anhang III Hochrisiko-Listen | Definition der High-Risk-Anwendungsfälle | **MAP** → Context, Impact Analysis; **GOV** → Risk Appetite & Criteria | Steuert Einstufung und Treatment |
| Konformität/Technische Doku | Technische Dossiers, Nachweisführung | **GOV** → Documentation & Records; **MEAS** → Metrics Reproducibility | Belegt Reifegrad gegenüber Auditoren |

---

## Hinweise zur Anwendung
1. **Top-down & Bottom-up:** Beginne mit **GOV**-Aktivitäten (Policies, Rollen), beschreibe mit **MAP** den Kontext und Nutzungszweck, sichere mit **MEAS** die Messbarkeit ab und betreibe mit **MAN** das System über den Lebenszyklus.  
2. **Metriken verbinden:** Genauigkeit, Robustheit, Bias und Drift sollten konsistent gemessen und in PMM-Prozesse (Art. 21) eingebunden werden.  
3. **Supply Chain:** Nutze **GOV/MAN**-Kontrollen für Modelle, Datenlieferanten und Tools, inkl. Verträge und Third-Party-Risk.  
4. **Nachweisführung:** Verknüpfe Anforderungen mit Artefakten (Datenblätter, Testberichte, Monitoring-Logs, Incident-Reports).

---

## Beispielhafte Artefakte
- Risk Register mit AI-spezifischen Szenarien  
- Data Sheet inkl. Provenance, Qualität, Bias-Checks  
- Robustness- und Security-Testprotokolle  
- PMM-Dashboard mit Metriken und Incidents

---

## Nächste Schritte
- Ergänzung um **AI Act ↔ OWASP Top 10 for LLM**.  
- Verlinkung in die Checklisten und Fallstudien für konsistente Audits.
