# CRISTAL+ para Claude

El marketplace de plugins de CRISTAL+ (Digital Express). Tiene un plugin: **CRISTAL+**
(`cristalmas`), que conecta Claude con tu CRISTAL+ con tu cuenta y tus permisos.

## Instalarlo

**En claude.ai, la app de escritorio o Cowork** (planes Pro, Max, Team y Enterprise):

1. **Customize → Plugins → Add → Add marketplace**, con la dirección de este repositorio:
   `https://github.com/CreadoresSAS/cristalmas-claude`.
2. Instalá **CRISTAL+** y, en su solapa **Connectors**, conectalo: Claude abre CRISTAL+, entrás con tu
   usuario y apretás **Permitir**.

En Team y Enterprise, un Owner puede dejarlo instalado para toda la organización desde
Organization settings → Plugins & skills.

**En Claude Code:**

```bash
claude plugin marketplace add CreadoresSAS/cristalmas-claude
claude plugin install cristalmas@softwarecristal
```

Después, en una sesión: `/mcp` → **cristal** → **Authenticate**.

## Quién lo puede usar

Las personas a las que su empresa les habilitó el conector en CRISTAL+ (Configurar Empresa →
Seguridad). Claude ve y hace lo mismo que la persona en CRISTAL+, y pide confirmación antes de crear
algo. La conexión se ve y se revoca en CRISTAL+, en Mi cuenta → Claude.
