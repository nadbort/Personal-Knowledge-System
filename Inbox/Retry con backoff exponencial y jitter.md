---
clipper: notes-ai
type: note
title: Retry con backoff exponencial y jitter
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# Retry con backoff exponencial y jitter

Reintentar a intervalos fijos sincroniza a todos los clientes que fallaron a la vez y vuelve a tumbar el servicio justo cuando se estaba recuperando. El backoff exponencial separa los reintentos, y el jitter los desordena.

```python
for intento in range(5):
    try:
        return llamar()
    except TransitorioError:
        espera = min(2 ** intento, 30) * random.uniform(0.5, 1.5)
        time.sleep(espera)
raise
```

Sin el jitter, el backoff solo retrasa la avalancha en vez de disolverla.
