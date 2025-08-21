---
title: Fallstudie – Predictive Maintenance (Fertigungsindustrie)
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, High-Risk, Predictive Maintenance, Case Study]
---

# Fallstudie 1: Predictive Maintenance (Fertigungsindustrie)

## Szenario
Ein Fertigungsunternehmen entwickelt ein KI-System für vorausschauende Wartung.  
Das System analysiert Sensordaten von Maschinen, um Ausfälle frühzeitig zu erkennen und Wartungszyklen zu optimieren.  
Beteiligte: Hersteller, Betreiber, Techniker. Daten: IoT-Sensoren, Wartungsprotokolle.

## AI Act Klassifizierung
- **Risikoeinstufung:** Hochrisiko (kritische Infrastruktur, Sicherheit der Beschäftigten).  
- **Relevante Artikel:** Art. 9, 10, 13, 14, 15, 16.

## Relevante Artikel
- Art. 9: Risikomanagementsystem.  
- Art. 10: Datenqualität, Bias-Kontrolle.  
- Art. 13: Transparenz für Anwender.  
- Art. 14: Menschliche Aufsicht durch Techniker.  
- Art. 15: Robustheit, Sicherheit, Genauigkeit.  
- Art. 16: Pflichten der Anbieter.

## AI/IT-Security Herausforderungen
1. Manipulation von Sensordaten (Data Poisoning).  
2. Evasion Attacks auf das Modell.  
3. API-Schnittstellen-Angriffe.  
4. Fehlende Bias-Kontrollen in den Daten.  

## Beratungsempfehlungen
- Implementierung von **Data Integrity Checks** und Signaturen für Sensordaten.  
- Nutzung sicherer APIs mit Authentifizierung & Verschlüsselung.  
- Red Teaming & Adversarial Testing zur Erkennung von Schwachstellen.  
- Bias-Analysen der Wartungsdaten.  

## Compliance-Roadmap
1. Einrichtung Risikomanagementsystem (Art. 9).  
2. Datenvalidierung und Governance-Prozesse (Art. 10).  
3. Monitoring und Logging der Betriebsdaten (Art. 15).  
4. Regelmäßige Bias- und Robustness-Tests.  
5. Incident Response Plan inkl. Meldepflichten.  

## Metriken und Tests
- Accuracy, Precision, Recall für Vorhersagen.  
- Robustness-Scores gegen Angriffe.  
- Bias-Detection-Tools (z. B. Fairness-Indikatoren).  

## Diskussionsfragen
1. Wie kann Bias in Sensordaten erkannt und reduziert werden?  
2. Welche Rolle spielen menschliche Techniker in der Überwachung?  

## JSON-Repräsentation
```json
{
  "scenario": "Predictive Maintenance in Manufacturing",
  "risk_level": "high",
  "articles": [9, 10, 13, 14, 15, 16],
  "security_challenges": ["data poisoning", "evasion attacks", "API attacks", "bias"],
  "recommendations": ["data integrity checks", "secure APIs", "red teaming", "bias analysis"],
  "roadmap": ["risk management", "data governance", "monitoring", "robustness tests", "incident response"]
}
```
