---
tags: [diseño, componentes]
---
# Componentes UI

## Primitivas y base (`components.jsx`)
`Hair` (texto hairline mono uppercase), `Mono`, `Btn` (variantes/tamaños/icono), `Input` (label, hint, foco navy), `Badge` (tonos semánticos, soft/solid), **`StatePill`** (píldora de estado del [[Capa - State machine|state machine]]), `Card` (eyebrow + título + acciones), **`DataRow`** (fila: alumno/empresa/programa/estado/actualizado), **`EventRow`** (fila del [[Capa - Event log|event log]]: ts/type/actor/entity/payload).

## Componentes de dominio (`domain-components.jsx`)
`DMSection`, `EntityCard`, `EntityDrawer`, `EntityGrid`, `KindFilter`, `RelationsTable`, `DecisionRow`, **`DomainMap`** (mapa visual de entidades con edges).

## Lienzo (`design-canvas.jsx`)
Canvas tipo Figma: secciones, artboards reordenables (grip-drag), labels editables inline, modo focus fullscreen (←/→/Esc), zoom/pan, persistencia a sidecar `.design-canvas.state.json`. Es **infraestructura para maquetar pantallas**, no pantallas finales.

Relacionado: [[Sistema de diseño]] · [[Modelo de dominio (índice)]]
