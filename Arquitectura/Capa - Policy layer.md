---
tags: [arquitectura, capa, core]
---
# Capa — Policy layer

Cada universidad tiene sus reglas: horas mínimas, documentación obligatoria, secuencia de aprobaciones, SLAs. Se modelan **como datos, no como lógica hardcodeada**.

> [!important] Por qué importa
> Es lo que hace el sistema **escalable** (configurar, no reprogramar, para cada cliente) y una **barrera de salida**: cuanto más personalizado, más difícil de reemplazar ([[Moat (ventaja competitiva)]]).

> [!note] Jerarquía de override (v0.3)
> Política de **programa** sobreescribe la de **unidad académica**, que sobreescribe la de **universidad**.

Entidad asociada: [[Entidad - PracticePolicy]] (sustituye `PolicySet` v0.2). Permisos por scope: [[Cuentas, roles y trust levels]].
