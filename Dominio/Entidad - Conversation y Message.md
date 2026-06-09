---
tags: [dominio, entidad, engagement]
---
# Conversation y Message · _Conversación / Mensaje_

> [!check] Decisión D-08 (2026-06-09)
> El chat lo inicia **empresa o universidad (Career Service); el alumno nunca inicia**, solo responde. Ver [[D-08 Chat quién inicia con quién]].

> Chat triangular. Reemplaza los 1.000 emails.

## Conversation
Hilo persistente entre 2 o 3 actores. Puede anclarse a un contexto ([[Entidad - Opportunity|Opportunity]], [[Entidad - InternshipRecord|InternshipRecord]], [[Entidad - Application|Application]]) o ser libre. Career Service puede supervisar/unirse (governance).

| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | |
| `tenant_id` | fk → Tenant | |
| `subject` | string? | |
| `context_type` | enum? | opportunity \| application \| internship \| free |
| `context_id` | uuid? | |
| `participants` | fk[] | Membership[] |
| `career_service_watching` | boolean | CS ve sin participar |
| `last_message_at` | timestamp | |

> [!note] Governance
> La supervisión del Career Service es **visible** para los participantes. Nunca chat oculto.

## Message
Texto + adjuntos. Edición limitada (ventana corta). No se borra: se marca como revocado, pero el evento queda.

| Campo | Tipo | Nota |
|---|---|---|
| `id` | uuid | |
| `conversation_id` | fk → Conversation | |
| `author_membership_id` | fk → Membership | |
| `body` | markdown | |
| `attachments` | Document[] | |
| `sent_at` | timestamp | |
| `edited_at` | timestamp? | |
| `revoked` | boolean | |

Relacionado: [[D-08 Chat quién inicia con quién]] · [[Modelo de dominio (índice)]]
