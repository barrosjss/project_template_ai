# Project Template AI (v2)

Este es un repositorio de **plantilla (template)** diseñado para proyectos de desarrollo humano-IA altamente eficientes. Su arquitectura se basa en el paper **arXiv:2602.11988 ("Evaluating AGENTS.md")**, priorizando el minimalismo para evitar el "Context Bloat" que degrada el rendimiento de la IA.

## 📖 Para el Desarrollador (Humano)

### 🚀 Inicio Rápido
1.  Clona este repositorio.
2.  Personaliza los archivos de contexto en el directorio raíz según sea necesario (ver sección de IA abajo).
3.  Consulta `docs/runbooks/onboarding.md` para la configuración local.

### 🏗️ Arquitectura del Proyecto
La documentación principal para humanos reside en el directorio `docs/`:
- **`docs/architecture.md`**: El diseño del sistema.
- **`docs/decisions/`**: Por qué se hicieron las cosas de cierta manera (ADR).

---

## 🤖 Para el Agente de IA (Claude, Antigravity, Windsurf)

Este repositorio está optimizado para que las IAs entiendan el contexto **no obvio** rápidamente:

- **`AGENTS.md`**: La fuente de verdad unificada y definitiva para cualquier agente (Claude, Antigravity, Windsurf, Cursor).

> [!IMPORTANT]
> **Minimalismo es clave.** No dupliques información que el agente ya puede deducir leyendo el código o la estructura de archivos (`ls`). Esto reduce costos de tokens y aumenta la precisión del agente.

---

> [!TIP]
> Consulta **`docs/ai_guidelines.md`** para aprender cómo mantener estos archivos de manera efectiva sin degradar el comportamiento de la IA.
