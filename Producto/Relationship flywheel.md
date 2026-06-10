---
tags: [producto, flywheel, core]
---
# Relationship flywheel

No es un truco viral: es la lógica de producto que convierte relaciones institucionales en crecimiento de red compuesto. Encaja con [[Tesis 1 - Relationship Expansion Engine]].

## Loop 1 — Activación de empresa liderada por universidad (wedge)
1. Universidad importa contactos de empresa (Excel/CRM) → [[Entidad - ContactImport]].
2. Sistema mapea, deduplica → [[Entidad - ImportedContact]] revisables.
3. Universidad **aprueba** a quién invitar (importar ≠ outreach).
4. Empresa recibe invitación contextual ("CETT te ha invitado…").
5. Empresa crea cuenta **gratis** + perfil mínimo (legal entity, site, contacto).
6. Empresa crea [[Entidad - MasterOpportunity|MasterOpportunity]] y la manda a revisión.
7. Universidad recibe [[Entidad - InstitutionalPosting|InstitutionalPosting]], valida y publica en su tablón.
8. Alumnos verificados aplican o son propuestos.
9. Candidato seleccionado → [[Entidad - PracticeCase|PracticeCase]] con convenio, firma y pre-start.
10. [[Entidad - SpecificAgreement|SpecificAgreement]] `fully_signed` → [[Entidad - SuccessFeeEvent|SuccessFeeEvent]].

## Loop 2 — Referral de universidad liderado por empresa
Empresa entiende el valor → recomienda otra universidad → [[Entidad - ReferralLead|ReferralLead]] + [[Entidad - InternalAlert|alerta interna]] inmediata → invitación contextual o research de contacto → universidad reclama cuenta `limited` → ventas la convierte a pago → la empresa gana [[Entidad - ReferralReward|reward]].

## Loop 3 — Captura de demanda de alumno
Alumno ve preview público → busca su universidad → si conectada: tablón institucional; si no: StudentDemandLead/activation request → universidad recibe señal de demanda agregada → el alumno puede verificarse después. Discovery público, **aplicación formal institucional**.

> [!note] Cada relación activada deja trazabilidad (quién originó, quién invitó, quién aceptó, qué se publicó, qué se firmó, qué resultado, qué nueva relación). **Ese grafo no se copia fácil: es el [[Moat (ventaja competitiva)|moat]].**

Caso narrativo: CETT → Hotusa → Escuela Galicia. Relacionado: [[Modelo de monetización]] · [[Workflows canónicos]]
