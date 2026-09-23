---
clipper: notes-ai
type: note
title: Reunión de ayer y una idea sobre caché
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# Reunión de ayer y una idea sobre caché

Ayer en la reunión de producto se decidió retrasar el rediseño hasta enero. Me quedé con la sensación de que nadie quería decir en voz alta que no llegamos.

Al salir se me ocurrió algo para el problema de rendimiento: cachear por clave compuesta (usuario + versión del documento) en vez de solo por documento invalida solo lo que cambió, y evita el purgado global que tanto nos cuesta.
