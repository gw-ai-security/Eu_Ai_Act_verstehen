---
title: Fallstudie – Healthcare Diagnostic AI (High-Risk)
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, Healthcare, High Risk, Diagnostic AI, Security]
---

# Fallstudie: Healthcare Diagnostic AI

## Szenario
Ein Krankenhaus nutzt ein KI-System zur Analyse medizinischer Bilder (Radiologie, CT/MRT). Ziel ist die Unterstützung der Ärzte bei der Diagnosestellung.

## AI Act Klassifizierung
- **Risikoeinstufung:** Hochrisiko (Annex III, Nr. 5 – Medizinische Geräte).  
- **Anwendbare Artikel:** Art. 9 (Risikomanagement), Art. 10 (Datenqualität), Art. 15 (Robustness), Art. 16 (Pflichten Anbieter), Art. 21 (Post-Market Monitoring).

## Relevante Artikel
- **Art. 9:** Systematisches Risikomanagement.  
- **Art. 10:** Datenqualität (Bias in Trainingsdaten vermeiden).  
- **Art. 15:** Robustheit und Genauigkeit (adversarial Tests, Drift Detection).  
- **Art. 21:** Monitoring und Reporting von Zwischenfällen.

## AI/IT Security Herausforderungen
1. Datenvergiftung durch manipulierte Trainingsdaten.  
2. Adversarial Attacks (gezielte Pixel-Manipulation).  
3. Bias durch nicht-repräsentative Patientendaten.  
4. Datenschutz (DSGVO, sensible Gesundheitsdaten).  
5. Ausfallsicherheit der Infrastruktur.

## Beratungsempfehlungen
- **Technisch:** Adversarial Robustness Tests, Privacy-Preserving ML.  
- **Organisatorisch:** Ärzte als Human-in-the-Loop.  
- **Prozessual:** Incident Response Playbook für Fehlentscheidungen.

## Compliance-Roadmap
1. DPIA/FRA nach DSGVO & AI Act durchführen.  
2. Bias-Tests in QA-Prozess integrieren.  
3. Red Teaming für adversarial robustness.  
4. PMM-Prozess mit Behörden-Meldungen.  

## Metriken & Tests
- Genauigkeit > 98 % (validierte Testsets).  
- Anzahl erkannter adversarial Angriffe.  
- Bias-Metriken (Demografie-Check).  

## Diskussionsfragen
1. Wie lassen sich Accuracy und Fairness balancieren?  
2. Wie stark soll Human Oversight integriert sein?
