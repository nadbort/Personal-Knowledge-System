---
clipper: notes-ai
type: note
title: El límite de la paginación por offset
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# El límite de la paginación por offset

LIMIT 20 OFFSET 100000 obliga a la base de datos a recorrer y descartar cien mil filas antes de devolver veinte. El coste crece con el número de página.

La paginación por cursor usa la última clave vista como punto de partida, así que cada página cuesta lo mismo. El precio es perder el salto directo a una página arbitraria.
