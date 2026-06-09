---
tags: [arquitectura, capa, core]
---
# Capa — Policy layer

Cada universidad tiene sus reglas: horas mínimas, documentación obligatoria, secuencia de aprobaciones, SLAs. Se modelan **como datos, no como lógica hardcodeada**.

> [!important] Por qué importa
> Es lo que hace el sistema **escalable** (configurar, no reprogramar, para cada cliente) y una **barrera de salida**: cuanto más personalizado, más difícil de reemplazar ([[Moat (ventaja competitiva)]]).

Entidad asociada: [[Entidad - PolicySet]]. Decisión relacionada de chat: [[D-08 Chat quién inicia con quién]].
