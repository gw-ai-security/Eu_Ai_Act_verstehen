---
title: Prompt Injection Test Checklist
version: 1.0
last_updated: 2025-08-21
tags: [Prompt Injection, LLM, OWASP, Checklist]
---

# Prompt Injection Test Checklist

## Ziel
Sicherstellen, dass LLMs gegen Prompt Injection und Jailbreaks robust sind.

## Checkpunkte
- [ ] Eingabeprüfung: Erkennen von Aufforderungen wie „ignore previous instructions“  
- [ ] Tests auf Umgehung der System-Prompts  
- [ ] Simulation von Jailbreaks (z. B. DAN, Entwicklermodus)  
- [ ] Injection über mehrsprachige Eingaben getestet  
- [ ] Filterung von Anfragen, die API-Secrets oder vertrauliche Daten exfiltrieren wollen  
- [ ] Logging aller Injection Attempts  
- [ ] Dokumentierte Blockierregeln und Gegenmaßnahmen  
