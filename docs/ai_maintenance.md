# Guía de Mantenimiento de IA (v2)

Esta guía se basa en las mejores prácticas del estudio **arXiv:2602.11988 ("Evaluating AGENTS.md")**, diseñadas para mantener la eficiencia de la IA y reducir costos.

## 🚫 Qué NO Incluir en Contexto de IA
- **Estructura de Directorios**: La IA ya puede ver (`ls -R`). No repitas esta información.
- **Resumen del README**: La IA ya lo lee como punto de entrada.
- **Estándares de Codificación Obvios**: No digas "usa indentación" si el código ya la tiene.
- **Contexto autogenerado por IA**: Si pides a una IA que escriba su contexto, tiende a ser redundante y confuso. **Escríbelo tú mismo (humano).**

## ✅ Qué SÍ Incluir
- **Decisiones de Arquitectura "Ocultas"**: Patrones que no son obvios a primera vista.
- **Límites de Migración**: "No toques la carpeta A porque migraremos a B el próximo mes".
- **Fuentes de Autoridad**: "Si la documentación dice X y el código dice Y, confía en el código (o en el ADR Z)".
- **Restricciones de Negocio**: "Este endpoint debe ser síncrono por la regulación A".

## 🛡️ Prevención de "Context Bloat"
1.  **Limpieza Mensual**: Revisa `CLAUDE.md`, `ANTIGRAVITY.md` y `WINDSURF.md`. Si una regla ya se ha vuelto natural en el código, bórrala del archivo de contexto.
2.  **Audit de Costos**: Si notas que las respuestas de la IA se vuelven lentas o repetitivas, reduce el tamaño de estos archivos. El minimalismo es poder.
3.  **Local Context**: Usa `CLAUDE.md` locales en subdirectorios solo si las reglas de ese módulo son muy distintas a las globales.

---

> [!CAUTION]
> Un archivo de contexto obsoleto es peor que no tener nada. La IA confiará en él y romperá el código actual.
