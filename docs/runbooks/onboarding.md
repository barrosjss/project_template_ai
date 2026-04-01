# Runbook: Onboarding del Proyecto

Este documento guía a un nuevo desarrollador (o una nueva IA) para poner en marcha el proyecto en su entorno local.

## 📋 Requisitos Previos
- Node.js >= 18
- Docker Desktop (opcional para DB local)
- [Cualquier otra dependencia]

## 🛠️ Configuración Inicial
1. **Clonar Repo**: `git clone [url]`
2. **Instalar Dependencias**: `npm install`
3. **Variables de Entorno**: Copiar `.env.example` a `.env` y configurar.
4. **Base de Datos**: `npm run db:up`

## 🏃 Ejecución
- Iniciar el servidor: `npm run dev`
- Ejecutar tests: `npm test`

---

> [!CAUTION]
> Asegúrate de no subir secretos al repositorio. Usa el gestor de secretos de tu elección.
