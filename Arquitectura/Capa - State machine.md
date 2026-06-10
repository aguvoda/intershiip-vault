---
tags: [arquitectura, capa]
---
# Capa — State machine

**Los estados solo se atraviesan mediante eventos** ([[Capa - Event log]]). En v0.3 **varias** entidades tienen máquina de estados, no solo el expediente. Cada objeto responde: estado, responsable, bloqueo, siguiente acción.

| Entidad | Estados |
|---|---|
| [[Entidad - ReferralLead\|ReferralLead]] | submitted → pending_review → approved → invited → opened → accepted → registered_limited → sales_qualified → converted_paid · rejected/expired/duplicate/opted_out |
| [[Entidad - MasterOpportunity\|MasterOpportunity]] | draft → ready_for_distribution → distributed → closed · cancelled/archived |
| [[Entidad - DistributionTarget\|DistributionTarget]] | selected → can_publish_now → institutional_posting_created · needs_review/needs_agreement/needs_activation/contact_needed/rejected |
| [[Entidad - InstitutionalPosting\|InstitutionalPosting]] | draft → under_review → needs_changes → published → applications_open → closed · rejected/cancelled |
| [[Entidad - StudentAccount\|StudentAccount]] | self_registered → email_verified → institution_pending_verification → institution_verified → alumni · rejected/deleted |
| [[Entidad - PracticeCase\|PracticeCase]] | created → eligibility_pending → agreement_draft → signature_pending → fully_signed → prestart_checklist_pending → ready_to_start → in_progress → completed → closed · eligibility_failed/prestart_blocked/cancelled/early_terminated |
| [[Entidad - SpecificAgreement\|SpecificAgreement]] | draft → pending_data → pending_review → pending_signature → fully_signed · cancelled |
| [[Entidad - SuccessFeeEvent\|SuccessFeeEvent]] | pending → invoice_ready → invoiced → paid · credited/disputed/cancelled |

> [!note] Stage lineal, readiness paralelo
> Un [[Entidad - PracticeCase|PracticeCase]] avanza en una fase principal, pero firmas, seguro, tutor, horas, fechas y elegibilidad avanzan en paralelo ([[Entidad - PreStartChecklist]]).

Relacionado: [[Modelo de dominio (índice)]] · [[Capa - Event log]]
