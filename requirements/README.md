# Requerimientos & Historias

Esta carpeta es la **Verdad Funcional** del proyecto. Se encarga de traducir la **Visión** (`knowledge/`) en pedazos accionables de software.

## 🎯 Objetivo
Separar el **"Qué"** (Requerimientos) del **"Cómo"** (Arquitectura Técnica). Esto permite que la IA entienda perfectamente qué funcionalidades debe implementar y probar antes de escribir una sola línea de código.

---

## 🏗️ Jerarquía Funcional

### 📂 [epics/](file:///Users/jesusbarros/Documents/GitHub/project_template_ai/requirements/epics/)
Agrupaciones lógicas de alto nivel. Una épica representa una característica grande o un módulo completo (ej: *Gestión de Usuarios*, *Dashboard de Analíticas*).

### 📂 [stories/](file:///Users/jesusbarros/Documents/GitHub/project_template_ai/requirements/stories/)
Unidades atómicas de valor para el usuario. Siguen el formato **STORY-XXX.md**. Cada historia debe ser lo suficientemente pequeña para implementarse de forma independiente.

---

## 🤖 Uso para el Agente de IA

El agente debe validar cada cambio contra la historia de usuario activa en este directorio:

1.  **Contexto**: Lee la épica y la historia antes de empezar.
2.  **Pruebas**: Los **Criterios de Aceptación** de la historia mandan sobre los tests unitarios e integrales.
3.  **Definition of Done (DoD)**: Una historia solo está terminada si cumple todos los criterios definidos en su archivo `.md`.

---

> [!TIP]
> Mantener las historias en archivos individuales permite que la IA cargue solo el contexto necesario para la tarea actual, evitando el **"Context Bloat"** y mejorando la precisión.
