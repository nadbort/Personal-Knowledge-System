---
clipper: notes-ai
type: note
title: Idempotencia en endpoints de pago
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# Idempotencia en endpoints de pago

Un endpoint idempotente devuelve el mismo resultado aunque el cliente reintente la misma petición. Se consigue con una clave de idempotencia que el cliente genera y el servidor guarda junto al resultado.

Sin esto, un reintento por timeout cobra dos veces. El cliente nunca puede saber si el timeout ocurrió antes o después de que el servidor procesara el cobro.
