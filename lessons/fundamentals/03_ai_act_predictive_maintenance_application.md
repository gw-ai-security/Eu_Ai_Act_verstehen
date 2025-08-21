---
title: Anwendung des EU AI Act auf Predictive Maintenance (High-Risk KI)
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, Cybersecurity, Predictive Maintenance, Application, Bloom-Level-3]
---

# Lesson 03: Anwendung des EU AI Act auf Predictive Maintenance

## Lernziel
Anwenden der EU AI Act-Anforderungen auf ein konkretes Praxis-Szenario:  
Ein Fertigungsunternehmen entwickelt ein **KI-System für vorausschauende Wartung (Predictive Maintenance)**.  
Dies ist die dritte Stufe (Anwenden) nach der Bloomschen Taxonomie.

---

## Aufgabe (Level 3 – Anwenden)
**Frage:**  
*Welche konkreten AI Act-Anforderungen bezüglich Cybersecurity und Daten-Governance müssen für ein Predictive Maintenance KI-System erfüllt werden?*

---

## Lösungserwartung

### Anwendbare Artikel (EU AI Act)
- **Art. 9 – Risikomanagementsystem**  
  Systematische Risikoidentifikation, -bewertung und -minderung (inkl. Cyberangriffe, Manipulation).

- **Art. 10 – Daten- und Daten-Governance**  
  Sicherstellung der Datenqualität: korrekte Sensordaten, Vollständigkeit, Schutz gegen Datenvergiftung.

- **Art. 13 – Transparenzpflichten**  
  Dokumentation, Nachvollziehbarkeit der Entscheidungslogik, Bereitstellung relevanter Informationen an Anwender.

- **Art. 14 – Menschliche Aufsicht**  
  Techniker müssen Entscheidungen des KI-Systems überprüfen und bei Fehlern eingreifen können.

- **Art. 15 – Robustheit, Sicherheit und Genauigkeit**  
  Schutz gegen Angriffe (z. B. Evasion Attacks), Absicherung von Schnittstellen, Fail-Safe Mechanismen, Genauigkeitsmetriken.

- **Art. 16 – Pflichten der Anbieter**  
  Anbieter müssen Sicherheitsmaßnahmen dokumentieren und kontinuierliche Überwachung sicherstellen.

---

### Konkrete AI/IT-Sicherheitsmaßnahmen
1. **Daten-Governance**  
   - Validierung der Sensordaten auf Integrität und Vollständigkeit.  
   - Schutz gegen Manipulation (z. B. digitale Signaturen, Anomalieerkennung).  
   - Bias-Prüfung, um falsche Wartungsempfehlungen zu vermeiden.

2. **Cybersecurity**  
   - Absicherung der Schnittstellen (API Security, Authentifizierung, Verschlüsselung).  
   - Monitoring & Logging von Angriffen oder untypischem Verhalten.  
   - Einsatz von Threat Modeling (STRIDE, LINDDUN) für Systemarchitektur.

3. **Modell-Sicherheit**  
   - Adversarial Testing (z. B. simulierte Evasion Attacks auf Sensordaten).  
   - Red Teaming für gezielte Angriffe auf Modelle und Infrastruktur.  
   - Regelmäßige Accuracy- und Robustness-Tests.

4. **Betrieb & Organisation**  
   - Rollenkonzepte (RBAC) für Zugriff auf Modelle und Daten.  
   - Incident Response Plan bei Sicherheitsvorfällen.  
   - Dokumentation und Audit-Trails.

---

## Praxis-Transfer
Ein Predictive Maintenance KI-System erkennt einen drohenden Maschinenausfall.  
- **Datenqualität**: Manipulierte Sensordaten könnten zu Fehlalarmen oder übersehenen Schäden führen.  
- **Sicherheit**: Angriffe auf die API könnten falsche Wartungsintervalle erzwingen.  
- **Robustheit**: Fail-Safe Mechanismus muss sicherstellen, dass Maschinen bei Anomalien in den sicheren Modus wechseln.

---

## Nächste Schritte
- Level 4 (Analysieren): Überschneidungen zwischen AI Act (Art. 15) und NIS2/DORA analysieren.  
- Fokus auf Synergien und mögliche Konflikte bei Cybersecurity-Anforderungen.

