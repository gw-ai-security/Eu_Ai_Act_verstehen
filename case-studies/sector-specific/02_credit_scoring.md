---
title: Fallstudie – Kreditwürdigkeitsprüfung (Banking)
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, High-Risk, Banking, Credit Scoring, Case Study]
---

# Fallstudie 2: Kreditwürdigkeitsprüfung (Banking)

## Szenario
Ein Finanzinstitut entwickelt ein KI-System zur automatisierten Kreditwürdigkeitsprüfung.  
Das System analysiert Kundendaten, Einkommen, Zahlungsverhalten und externe Datenquellen, um Kreditentscheidungen zu treffen.  
Beteiligte: Bank, Kreditkunden, Aufsichtsbehörden.

## AI Act Klassifizierung
- **Risikoeinstufung:** Hochrisiko (Finanzdienstleistungen, Auswirkungen auf Grundrechte).  
- **Relevante Artikel:** Art. 10, 13, 14, 15, 21.

## Relevante Artikel
- Art. 10: Datenqualität, Fairness, Vermeidung diskriminierender Bias.  
- Art. 13: Transparenz gegenüber Kunden.  
- Art. 14: Menschliche Überprüfbarkeit von Kreditentscheidungen.  
- Art. 15: Robustheit, Sicherheit und Genauigkeit des Modells.  
- Art. 21: Post-Market-Monitoring.  

## AI/IT-Security Herausforderungen
1. Bias und Diskriminierung (Geschlecht, Herkunft, Alter).  
2. Datenvergiftung bei Trainingsdaten.  
3. Prompt Injection/Manipulation durch manipulierte Eingaben.  
4. Datenschutzverletzungen bei sensiblen Finanzdaten.  

## Beratungsempfehlungen
- Fairness- und Bias-Checks (z. B. Disparate Impact Analysis).  
- Einsatz sicherer Datenpipelines und Validierungsmechanismen.  
- Secure SDLC mit Privacy by Design.  
- Audit-Prozesse und regelmäßige Überprüfungen.  

## Compliance-Roadmap
1. Einführung eines Data Governance Frameworks.  
2. Transparenz-Reports für Kunden.  
3. Bias- und Accuracy-Tests in regelmäßigen Abständen.  
4. Integration in Incident Response und Post-Market-Monitoring (Art. 21).  
5. Zusammenarbeit mit Datenschutz- und Aufsichtsbehörden.  

## Metriken und Tests
- Bias Detection Scores (z. B. Equal Opportunity, Statistical Parity).  
- Accuracy, Precision/Recall.  
- Explainability-Indikatoren (z. B. SHAP, LIME).  

## Diskussionsfragen
1. Wie kann Fairness mit Robustheit in Kreditentscheidungen kombiniert werden?  
2. Welche Anforderungen ergeben sich aus DSGVO zusätzlich zum AI Act?  

## JSON-Repräsentation
```json
{
  "scenario": "Credit Scoring in Banking",
  "risk_level": "high",
  "articles": [10, 13, 14, 15, 21],
  "security_challenges": ["bias", "data poisoning", "prompt injection", "data privacy"],
  "recommendations": ["fairness checks", "secure data pipelines", "privacy by design", "audits"],
  "roadmap": ["data governance", "transparency reports", "bias tests", "incident response", "regulatory collaboration"]
}
```
