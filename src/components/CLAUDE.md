# Contexto Local: Componentes de UI

Este archivo rige las reglas de desarrollo dentro de la carpeta `src/components/`.

## 🎨 Principios de Diseño
- Usa **diseño atómico**.
- Si un componente tiene más de 100 líneas, sepáralo en sub-componentes.
- Usa **Composition Patterns** en lugar de herencia.

## 🧱 Estructura de Componente
Cada componente debe tener:
1. `index.tsx` (Lógica principal).
2. `styles.css` (Estilos encapsulados).
3. `test.spec.tsx` (Pruebas unitarias).

## 🚀 Reglas Específicas
- No uses `useEffect` si la lógica puede resolverse con `useMemo`.
- Mantén las Props documentadas con JSDoc.

---

> [!IMPORTANT]
> Estas reglas sobreescriben o complementan el `CLAUDE.md` del root para esta carpeta específica.
