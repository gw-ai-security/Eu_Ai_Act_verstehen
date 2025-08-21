---
title: Art. 15 EU AI Act – Robustheit, Sicherheit und Genauigkeit
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, Cybersecurity, Robustness, Accuracy, Bloom-Level-2]
---

# Lesson 02: Art. 15 EU AI Act – Robustheit, Sicherheit und Genauigkeit

## Lernziel
Verstehen der **Bedeutung von Art. 15 EU AI Act** für Hochrisiko-KI-Systeme und Ableitung praktischer AI/IT-Sicherheitsmaßnahmen.  
Dies ist die zweite Stufe (Verstehen) nach der Bloomschen Taxonomie.

---

## Aufgabe (Level 2 – Verstehen)
**Frage:**  
*Erläutere die Bedeutung von „Robustheit, Sicherheit und Genauigkeit“ (Art. 15) für Hochrisiko-KI-Systeme. Welche spezifischen AI/IT-Sicherheitsmaßnahmen leiten sich daraus ab?*

---

## Lösungserwartung

### Bedeutung Art. 15 EU AI Act
- **Robustheit** → Das KI-System muss zuverlässig funktionieren, auch bei Angriffen, Fehlern oder ungewöhnlichen Eingaben.  
- **Sicherheit** → Schutz gegen Cyberangriffe, Manipulation und Fehlfunktionen; keine Gefährdung von Menschen oder kritischer Infrastruktur.  
- **Genauigkeit** → Ergebnisse müssen präzise, nachvollziehbar und in definierten Toleranzgrenzen liegen.  

### Abgeleitete Sicherheitsmaßnahmen
1. **Secure Development Lifecycle (SDLC)** → Security by Design, kontinuierliche Sicherheitsprüfungen.  
2. **Threat Modeling** → STRIDE, LINDDUN zur Analyse möglicher Angriffsvektoren.  
3. **Red Teaming & Adversarial Testing** → gezielte Angriffe (z. B. Evasion, Prompt Injection, Datenvergiftung) simulieren.  
4. **Monitoring & Logging** → Laufende Überwachung, Anomalieerkennung, Audit-Trails.  
5. **Fail-Safe Mechanismen** → Systeme müssen im Fehlerfall sicher abschalten oder einen sicheren Modus aktivieren.  
6. **Accuracy & Bias Tests** → Regelmäßige Validierung der Modellleistung (z. B. Precision, Recall, Bias-Checks).  

---

## Praxis-Transfer
**Beispiel: KI-System zur Kreditwürdigkeitsprüfung (High-Risk)**  
- **Robustheit**: Schutz gegen Datenvergiftung im Training.  
- **Sicherheit**: Absicherung der API-Schnittstellen gegen Manipulation.  
- **Genauigkeit**: Regelmäßige Validierung gegen Bias (z. B. Geschlecht, Herkunft).  

---

## Nächste Schritte
- Übergang zu Level 3 (Anwenden):  
  Szenario *Predictive Maintenance* – welche AI Act-Anforderungen müssen dort konkret umgesetzt werden?

