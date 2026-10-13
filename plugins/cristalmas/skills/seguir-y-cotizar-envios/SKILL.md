---
name: seguir-y-cotizar-envios
description: Seguir un envío por su número de seguimiento, ver su guía, su retiro o sus recepciones, cotizar un envío o pedir un retiro en CRISTAL+. Usala cuando alguien da un número como 0001-000000123456-U o -Z, pregunta dónde está una carga, cuánto cuesta mandar algo o quiere que vayan a buscar una carga.
---

# Seguir, cotizar y pedir retiros en CRISTAL+

- **Seguir**: `seguir_envio` con el número (un -U es el grupo: retiro, recepciones y guías; un -Z,
  una guía). Para el detalle, `ver_guia`, `ver_retiro` o `ver_recepcion`. Si contesta que no lo
  encuentra, puede no existir o no ser de esa cuenta: no adivines cuál.
- **Cotizar**: las localidades van por número. Buscalas con `buscar_localidades` (por nombre o código
  postal) y, si hay varias parecidas, preguntá cuál. Después `cotizar_envio` con kilos, bultos y lo
  que se sepa. La cotización no graba nada y no incluye impuestos.
- **Pedir un retiro**: `pedir_retiro` **crea** el retiro. Antes, juntá cliente, domicilio con su
  localidad, la franja horaria y la forma de pago, mostrá el resumen y esperá que la persona lo
  confirme. Si vuelve con errores por campo, corregí esos campos y nada más.
