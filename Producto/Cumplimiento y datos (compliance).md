---
tags: [producto, compliance, legal]
---
# Cumplimiento y datos (compliance)

> [!warning] Compliance es arquitectura, no back-office
> El flywheel depende de **importar, invitar y activar contactos profesionales** entre instituciones. Las notas legales son riesgos de producto, **no asesoría**: validar con abogado antes de lanzar.

## Principios de import de contactos
- Cada [[Entidad - ImportedContact|contacto importado]] con: actor fuente, timestamp, contexto de relación y propósito.
- **Importar no dispara invitaciones automáticas** → paso de revisión/aprobación obligatorio.
- Cada [[Entidad - Invitation|invitación]] con contexto claro, identidad del emisor, motivo y opt-out.
- do-not-contact / bounced / wrong-person / opted-out = estados de **sistema**, no notas.
- Minimización de datos: solo campos de contacto profesional necesarios.

## Notas legales (España/UE) — validar con counsel
- **Datos de contacto profesional:** la AEPD/LOPDGDD presume interés legítimo bajo condiciones (solo datos profesionales necesarios; fin = mantener relación con la entidad). No es permiso general para uso comercial no relacionado.
- **Interés legítimo:** EDPB Guidelines 1/2024 art. 6(1)(f) RGPD → evaluación estructurada (interés, necesidad, balance). Documentar antes de lanzar.
- **Comunicaciones electrónicas:** LSSI (Ley 34/2002, art. 21) es estricta → decidir si cada invitación es operativa/institucional/comercial y diseñar copy, emisor y opt-out en consecuencia.
- **Seguridad Social:** desde 1-ene-2024 los alumnos en prácticas (remuneradas o no) están incluidos en la Seguridad Social → refuerza el [[Entidad - PreStartChecklist|checklist de readiness]] aunque no haya automatización en MVP.

## Campos mínimos de compliance
ImportedContact: source_actor, uploaded_by, source_file, relationship_context, purpose, opt_out_status. · Invitation: template_id, sender_context, legal_basis_tag, opt_out_link, timestamps. · ReferralLead: referrer, target_contact, referral_reason, review_status, assigned_owner. · StudentAccount: consent/version, verification_status, data_source, deletion_request. · PracticeCase: eligibility, agreement, signature, pre-start, audit log.

## Riesgos principales
percepción de spam · pérdida de control de la universidad · bypass · ambigüedad de base legal · MVP bloat. Mitigaciones en [[MVP v0.3]] y [[Distribución MasterOpportunity vs InstitutionalPosting]].

Relacionado: [[Entidad - AttributionEvent]] · [[Agente - Compliance & Audit]] · [[Cuentas, roles y trust levels]]
