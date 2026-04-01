# AGENTS.md (Unificado & Minimalista)

Este archivo es la **fuente de verdad suprema** para cualquier agente de IA. No repitas información que ya existe en el código o estructura de carpetas (`ls`). Concéntrate en lo no obvio y las pautas que un humano prioriza.

## 🏛️ Autoridad Técnica y de Negocio
Si tienes dudas sobre el **por qué (negocio)** o el **cómo (técnico)**, consulta:
- `knowledge/vision.md`: Propósito, modelo de negocio e identidad.
- `docs/architecture.md`: Diseño global del sistema.
- `docs/decisions/`: ADRs que explican los "por qués" históricos técnicos.

## 📜 Reglas de Oro (No Obvias)
Aquello que no puedes deducir del código y que los humanos priorizan:
1.  **Migración Progresiva**: No refactorices módulos completos a menos que se solicite; respeta los límites definidos en los ADRs.
2.  **No-Go Zones**: Si una carpeta no está en el `README` principal, trátala como código legado o privado; no la modifiques sin confirmación.
3.  **Patrón de Composición**: Preferimos la composición sobre la herencia; mantén lo minimalista.
4.  **Audit de Contexto**: Como agente, si detectas que una regla en este archivo ya es evidente en el código, bórrala o sugiérelo para reducir "Context Bloat".

## 🛠️ Herramientas y Operaciones
- Consulta el `package.json` para comandos de ejecución (`dev`, `test`, `build`).
- Si usas herramientas de edición (como `multi_replace`), agrúpalas para minimizar el uso de tokens.

---

> [!TIP] 
> Mantén este archivo corto. El minimalismo es poder para una IA (mejor rendimiento y menos costos).
