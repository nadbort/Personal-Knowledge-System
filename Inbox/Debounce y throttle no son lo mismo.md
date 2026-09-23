---
clipper: notes-ai
type: note
title: Debounce y throttle no son lo mismo
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# Debounce y throttle no son lo mismo

Debounce espera a que pare la ráfaga y ejecuta una sola vez al final: sirve para un buscador que no debe consultar en cada tecla.

Throttle ejecuta como mucho una vez cada X milisegundos durante la ráfaga: sirve para el scroll, donde quieres actualizar mientras ocurre pero no en cada píxel.
