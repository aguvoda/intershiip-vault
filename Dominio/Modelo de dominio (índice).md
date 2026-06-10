---
tags: [dominio, moc, core]
---
# Modelo de dominio (índice)

> [!check] Fuente de verdad (2026-06-10) — v0.3 "Relationship Flywheel"
> El dominio se reorganiza en **8 capas**. El cambio central: ya no empieza en una oferta, empieza en un **contacto** y la **relación institucional** detrás. La oferta se separa en [[Entidad - MasterOpportunity|MasterOpportunity]] (empresa, una vez) e [[Entidad - InstitutionalPosting|InstitutionalPosting]] (institución, controla). La práctica legal es [[Entidad - PracticeCase|PracticeCase]]. Sustituye al modelo v0.2 (Opportunity única / InternshipRecord / MatchThread).

## Cadena ejecutiva mínima (debe quedar trazable)
Contacto → [[Entidad - ReferralLead|ReferralLead]] → [[Entidad - Invitation|Invitation]] → Account → [[Entidad - InstitutionalRelationship|InstitutionalRelationship]] → [[Entidad - MasterOpportunity|MasterOpportunity]] → [[Entidad - InstitutionalPosting|InstitutionalPosting]] → [[Entidad - Application|Application]] → [[Entidad - PracticeCase|PracticeCase]] → [[Entidad - SpecificAgreement|SpecificAgreement]] (fully_signed) → [[Entidad - SuccessFeeEvent|SuccessFeeEvent]] → [[Entidad - ReferralReward|ReferralReward]] / expansión de red.

## Entidades por capa
1. **Network activation** — [[Entidad - ContactImport|ContactImport]] · [[Entidad - ImportedContact|ImportedContact]] · [[Entidad - ReferralLead|ReferralLead]] · [[Entidad - Invitation|Invitation]] · [[Entidad - AttributionEvent|AttributionEvent]] · [[Entidad - InternalAlert|InternalAlert]]
2. **Relationship** — [[Entidad - InstitutionalRelationship|InstitutionalRelationship]] · [[Entidad - RelationshipActivity|RelationshipActivity]] · RelationshipHealthScore *(fase 2 → [[Entidad - Avanzadas (fase 2)]])*
3. **University structure** — [[Entidad - University|University]] · [[Entidad - AcademicUnit|AcademicUnit]] · [[Entidad - AcademicProgram|AcademicProgram]] · [[Entidad - PracticePolicy|PracticePolicy]]
4. **Company structure** — [[Entidad - Organization|Organization]] · [[Entidad - LegalEntity|LegalEntity]] · [[Entidad - Site|Site]] · [[Entidad - AuthorizedSigner|AuthorizedSigner]]
5. **Opportunity distribution** — [[Entidad - MasterOpportunity|MasterOpportunity]] · [[Entidad - DistributionTarget|DistributionTarget]] · [[Entidad - InstitutionalPosting|InstitutionalPosting]] · [[Entidad - SuggestedInstitution|SuggestedInstitution]] · [[Entidad - InstitutionContact|InstitutionContact]] · [[Entidad - CompanyInterest|CompanyInterest]]
6. **Student access** — [[Entidad - Person|Person]] · [[Entidad - StudentAccount|StudentAccount]] · [[Entidad - UniversityEnrollment|UniversityEnrollment]] · [[Entidad - StudentInterest|StudentInterest]] · [[Entidad - Application|Application]]
7. **Practice operations** — [[Entidad - PracticeCase|PracticeCase]] · [[Entidad - SpecificAgreement|SpecificAgreement]] · [[Entidad - SignatureRequest|SignatureRequest]] · [[Entidad - PreStartChecklist|PreStartChecklist]]
8. **Revenue & reward** — [[Entidad - SuccessFeeEvent|SuccessFeeEvent]] · [[Entidad - ReferralReward|ReferralReward]]

**Avanzadas (fase 2):** HoursRecord, Incident, Addendum, Evaluation, Certificate, EmploymentOutcome, RelationshipHealthScore, FrameworkAgreement → [[Entidad - Avanzadas (fase 2)]].

## Reglas de separación (no mezclar)
Lead ≠ Contact ≠ Account ≠ Relationship. Mezclarlos rompe producto, compliance, atribución y UX. **Importar ≠ invitar ≠ activo ≠ pagable.** Discovery puede ser público; la **aplicación formal exige verificación institucional**.

## Terminología
| Término | Definición |
|---|---|
| Lead | Señal de relación/cuenta potencial, aún no activada |
| Contact | Persona con datos de contacto profesional. No es una cuenta |
| Account | Entidad que puede operar a algún nivel de permiso |
| MasterOpportunity | Oferta creada por empresa, para distribución |
| InstitutionalPosting | Publicación específica de una institución derivada de la oferta madre |
| StudentInterest | Interés no formal de alumno no verificado |
| Application | Candidatura formal de alumno verificado |
| PracticeCase | Expediente legal-operativo de prácticas |
| SpecificAgreement | Convenio específico ligado al PracticeCase |
| SuccessFeeEvent | Evento de facturación por práctica firmada |

Mapa de relaciones: [[Relaciones del dominio]] · estados: [[Capa - State machine]] · monetización: [[Modelo de monetización]] · decisiones: [[00 Pendientes y Dudas]]
