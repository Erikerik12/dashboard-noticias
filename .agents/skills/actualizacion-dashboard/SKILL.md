---
name: actualizacion-dashboard
description: Actualiza de forma segura la marca de tiempo solicitada en ACTUALIZAR_DESDE_CHAT.md del repositorio Erikerik12/dashboard-noticias y devuelve el enlace del dashboard.
---

# Actualización Dashboard

Cuando se invoque este skill:

1. Trabaja exclusivamente en el repositorio `Erikerik12/dashboard-noticias`, rama `main`.
2. Lee `ACTUALIZAR_DESDE_CHAT.md` desde `main`. No asumas que existe: si falta, detente y solicita que se cree o indique su ubicación. No inventes su contenido.
3. Conserva el contenido íntegro del archivo salvo la única línea que comienza exactamente con `Última solicitud desde tu LLM:`.
4. Obtén la fecha y hora local actual con segundos y zona horaria explícita. Usa formato ISO 8601, por ejemplo `2026-11-18T22:41:49-06:00`.
5. Reemplaza únicamente esa línea con `Última solicitud desde tu LLM: <fecha-hora>`. Si no existe exactamente una línea coincidente, detente y reporta el problema.
6. Actualiza el archivo en `main` usando su SHA actual. No cambies ningún otro contenido o archivo durante esta operación.
7. Verifica en GitHub el commit resultante y vuelve a leer el archivo desde `main` para confirmar el valor guardado. No declares éxito si GitHub rechaza el cambio o la verificación falla.
8. No modifiques nunca `index.html`, `noticias.json`, `actualizar_noticias.py` ni `.github/workflows/actualizar.yml`.
9. Informa el resultado del commit, el valor guardado y el enlace público del dashboard: `https://erikerik12.github.io/dashboard-noticias/`. Aclara que cambiar la marca de tiempo no ejecuta por sí mismo la actualización de noticias ni demuestra que el dashboard se haya actualizado.
