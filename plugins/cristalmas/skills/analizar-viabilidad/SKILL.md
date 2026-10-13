---
name: analizar-viabilidad
description: Analizar si un pedido o una tarea de CRISTAL+ se puede hacer, qué decisiones de arquitectura (ADR) toca y de qué tamaño es. Usala cuando alguien pega un pedido de un cliente, pregunta «¿se puede hacer…?», «¿cuánto lleva…?», «¿qué ADR aplica…?» o pide un análisis de viabilidad.
---

# Analizar la viabilidad de un pedido de CRISTAL+

1. Pedí el método con la herramienta `metodo_de_trabajo` del conector CRISTAL+, con
   `metodo: "analizar_viabilidad"`, y seguilo tal cual: el método vive en el servidor y es el mismo
   que usan los analistas de Digital Express.
2. Buscá y leé los ADR con `buscar_documentacion` (tipo `decision`) y `leer_documento`. Cada
   afirmación lleva su fuente («ADR 0065, Decisión 19»). Lo que no esté documentado va como
   supuesto a validar con desarrollo, nunca como un hecho.
3. Si la herramienta `metodo_de_trabajo` no está, la cuenta no tiene acceso a la documentación
   técnica: decilo y no inventes el análisis.
4. Si al final se decide hacerla y está la herramienta `crear_tarea`: antes buscá con
   `buscar_tareas` si ya hay una parecida, mostrá el resumen y creala sólo cuando la persona lo
   confirme.
