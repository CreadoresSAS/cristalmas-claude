---
name: atender-un-caso
description: "Atender un caso de la mesa de ayuda de CRISTAL+ (un ticket, TKT-#…): leerlo, buscar si ya está resuelto o documentado, dejarle una nota o un borrador de respuesta, o escalarlo a desarrollo como tarea. Usala cuando alguien nombra un caso o un ticket, pega el pedido de «Consultar a Claude» de la bandeja, o pregunta qué contestarle a un cliente que reclamó."
---

# Atender un caso de la mesa de ayuda de CRISTAL+

1. **Leelo entero** con `ver_caso` (el número, sin el «TKT-#»). Si no sabés el número, buscalo con
   `buscar_casos` por texto; para ver qué más reclamó ese cliente, `buscar_casos` con la `cuenta`
   del solicitante. Los adjuntos vienen por nombre: no los podés abrir; si hacen falta, pedile a la
   persona que los mire en CRISTAL+ con el enlace del caso.
2. **Si es sobre un envío o un comprobante** (`sobre`), miralo: `seguir_envio` o `ver_guia` con su
   código de seguimiento.
3. **Buscá si ya está resuelto o documentado** con `buscar_documentacion` (primero las guías; los ADR
   si hay que explicar por qué funciona así) y, si parece un error o un pedido nuevo, `buscar_tareas`
   por si ya se pidió. Si la documentación no lo trae, probá con otras palabras antes de concluir; y
   que no esté documentado **no quiere decir que no esté hecho**.
4. **Dejá lo que encontraste** con `anotar_en_caso`:
   - `nota`: el diagnóstico, interno, con la guía o el ADR de donde sale.
   - `borrador`: la respuesta para el solicitante, en su idioma y sin nombres de tablas ni de campos.
     **No se le manda**: la revisa y la manda quien atiende el caso desde CRISTAL+.
   Antes de guardar, mostrale el texto a la persona y esperá que lo confirme.
5. **Si hace falta desarrollo**: pedí el método `analizar_viabilidad` con `metodo_de_trabajo`, seguilo,
   y si está `crear_tarea`, mostrá la tarea redactada y creala con `caso` cuando la persona lo
   confirme: queda vinculada y el caso pasa a esperar desarrollo.

Nada le llega al cliente desde acá. Si no tenés `ver_caso`, la cuenta no tiene acceso a la bandeja de
casos: decilo.
