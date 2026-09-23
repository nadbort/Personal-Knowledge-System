---
clipper: notes-ai
type: note
title: Docker: capas y healthcheck
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# Docker: capas y healthcheck

Copiar package.json e instalar dependencias ANTES de copiar el código fuente hace que la capa de node_modules se reutilice entre builds. Si copias todo de golpe, cualquier cambio en el código invalida la caché y reinstala todo.

Otra cosa: sin HEALTHCHECK el orquestador da por sano un contenedor que arrancó pero cuyo proceso está colgado. Un contenedor "up" no significa un servicio que responde.
