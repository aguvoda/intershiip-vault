---
tags: [producto, permisos, arquitectura]
---
# Cuentas, roles y trust levels

## Account modes
| Cuenta | Estado | Puede | No puede |
|---|---|---|---|
| **University limited** | limited | reclamar perfil, ver referral, datos básicos, pedir demo | operar prácticas, validar postings reales, invitar en bulk, reporting |
| **University active** | paid active | gestionar estructura, empresas, postings, alumnos verificados, [[Entidad - PracticeCase\|PracticeCases]] | integraciones enterprise (salvo plan) |
| **University premium** | paid premium | multi-unit governance, integraciones, reporting avanzado | — |
| **Company free** | active free | registro, perfil, crear [[Entidad - MasterOpportunity\|MasterOpportunities]], pedir distribución, revisar candidatos | evitar success fee al firmar |
| **Student self-registered** | unverified | perfil, previews, [[Entidad - StudentInterest\|interés]], pedir activación | candidatura formal |
| **Student verified** | institution_verified | aplicar, firmar, reportar, evaluar, certificado | aplicar fuera de su scope |

## Trust levels
`low` = auto-registrado, sin verificar · `medium` = email/dominio institucional confirmado · `high` = importado/invitado/validado por universidad de pago o admin de empresa verificada · `critical` = firmante autorizado, admin universidad, rol sensible a compliance.

## Scopes (permisos siempre acotados)
University → AcademicUnit → AcademicProgram (lado universidad); Organization → LegalEntity → Site (lado empresa). **El producto se rompe en universidades grandes si los permisos son globales por defecto.** Un coordinador de Economía no debería ver Derecho.

## Matriz de permisos (resumen)
Universidad admin: gestiona import/invitación/postings/students/PracticeCase. Coordinador de unidad: lo mismo **scoped**. Empresa admin: crea MasterOpportunity, revisa candidatos, firma, ve sus referrals/fees. Alumno: su perfil, interés, candidatura/firma propias. Internshiip admin: gestiona todo + leads + alertas + fees + rewards.

Relacionado: [[Entidad - University]] · [[Entidad - StudentAccount]] · [[Cumplimiento y datos (compliance)]] · [[D-02 Tutor rol global vs por programa]]
