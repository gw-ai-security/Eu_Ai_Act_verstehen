---
title: Fallstudie – HR-Chatbot (Limited-Risk-System)
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, Limited Risk, Chatbot, HR, Transparency, Security]
---

# Fallstudie: HR-Chatbot für interne Anfragen

## Szenario
Ein Unternehmen setzt einen KI-gestützten Chatbot im HR-Bereich ein. Mitarbeitende können über den Chatbot Informationen zu Urlaub, Krankmeldungen, Gehaltsabrechnungen und internen Richtlinien abfragen.  
Die KI greift auf interne Dokumentationen und HR-Systeme (z. B. Zeiterfassung, Policies) zu, um automatisierte Antworten bereitzustellen.

## AI Act Klassifizierung
- **Risikoeinstufung:** Eingeschränktes Risiko (Limited Risk)  
- **Begründung:** Kein Hochrisiko-Anwendungsfall nach Anhang III. Potenzielle Auswirkungen auf Grundrechte sind begrenzt.  
- **Anwendbare Artikel:** Transparenzpflichten (Art. 52 AI Act).

## Relevante Artikel
- **Art. 52 – Transparenzpflichten:** Nutzer müssen darüber informiert werden, dass sie mit einem KI-System interagieren.  
- **Art. 10 – Datenqualität:** Sicherstellung, dass die Trainings- und Wissensdaten aktuell und korrekt sind.  
- **Art. 15 – Sicherheit und Genauigkeit:** Basiskontrollen für Robustheit und Schutz vor Angriffen.

## AI/IT Security Herausforderungen
1. Datenlecks durch unsichere Schnittstellen zu HR-Systemen.  
2. Prompt Injection (Manipulation von Anfragen, um vertrauliche Informationen zu extrahieren).  
3. Veraltete oder unvollständige Wissensdaten → fehlerhafte Antworten.  
4. Fehlende Transparenz → Mitarbeitende wissen nicht, dass sie mit einer KI interagieren.  

## Beratungsempfehlungen
- **Technisch:** Zugriffskontrolle (RBAC), Input-Filter gegen Prompt Injection, regelmäßige Updates der Wissensbasis.  
- **Organisatorisch:** Transparenzhinweis für Mitarbeitende („Sie interagieren mit einem KI-System“).  
- **Prozessual:** Regelmäßige HR-Reviews der Antworten, Incident-Response-Plan für Fehlfunktionen.

## Compliance-Roadmap
1. Implementierung eines Transparenzbanners für Chatbot-Nutzer.  
2. Zugriff auf sensible Daten beschränken (RBAC, API-Gateways).  
3. Prompt Injection Tests & Red Teaming einführen.  
4. HR-Review-Prozess für die Wissensbasis etablieren.  

## Metriken und Tests
- **Genauigkeit:** Anteil korrekter Antworten (z. B. ≥ 95 %).  
- **Security:** Anzahl blockierter Prompt Injection Attempts.  
- **Datenqualität:** Aktualisierungsrate der HR-Daten (z. B. alle 30 Tage).  
- **User Experience:** Nutzerfeedback zum Vertrauen in den Chatbot.

## Diskussionsfragen
1. Wie kann ein HR-Chatbot so gestaltet werden, dass er Transparenzanforderungen erfüllt, ohne die Nutzerfreundlichkeit zu beeinträchtigen?  
2. Welche zusätzlichen Kontrollen sind notwendig, wenn der Chatbot Zugriff auf besonders sensible HR-Daten erhält?  

## JSON/YAML-Repräsentation
Siehe separate Dateien im gleichen Ordner.
