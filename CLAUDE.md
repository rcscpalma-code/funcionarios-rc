# funcionarios-rc — Frontend

Asistente jurídico de Registro Civil. Este repositorio contiene **solo el
frontend**: una single-page app en `index.html` más las páginas estáticas
de ayuda y privacidad.

> ⚠️ **Este repositorio es PÚBLICO** (lo exige GitHub Pages en el plan
> gratuito). No añadir aquí credenciales, IDs internos de Drive/Sheets,
> notas de arquitectura, ni documentación de cómo funciona el sistema por
> dentro. Todo eso vive en el repositorio privado del backend.

## Reglas de trabajo en este proyecto

- **Comunicar siempre en castellano**: explicaciones, resúmenes, mensajes
  de commit, nombres de archivos nuevos y comentarios de código. Aunque
  el mensaje llegue en otro idioma, responder y trabajar en castellano.
- **Nunca afirmar un hecho legal** (contenido de un artículo, fechas,
  plazos, reglas de competencia) de memoria ni a partir de un resumen.
  Verificar siempre contra el texto literal del BOE, o con búsqueda web
  citando fuentes. Un dato incorrecto en materia de Registro Civil causa
  perjuicios reales a los interesados.
- **Una tarea a la vez.** No proponer varias mejoras en paralelo sin que
  se pidan.
- **Cambios quirúrgicos en `index.html`.** Es un archivo grande y
  monolítico: editar por búsqueda/reemplazo exacto, nunca regenerarlo
  entero.
- **Verificar la sintaxis antes de entregar** cualquier cambio en el JS
  embebido.

## Contexto que no está aquí

El histórico del proyecto, la arquitectura, el backend (Google Apps
Script) y las decisiones técnicas acumuladas están en el repositorio
privado **`rcscpalma-code/funcionarios-rc-backend-`**, en su `CLAUDE.md`.

**Si la tarea toca el backend, el comportamiento del asistente, o
cualquier cosa más allá de la interfaz, añade primero ese repositorio a
la sesión y lee su `CLAUDE.md` antes de proponer nada.**

## Despliegue

Se publica en GitHub Pages automáticamente al hacer push a `main`:
https://rcscpalma-code.github.io/funcionarios-rc/

Un commit correcto no garantiza que el despliegue haya ido bien —
comprobar la pestaña **Actions** hasta verlo en verde. Ha habido casos de
`build` en verde con `deploy` fallando en silencio (se resuelve con
"Re-run jobs").

## Archivos

| Archivo | Contenido |
|---|---|
| `index.html` | La aplicación completa (UI, lógica de chat, historial, panel de administración) |
| `manual-ayuda-usuario.html` | Manual de usuario, enlazado desde el botón "Ayuda" |
| `privacidad.html` | Política de privacidad |
