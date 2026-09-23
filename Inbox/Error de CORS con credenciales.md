---
clipper: notes-ai
type: note
title: Error de CORS con credenciales
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# Error de CORS con credenciales

El navegador rechaza una respuesta con Access-Control-Allow-Origin: * cuando la petición se hizo con credentials: 'include'. No es un fallo del servidor: la especificación lo prohíbe para que una página cualquiera no pueda leer respuestas autenticadas de otro sitio.

La solución es devolver el origen concreto que hizo la petición y añadir Access-Control-Allow-Credentials: true.
