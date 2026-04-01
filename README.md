# AI-Powered Project Template

Este es un repositorio de **plantilla (template)** diseñado para estructurar proyectos de desarrollo potenciados por IA (Claude, Cursor, Antigravity, etc.). Esta arquitectura está optimizada para proporcionar el máximo contexto a los modelos de lenguaje, permitiéndoles ser más precisos y autónomos en la generación de código.

## 🏗️ Arquitectura de Contexto

La estructura del proyecto está organizada para separar el **cerebro** del proyecto (contexto de IA) de la **lógica** de la aplicación:

### 1. `CLAUDE.md` (El Cerebro)
Este archivo es la fuente de verdad absoluta para cualquier IA que trabaje en el repositorio. Contiene:
- Propósito del proyecto.
- Guías de estilo de código (TypeScript, CSS, naming conventions).
- Tecnologías principales.
- Reglas fundamentales que la IA debe seguir sin excepción.

### 2. `docs/` (Base de Conocimiento)
Ubicación para decisiones de diseño y documentación técnica de largo plazo:
- **`architecture.md`**: Descripción del diseño del sistema.
- **`decisions/` (ADR)**: Registro de decisiones de arquitectura con sus motivos (¿Por qué elegimos esta base de datos? ¿Por qué esta librería de estados?).
- **`runbooks/`**: Guías paso a paso para tareas operativas (Despliegue, Onboarding, Troubleshooting).

### 3. `.claude/` (Configuración de IA)
Carpeta para archivos técnicos que interactúan directamente con el motor de la IA:
- **`settings.json`**: Permisos de herramientas y configuraciones específicas del agente.
- **`hooks/`**: Verificaciones automáticas antes/después de ciertas acciones.
- **`skills/`**: Flujos de trabajo específicos (e.g., cómo hacer un code review, cómo refactorizar un componente).

### 4. `tools/` (Herramientas y Prompts)
- **`prompts/`**: Una biblioteca de prompts optimizados para tareas recurrentes.
- **`scripts/`**: Scripts personalizados que ayudan a la IA a realizar tareas complejas (e.g., limpieza de datos, generación de tipos).

### 5. `src/` (Código con Contexto Modular)
El código de la aplicación. Se fomenta el uso de archivos `CLAUDE.md` locales en subdirectorios específicos (e.g., `src/ui/CLAUDE.md`) para proporcionar reglas acotadas a componentes o módulos particulares.

---

## 🚀 Cómo usar esta plantilla

1. **Usa el repo como base**: Clona o utiliza este template para tu nuevo proyecto.
2. **Personaliza `CLAUDE.md`**: Define tus reglas de oro y stack tecnológico.
3. **Documenta tus ADRs**: No pierdas el rastro de por qué tomaste ciertas decisiones; la IA usará esta historia para guiar sus futuras propuestas.
4. **Agrega Skills**: Si encuentras un flujo que funciona bien con la IA, documéntalo en `.claude/skills/` para que sea reproducible.

---

> [!TIP]
> Mantén tus archivos de contexto actualizados. Una IA es tan buena como el contexto que recibe.
