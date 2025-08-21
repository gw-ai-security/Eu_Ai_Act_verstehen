---
title: Mapping EU AI Act ↔ OWASP Top 10 for LLM
version: 1.0
last_updated: 2025-08-21
tags: [AI Act, OWASP, LLM, Standards Mapping, Security, Compliance]
---

# Mapping EU AI Act ↔ OWASP Top 10 for LLM

Dieses Dokument verknüpft zentrale Anforderungen des **EU AI Act (2024/1689)** mit Risiken und Controls aus den **OWASP Top 10 for LLM Applications**. Ziel ist eine praxisnahe Brücke zwischen Regulierung und operativer Anwendungssicherheit.

---

## OWASP Top 10 for LLM (Kurzüberblick)
- **LLM01 Prompt Injection** – Manipulation von Anweisungen und Kontext.  
- **LLM02 Insecure Output Handling** – Ungeprüfte Modellantworten führen zu Folgeangriffen.  
- **LLM03 Training Data Poisoning** – Bösartige Daten beeinflussen Modellverhalten.  
- **LLM04 Model Denial of Service** – Ressourcenerschöpfung, Kosten- oder Verfügbarkeitsangriffe.  
- **LLM05 Supply Chain Vulnerabilities** – Abhängigkeiten, Modelle, Datensätze, Bibliotheken.  
- **LLM06 Sensitive Information Disclosure** – Preisgabe von Geheimnissen/Personendaten.  
- **LLM07 Insecure Plugin Design** – Erweiterungen/Tools mit übermäßigen Rechten oder unsicheren Schnittstellen.  
- **LLM08 Excessive Agency** – Übermäßige Aktionsrechte ohne ausreichende Kontrollen.  
- **LLM09 Overreliance** – Unkritische Nutzung ohne Validierung/Human Oversight.  
- **LLM10 Model Theft** – Exfiltration/Diebstahl von Modellen, Gewichten oder IP.

---

## Mapping-Tabelle

| OWASP LLM Risk | AI Act Bezug | Begründung der Zuordnung | Beispielkontrollen und Evidenzen |
|---|---|---|---|
| LLM01 Prompt Injection | Art. 15, Art. 9, Art. 13 | Angriff auf Robustheit/Genauigkeit; Risiko im Risikomanagement zu adressieren; Transparenz über Limitierungen | Input-Filter/Policies, Content Safety Gates, Adversarial Testfälle; Red-Team-Reports; Prompt-Sicherheitsrichtlinie |
| LLM02 Insecure Output Handling | Art. 15, Art. 13, Art. 14 | Unsichere Weiterverarbeitung von Modellantworten gefährdet Sicherheit und Nutzer; Human Oversight notwendig | Output-Sandboxing, Escaping/Validation, Allow/Deny-Listen; SOP für menschliche Freigabe; Logging von Outputs |
| LLM03 Training Data Poisoning | Art. 10, Art. 15, Art. 9 | Datenqualität, Provenance und Manipulationsschutz sind Pflicht; Robustheitstests erforderlich | Datenherkunftsnachweise, Signaturen, Data Versioning; Data Quality Reports; Poisoning-Detektion; SBOM für Datensätze |
| LLM04 Model Denial of Service | Art. 15, Art. 16 | Verfügbarkeit ist Sicherheitsziel; Anbieterpflichten zu Betrieb/Resilienz | Rate Limiting, Quotas, Caching, Backoff; DoS-Runbooks; Kapazitäts- und Lasttestprotokolle |
| LLM05 Supply Chain Vulnerabilities | Art. 16, Art. 9, Art. 15 | Drittparteien/Abhängigkeiten im Risikomanagement; Sicherheit über den Lebenszyklus | Third-Party Risk Assessments, SBOM/MLSBOM, Signierte Modelle; Patch- und Dependency-Management; Lieferantenverträge |
| LLM06 Sensitive Information Disclosure | Art. 10, Art. 13, Art. 15, DSGVO-Bezug | Datenschutz, Geheimnisschutz, Transparenz und Security | PII-Redaction, Data Minimization, Differential Privacy; Secret Scanners; Privacy Impact Assessments; Zugriffskontrolle |
| LLM07 Insecure Plugin Design | Art. 15, Art. 14, Art. 16 | Schnittstellen/Tools benötigen sichere Gestaltung und Human Oversight; Anbieterpflichten | Least-Privilege für Tools, OAuth/Scopes, Safe Tool Invocation, Threat Modeling der Plugins, Pen-Tests; Freigabeprotokolle |
| LLM08 Excessive Agency | Art. 14, Art. 15 | Human Oversight, Fail-Safe, Begrenzung von Aktionen sind gefordert | Policy Engine für Aktionen, Approval-Workflows, Rollback/Not-Aus; Audit-Trails; Simulationstests |
| LLM09 Overreliance | Art. 13, Art. 14 | Transparenz über Grenzen; menschliche Überwachung zur Fehlerrate und Kontextprüfung | Nutzerhinweise, Confidence/Uncertainty-Disclosure, Dual Control, 4-Augen-Prinzip; Schulungsnachweise |
| LLM10 Model Theft | Art. 15, Art. 16 | Schutz von Modellen/Weights/IP als Sicherheits- und Anbieterpflicht | Model Encryption/At-Rest/Transit, Access Control, Canary Weights, Watermarking; Exfiltration-Detection; Key-Management-Evidenzen |

---

## Umsetzungsleitfaden
1. **Threat Modeling für LLM-Use-Cases**: Identifiziere OWASP-Risiken pro Architekturkomponente und weise AI‑Act‑Artikel zu.  
2. **Kontrollkatalog konsolidieren**: Verbinde OWASP‑Kontrollen mit ISMS‑Kontrollen (ISO/IEC 27001) und AI‑spezifischen Prozessen (ISO/IEC 42001, 23894).  
3. **Tests & Evidenz**: Adversarial Testpläne, Red‑Team‑Szenarien, Privacy/Bias/Robustness‑Metriken, PMM‑Dashboards (Art. 21).  
4. **Betrieb & Monitoring**: SIEM‑Integration, Alerting auf Prompt‑ und Output‑Anomalien, Model‑Drift und Exfiltrationsindikatoren.  
5. **Nachweisführung**: Verknüpfe jede AI‑Act‑Pflicht mit konkreten Artefakten im Repo (Technische Doku, Logs, Reports, Playbooks).

---

## Beispielhafte Artefakte und Pfade
- **Policies**: `/tools/templates/prompt-security-policy.md`  
- **Testkatalog**: `/tools/checklists/adversarial-test-cases.md`  
- **SBOM/MLSBOM**: `/tools/templates/mlsbom.yaml`  
- **Runbooks**: `/tools/templates/incident-playbook-llm.md`  
- **Monitoring**: Dashboards/Alert-Regeln im Ordner `/tools/`

---

## Commit-Vorschläge (Conventional Commits)
- `docs(standards): add ai act ↔ owasp llm mapping`  
- `feat(security): add adversarial test checklist for owasp llm01-llm10`  
- `chore(compliance): link mapping to lessons and case studies`

