---
title: Prompt Security Policy (LLM)
version: 1.0
last_updated: 2025-08-21
tags: [Prompt Injection, OWASP, LLM, Security Policy]
---

# Prompt Security Policy

## Zweck
Diese Policy definiert Regeln zum Schutz von LLM-Systemen vor **Prompt Injection**, **Jailbreaks** und **unsicheren Eingaben**.

## Geltungsbereich
- Alle KI-gestützten Chatbots, Assistenten und LLM-APIs.
- Eingaben von internen und externen Nutzern.

## Policy-Regeln
1. **Input Validation:**  
   - Alle Eingaben werden auf verdächtige Muster geprüft (z. B. „ignore previous instructions“, „system prompt disclosure“).
2. **Context Isolation:**  
   - Training-/System-Prompts sind getrennt von User Prompts zu behandeln.
3. **Output Filtering:**  
   - Modellantworten werden auf potenziell schädliche Inhalte geprüft (XSS, SQL-Injection).
4. **Access Control:**  
   - Sensible Informationen (Secrets, PII) dürfen nicht über Prompts preisgegeben werden.
5. **Testing & Red Teaming:**  
   - Regelmäßige Tests auf Injection-Resilienz (OWASP LLM01).

## Verantwortlichkeiten
- **AI Security Team:** Umsetzung technischer Controls.
- **DevOps/MLOps:** Integration in Pipelines.
- **Compliance Officer:** Überprüfung auf AI Act Art. 15 & 52.

## Nachweise
- Red Team Reports
- Blockierte Injection Attempts (Logs)
- Dokumentierte Sicherheitsrichtlinien
