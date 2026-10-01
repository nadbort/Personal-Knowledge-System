---
type: zettel
title: "El bucle agéntico: prompt, planificar, usar herramientas, evaluar, repetir"
aliases:
  - Bucle agéntico
  - "Agente de código: proceso de resolución"
created: 2026-10-01
tags:
  - clipping/video
source_url: https://www.udemy.com/course/curso-completo-de-claude-code-crea-aplicaciones-con-ia/learn/lecture/55373327
origen: "Curso Completo de Claude Code: Crea Aplicaciones con IA - 3. ¿Qué es Claude Code y por qué es diferente?"
---

# El bucle agéntico: prompt, planificar, usar herramientas, evaluar, repetir

Un bucle agéntico es el proceso que utiliza un agente de código para resolver el problema de un usuario. Consta de cinco fases:

1. **Prompt**: comienza con un mensaje del usuario describiendo qué se quiere hacer y cuál es el resultado esperado.
2. **Planifica**: el agente con esa información comienza a planificar y decidir cuáles son los pasos para resolver ese problema.
3. **Herramienta**: utiliza sus herramientas para leer, editar, crear, ejecutar bash y otros comandos si es necesario.
4. **Evalúa**: analiza si es el resultado esperado por el usuario, haciendo tests.
5. **¿Listo?**: el agente se pregunta si es el resultado esperado. Si lo es, responde al usuario diciendo que es el resultado esperado; si no lo es, se repite y vuelve a la fase de herramientas.

<!-- notes-ai:contexto-tecnico -->
> [!tip] Contexto Técnico Asistido
> **Sintaxis y parámetros**
> El **bucle agéntico** es el ciclo que Claude Code sigue para resolver una tarea: **prompt** del usuario, **planificación**, uso de **herramientas** para leer/editar/crear/ejecutar comandos, **evaluación** del resultado y repetición hasta completar la tarea. La documentación lo resume como un ciclo de **recopilar contexto**, **tomar acción** y **verificar resultados**. En el SDK se describe explícitamente como: evaluar el prompt, llamar herramientas, recibir resultados y repetir hasta terminar.
>
> ```text
> prompt -> planificar -> usar herramientas -> evaluar -> repetir
> ```
>
> **Prerrequisitos**
> Requiere un entorno donde el agente pueda acceder a herramientas y contexto; la documentación oficial lo sitúa sobre el modelo y las herramientas del entorno. No se indica una versión mínima en las páginas consultadas.
>
> **Errores comunes**
> Un fallo frecuente es asumir que el ciclo termina tras la primera acción: la documentación insiste en que el agente repite mientras no obtenga un resultado final correcto. También puede fallar si no hay herramientas disponibles o si el contexto es insuficiente para decidir el siguiente paso.
>
> **Documentación**
> - [How Claude Code works - Claude Code Docs](<https://code.claude.com/docs/en/how-claude-code-works>)
> - [How the agent loop works - Claude Code Docs](<https://code.claude.com/docs/en/agent-sdk/agent-loop>)
> - [Glossary - Claude Code Docs](<https://code.claude.com/docs/en/glossary>)
<!-- /notes-ai:contexto-tecnico -->

<!-- notes-ai:pregunta -->
## Pregunta

> [!question] ¿Cómo podrías aplicar este bucle agéntico para automatizar una tarea repetitiva en tu proyecto actual?
<!-- /notes-ai:pregunta -->

<!-- notes-ai:conexiones -->
## Conexiones

- [[Permanent Notes/Claude Code es un agente, no un chatbot ni un copilot|Claude Code es un agente, no un chatbot ni un copilot]] — surgió de la misma nota de bandeja
<!-- /notes-ai:conexiones -->
