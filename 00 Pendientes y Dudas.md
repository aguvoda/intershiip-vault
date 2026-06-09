---
tags: [pendiente, indice]
---
# ⚠️ Pendientes y dudas (centralizado)

> [!warning] Cómo usar esta nota
> Registro único de lo que está **sin definir o en tensión**. Lo cerrado baja a **✅ Resueltos** con fecha y decisión.
> Última actualización: 2026-06-09

## 🔴 Bloqueantes
- [x] ~~**Naming de marca**~~ → **RESUELTO**: `Internshiip.com`. Ver [[Naming de marca (pendiente)]].
- [x] ~~**Memo ↔ dominio**~~ → **RESUELTO**: fuente de verdad = **modelo de dominio actual** ([[Entidad - Opportunity|Opportunity]] como puerta de entrada). Ver [[Modelo de dominio (índice)]].
- [ ] **Pricing** → **APLAZADO** (se define más adelante). Ver [[Pricing]].

## 🟠 Decisiones de arquitectura (todas cerradas salvo dual)
- [x] ~~[[D-01 Opportunity polimórfica]]~~ → **RESUELTO**: Opportunity entidad única = una oferta, **sin subtipos**.
- [x] ~~[[D-02 Tutor rol global vs por programa]]~~ → **RESUELTO**: tutor **por programa**.
- [x] ~~[[D-03 Empresas globales vs por tenant]]~~ → **RESUELTO**: **perfil global**.
- [x] ~~[[D-04 Application por intento vs MatchThread]]~~ → **RESUELTO**: Application atómica + **[[Entidad - MatchThread|MatchThread]]**.
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
- [ ] **T1 — Esquemas de subentidades pendientes:** `AuditCase`, `AgreementTemplate`, `RubricTemplate`. _(Descartadas: `TutorDelegation`, `TFGProposal`, `OrganizationTenantLink`. Definida: `MatchThread`.)_
- [x] ~~**T2 — Stack final**~~ → **RESUELTO**: .NET 10 / Next.js (Vercel) / Flutter / PostgreSQL / Azure. Ver [[Stack técnico]].
- [ ] **T3 — RBAC permisos finos por rol** — sin definir.

## ✅ Resueltos (2026-06-09)
- **B1 Naming** → `Internshiip.com`.
- **B2 Fuente de verdad** → modelo de dominio actual (Opportunity = puerta de entrada).
- **D-01 Opportunity** → entidad única "una oferta", sin subtipos.
- **D-02 Tutor** → por programa.
- **D-03 Empresas** → perfil global.
- **D-04 Candidaturas** → Application atómica + MatchThread.
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
- **Pricing** (aplazado) · **D-09 Formación dual** (diferida) · **T1** esquemas de plantillas/AuditCase · **T3** RBAC fino · duda menor: ¿[[Javier (CETT)|Javier]] = [[Xavi (CEO)|Xavi]]?
