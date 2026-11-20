# CRISTAL+ para Claude

El marketplace de plugins de CRISTAL+ (Digital Express). Tiene dos plugins:

- **CRISTAL+** (`cristalmas`), que conecta Claude con tu CRISTAL+ con tu cuenta y tus permisos. Es el
  que instala cualquier empresa.
- **CRISTAL+ para Digital Express** (`cristalmas-interno`), con los métodos de los analistas de Digital
  Express. Es sólo para su personal y necesita el anterior instalado.

## Instalarlo

**En claude.ai, la app de escritorio o Cowork** (planes Pro, Max, Team y Enterprise). No lo busques
en el buscador de Plugins: no aparece ahí, se agrega con su dirección.

1. **Personalización → Plugins → + Agregar → Agregar marketplace → Agregar desde un repositorio**
   (*Customize → Plugins → Add → Add marketplace*). En **URL**, pegá
   `https://github.com/CreadoresSAS/cristalmas-claude` y apretá **Sincronizar**. Si aparece un aviso
   sobre la «Claude GitHub App», cerralo: no hace falta.
2. En la lista aparece **CRISTAL+**: apretá **Agregar**.
3. Abrí **CRISTAL+**, solapa **Conectores**, y apretá **Conectar** junto a **cristal**. Claude muestra el
   conector ya completo: **Continuar** y **Agregar**, sin cambiar nada.
4. Apretá **Conectar** otra vez: Claude abre CRISTAL+, entrás con tu usuario y apretás **Permitir**.

En Team y Enterprise también lo agrega cada persona. Si no ves **Agregar marketplace**, tu organización
de Claude lo tiene apagado: pedíselo a quien la administra.

**En Claude Code:**

```bash
claude plugin marketplace add CreadoresSAS/cristalmas-claude
claude plugin install cristalmas@softwarecristal
```

Después, en una sesión: `/mcp` → **cristal** → **Authenticate**.

**El personal de Digital Express** agrega además **CRISTAL+ para Digital Express**: en claude.ai, con
**Agregar** en la misma lista; en Claude Code, con `claude plugin install cristalmas-interno@softwarecristal`.

## Quién lo puede usar

Las personas a las que su empresa les habilitó el conector en CRISTAL+ (Configurar Empresa →
Seguridad). Claude ve y hace lo mismo que la persona en CRISTAL+, y pide confirmación antes de crear
algo. La conexión se ve y se revoca en CRISTAL+, en Mi cuenta → Mi IA.

## Privacidad

El plugin no junta datos por su cuenta: trae las instrucciones para Claude y la dirección del conector.
Qué recibe y qué guarda CRISTAL+ cuando Claude lo consulta, cuánto tiempo y cómo pedir que se borre está
en la [política de privacidad de CRISTAL+](https://mas.softwarecristal.ar/privacidad/#conector-ia).
