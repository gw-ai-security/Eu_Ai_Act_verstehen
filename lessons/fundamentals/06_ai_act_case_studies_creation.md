---
title: Erstellung von Fallstudien nach EU AI Act & Cybersecurity-Anforderungen
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, Case Studies, Creation, Bloom-Level-6]
---

# Lesson 06: Erstellung von Fallstudien nach EU AI Act & Cybersecurity-Anforderungen

## Lernziel
Entwicklung umfassender Fallstudien, die die Anforderungen des EU AI Act mit AI/IT-Security-Aspekten verbinden.  
Dies ist die sechste Stufe (Erschaffen) nach der Bloomschen Taxonomie.

---

## Aufgabe (Level 6 – Erschaffen)
**Aufgabe:**  
*Erstelle zwei umfassende Fallstudien nach dem vorgegebenen Template. Die Fallstudien sollen Szenario, Klassifizierung, relevante Artikel, AI/IT-Sicherheitsherausforderungen, Empfehlungen, Roadmap, Metriken und Diskussionsfragen beinhalten.*

---

## Fallstudien-Template

### Szenario
- Beschreibung des KI-Systems (Zweck, beteiligte Parteien, Datenflüsse).

### AI Act Klassifizierung
- Risikoeinstufung (hoch, begrenzt, minimal) mit Begründung.
- Anwendbare Artikel/Anhänge.

### Relevante Artikel
- Spezifische Artikel mit kurzer Erklärung ihrer Relevanz.

### AI/IT-Security Herausforderungen
- 3–5 konkrete Risiken (z. B. Datenvergiftung, Prompt Injection, Modell-Leaks, Shadow AI).

### Beratungsempfehlungen
- Technische, organisatorische, prozessuale Maßnahmen.

### Compliance-Roadmap
- Schritt-für-Schritt Plan zur Umsetzung.

### Metriken und Tests
- Robustness-Tests, Bias-Analysen, Security-Assessments, Privacy-Checks.

### Diskussionsfragen
- 2–3 offene Fragen für Community-Diskussion.

### JSON/YAML-Repräsentation
- Strukturierte Daten zur Weiterverarbeitung.

---

## Beispiel – Kurzer Einstieg

### Fallstudie 1: Predictive Maintenance (Fertigungsindustrie)
- **Szenario:** KI-System erkennt frühzeitig Maschinenausfälle.  
- **Klassifizierung:** Hochrisiko (kritische Infrastruktur).  
- **Artikel:** Art. 9, 10, 13, 14, 15, 16.  
- **Risiken:** Manipulation von Sensordaten, API-Angriffe, Bias in Wartungsmodellen.  
- **Empfehlungen:** Data Integrity Checks, Secure APIs, Red Teaming.  
- **Roadmap:** SDLC + Monitoring + Incident Response.  
- **Metriken:** Accuracy, Precision/Recall, Robustness-Scores.  
- **Diskussionsfragen:** Wie lässt sich Bias in Sensordaten erkennen?  
- **JSON/YAML:** strukturierte Repräsentation.  

### Fallstudie 2: Kreditwürdigkeitsprüfung (Banking)
- **Szenario:** KI entscheidet über Kreditzusagen.  
- **Klassifizierung:** Hochrisiko (Finanzdienstleistungen).  
- **Artikel:** Art. 10, 13, 14, 15, 21.  
- **Risiken:** Bias (Diskriminierung), Datenvergiftung, Prompt Injection.  
- **Empfehlungen:** Fairness-Checks, Security by Design, Audit-Prozesse.  
- **Roadmap:** Governance-Framework, Monitoring, DSGVO-Verknüpfung.  
- **Metriken:** Bias-Detection Scores, Explainability-Indikatoren.  
- **Diskussionsfragen:** Wie verbindet man Fairness und Robustheit?  

---

## Nächste Schritte
- Die Fallstudien werden in **/case-studies/high-risk-systems/** bzw. **/case-studies/sector-specific/** abgelegt.  
- Jede Fallstudie erhält eine eigene Datei und JSON/YAML-Representation.

