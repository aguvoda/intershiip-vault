---
tags: [producto, mvp, core]
---
# MVP v0.3

> [!note] Objetivo del MVP
> Probar que una universidad puede activar su red de empresas, una empresa crear una oportunidad, la universidad publicarla institucionalmente, un alumno verificado convertirse en [[Entidad - PracticeCase|PracticeCase]] firmado, la empresa ser facturada y la empresa referir otra universidad.

El MVP es **deliberadamente estrecho**: probar el flywheel con un loop de activación liderado por universidad y un loop de referral liderado por empresa. Coherente con [[Estrategia de entrada (GTM)|GTM]] (profundidad / una universidad) y [[Plan de lanzamiento 30 días]].

## Incluido
Activación de red (import Excel, mapeo, dedupe, revisión, aprobación, tracking) · onboarding empresa (invitación contextual, signup free, perfil, legal entity/site) · [[Entidad - MasterOpportunity|MasterOpportunity]] + selección de targets · [[Entidad - InstitutionalPosting|InstitutionalPosting]] (revisar/publicar/rechazar) · verificación de alumno (verificados aplican; auto-registrados solo interés) · [[Entidad - PracticeCase|PracticeCase]] mínimo (estados de convenio/firma/pre-start) · [[Entidad - SuccessFeeEvent|SuccessFeeEvent]] al `fully_signed` · referral de empresa + alertas + cuenta limited · [[Entidad - ReferralReward|reward]] (earned solo en conversión) · admin console (pipeline, alertas, cola contacto, fees, rewards).

## Excluido
Marketplace público completo · aplicación formal de no verificados · voice-first ([[Tesis 5 - Voice-First Student Experience]]) · IA matching más allá de sugerencias simples · integraciones SIS/LMS/SSO profundas ([[Tesis 6 - Integration Infrastructure Layer]]) · automatización Seguridad Social · integración firma completa si el estado manual basta · rewards más allá de 1er nivel · scoring de relación avanzado · app móvil completa · eventos/retos/TFG/TFM ([[D-07 Challenges y TFG]]).

## Guardrails
No sobreconstruir coverage de convenios si la universidad piloto valida manual (mantener hooks de datos) · no automatizar outreach a no-clientes sin revisión · que los previews públicos no se vuelvan job board antes de probar confianza institucional · no pagar rewards antes de que atribución y billing sean fiables · no IA/voz hasta que datos de alumno y verificación estén limpios.

## Criterios de éxito
contactos importados suficientes · aceptación de invitación (ancladas en contexto universidad) · empresas activadas crean ≥1 MasterOpportunity · tasa de aprobación de postings · PracticeCases que llegan a `fully_signed` · cobro de success fee sin fricción mayor · empresas que recomiendan universidades · conversión limited→pago.

## Checklist fatal antes del piloto
¿CETT importa contactos sin enviar emails auto? ¿cada contacto muestra quién lo subió y por qué? ¿Hotusa crea una MasterOpportunity y ve estados de target? ¿CETT aprueba un InstitutionalPosting sin verlo como marketplace? ¿un alumno no verificado expresa interés sin aplicar formal? ¿un PracticeCase llega a `fully_signed` y dispara SuccessFeeEvent? ¿Hotusa recomienda Escuela Galicia y dispara alerta? ¿Escuela Galicia se registra limited sin acceso pleno?

Relacionado: [[Workflows canónicos]] · [[Roadmap 12 meses]] · [[Stack técnico]]
