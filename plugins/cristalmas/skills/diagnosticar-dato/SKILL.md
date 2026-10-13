---
name: diagnosticar-dato
description: Diagnosticar y reparar un dato que quedó mal en una base de CRISTAL+ (un comprobante, un saldo, un estado que no cuadra). Usala cuando alguien cuenta que algo se ve mal en pantalla, que un número no cierra o pide una receta de reparación.
---

# Diagnosticar y reparar un dato de CRISTAL+

1. Pedí el método con `metodo_de_trabajo` del conector CRISTAL+, con `metodo: "diagnosticar_dato"`,
   y seguilo tal cual.
2. Qué tablas y campos tocan el caso sale de `buscar_en_modelo`, que lee la base del servidor real;
   los porqués, de `buscar_documentacion`.
3. Toda consulta que propongas primero sólo mira; una reparación va con su guarda, su verificación
   y cómo se deshace. Nunca una escritura que no esté acotada al caso.
4. Si `metodo_de_trabajo` contesta que no hay permiso o `buscar_en_modelo` no está, la cuenta no
   tiene el nivel técnico: decilo y no sigas.
