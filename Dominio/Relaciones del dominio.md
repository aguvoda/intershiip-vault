---
tags: [dominio, relaciones]
---
# Relaciones del dominio

Cardinalidades y reglas clave del modelo v0.3. Ver [[Modelo de dominio (índice)]].

| Origen | Card. | Destino | Regla |
|---|---|---|---|
| [[Entidad - ContactImport\|ContactImport]] | 1..n | ImportedContact | Importar **no** envía invitaciones automáticas |
| [[Entidad - ImportedContact\|ImportedContact]] | 0..1 | ReferralLead | Solo tras revisión, dedupe y contexto suficiente |
| [[Entidad - ReferralLead\|ReferralLead]] | 0..n | Invitation | Un lead puede recibir varias invitaciones controladas |
| [[Entidad - InstitutionalRelationship\|InstitutionalRelationship]] | 1..n | MasterOpportunity / InstitutionalPosting | La relación es el activo de red; las ofertas son actividad dentro |
| [[Entidad - MasterOpportunity\|MasterOpportunity]] | 1..n | DistributionTarget | Una oferta madre apunta a varias instituciones |
| [[Entidad - DistributionTarget\|DistributionTarget]] | 0..1 | InstitutionalPosting | Solo si `can_publish_now`; si no → ReferralLead / CompanyInterest |
| [[Entidad - MasterOpportunity\|MasterOpportunity]] | 1..n | InstitutionalPosting | Una oferta → muchas publicaciones institucionales |
| [[Entidad - InstitutionalPosting\|InstitutionalPosting]] | 0..n | Application | Solo alumnos **verificados** crean candidaturas formales |
| [[Entidad - StudentAccount\|StudentAccount]] | 0..n | StudentInterest | Interés no formal (no genera candidatura) |
| [[Entidad - Application\|Application]] | 0..1 | PracticeCase | Solo una candidatura **seleccionada** crea PracticeCase |
| [[Entidad - PracticeCase\|PracticeCase]] | 1 | SpecificAgreement | El convenio + firmas = disparador de monetización |
| [[Entidad - SpecificAgreement\|SpecificAgreement]] | 1..n | SignatureRequest | Empresa, alumno y universidad firman por separado |
| SpecificAgreement `fully_signed` | 1 | [[Entidad - SuccessFeeEvent\|SuccessFeeEvent]] | Fee solo al firmar del todo |
| ReferralLead `converted` | 0..1 | [[Entidad - ReferralReward\|ReferralReward]] | Reward por conversión de pago / práctica firmada, no por alta |
| [[Entidad - University\|University]] | 1..n | AcademicUnit → AcademicProgram | Jerarquía anidada |
| [[Entidad - Organization\|Organization]] | 1..n | LegalEntity → Site | Una empresa ≠ un CIF |
| [[Entidad - StudentAccount\|StudentAccount]] | 1..n | UniversityEnrollment | Fuente de verdad de elegibilidad formal |

## Source of truth
- Matrícula y elegibilidad del alumno → controla la **universidad**, no el alumno auto-registrado.
- InstitutionalPosting → controla la **institución**, aunque derive de una MasterOpportunity de empresa.
- SpecificAgreement / PracticeCase → fuente de verdad de la monetización por práctica firmada.
- [[Entidad - AttributionEvent\|AttributionEvent]] → **append-only**, nunca se sobreescribe; los rewards se disputan, la atribución permanece.

Relacionado: [[Modelo de dominio (índice)]] · [[Distribución MasterOpportunity vs InstitutionalPosting]] · [[Capa - State machine]]
