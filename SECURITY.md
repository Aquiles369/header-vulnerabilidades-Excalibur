# Política de seguridad

## 🧠 Resumen

**Header·Vulnerabilidades — Excalibur** es una herramienta web completamente **offline** diseñada para facilitar el mapeo entre vulnerabilidades y encabezados HTTP sin depender de un backend ni conexión a Internet.  
Toda la información vive en memoria del navegador y puede almacenarse opcionalmente en `localStorage`.

---

## 🔒 Principios de seguridad

- **Sin backend:** todos los datos permanecen en tu navegador y nunca salen a servidores externos.
- **Persistencia opcional:** por defecto los datos se mantienen en memoria; se puede activar `localStorage` si se requiere guardar el estado.
- **Exportación controlada:** los datos se exportan/importan manualmente en formato `.json`.
- **Contenido seguro:** todos los datos se procesan como texto plano; no se ejecuta nada del contenido mostrado en tablas o notas.
- **Interfaz segura:** sin uso de `eval()` ni dependencias externas cargadas desde CDNs.
- **Modo laboratorio:** ideal para entornos aislados, auditorías sin conexión y pruebas en laboratorio.

---

## ⚠️ Buenas prácticas recomendadas

- Usar la herramienta en entornos controlados o máquinas locales.
- No guardar información extremadamente sensible en descripciones o campos.
- Revisar siempre el contenido del archivo `.json` antes de compartirlo.
- Eliminar o resetear los datos antes de distribuir la herramienta a terceros.
- Mantener el navegador actualizado con los últimos parches de seguridad.

---

## 🐛 Reporte de vulnerabilidades

Si detectás un comportamiento inesperado o posible vulnerabilidad:

1. No abras un *issue* público.
2. Contactá al autor por mensaje privado (GitHub o Discord).
3. Incluí pasos detallados para reproducir el problema y el entorno utilizado.

Los reportes se revisarán con prioridad.

---

## 🛠️ Alcance del modelo de seguridad

| Área                              | Estado                         |
|----------------------------------|-------------------------------|
| Backend / API                    | ❌ No aplica (no existe)      |
| Base de datos remota            | ❌ No aplica                  |
| Persistencia en memoria         | ✅ Por defecto                |
| Persistencia local (`localStorage`) | ✅ Opcional y segura         |
| Sanitización de contenido       | ✅ Procesado como texto plano |
| Dependencias externas           | ✅ Sin dependencias externas  |
| Exportación / Importación JSON  | ✅ Manual y controlada       |

---

## 🧪 Nota importante

Esta herramienta fue creada para fines **éticos, educativos y legales** en contextos de bug bounty, auditorías web y pentesting. No debe utilizarse sin autorización sobre sistemas en producción.

---

**“Excalibur — conocimiento táctico sin fugas. Tu mapa vuln ↔ header vive en tu navegador.”**
