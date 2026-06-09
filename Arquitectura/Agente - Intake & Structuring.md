---
tags: [arquitectura, agentes]
---
# Agente — Intake & Structuring

**Activador:** recepción de email, PDF o Word.
**Función:** extrae campos al [[Entidad - InternshipRecord|InternshipRecord]], genera checklist de documentos y propone el estado inicial.

Convierte el caos no estructurado (correos, adjuntos) en datos del [[Capa - Grafo de entidades|grafo]]. Sujeto a los [[Capa - Agent layer|límites estrictos]] (no cambia estado sin humano).
