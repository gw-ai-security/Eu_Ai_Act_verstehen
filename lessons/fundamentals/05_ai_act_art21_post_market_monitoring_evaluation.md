---
title: Bewertung der Post-Market-Monitoring-Anforderungen (Art. 21 EU AI Act)
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, Post-Market-Monitoring, Evaluation, Bloom-Level-5]
---

# Lesson 05: Bewertung der Post-Market-Monitoring-Anforderungen (Art. 21 EU AI Act)

## Lernziel
Kritische Bewertung der Anforderungen aus **Art. 21 EU AI Act** zum Post-Market-Monitoring (PMM) aus IT-Sicherheitssicht.  
Dies ist die fünfte Stufe (Bewerten) nach der Bloomschen Taxonomie.

---

## Aufgabe (Level 5 – Bewerten)
**Frage:**  
*Bewerte die Post-Market-Monitoring-Anforderungen (Art. 21) aus IT-Sicherheitssicht. Welche Empfehlungen würdest du Herstellern für eine sichere und effiziente Umsetzung geben?*

---

## Lösungserwartung

### Inhalt von Art. 21 EU AI Act – Post-Market-Monitoring
- Anbieter von Hochrisiko-KI-Systemen müssen ein **kontinuierliches Monitoring-System** einführen.  
- Ziel: Erfassung, Analyse und Dokumentation von Risiken, Vorfällen und Performance-Problemen im Betrieb.  
- Hersteller sind verpflichtet, **Meldungen an Behörden** vorzunehmen, wenn erhebliche Sicherheitsrisiken auftreten.  

### Bewertung aus IT-Sicherheitssicht
**Stärken:**  
- Frühzeitige Erkennung neuer Bedrohungen (z. B. Zero-Day Exploits, neue Angriffsmuster).  
- Fördert einen „Security by Monitoring“-Ansatz und kontinuierliche Verbesserung.  
- Ermöglicht Incident Response und schnelle Anpassung von Kontrollen.  

**Schwächen / Herausforderungen:**  
- Hoher organisatorischer und technischer Aufwand (Monitoring-Infrastruktur, Personal).  
- Gefahr von **Datenüberflutung** (False Positives, unklare Risikoeinschätzung).  
- Abhängigkeit von der Qualität der Logging- und Reporting-Systeme.  
- Unterschiedliche regulatorische Anforderungen (AI Act vs. NIS2/DORA) können zu Mehraufwand führen.  

### Empfehlungen für Hersteller
1. **Integration in bestehende Security-Prozesse**  
   - Monitoring in SIEM-/SOAR-Systeme integrieren.  
   - Nutzung etablierter Frameworks (z. B. NIST CSF, ISO 27035 für Incident Management).  

2. **Risikobasierte Priorisierung**  
   - Kritische Ereignisse hervorheben, um False Positives zu reduzieren.  
   - Automatisierte Alerts & Eskalationsmechanismen.  

3. **Technische Umsetzung**  
   - Lückenlose Protokollierung (Audit Trails).  
   - Anomalieerkennung mit ML-gestützten Tools.  
   - Härtung von MLOps/LLMOps-Pipelines mit Monitoring-Kontrollen.  

4. **Prozessuale Maßnahmen**  
   - Regelmäßige Reviews und Updates des PMM.  
   - Klare Rollen & Verantwortlichkeiten (CISO, Data Protection Officer, AI Compliance Officer).  
   - Schulungen für Entwickler und Betriebspersonal.  

---

## Praxis-Transfer
Ein Hersteller von **medizinischen Diagnosesystemen** (High-Risk) setzt KI zur Bildanalyse ein.  
- PMM erkennt unerwartete Fehlklassifikationen nach Software-Update.  
- IT-Security muss sicherstellen, dass Logs revisionssicher gespeichert werden.  
- Behörde muss informiert werden → Verbindung zu regulatorischen Pflichten aus DSGVO (Meldepflicht bei Datenpannen) und NIS2.  

---

## Nächste Schritte
- Level 6 (Erschaffen): Erstellung umfassender Fallstudien, inkl. Szenario, Security-Risiken, Compliance-Roadmap und JSON/YAML-Repräsentation.

