---
title: Lesson 7 – DPIA & Grundrechts‑Folgenabschätzung (FRA) für KI
version: 1.0
last_updated: 2025-08-21
tags: [EU AI Act, DSGVO, Art.35, FRA, Risk Assessment, Security, NIST AI RMF, ISO/IEC 23894, ISO/IEC 42001]
---

# Lernziele und Erfolgskriterien
**Ziele**
- Unterschiede und Verzahnung von DSGVO‑DPIA (Art. 35) und AI‑Act‑Grundrechts‑Folgenabschätzung (FRA) verstehen.
- Einen integrierten Assessmentsprozess für Hochrisiko‑KI entwerfen und anwenden.
- Prüfkriterien, Evidenzen und Eskalationswege definieren.

**Erfolgskriterien**
- Abgeschlossene DPIA & FRA mit dokumentierten Risiken, Maßnahmen, Rest‑Risiko‑Begründung und Freigaben.
- Revisionsfähige Artefakte (Templates, Risk Register, Decision Log) im Repo.

---

# Kerninhalte (kompakt)
- **Auslöser DPIA (DSGVO Art. 35):** systematische, umfangreiche Verarbeitung, neue Technologien, besondere Datenkategorien, Personenprofiling.
- **Auslöser FRA (AI Act, Hochrisiko‑KI):** Bewertung von Auswirkungen auf Gesundheit, Sicherheit und Grundrechte; anhand Zweckbestimmung, Kontext, Stakeholdern.
- **Prozessintegration:** Gemeinsame Scoping‑Phase → Datenfluss & Zweck → Risiko‑Identifikation (Privacy, Security, Ethics, Safety) → Kontrollen & Tests → Rest‑Risiko → Freigabe → Monitoring.
- **Rollen:** Verantwortlicher/Provider, DSB, CISO, Produktverantwortliche, Legal/Compliance, Human Oversight, betroffene Stakeholder.

---

# Bloom-Aufgaben mit Lösungserwartungen
1. **Erinnern:** Nenne drei typische DPIA‑Trigger und zwei FRA‑Trigger.  
   _Erwartung:_ z. B. umfangreiche Profilbildung; besondere Kategorien; öffentlich zugängliche Bereiche; für FRA: Hochrisiko‑Use‑Case; erhebliche Grundrechtsauswirkung.
2. **Verstehen:** Erläutere, warum „Robustheit & Genauigkeit“ Sicherheitsrelevanz für FRA hat.  
   _Erwartung:_ Fehlklassifikationen können Grundrechte verletzen; Security‑Angriffe (Evasion/Poisoning) beeinflussen Genauigkeit → höhere Risiken.
3. **Anwenden:** Führe ein Scoping für ein Predictive‑Maintenance‑System durch (Sensor‑Daten + Wartungsplanung).  
   _Erwartung:_ Datenarten, Betroffene (Mitarbeitende), Zwecke, rechtl. Grundlagen, Risiken (z. B. Leistungsüberwachung).
4. **Analysieren:** Mappe identifizierte Risiken zu Kontrollen und zeige Lücken auf.  
   _Erwartung:_ Threat→Control→Evidence‑Kette, z. B. Prompt‑Injection→Input‑Filter/Policy→Red‑Team‑Report.
5. **Bewerten:** Begründe die Freigabe trotz Rest‑Risiko und definiere Monitoring‑KPIs.  
   _Erwartung:_ Risikoakzeptanz durch Management; KPIs wie Drift‑Rate, False‑Positive‑Quote, Security‑Findings‑SLA.
6. **Erschaffen:** Erstelle eine integrierte DPIA+FRA für den Fall (Template unten) und committed sie ins Repo.

---

# Praxisbeispiel: Predictive Maintenance (Fertigung)
- **Datenflüsse:** Maschinensensorik → Feature‑Store → Modelltraining → Inferenz → Wartungsaufträge.
- **Potenzielle Risiken:** Mitarbeiterprofiling durch indirekte Ableitungen, Zweckänderung, Datenvergiftung, Modell‑Evasion, fehlerhafte Priorisierung mit Sicherheitsfolgen.
- **Kontrollen:** Datenminimierung, Zweckbindung, RBAC/Secrets, Dataset‑Versionierung, Adversarial Testing, Human Oversight, Incident‑Playbooks.

---

# Security- und Compliance‑Mappings (Auszug)
| AI‑Act‑Anforderung | DSGVO‑Bezug | Standard/Control | Evidenz/Nachweis |
|---|---|---|---|
| Art. 9 Risikomanagement | Art. 24, 25, 32 | **ISO/IEC 23894** (AI RM), **ISO/IEC 42001** (AIMS), **NIST AI RMF** (MAP/MANAGE) | Risk Register, RA‑Workshop‑Protokolle |
| Art. 10 Daten & Data Governance | Art. 5, 6, 9, 35 | **ISO/IEC 27001/27002** (A.8, A.5.12), **SP 800‑53** (PT‑2, AR‑2) | Data‑Lineage, DQ‑Berichte, DSFA |
| Art. 13 Transparenz | Art. 12–14 | **NIST AI RMF** (GOV‑2), **OWASP LLM‑A1** | Model Cards, Nutzerhinweise |
| Art. 14 Human Oversight | Art. 22 | **SP 800‑53** (IR‑4, AU‑6), **ISO 42001** | SOPs, 4‑Augen‑Prinzip |
| Art. 15 Robustheit/Genauigkeit | Art. 32 | **ENISA AI Threat Landscape**, **OWASP LLM Top10** | Red‑Team‑Report, Robustness‑Tests |
| Art. 16 Logging/Traceability | Art. 30 | **ISO/IEC 27001** (A.8.15, A.8.16) | Audit‑Logs, Modell‑ und Datenversionen |

---

# GitHub‑Ready‑Artefakte

## 1) DPIA+FRA‑Checklist (Kurz)
- Zweck, Rechtsgrundlage, Betroffene, Datenarten, Empfänger, Speicherfristen  
- Risikoquellen: Privacy, Security, Safety, Ethics, Bias  
- Kontrollen: technisch, organisatorisch, prozessual  
- Tests: Robustness, Bias, Privacy, Security (Red Team, Pen‑Test)  
- Rest‑Risiko & Entscheidung, Verantwortliche, Review‑Zyklus

## 2) YAML‑Template: Integrierte DPIA & FRA
```yaml
id: PM-001
system: predictive-maintenance
version: 1.0
owner: ops-ml@example.com
scope:
  purposes: ["Wartungsprognose", "Sicherheitsrelevante Störungsprävention"]
  legal_basis: ["Art.6(1)(f) DSGVO – berechtigtes Interesse"]
  data_subjects: ["Mitarbeitende", "Dienstleister"]
data_inventory:
  categories: ["Sensorik", "Wartungslogs", "Schichtpläne(minimiert)"]
  special_categories: false
risk_assessment:
  privacy_risks: ["indirekte Leistungsbewertung", "Zweckänderung"]
  security_risks: ["Datenvergiftung", "Model Evasion", "Prompt Injection (UI/Chat)"]
  ethics_fairness: ["Verzerrte Zuweisung von Wartungsaufträgen"]
controls:
  technical: ["RBAC", "Secrets Mgmt", "Data/Model Versioning", "Adversarial Tests"]
  organizational: ["Human Oversight SOP", "Least Privilege", "Third‑Party Due Diligence"]
  process: ["Change Control", "Model Risk Committee", "Incident Response"]
testing:
  robustness: ["Stress/Noise/Evasion‑Szenarien"]
  bias: ["Subgruppen‑Fehlerquoten", "Equalized Odds‑Check"]
  privacy: ["PIA‑Checks", "Data Minimization Audit"]
  security: ["Red Team Exercises", "SBOM/Dependency Audit"]
residual_risk:
  level: "low"
  justification: "Kontrollen und Monitoring senken Eintrittswahrscheinlichkeit und Auswirkung"
approval:
  dpo_signoff: true
  ciso_signoff: true
  business_owner_signoff: true
monitoring:
  kpis: ["Drift‑Rate", "FP/FN‑Quote", "Security Findings MTTR"]
  review_cycle_days: 90
```

## 3) Decision Log (Markdown)
```md
# Decision Log – Predictive Maintenance
- 2025‑08‑21: Rechtsgrundlage bestätigt (Art.6(1)(f)); Interessenabwägung dokumentiert.
- 2025‑08‑21: Red‑Team‑Szenarien genehmigt; Evasion‑Testkatalog v1.
- 2025‑08‑21: Rest‑Risiko „low“ akzeptiert durch Management.
```

## 4) Commit‑Vorschläge (Conventional Commits)
- `feat(lessons): add integrated DPIA+FRA template for high‑risk AI`
- `docs(risk): add decision log & checklist for PM system`
- `chore(templates): add yaml schema for assessments`

---

# Metriken und Tests (konkret)
- **Robustheit:** Accuracy@Top‑K, Worst‑Group‑Accuracy, Evasion‑Resilienzrate.  
- **Bias:** Subgruppen‑FPR/FNR‑Gap ≤ definiertem Threshold; PDP/SHAP‑Review.  
- **Privacy:** Re‑Ident‑Risiko‑Score, Datensparsamkeit (Features reduziert).  
- **Security:** Mean Time to Detection/Response, erfolgreiche Blockquote‑Rate bei Prompt‑Attacks, SBOM‑Risiken geschlossen.

---

# Verständnisfragen
**MCQ**
1) Welche Kombination beschreibt am besten die integrierte Bewertung?  
A) Nur DPIA. B) Nur FRA. C) DPIA + FRA gemeinsam mit Security‑Tests. D) Nur Pen‑Test.  
_Lösung: C._

2) Welcher Test gehört primär zu Robustheit?  
A) Re‑Ident‑Risiko. B) Evasion‑Tests. C) Interessenabwägung. D) Verarbeitungsverzeichnis.  
_Lösung: B._

**Offene Fragen (Bewertungsrubrik: 0–5 Punkte je Kriterium Relevanz/Tiefe/Evidenz)**
- Begründe die Wahl der Rechtsgrundlage und dokumentiere die Interessenabwägung.
- Entwirf einen Monitoring‑Plan, der Drift und Security‑Events zusammenführt.

---

# Nächste Schritte
1. Repo‑Ordner `/tools/templates/` um das YAML‑Template ergänzen.  
2. Erste DPIA+FRA für einen realen Use‑Case erstellen und reviewen.  
3. Red‑Team‑Szenarien durchspielen, Findings in Controls rückkoppeln.  
4. Monitoring‑KPIs in das Betriebsdashboard integrieren.
