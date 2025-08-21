---
title: Analyse der Überschneidungen EU AI Act Art. 15 und NIS2/DORA
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, NIS2, DORA, Cybersecurity, Analysis, Bloom-Level-4]
---

# Lesson 04: Analyse der Überschneidungen zwischen EU AI Act (Art. 15) und NIS2/DORA

## Lernziel
Analysieren der Gemeinsamkeiten und Unterschiede zwischen den Cybersicherheitsanforderungen des **EU AI Act (Art. 15)** und den Vorgaben aus **NIS2** sowie **DORA**.  
Dies ist die vierte Stufe (Analysieren) nach der Bloomschen Taxonomie.

---

## Aufgabe (Level 4 – Analysieren)
**Frage:**  
*Analysiere Überschneidungen zwischen den Cybersicherheitsanforderungen des EU AI Act (Art. 15) und den Regelungen aus NIS2 und DORA. Wo entstehen Synergien, wo potenzielle Konflikte?*

---

## Lösungserwartung

### EU AI Act – Art. 15 (Robustheit, Sicherheit, Genauigkeit)
- Systeme müssen gegen Cyberangriffe, Manipulation und Fehlfunktionen geschützt sein.  
- Genauigkeits- und Robustheitsprüfungen sind verpflichtend.  
- Sicherheit ist ein Kernelement bei Hochrisiko-KI-Systemen.  

### NIS2 (Richtlinie über Netz- und Informationssicherheit)
- Fokus auf **Kritische Infrastrukturen** (z. B. Energie, Gesundheit, Transport, Finanzwesen).  
- Anforderungen: Risikomanagement, Meldung von Sicherheitsvorfällen, Business Continuity.  
- Verbindliche Mindestmaßnahmen: Incident Response, Penetration Tests, Verschlüsselung, Patch-Management.  

### DORA (Digital Operational Resilience Act)
- Spezifisch für den **Finanzsektor**.  
- Anforderungen: ICT-Risikomanagement, Testing (inkl. Threat-Led Penetration Testing), Drittanbieter-Management.  
- Schwerpunkt auf **operativer Resilienz** und Regulierung von Dienstleistern (z. B. Cloud-Anbieter).  

---

### Überschneidungen / Synergien
1. **Risikomanagement**  
   - AI Act (Art. 15) verlangt systematisches Risikomanagement.  
   - NIS2/DORA fordern umfassende Risiko- und Resilienzkonzepte.  
   → Synergie: Gemeinsame Risiko-Frameworks nutzbar (z. B. ISO 27005, NIST).  

2. **Security Controls**  
   - AI Act: Schutz vor Angriffen auf Modelle/Daten.  
   - NIS2/DORA: Schutz kritischer Systeme, Netzwerke und Dienste.  
   → Synergie: Einheitliche Kontrollen wie Monitoring, Logging, Red Teaming.  

3. **Incident Response**  
   - AI Act implizit über Robustheit.  
   - NIS2/DORA explizit: Meldepflichten, Response-Pläne.  
   → Synergie: AI-Systeme können in bestehende Incident Response-Prozesse integriert werden.  

4. **Testing & Validierung**  
   - AI Act: Robustheits- und Genauigkeitstests für Modelle.  
   - DORA: Threat-Led Penetration Testing (TLPT).  
   → Synergie: AI-spezifische Tests lassen sich in Security-Tests integrieren.  

---

### Potenzielle Konflikte
- **Scope-Unterschiede**:  
  AI Act bezieht sich auf alle Hochrisiko-KI-Systeme, NIS2/DORA auf bestimmte Branchen.  
- **Nachweisführung**:  
  AI Act fokussiert auf Dokumentation für Konformität, NIS2/DORA stärker auf regulatorische Prüfungen.  
- **Verantwortlichkeiten**:  
  Anbieterpflichten (AI Act) vs. Betreiberpflichten (NIS2/DORA) können Überschneidungen erzeugen.  

---

## Praxis-Transfer
Ein **Bankinstitut** setzt KI-Systeme zur Betrugserkennung ein.  
- AI Act (Art. 15) verlangt robuste und sichere Modelle.  
- NIS2 fordert Sicherheit im gesamten Netzwerk- und Informationssystem.  
- DORA schreibt ICT-Risikomanagement und resiliente Prozesse vor.  

Analyse: Durch Kombination von AI Act, NIS2 und DORA ergibt sich ein **ganzheitliches Security-Framework**, jedoch mit potenziell höherem Dokumentationsaufwand.  

---

## Nächste Schritte
- Level 5 (Bewerten): Kritische Bewertung der Post-Market-Monitoring-Anforderungen (Art. 21 AI Act) aus IT-Sicherheitssicht.  
- Ableitung von Empfehlungen für Hersteller.

