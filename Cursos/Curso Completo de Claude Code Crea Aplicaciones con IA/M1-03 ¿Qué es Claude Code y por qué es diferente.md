---
clipper: notes-ai
type: lesson
title: ¿Qué es Claude Code y por qué es diferente?
course: "[[Cursos/Curso Completo de Claude Code Crea Aplicaciones con IA/_curso|Curso Completo de Claude Code: Crea Aplicaciones con IA]]"
course_id: udemy-curso-completo-de-claude-code-crea-aplicaciones-con-ia
url: https://www.udemy.com/course/curso-completo-de-claude-code-crea-aplicaciones-con-ia/learn/lecture/55373327
platform: udemy
module: 1
order: 3
status: capturando
created: 2026-09-27T16:43:16.176Z
updated: 2026-10-08T15:42:26.090Z
---

<!-- notes-ai:resumen -->
<!-- /notes-ai:resumen -->

- [0:50](<https://www.udemy.com/course/curso-completo-de-claude-code-crea-aplicaciones-con-ia/learn/lecture/55373327?start=50>) Claude Code se diferencia de un chatbot y un copilot porque Claude code es un agente de codigo que toma decisiones, ejecuta acciones y verifica resultados. <!-- c:8489c39e -->
  ![[Cursos/Curso Completo de Claude Code Crea Aplicaciones con IA/_capturas/Curso Completo de Claude Code Crea Aplic 0-50 df0bb6.jpg]]
- [6:40](<https://www.udemy.com/course/curso-completo-de-claude-code-crea-aplicaciones-con-ia/learn/lecture/55373327?start=400>) Un bucle agentico es el proceso que utiliza un agente de codigo para poder resolver el problema de un usuario. <!-- c:d506562b -->

  1- Prompt: comienza con un mensaje del usuario describiendo que se quiere hacer y cual es el resultado esperado.

  2- Planifica: el agente con esa informacion comienza a planificar y decidir cuales son los pasos para resolver ese problema.

  3- Herramienta: utiliza sus herramientas para leer, editar, crear, ejecuta bash y otros comandos si es necesario

  4- Evalua: Analiza si es el resultado esperado por el usuario, haciendo tests.

  5- Listo? El agente se pregunta si es el resultado esperado, si lo es responde al usuario diciendo que es el resultado esperado, sino lo es se repite y vuelva a la fase de herramientas.
  ![[Cursos/Curso Completo de Claude Code Crea Aplicaciones con IA/_capturas/Curso Completo de Claude Code Crea Aplic 6-40 5b602b.jpg]]

> [!abstract] Idea: Claude Code es un agente, no un chatbot ni un copilot <!-- c:992ce063 -->
> Claude Code se diferencia de un chatbot y de un copilot porque es un **agente de código**: toma decisiones, ejecuta acciones y verifica resultados. Un chatbot solo conversa; un copilot sugiere fragmentos; un agente opera sobre el entorno de desarrollo de forma autónoma.
>
> > [!question] ¿En qué tareas de tu flujo de desarrollo un agente como Claude Code podría tomar decisiones y ejecutar acciones sin tu supervisión constante?

> [!abstract] Idea: El bucle agéntico: prompt, planificar, usar herramientas, evaluar, repetir <!-- c:aa18a16b -->
> Un bucle agéntico es el proceso que utiliza un agente de código para resolver el problema de un usuario. Consta de cinco fases:
>
> 1. **Prompt**: comienza con un mensaje del usuario describiendo qué se quiere hacer y cuál es el resultado esperado.
> 2. **Planifica**: el agente con esa información comienza a planificar y decidir cuáles son los pasos para resolver ese problema.
> 3. **Herramienta**: utiliza sus herramientas para leer, editar, crear, ejecutar bash y otros comandos si es necesario.
> 4. **Evalúa**: analiza si es el resultado esperado por el usuario, haciendo tests.
> 5. **¿Listo?**: el agente se pregunta si es el resultado esperado. Si lo es, responde al usuario diciendo que es el resultado esperado; si no lo es, se repite y vuelve a la fase de herramientas.
>
> > [!tip] Contexto Técnico Asistido
> > **Sintaxis y parámetros**
> > El **bucle agéntico** es el ciclo que Claude Code sigue para resolver una tarea: **prompt** del usuario, **planificación**, uso de **herramientas** para leer/editar/crear/ejecutar comandos, **evaluación** del resultado y repetición hasta completar la tarea. La documentación lo resume como un ciclo de **recopilar contexto**, **tomar acción** y **verificar resultados**. En el SDK se describe explícitamente como: evaluar el prompt, llamar herramientas, recibir resultados y repetir hasta terminar.
> >
> > ```text
> > prompt -> planificar -> usar herramientas -> evaluar -> repetir
> > ```
> >
> > **Prerrequisitos**
> > Requiere un entorno donde el agente pueda acceder a herramientas y contexto; la documentación oficial lo sitúa sobre el modelo y las herramientas del entorno. No se indica una versión mínima en las páginas consultadas.
> >
> > **Errores comunes**
> > Un fallo frecuente es asumir que el ciclo termina tras la primera acción: la documentación insiste en que el agente repite mientras no obtenga un resultado final correcto. También puede fallar si no hay herramientas disponibles o si el contexto es insuficiente para decidir el siguiente paso.
> >
> > **Documentación**
> > - [How Claude Code works - Claude Code Docs](<https://code.claude.com/docs/en/how-claude-code-works>)
> > - [How the agent loop works - Claude Code Docs](<https://code.claude.com/docs/en/agent-sdk/agent-loop>)
> > - [Glossary - Claude Code Docs](<https://code.claude.com/docs/en/glossary>)
>
> > [!question] ¿Cómo podrías aplicar este bucle agéntico para automatizar una tarea repetitiva en tu proyecto actual?

<!-- notes-ai:nav -->
📚 [[Cursos/Curso Completo de Claude Code Crea Aplicaciones con IA/_curso|Curso Completo de Claude Code: Crea Aplicaciones con IA]]
<!-- /notes-ai:nav -->
