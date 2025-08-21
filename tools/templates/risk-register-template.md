---
title: Risk Register Template (AI Act & DSGVO)
version: 1.0
last_updated: 2025-08-21
tags: [Template, Risk Register, AI Act, DSGVO, Compliance, Security]
---

# Risk Register Template

Dieses Template dient zur strukturierten Erfassung, Bewertung und Behandlung von Risiken im Rahmen von EU AI Act Assessments, DPIA (DSGVO Art. 35) und Grundrechts-Folgenabschätzungen.

---

## Risiko-Eintrag (Beispielstruktur)

### Risiko-ID
- **ID:** R-001

### Beschreibung
- **Titel:** <Kurze Risikobezeichnung>
- **Beschreibung:** <Detaillierte Beschreibung des Risikos>
- **Kategorie:** <Privacy / Security / Fairness / Safety / Compliance / Operational>

### Bewertung
- **Eintrittswahrscheinlichkeit:** <niedrig / mittel / hoch>
- **Auswirkung:** <niedrig / mittel / hoch>
- **Risikostufe (Impact x Wahrscheinlichkeit):** <z. B. hoch>

### Ursachen & Bedrohungen
- **Threat Source:** <z. B. externer Angreifer, interner Fehler>
- **Threat Event:** <z. B. Datenvergiftung, Evasion Attack>

### Betroffene Assets
- **Systemkomponenten:** <z. B. Modell, API, Datenbank>
- **Betroffene Personen:** <z. B. Kunden, Mitarbeitende>

### Maßnahmen (Kontrollen)
- **Technische Kontrollen:** <z. B. Verschlüsselung, RBAC, Monitoring>
- **Organisatorische Kontrollen:** <z. B. Policies, Trainings>
- **Prozessuale Kontrollen:** <z. B. Incident Response, Audits>

### Rest-Risiko
- **Bewertung nach Kontrollen:** <low / medium / high>
- **Begründung:** <Warum verbleibt ein Rest-Risiko?>

### Verantwortlichkeiten
- **Owner:** <Rollen/Personen>
- **Review-Zyklus:** <z. B. alle 90 Tage>

---

## Commit-Vorschläge (Conventional Commits)
- `feat(risk): add new risk entry for <Risiko>`
- `docs(risk): update risk register with mitigations`
- `chore(risk): review and re-assess risks`
