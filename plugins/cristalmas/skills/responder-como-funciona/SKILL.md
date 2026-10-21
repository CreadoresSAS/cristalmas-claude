---
name: responder-como-funciona
description: Contestar cómo funciona algo en CRISTAL+, cómo se hace una tarea, cómo se calcula un importe o por qué está hecho así, con la documentación oficial. Usala cuando alguien pregunta «¿cómo se…?», «¿dónde está…?», «¿se puede…?», «¿cómo calcula…?» o «¿está hecho…?» sobre CRISTAL+.
---

# Contestar cómo funciona algo en CRISTAL+

1. **Buscá en la documentación** con `buscar_documentacion`, en palabras de negocio. Las guías dicen
   cómo se usa; los ADR (tipo `decision`), por qué se decidió así. Leé lo que sirva con
   `leer_documento` y **citá la fuente** (la guía, o «ADR 0149, Decisión 26»).
2. **Si no aparece, probá otra vez** con otras palabras: un sinónimo, el nombre de la pantalla, el
   singular o el plural, la palabra bien escrita (contrarreembolso va con doble r).
3. **Si sigue sin aparecer, decí que no lo encontrás en la documentación**, y nunca que no está
   hecho ni que no existe. La documentación de cada servidor es la de su última versión publicada
   (`documentacionAl`): algo reciente puede estar hecho y todavía no haber llegado.
4. **Lo marcado `proximaVersion`** está hecho, pero el servidor de la persona todavía no instaló la
   versión que lo trae: decíselo así («llega con la próxima versión»).
5. Si la pregunta es un número de su empresa (cuántos, cuánto, promedios), no es documentación: se
   consulta con `catalogo_de_datos` y `consultar_datos`.
