# Changelog

Todas las versiones siguen el formato [SemVer].

## [v1.0.0] - 2025-10-03
### Añadido
- **Header·Vulnerabilidades — Excalibur**: herramienta 100% offline para mapear vulnerabilidades ↔ encabezados HTTP.
- Tres grandes secciones:
  - **Cliente**: Open Redirect → Location, CSRF → SameSite, CORS → Access-Control-Allow-Origin, etc.
  - **Servidor**: SSRF → Content-Type, IDOR → Authorization, CRLF → Transfer-Encoding, etc.
  - **Otras**: API Key Leaks → Authorization / X-API-Key, S3 → ACAO, Session Fixation → Set-Cookie, etc.
- **Buscador global** por nombre de vulnerabilidad, encabezado o resumen táctico.
- Alta masiva de vulnerabilidades (`Nombre: encabezado – resumen` o una por línea).
- Tablas editables con scroll suave, resaltado automático y navegación instantánea.
- Exportación / Importación en formato JSON para compartir o versionar tu checklist.
- **Resumen táctico** por cada vulnerabilidad, ideal para reportes rápidos.
- Interfaz minimalista y directa: tema oscuro, tabla única HTML, sin dependencias externas.
- Persistencia opcional con `localStorage`.

### Cambiado
- N/A — versión inicial.

### Corregido
- N/A — versión inicial.

### Notas
- Licencia: MIT.
- 100% offline. HTML plano, sin backend ni conexión a Internet.
- Datos en memoria por defecto; opcional guardar en `localStorage`.
