# FetoStudios Client

Launcher de los eventos de FetoStudios.

**Descargar:** [FetoStudios-Setup.exe](../../releases/latest/download/FetoStudios-Setup.exe) (Windows 10/11)

## Para el staff: cómo cargar eventos

Editá `eventos.json` desde la web de GitHub (lápiz ✏️ → «Commit changes»). En unos minutos
todos los launchers lo ven: aparece en «Explorar eventos», el código empieza a funcionar
y se mandan los recordatorios.

| Campo | Qué es |
|---|---|
| `codeHash` | **Huella** del código que se reparte en el Discord. Generala con `CODIGO.bat`: así el código no se puede leer acá, pero el launcher lo reconoce. (También se puede poner `"code": "FETO-SMP"` si no importa que sea público.) |
| `name` / `full` | Nombre corto y nombre completo |
| `date` | Fecha y hora con zona horaria: `2026-11-28T18:00:00-03:00` |
| `loader` / `mc` | `Fabric`, `Quilt`, `Forge`, `NeoForge` o `Vanilla`, y la versión de Minecraft |
| `mods` | Lista de mods de Modrinth: `{ "modrinth": "sodium" }` (o `{ "url": "…", "file": "…" }`) |
| `server` | Dirección del servidor (el launcher entra directo) |
| `ram` | Memoria recomendada en GB |
| `palette` | Color del paisaje: `night`, `dusk`, `deep` o `void` |
| `live` | `true` mientras el evento está en vivo |

`news` son las novedades que aparecen en la campanita del launcher.

## Para el staff: panel dentro del launcher

En el launcher: **Ajustes › Herramientas de staff** (pide el código de staff). Aparece la sección **Staff**, donde podés:

- Traer los eventos publicados, editarlos o crear nuevos con un formulario (el código se guarda como huella solo).
- Copiar el JSON y pegarlo en `eventos.json` acá en GitHub (botón **Abrir en GitHub**).

## Capas de FetoStudios

Las capas van en la carpeta `capas/` de este repositorio, con el **nombre exacto** del jugador en Minecraft:
`capas/Jere_123.png`. Las diseñás en el panel de staff (**Guardar PNG**) y las subís con **Subir a GitHub**.

Las ve todo el que juega con FetoStudios Client en instancias con mods (el launcher instala CustomSkinLoader).
Se activan desde la segunda vez que se abre cada instancia.
