---
clipper: notes-ai
type: note
title: Postgres: índices parciales y pool de conexiones
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# Postgres: índices parciales y pool de conexiones

Un índice parcial con WHERE deleted_at IS NULL ocupa una fracción del índice completo y sirve igual, porque casi todas las consultas filtran por ahí de todos modos.

Nota distinta: Postgres reserva memoria por conexión, así que mil conexiones directas lo tumban. Por eso se pone PgBouncer delante y la aplicación abre un pool pequeño.
