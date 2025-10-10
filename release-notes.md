# Release Notes — v1.0.0 (2025-10-03)

## Resumen
Primera versión de **Header·Vulnerabilidades — Excalibur**, un visor/gestor web 100% offline para mapear rápidamente vulnerabilidades con sus encabezados HTTP relacionados.  
La herramienta conecta findings comunes (Open Redirect, CSRF, SSRF, XXE, XSS, etc.) con el header asociado y un resumen táctico, en un solo panel navegable, rápido y sin conexión.

## Problema que resuelve
En bug bounty, el vínculo entre vulnerabilidad y encabezado suele estar disperso entre wikis, RFC, blogs o notas sueltas. Esto ralentiza el análisis y el reporte.  
Excalibur resuelve ese caos con un **hub offline navegable** que conecta tipo de vulnerabilidad, header y resumen explicativo. Resultado: menos pestañas abiertas, más impacto y velocidad en tus reportes.

## Qué aporta
- 🧠 **Mapa mental inmediato**: tablas por Cliente, Servidor y Otras vulnerabilidades con el header relevante y explicación corta.
- ⚡ **Búsqueda instantánea**: filtra por nombre, encabezado o resumen con scroll suave y resaltado automático.
- 🛡️ **Privacidad y resiliencia**: 100% offline, sin backend. Persistencia opcional con `localStorage`.
- 📋 **Listo para reportar**: cada fila incluye resumen táctico para facilitar la redacción de informes sin salir de la herramienta.

## Características destacadas
- **Secciones principales**:
  - Cliente: Open Redirect → Location, CSRF → SameSite, CORS → ACAO, Cookies → Set-Cookie, XXE → Content-Type, etc.
  - Servidor: SSRF → Content-Type, IDOR/ATO → Authorization, CRLF/Smuggling → Transfer-Encoding, Race Conditions → Authorization, etc.
  - Otras: API Key Leaks → X-API-Key, Reverse Proxy Bypass → X-Forwarded-*, Session Fixation → Set-Cookie, etc.
- **Alta masiva**: carga rápida de vulnerabilidades (una por línea o `Nombre: encabezado – resumen`).
- **Buscador global**: panel fijo superior o lateral, con salto directo al primer resultado.
- **Exportar / Importar JSON**: comparte tu checklist o restaura un pack completo.
- **Resumen táctico** en cada fila: explicación rápida lista para copy-paste en reportes.

## Uso rápido
1. Abre el archivo `.html` en tu navegador.
2. Elegí la sección (Cliente / Servidor / Otras).
3. Usá el buscador para encontrar por nombre, encabezado o resumen.
4. Exportá tu checklist en JSON o importá uno existente.
5. (Opcional) Activá persistencia con `localStorage`.

## Interfaz
- Tema oscuro minimalista.
- Tabla principal con scroll suave y resaltado.
- Panel superior o lateral con buscador global.

## Roadmap futuro
- 🧪 Añadir enlaces a documentación oficial (RFC, OWASP, etc.) desde cada fila.
- 📊 Estadísticas de uso por categoría.
- 🧠 Sugerencias automáticas de encabezados relacionados.

## Licencia
- MIT — Uso responsable y legal únicamente.

---

*"Excalibur — tu mapa de vulnerabilidades y encabezados. Búscalo. Offline, al toque."*
