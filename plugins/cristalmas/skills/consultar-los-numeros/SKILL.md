---
name: consultar-los-numeros
description: Contestar preguntas con números de CRISTAL+ —cuántas guías, cuántos kilos, promedios, comparaciones por mes, por cliente, por destino o por sucursal— con los datos reales de la empresa. Usala ante cualquier «cuántos», «cuánto», «promedio», «comparame», «ranking» o «evolución» sobre la operación.
---

# Consultar los números de CRISTAL+

1. **Nunca estimes ni inventes un número.** Si no lo podés consultar, decilo.
2. Mirá qué hay con `catalogo_de_datos`: cada conjunto dice qué es cada fila, sus dimensiones (por
   qué se agrupa), sus medidas (qué se calcula) y sus filtros. Usá las claves **exactas**.
3. Consultá con `consultar_datos`: uno o varios cortes (hasta 3 dimensiones y 8 medidas cada uno),
   con filtros de fecha `AAAA-MM-DD`. Para un período, poné siempre `desde` y `hasta`.
4. Leé el `comoLeer` que vuelve con los datos:
   - una medida **no aditiva** (un promedio, un «por guía») no se suma entre grupos;
   - una fila **«Otros»** junta a los que quedaron fuera del ranking: no digas nada de uno de ellos;
   - una fila **«Reservado»** protege datos de pocas personas: no la deduzcas por diferencia;
   - los `avisos` dicen si algo de lo pedido no se usó.
5. Mostrá el número con su período y su filtro, y ofrecé el corte siguiente que tenga sentido.
