# CRISTAL+ para Digital Express

Los métodos de trabajo de los analistas de Digital Express, para usar desde Claude con el conector de
CRISTAL+:

- **Analizar la viabilidad** de un pedido: si se puede hacer, qué decisiones de arquitectura toca y de
  qué talla es. Para una tarea ya cargada no hace falta: CRISTAL+ la analiza solo, y el resultado se lee
  en la solapa «Análisis IA» de la tarea.
- **Diagnosticar un dato** que quedó mal en una base, y armar la receta para repararlo.

## Quién lo puede usar

El personal de Digital Express. El conector entrega el método de análisis con el nivel técnico de la
Ayuda (Interno, Gurú y Dios), y el de diagnóstico con el de Gurú y Dios. A cualquier otra cuenta no se
los ofrece.

## Instalarlo

Necesita el plugin **CRISTAL+** (`cristalmas`), que trae el conector: estas skills usan sus herramientas.

**En claude.ai, la app de escritorio o Cowork:** con el marketplace de CRISTAL+ ya agregado (los pasos
están en el [README del repositorio](https://github.com/CreadoresSAS/cristalmas-claude#readme)),
**Agregar** en **CRISTAL+ para Digital Express**.

**En Claude Code:**

```bash
claude plugin marketplace add CreadoresSAS/cristalmas-claude
claude plugin install cristalmas@softwarecristal
claude plugin install cristalmas-interno@softwarecristal
```

## Por qué va aparte

Los dos métodos viven en el servidor de CRISTAL+, y la skill se los pide al conector cuando arranca: así
cambian sin publicar otra versión del plugin. El directorio de plugins de Claude no admite que una skill
traiga sus instrucciones de afuera, así que este plugin no se publica ahí. El de CRISTAL+ sí.
