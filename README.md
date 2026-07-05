<p align="center">
  <img width="192" height="192" alt="PokeCompanion Logo" src="https://github.com/user-attachments/assets/abbb1023-e861-47cc-918e-90e473aff093" />
</p>

<h1 align="center">PokeCompanion GEN3</h1>

<p align="center">
  <strong>LockeWeb Companion for Pokémon Generation III Nuzlocke runs</strong><br>
  <strong>Companion LockeWeb para partidas Nuzlocke de Pokémon Generación III</strong>
</p>

<p align="center">
  <a href="https://github.com/vngnzz/Lockeweb-Companion/releases"><strong>Download latest releases / Descargar últimas versiones</strong></a>
</p>

---

<details open>
<summary><strong>🇪🇸 README en castellano</strong></summary>

<br>

<img width="1920" height="911" alt="PokeCompanion GEN3 banner" src="https://github.com/user-attachments/assets/8d920c62-5ebc-4aa8-864c-472cabbcd205" />

<details open>
<summary><strong>¿Qué es PokeCompanion GEN3?</strong></summary>

<br>

**PokeCompanion GEN3** es una **webapp companion local** orientada a partidas de Pokémon de **tercera generación**. Está pensada especialmente para runs **Nuzlocke / LockeWeb** y funciona junto a **mGBA** mediante scripts Lua y un pequeño servidor local.

La versión **v2.0 — Hall of Fame** es compatible con los cinco títulos principales de GEN3:

| Juego | Compatibilidad |
|---|---|
| Pokémon Rubí | Soportado |
| Pokémon Zafiro | Soportado |
| Pokémon Esmeralda | Soportado |
| Pokémon Rojo Fuego | Soportado |
| Pokémon Verde Hoja | Soportado |

La app lee información de la partida en vivo y la muestra en una interfaz web: equipo, ficha de entrenador, mochila, cementerio, checklist y utilidades para documentar la run.

El desarrollo sigue en curso. La versión **v2.0 — Hall of Fame** estabiliza la base GEN3 completa, pero se seguirán añadiendo mejoras, nuevas funciones y ajustes en futuras versiones.

</details>

---

<details>
<summary><strong>Objetivo del proyecto</strong></summary>

<br>

PokeCompanion nace para convertir una partida Nuzlocke clásica en una experiencia más visual, cómoda y organizada.

Sus objetivos principales son:

- Mostrar información útil de la partida sin modificar la ROM.
- Evitar cheats, editores de saves o herramientas invasivas.
- Ayudar a registrar encuentros, capturas, muertes y progreso.
- Facilitar el seguimiento de la run desde una interfaz web clara.
- Mantener perfiles separados para cada juego.
- Servir como base abierta para futuras mejoras de la comunidad.

PokeCompanion es un **companion**, no un editor de partidas.

</details>

---

<details>
<summary><strong>Funciones principales</strong></summary>

<br>

<table border="0" cellspacing="0" cellpadding="12" style="border:0;border-collapse:collapse;">
<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="314" height="595" alt="Registro de captura" src="https://github.com/user-attachments/assets/5c25089f-6ef7-41c8-a7ca-c92b563eabcb" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Registro y control de la run

Permite registrar y controlar la partida desde la web: encuentros, capturas, rutas, estados, progreso y datos útiles de la run.

Esta parte está pensada para complementar la lectura automática con decisiones manuales propias de una Nuzlocke.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Live Team" src="https://github.com/user-attachments/assets/fa719680-1cd2-41c9-a821-9283cb920209" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Live Team

Muestra el equipo actual leído desde mGBA, incluyendo Pokémon, motes, niveles, vida, estados y datos relevantes.

El objetivo es tener una vista rápida del equipo sin revisar manualmente cada dato dentro del juego.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="338" height="424" alt="Trainer Card" src="https://github.com/user-attachments/assets/9c9bc5d5-fccf-4248-b0c5-c5d355b9b3c0" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Ficha de entrenador

La Trainer Card muestra información clave del perfil activo:

- Nombre del entrenador.
- ID de entrenador.
- Dinero.
- Medallas.
- Estado de Liga Pokémon.
- Juego activo.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="345" height="567" alt="Mochila" src="https://github.com/user-attachments/assets/496da4c5-672c-4fd7-abcc-0334cc87028a" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Mochila

Lee y muestra la mochila del jugador, incluyendo objetos relevantes de la partida.

Esto permite consultar recursos importantes de la run desde la web sin tener que abrir constantemente los menús del juego.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Cementerio" src="https://github.com/user-attachments/assets/aff5f030-a57c-46d7-bf7d-c1b1db7c5d64" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Cementerio Nuzlocke

La **Caja 14** funciona como cementerio.

Los Pokémon colocados ahí aparecen automáticamente en la sección de muertos, permitiendo mantener visible el historial de bajas de la run.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Checklist" src="https://github.com/user-attachments/assets/07c630ec-c321-4051-a267-7186e8ac71ff" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Checklist

Incluye una checklist para controlar encuentros, capturas y progreso manual por juego.

Desde v2.0, estos datos se separan por perfil para evitar que una partida contamine los datos de otra.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Exportación Pokémon Showdown / PokéPaste" src="https://github.com/user-attachments/assets/517f7980-c9f8-48f9-b081-60656a28c1a6" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Exportación a Pokémon Showdown mediante PokéPaste

Permite generar una exportación del equipo en formato compatible con **Pokémon Showdown / PokéPaste**.

El objetivo es evitar configurar manualmente tu equipo en Showdown: PokeCompanion lee tu equipo desde mGBA y genera un texto reutilizable.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Backup" src="https://github.com/user-attachments/assets/11f7630c-f437-4ebe-af9e-a7cd6b9f075c" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Backups y datos locales

PokeCompanion guarda datos locales en el navegador y permite gestionar información útil de la run.

Esta función ayuda a conservar y mover datos importantes cuando estás documentando una partida larga.

</td>
</tr>
</table>

</details>

---

<details>
<summary><strong>Compatibilidad</strong></summary>

<br>

| Juego | Estado |
|---|---|
| Pokémon Rubí | Soportado |
| Pokémon Zafiro | Soportado |
| Pokémon Esmeralda | Soportado |
| Pokémon Rojo Fuego | Soportado |
| Pokémon Verde Hoja | Soportado |

La versión 2.0 ha sido validada con lectura completa de equipo, mochila, ficha de entrenador, dinero, medallas, cementerio/Caja 14, checklist y datos manuales por perfil.

</details>

---

<details>
<summary><strong>Instalación y uso</strong></summary>

<br>

### Requisitos

- Windows 10/11.
- Node.js instalado.
- mGBA con soporte Lua.
- ROM compatible de Pokémon GEN3.
- Save funcional de la partida.
- Navegador moderno: Chrome, Edge, Firefox o equivalente.

> PokeCompanion no incluye ROMs, BIOS, saves comerciales ni archivos oficiales de Pokémon. Debes usar tus propias copias legales.

### Instalación rápida

1. Descarga la última versión desde:

   [GitHub Releases](https://github.com/vngnzz/Lockeweb-Companion/releases)

2. Extrae el ZIP en una carpeta local.

3. Instala **Node.js LTS** desde la web oficial de Node.js si no lo tienes instalado.

4. Ejecuta **`abrir_lockeweb.bat`** como administrador.

5. Mantén abierta la ventana que se abre mientras estés jugando.

> La primera vez puede tardar un poco porque el `.bat` prepara las dependencias internas del companion.

### Uso con mGBA

1. Abre tu ROM en mGBA.

2. Carga el script Lua correspondiente al juego:

```text
lua/pokeconnect_ruby_sender.lua
lua/pokeconnect_sapphire_sender.lua
lua/pokeconnect_emerald_sender.lua
lua/pokeconnect_firered_sender.lua
lua/pokeconnect_leafgreen_sender.lua
```

3. Abre la web local que indique la ventana del companion.

Usa siempre el script dedicado del juego que estés ejecutando.

</details>

---

<details>
<summary><strong>Datos locales y perfiles</strong></summary>

<br>

Desde v2.0, PokeCompanion separa los datos por juego para evitar contaminación entre perfiles.

Esto afecta a:

- Checklist.
- Encuentros.
- Capturas.
- Roster.
- Últimos datos en vivo.
- Capturas/manual snapshots.
- Datos auxiliares de la run.

</details>

---

<details>
<summary><strong>Solución de problemas</strong></summary>

<br>

Si la web no recibe datos:

- Comprueba que `abrir_lockeweb.bat` está abierto.
- Comprueba que mGBA tenga cargado el script Lua correcto.
- Revisa que no estés usando el script de otro juego.
- Mira la consola de mGBA por si aparece un error Lua.
- Si es la primera ejecución, espera a que termine la preparación inicial.

Si el `.bat` falla:

- Comprueba que Node.js está instalado.
- Ejecuta `abrir_lockeweb.bat` como administrador.
- Revisa que hayas extraído el ZIP antes de ejecutarlo.

Si el cementerio no aparece:

- Comprueba que los Pokémon estén en la **Caja 14** del PC del juego.

Si la checklist muestra datos antiguos:

- Puede quedar información legacy en el navegador si vienes de una versión anterior. Exporta tus datos si lo necesitas y limpia el perfil afectado.

</details>

---

<details>
<summary><strong>Open Source</strong></summary>

<br>

PokeCompanion GEN3 es un proyecto **Open Source**.

Puedes revisar el código, modificarlo, adaptarlo a tus necesidades y proponer mejoras mediante issues o pull requests en GitHub.

</details>

---

<details>
<summary><strong>Créditos</strong></summary>

<br>

- Proyecto creado y mantenido por **vngnzz**.
- Gracias a **mGBA** por el emulador y soporte Lua.
- Gracias a **PokeAPI / sprites** por recursos y referencias visuales usadas por la comunidad.
- Gracias a **Pokémon Showdown** por el formato de equipos que inspira la exportación compatible con Showdown / PokéPaste.
- Gracias a la comunidad de investigación de Pokémon GEN3, save research, RAM mapping, decompilaciones y ROM hacking.

</details>

---

<details>
<summary><strong>Aviso legal</strong></summary>

<br>

PokeCompanion GEN3 es un proyecto fan-made y no oficial.

No está afiliado, patrocinado ni aprobado por Nintendo, Game Freak, Creatures Inc., The Pokémon Company ni ninguna entidad propietaria de la marca Pokémon.

Pokémon y todos los nombres, sprites, marcas y elementos relacionados pertenecen a sus respectivos propietarios.

Este repositorio no incluye ROMs, BIOS, saves comerciales ni archivos oficiales de Pokémon.

</details>

</details>

---

<details>
<summary><strong>🇬🇧 README in English</strong></summary>

<br>

<img width="1920" height="911" alt="PokeCompanion GEN3 banner" src="https://github.com/user-attachments/assets/8d920c62-5ebc-4aa8-864c-472cabbcd205" />

<details open>
<summary><strong>What is PokeCompanion GEN3?</strong></summary>

<br>

**PokeCompanion GEN3** is a **local web companion app** for **third-generation Pokémon games**. It is designed especially for **Nuzlocke / LockeWeb** runs and works with **mGBA** through Lua scripts and a small local server.

The **v2.0 — Hall of Fame** release is compatible with the five main GEN3 titles:

| Game | Compatibility |
|---|---|
| Pokémon Ruby | Supported |
| Pokémon Sapphire | Supported |
| Pokémon Emerald | Supported |
| Pokémon FireRed | Supported |
| Pokémon LeafGreen | Supported |

The app reads live game information and displays it in a web interface: party, Trainer Card, bag, cemetery, checklist, and tools to document the run.

Development is still ongoing. **v2.0 — Hall of Fame** stabilizes the full GEN3 foundation, but new improvements, features, and adjustments will be added in future versions.

</details>

---

<details>
<summary><strong>Project goal</strong></summary>

<br>

PokeCompanion was created to turn a classic Nuzlocke run into a more visual, comfortable, and organized experience.

Main goals:

- Display useful game information without modifying the ROM.
- Avoid cheats, save editors, or invasive tools.
- Help track encounters, captures, deaths, and progress.
- Make the run easier to follow through a clear web interface.
- Keep data separated per game profile.
- Serve as an open foundation for future community improvements.

PokeCompanion is a **companion**, not a save editor.

</details>

---

<details>
<summary><strong>Main features</strong></summary>

<br>

<table border="0" cellspacing="0" cellpadding="12" style="border:0;border-collapse:collapse;">
<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="314" height="595" alt="Capture registry" src="https://github.com/user-attachments/assets/5c25089f-6ef7-41c8-a7ca-c92b563eabcb" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Run tracking

Track manual run data from the web: encounters, captures, routes, states, progress, and useful run information.

This feature is designed to complement automatic reading with the manual decisions that are part of a Nuzlocke run.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Live Team" src="https://github.com/user-attachments/assets/fa719680-1cd2-41c9-a821-9283cb920209" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Live Team

Displays the current party read from mGBA, including Pokémon, nicknames, levels, HP, status, and relevant data.

The goal is to provide a quick team overview without manually checking every detail in-game.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="338" height="424" alt="Trainer Card" src="https://github.com/user-attachments/assets/9c9bc5d5-fccf-4248-b0c5-c5d355b9b3c0" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Trainer Card

The Trainer Card displays key active profile information:

- Trainer name.
- Trainer ID.
- Money.
- Badges.
- Pokémon League state.
- Active game.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="345" height="567" alt="Bag" src="https://github.com/user-attachments/assets/496da4c5-672c-4fd7-abcc-0334cc87028a" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Bag

Reads and displays the player's bag, including relevant items from the run.

This makes it easier to check important resources from the web without constantly opening the in-game menus.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Cemetery" src="https://github.com/user-attachments/assets/aff5f030-a57c-46d7-bf7d-c1b1db7c5d64" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Nuzlocke Cemetery

**Box 14** works as the cemetery.

Pokémon placed there automatically appear in the death box section, keeping the run's losses visible.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Checklist" src="https://github.com/user-attachments/assets/07c630ec-c321-4051-a267-7186e8ac71ff" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Checklist

Includes a checklist to track encounters, captures, and manual progress per game.

Since v2.0, this data is separated per profile to prevent one run from contaminating another.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Pokémon Showdown / PokéPaste export" src="https://github.com/user-attachments/assets/517f7980-c9f8-48f9-b081-60656a28c1a6" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Pokémon Showdown export through PokéPaste

Generates a team export compatible with **Pokémon Showdown / PokéPaste**.

The goal is to avoid manually configuring your team in Showdown: PokeCompanion reads your party from mGBA and generates reusable text.

</td>
</tr>

<tr style="border:0;">
<td width="42%" align="center" valign="middle" style="border:0;">
  <img width="100%" alt="Backup" src="https://github.com/user-attachments/assets/11f7630c-f437-4ebe-af9e-a7cd6b9f075c" />
</td>
<td width="58%" valign="middle" style="border:0;">

### Backups and local data

PokeCompanion stores local browser data and helps manage useful run information.

This helps preserve and move important data when documenting a long run.

</td>
</tr>
</table>

</details>

---

<details>
<summary><strong>Compatibility</strong></summary>

<br>

| Game | Status |
|---|---|
| Pokémon Ruby | Supported |
| Pokémon Sapphire | Supported |
| Pokémon Emerald | Supported |
| Pokémon FireRed | Supported |
| Pokémon LeafGreen | Supported |

Version 2.0 has been validated with full reading of party, bag, Trainer Card, money, badges, cemetery/Box 14, checklist, and manual per-profile data.

</details>

---

<details>
<summary><strong>Installation and usage</strong></summary>

<br>

### Requirements

- Windows 10/11.
- Node.js installed.
- mGBA with Lua support.
- Compatible Pokémon GEN3 ROM.
- Working save file.
- Modern browser: Chrome, Edge, Firefox, or equivalent.

> PokeCompanion does not include ROMs, BIOS files, commercial saves, or official Pokémon files. Use your own legal copies.

### Quick installation

1. Download the latest version from:

   [GitHub Releases](https://github.com/vngnzz/Lockeweb-Companion/releases)

2. Extract the ZIP into a local folder.

3. Install **Node.js LTS** from the official Node.js website if you do not already have it installed.

4. Run **`abrir_lockeweb.bat`** as administrator.

5. Keep the opened window running while you play.

> The first launch may take a little while because the `.bat` prepares the companion's internal dependencies.

### Usage with mGBA

1. Open your ROM in mGBA.

2. Load the Lua script matching your game:

```text
lua/pokeconnect_ruby_sender.lua
lua/pokeconnect_sapphire_sender.lua
lua/pokeconnect_emerald_sender.lua
lua/pokeconnect_firered_sender.lua
lua/pokeconnect_leafgreen_sender.lua
```

3. Open the local web page shown by the companion window.

Always use the dedicated script for the game you are running.

</details>

---

<details>
<summary><strong>Local data and profiles</strong></summary>

<br>

Since v2.0, PokeCompanion separates data by game to prevent cross-profile contamination.

This applies to:

- Checklist.
- Encounters.
- Captures.
- Roster.
- Latest live data.
- Manual snapshots.
- Auxiliary run data.

</details>

---

<details>
<summary><strong>Troubleshooting</strong></summary>

<br>

If the web app is not receiving data:

- Check that `abrir_lockeweb.bat` is open.
- Check that mGBA has loaded the correct Lua script.
- Make sure you are not using a script from another game.
- Check the mGBA console for Lua errors.
- On first launch, wait for the initial setup to finish.

If the `.bat` fails:

- Check that Node.js is installed.
- Run `abrir_lockeweb.bat` as administrator.
- Make sure you extracted the ZIP before running it.

If the cemetery does not appear:

- Make sure the Pokémon are placed in **Box 14** in the in-game PC.

If the checklist shows old data:

- Some legacy browser data may remain if you are upgrading from an older version. Export your data if needed and clear the affected profile.

</details>

---

<details>
<summary><strong>Open Source</strong></summary>

<br>

PokeCompanion GEN3 is an **Open Source** project.

You can review the code, modify it, adapt it to your needs, and propose improvements through GitHub issues or pull requests.

</details>

---

<details>
<summary><strong>Credits</strong></summary>

<br>

- Created and maintained by **vngnzz**.
- Thanks to **mGBA** for the emulator and Lua support.
- Thanks to **PokeAPI / sprites** for community resources and visual references.
- Thanks to **Pokémon Showdown** for the team format that inspires the Showdown / PokéPaste-compatible export.
- Thanks to the Pokémon GEN3 research, save research, RAM mapping, decompilation, and ROM hacking communities.

</details>

---

<details>
<summary><strong>Legal notice</strong></summary>

<br>

PokeCompanion GEN3 is an unofficial fan-made project.

It is not affiliated with, sponsored by, or endorsed by Nintendo, Game Freak, Creatures Inc., The Pokémon Company, or any entity that owns the Pokémon brand.

Pokémon and all related names, sprites, trademarks, and assets belong to their respective owners.

This repository does not include ROMs, BIOS files, commercial saves, or official Pokémon files.

</details>

</details>
