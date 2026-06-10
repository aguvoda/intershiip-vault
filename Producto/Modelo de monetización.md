---
tags: [producto, negocio, monetizacion, core]
---
# Modelo de monetización

Dos motores. Detalle de cifras en [[Pricing]].

| Actor | Gratis / limitado | Disparador de pago | Razón |
|---|---|---|---|
| **Empresa** | registro, perfil, crear/distribuir ofertas, revisar candidatos | **success fee** cuando [[Entidad - SpecificAgreement\|SpecificAgreement]] = `fully_signed` (=práctica activada, 39 €) | reduce fricción, alinea coste a formalización exitosa |
| **Universidad invitada** | reclamar perfil, ver invitación, demo limitada | suscripción para **operar** (publicar, validar, gestionar alumnos) | evita uso pleno gratis, hace accionables los referral leads |
| **Universidad cliente** | — | **suscripción anual** (School/Institution/Pro/Enterprise) + módulos premium | tiene el mayor dolor operativo y rol de control |
| **Alumno** | auto-registro, discovery, interés | sin fee directo | la demanda es señal de crecimiento, no monetización |

## Disparador del success fee
Cobrar a la empresa en `SpecificAgreement.status = fully_signed`. Más auditable que "candidato seleccionado", más cercano al valor que "oferta publicada". Atado a PracticeCase + empresa + universidad + convenio + timestamp. **Siempre crear [[Entidad - SuccessFeeEvent|SuccessFeeEvent]]** aunque la factura sea manual.

## Reglas de referral reward
Empresa→universidad: reward cuando la universidad **paga**. Universidad→empresa: reward cuando hay primera práctica **firmada**. Cadena indirecta: solo referrer directo en MVP. Rewards **solo** sobre conversión de pago o práctica firmada (evita gaming).

## Premium (Enterprise)
No se justifica por más usuarios sino por **complejidad absorbida**: multi-campus/unit, políticas por programa, integraciones (SIS/LMS/SSO/firma/BI), compliance dashboard, auditoría, reporting de acreditación, CS dedicado.

## Riesgos de monetización
Bypass (cerrar fuera) → hacer PracticeCase/firma/reporting valiosos para quedarse dentro · cuenta limitada demasiado generosa → muestra demanda pero no opera · success fee tardío → emparejar con suscripción universidad · rewards prematuros → solo en conversión · calidad de postings gratis → revisión institucional + trust + rate limits.

Relacionado: [[Pricing]] · [[Modelo RaaS]] · [[Relationship flywheel]] · [[Cuentas, roles y trust levels]]
