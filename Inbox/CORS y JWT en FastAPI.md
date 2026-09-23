---
clipper: notes-ai
type: note
title: CORS y JWT en FastAPI
source: nota rápida
created: 2026-09-21
tags:
  - fleeting
test: true
---

# CORS y JWT en FastAPI

Para configurar el middleware en FastAPI se usa add_middleware(CORSMiddleware) pero dio error de headers al usar wildcard con credenciales. Resulta que allow_origins=["*"] no es válido si allow_credentials=True: hay que listar los orígenes explícitamente.

Aparte de eso, decidimos que el refresh token vaya en una cookie HttpOnly y el access token en memoria, nunca en localStorage, porque cualquier XSS lo leería.
