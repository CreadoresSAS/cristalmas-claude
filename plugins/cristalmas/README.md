# CRISTAL+

CRISTAL+ en Claude: consultá la documentación de CRISTAL+ y los datos de tu empresa, seguí y cotizá
envíos, pedí retiros, atendé los casos de la mesa de ayuda y analizá pedidos, desde una conversación,
en claude.ai, en la app de escritorio, en el celular, en Cowork y en Claude Code.

## Instalarlo

En claude.ai, la app de escritorio o Cowork: **Personalización → Plugins → + Agregar → Agregar
marketplace → Agregar desde un repositorio**, con `https://github.com/CreadoresSAS/cristalmas-claude`,
y **Sincronizar**. Después **Agregar** en **CRISTAL+**. El paso a paso está en el
[README del repositorio](https://github.com/CreadoresSAS/cristalmas-claude#readme).

En Claude Code:

```
/plugin install cristalmas --marketplace CreadoresSAS/cristalmas-claude
```

## Cómo se usa

1. En el plugin, solapa **Conectores**: **Conectar** junto a **cristal** (Continuar y Agregar, sin
   cambiar nada) y **Conectar** otra vez.
2. Claude abre CRISTAL+: entrá con tu usuario, revisá la empresa y apretá **Permitir**.
3. Preguntá en castellano: «¿cuál es el promedio de kilos por guía por mes en 2025?», «¿dónde está
   el envío 0001-000000123456-U?», «¿cuánto sale mandar 30 kilos a Córdoba?», «¿cómo se calcula
   el recargo de una devolución?», «¿qué le contesto al cliente del caso 100255?», «¿se puede hacer
   este pedido del cliente?».

Claude trabaja **con tu cuenta y tus permisos**: ve y hace lo mismo que vos en CRISTAL+, en la empresa
con la que te conectaste, y te pide confirmación antes de crear algo. Lo habilita quien administra los
permisos de tu empresa (Configurar Empresa → Seguridad). La conexión se ve y se revoca en CRISTAL+,
en Mi cuenta → Claude.

## Qué datos viajan

Lo que Claude consulta sale de tu CRISTAL+ por `mas.softwarecristal.ar` y entra a tu conversación con
Claude. Las consultas de números devuelven totales y agrupados; los grupos con datos de pocas personas
salen como «Reservado». El plugin no guarda nada por su cuenta.

## Si tu empresa usa otro servidor de CRISTAL+

El conector de este plugin es el del servidor central. Si tu empresa tiene un servidor propio, agregá
el conector por su dirección (`https://<tu servidor>/api/v3/mcp`) como conector personalizado; la
dirección está en CRISTAL+, en Mi cuenta → Claude.
