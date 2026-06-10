---
tags: [producto, workflows]
---
# Workflows canónicos

Los 6 flujos que vertebran PRD, tickets y prototipo. Todo lo de fuera es fase 2 salvo que sea necesario para probar el loop. Mapean a las **6 pantallas MVP**.

**A — Universidad importa red de empresas:** abrir "Activar red" → subir Excel (empresa, email, rol, contexto) → mapear columnas, marcar faltantes → deduplicar contra contactos/empresas/do-not-contact → revisar y aprobar invitaciones → enviar invitaciones contextuales + tracking → contactos aceptados = cuentas/leads de empresa.

**B — Empresa recibe invitación:** mensaje anclado en la relación ("CETT te ha invitado…") → crea cuenta free → completa perfil mínimo (legal entity, site, contacto) → primera tarea: crear/revisar [[Entidad - MasterOpportunity|MasterOpportunity]].

**C — Empresa crea y distribuye MasterOpportunity:** crea una vez → sistema sugiere instituciones activas/potenciales → empresa selecciona targets → activos: crear [[Entidad - InstitutionalPosting]]; inactivos con contacto: [[Entidad - ReferralLead]]; sin contacto: [[Entidad - CompanyInterest]] + alerta → resumen de estado de distribución.

**D — Revisión de InstitutionalPosting:** universidad recibe posting → sistema chequea relación, convenio/cobertura, unidad y programa → aprueba / pide cambios / rechaza → aprobado = visible en su tablón → empresa ve estado por institución.

**E — Candidatura verificada → PracticeCase:** alumno verificado aplica o universidad lo propone → empresa revisa y selecciona → sistema crea [[Entidad - PracticeCase]] → universidad valida elegibilidad y crea [[Entidad - SpecificAgreement]] → firman empresa/alumno/universidad → `fully_signed` → [[Entidad - SuccessFeeEvent]].

**F — Empresa recomienda universidad:** "Recomendar universidad" → datos de contacto/contexto → [[Entidad - ReferralLead]] (referrer=empresa) → **alerta interna inmediata** → invitación o research → universidad reclama `limited` → ventas convierte a pago → reward de empresa `earned`.

## 6 pantallas MVP
Activar red de empresas (univ) · Landing de invitación (empresa) · Crear MasterOpportunity (empresa) · Revisión de InstitutionalPosting (univ) · Detalle de PracticeCase (univ/empresa/alumno) · Recomendar universidad (empresa).

## Control Center (coordinador)
No es dashboard genérico, es centro de control operativo: nuevas cuentas desde invitaciones · postings esperando revisión · intereses de empresa que requieren research · PracticeCases pendientes de firma · SpecificAgreements firmados (billing) · referrals empresa→universidad · universidades limited en pipeline · rewards pending/earned/applied.

Relacionado: [[Relationship flywheel]] · [[MVP v0.3]] · [[Distribución MasterOpportunity vs InstitutionalPosting]]
