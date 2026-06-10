---
tags: [pendiente, indice]
---
# ⚠️ Pendientes y dudas (centralizado)

> [!warning] Cómo usar esta nota
> Registro único de lo que está **sin definir o en tensión**. Lo cerrado baja a **✅ Resueltos** con fecha y decisión.
> Última actualización: 2026-06-10 · **Dominio migrado a v0.3 (Relationship Flywheel)** — ver [[Modelo operativo v0.3 (índice)]].

## 🔴 Bloqueantes
- [x] ~~**Naming de marca**~~ → **RESUELTO**: `Internshiip.com`. Ver [[Naming de marca (pendiente)]].
- [x] ~~**Memo ↔ dominio**~~ → **RESUELTO**: fuente de verdad = **modelo de dominio v0.3**, organizado por la [[Entidad - InstitutionalRelationship|relación institucional]] (no por una oferta). Ver [[Modelo de dominio (índice)]].
- [x] ~~**Pricing**~~ → **RESUELTO (2026-06-10)**: Product & Pricing Strategy v0.1. Universidad School 13k / Institution 36k / University Pro 72k / Enterprise 150k+; early adopter (Founding Partner) 9.5k/24k/48k; Employer Presence 6k/Engagement 18k/Network 60k+; fee 39 €/práctica activada. Ver [[Pricing]].

## 🟠 Decisiones de arquitectura (todas cerradas salvo dual)
- [x] **Opportunity** → **SUPERADA por v0.3**: se separa en [[Entidad - MasterOpportunity|MasterOpportunity]] (empresa) + [[Entidad - InstitutionalPosting|InstitutionalPosting]] (institución). La vieja D-01 (entidad única) queda eliminada.
- [x] ~~[[D-02 Tutor rol global vs por programa]]~~ → **RESUELTO**: tutor **por programa**.
- [x] ~~[[D-03 Empresas globales vs por tenant]]~~ → **RESUELTO**: **perfil global**.
- [x] **Candidaturas** → **SUPERADA por v0.3**: `MatchThread` se elimina; el trayecto se ve vía [[Entidad - Application|Application]] + [[Entidad - RelationshipActivity|RelationshipActivity]]. La vieja D-04 queda eliminada.
- [x] ~~[[D-05 LMS push vs pull]]~~ → **RESUELTO para MVP**: export manual/CSV; LTI post-MVP.
- [x] ~~[[D-06 Convenio curricular + extracurricular]]~~ → **RESUELTO**: soportar `modality=mixed`.
- [x] ~~[[D-07 Challenges y TFG]]~~ → **RESUELTO**: **eliminados del modelo** (y con ellos la entidad Activity).
- [x] ~~[[D-08 Chat quién inicia con quién]]~~ → **RESUELTO**: inicia empresa o universidad, **nunca el alumno**.
- [ ] [[D-09 Formación dual]] — **DIFERIDA** (sin decidir; fuera del MVP).

## 🟡 Negocio
- [x] ~~**¿CETT es Fase 1?**~~ → **RESUELTO: NO**. Ver [[CETT (cliente piloto)]].
- [x] ~~**Profundidad vs catálogo**~~ → **RESUELTO**: **Palantir (profundidad) guía el MVP**. Ver [[Estrategia de entrada (GTM)]].
- [x] ~~**Voz en MVP**~~ → **RESUELTO**: fuera del MVP. Ver [[Tesis 5 - Voice-First Student Experience]].
- [x] ~~**Kombo / integraciones**~~ → **RESUELTO**: ninguna en la primera versión. Ver [[Tesis 6 - Integration Infrastructure Layer]].

## 🟢 Técnicas
- [ ] **T1 — Entidades fase 2 pendientes de esquema:** ver [[Entidad - Avanzadas (fase 2)]] (Evaluation, Certificate, EmploymentOutcome, HoursRecord, Incident, Addendum, FrameworkAgreement, RelationshipHealthScore). _(Descartadas: `TutorDelegation`, `TFGProposal`, `OrganizationTenantLink`, `MatchThread`, `Activity`.)_
- [x] ~~**T2 — Stack final**~~ → **RESUELTO**: .NET 10 / Next.js (Vercel) / Flutter / PostgreSQL / Azure. Ver [[Stack técnico]].
- [ ] **T3 — RBAC/permisos por scope** — modelo definido en [[Cuentas, roles y trust levels]]; falta detalle fino de implementación.
- [ ] **T4 — Compliance pre-lanzamiento** — base legal de contactos, caracterización de invitaciones (LSSI), readiness Seguridad Social. Ver [[Cumplimiento y datos (compliance)]].

## ✅ Resueltos (2026-06-10)
- **Pricing** → Product & Pricing Strategy v0.1 (School 13k / Institution 36k / University Pro 72k / Enterprise 150k+; early adopter 9.5/24/48k; Employer plans; fee 39 €/práctica). Ver [[Pricing]] · [[Founding Partner Program]] · [[Modelo de monetización]].

## ✅ Resueltos (2026-06-09)
- **B1 Naming** → `Internshiip.com`.
- **B2 Fuente de verdad** → modelo de dominio v0.3 (relación institucional en el centro). _Nota: las decisiones D-01 (Opportunity única) y D-04 (MatchThread) de 2026-06-09 quedaron **superadas** por v0.3 el 2026-06-10._
- **D-02 Tutor** → por programa.
- **D-03 Empresas** → perfil global.
- **D-05 LMS (MVP)** → export manual/CSV; LTI post-MVP.
- **D-06 Convenio** → soportar mixed.
- **D-07 Challenges/TFG** → eliminados del modelo (Activity eliminada).
- **D-08 Chat** → lo inicia empresa o universidad, nunca el alumno.
- **N1 CETT** → no es la Fase 1 oficial.
- **N2 MVP** → guiado por profundidad (Palantir).
- **N3 Voz** → fuera del MVP.
- **N4 Integraciones** → sin Kombo/LMS en MVP.
- **T2 Stack** → .NET 10 / Next.js (Vercel) / Flutter / PostgreSQL / Azure.

## ⏳ Sigue abierto
- **D-09 Formación dual** (diferida) · **T1** esquemas de plantillas/AuditCase · **T3** RBAC fino · duda menor: ¿[[Javier (CETT)|Javier]] = [[Xavi (CEO)|Xavi]]?
