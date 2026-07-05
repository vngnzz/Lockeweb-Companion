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

## ¿Qué es PokeCompanion GEN3?

**PokeCompanion GEN3** es una **webapp companion local** orientada a partidas de Pokémon de **tercera generación**. Está pensada especialmente para runs **Nuzlocke / LockeWeb** y funciona junto a **mGBA** mediante scripts Lua y un pequeño servidor local.

La app lee información de la partida en vivo y la muestra en una interfaz web: equipo, ficha de entrenador, mochila, cementerio, checklist y utilidades para documentar la run.

El desarrollo sigue en curso. La versión **v2.0 — Hall of Fame** estabiliza la base GEN3 completa, pero se seguirán añadiendo mejoras, nuevas funciones y ajustes en futuras versiones.

---

## Objetivo del proyecto

PokeCompanion nace para convertir una partida Nuzlocke clásica en una experiencia más visual, cómoda y organizada.

Sus objetivos principales son:

- Mostrar información útil de la partida sin modificar la ROM.
- Evitar cheats, editores de saves o herramientas invasivas.
- Ayudar a registrar encuentros, capturas, muertes y progreso.
- Facilitar el seguimiento de la run desde una interfaz web clara.
- Mantener perfiles separados para cada juego.
- Servir como base abierta para futuras mejoras de la comunidad.

PokeCompanion es un **companion**, no un editor de partidas.

---

## Funciones principales

### Registro y control de la run

Permite llevar un seguimiento manual de la partida: encuentros, capturas, rutas, estados, progreso y datos útiles de la run.

### Live Team

Muestra el equipo actual leído desde mGBA, incluyendo Pokémon, motes, niveles, vida, estados y datos relevantes.

### Ficha de entrenador

La Trainer Card muestra nombre, ID, dinero, medallas, estado de Liga Pokémon y juego activo.

<img width="338" height="424" alt="Trainer Card" src="https://github.com/user-attachments/assets/9c9bc5d5-fccf-4248-b0c5-c5d355b9b3c0" />

### Mochila

Lee y muestra la mochila del jugador, incluyendo objetos relevantes de la partida.

<img width="345" height="567" alt="Mochila" src="https://github.com/user-attachments/assets/496da4c5-672c-4fd7-abcc-0334cc87028a" />

### Cementerio Nuzlocke

La **Caja 14** funciona como cementerio. Los Pokémon colocados ahí aparecen automáticamente en la sección de muertos.

<img width="1902" height="477" alt="Cementerio" src="https://github.com/user-attachments/assets/aff5f030-a57c-46d7-bf7d-c1b1db7c5d64" />

### Checklist

Incluye checklist para controlar encuentros, capturas y progreso manual por juego.

<img width="1920" height="911" alt="Checklist" src="https://github.com/user-attachments/assets/07c630ec-c321-4051-a267-7186e8ac71ff" />

### Exportación a Pokémon Showdown mediante PokéPaste

Permite generar una exportación del equipo en formato compatible con **Pokémon Showdown / PokéPaste**, evitando tener que configurar manualmente cada Pokémon en Showdown.

<img width="1886" height="718" alt="Exportación Pokémon Showdown / PokéPaste" src="https://github.com/user-attachments/assets/517f7980-c9f8-48f9-b081-60656a28c1a6" />

### Backups y datos locales

PokeCompanion guarda datos locales en el navegador y permite gestionar información útil de la run.

<img width="1886" height="558" alt="Backup" src="https://github.com/user-attachments/assets/11f7630c-f437-4ebe-af9e-a7cd6b9f075c" />

---

## Compatibilidad

| Juego | Estado |
|---|---|
| Pokémon Rubí | Soportado |
| Pokémon Zafiro | Soportado |
| Pokémon Esmeralda | Soportado |
| Pokémon Rojo Fuego | Soportado |
| Pokémon Verde Hoja | Soportado |

La versión 2.0 ha sido validada con lectura completa de equipo, mochila, ficha de entrenador, dinero, medallas, cementerio/Caja 14, checklist y datos manuales por perfil.

---

## Instalación y uso

### Requisitos

- Windows 10/11.
- Node.js instalado.
- mGBA con soporte Lua.
- ROM compatible de Pokémon GEN3.
- Save funcional de la partida.
- Navegador moderno: Chrome, Edge, Firefox o equivalente.

> PokeCompanion no incluye ROMs, BIOS, saves comerciales ni archivos oficiales de Pokémon. Debes usar tus propias copias legales.

### Pasos

1. Descarga la versión más reciente desde:

   [GitHub Releases](https://github.com/vngnzz/Lockeweb-Companion/releases)

2. Extrae el ZIP en una carpeta local.

3. Abre una terminal en la carpeta del proyecto e instala dependencias:

```bash
npm install
```

4. Inicia el companion:

```bash
npm start
```

5. Abre la web local indicada por la consola, normalmente:

```text
http://localhost:3000
```

6. Abre tu ROM en mGBA y carga el script Lua correspondiente:

```text
lua/pokeconnect_ruby_sender.lua
lua/pokeconnect_sapphire_sender.lua
lua/pokeconnect_emerald_sender.lua
lua/pokeconnect_firered_sender.lua
lua/pokeconnect_leafgreen_sender.lua
```

Usa siempre el script dedicado del juego que estés ejecutando.

---

## Datos locales y perfiles

Desde v2.0, PokeCompanion separa los datos por juego para evitar contaminación entre perfiles.

Esto afecta a:

- Checklist.
- Encuentros.
- Capturas.
- Roster.
- Últimos datos en vivo.
- Capturas/manual snapshots.
- Datos auxiliares de la run.

---

## Solución de problemas

Si la web no recibe datos:

- Comprueba que el servidor local esté arrancado.
- Comprueba que mGBA tenga cargado el script Lua correcto.
- Revisa que no estés usando el script de otro juego.
- Mira la consola de mGBA por si aparece un error Lua.
- Verifica que el puerto local no esté bloqueado.

Si el cementerio no aparece:

- Comprueba que los Pokémon estén en la **Caja 14** del PC del juego.

Si la checklist muestra datos antiguos:

- Puede quedar información legacy en el navegador si vienes de una versión anterior. Exporta tus datos si lo necesitas y limpia el perfil afectado.

---

## Open Source

PokeCompanion GEN3 es un proyecto **Open Source**.

Puedes revisar el código, modificarlo, adaptarlo a tus necesidades y proponer mejoras mediante issues o pull requests en GitHub.

---

## Créditos

- Proyecto creado y mantenido por **vngnzz**.
- Gracias a **mGBA** por el emulador y soporte Lua.
- Gracias a **PokeAPI / sprites** por recursos y referencias visuales usadas por la comunidad.
- Gracias a **Pokémon Showdown** por el formato de equipos que inspira la exportación compatible con Showdown / PokéPaste.
- Gracias a la comunidad de investigación de Pokémon GEN3, save research, RAM mapping, decompilaciones y ROM hacking.

---

## Aviso legal

PokeCompanion GEN3 es un proyecto fan-made y no oficial.

No está afiliado, patrocinado ni aprobado por Nintendo, Game Freak, Creatures Inc., The Pokémon Company ni ninguna entidad propietaria de la marca Pokémon.

Pokémon y todos los nombres, sprites, marcas y elementos relacionados pertenecen a sus respectivos propietarios.

Este repositorio no incluye ROMs, BIOS, saves comerciales ni archivos oficiales de Pokémon.

</details>

---

<details>
<summary><strong>🇬🇧 README in English</strong></summary>

<br>

<img width="1920" height="911" alt="PokeCompanion GEN3 banner" src="https://github.com/user-attachments/assets/8d920c62-5ebc-4aa8-864c-472cabbcd205" />

## What is PokeCompanion GEN3?

**PokeCompanion GEN3** is a **local web companion app** for **third-generation Pokémon games**. It is designed especially for **Nuzlocke / LockeWeb** runs and works with **mGBA** through Lua scripts and a small local server.

The app reads live game information and displays it in a web interface: party, Trainer Card, bag, cemetery, checklist, and tools to document the run.

Development is still ongoing. **v2.0 — Hall of Fame** stabilizes the full GEN3 foundation, but new improvements, features, and adjustments will be added in future versions.

---

## Project goal

PokeCompanion was created to turn a classic Nuzlocke run into a more visual, comfortable, and organized experience.

Main goals:

- Display useful game information without modifying the ROM.
- Avoid cheats, save editors, or invasive tools.
- Help track encounters, captures, deaths, and progress.
- Make the run easier to follow through a clear web interface.
- Keep data separated per game profile.
- Serve as an open foundation for future community improvements.

PokeCompanion is a **companion**, not a save editor.

---

## Main features

### Run tracking

Track manual run data: encounters, captures, routes, states, progress, and useful run information.

### Live Team

Displays the current party read from mGBA, including Pokémon, nicknames, levels, HP, status, and relevant data.

### Trainer Card

The Trainer Card displays name, ID, money, badges, Pokémon League state, and active game.

<img width="338" height="424" alt="Trainer Card" src="https://github.com/user-attachments/assets/9c9bc5d5-fccf-4248-b0c5-c5d355b9b3c0" />

### Bag

Reads and displays the player's bag, including relevant items from the run.

<img width="345" height="567" alt="Bag" src="https://github.com/user-attachments/assets/496da4c5-672c-4fd7-abcc-0334cc87028a" />

### Nuzlocke Cemetery

**Box 14** works as the cemetery. Pokémon placed there automatically appear in the death box section.

<img width="1902" height="477" alt="Cemetery" src="https://github.com/user-attachments/assets/aff5f030-a57c-46d7-bf7d-c1b1db7c5d64" />

### Checklist

Includes a checklist to track encounters, captures, and manual progress per game.

<img width="1920" height="911" alt="Checklist" src="https://github.com/user-attachments/assets/07c630ec-c321-4051-a267-7186e8ac71ff" />

### Pokémon Showdown export through PokéPaste

Generates a team export compatible with **Pokémon Showdown / PokéPaste**, avoiding the need to manually configure each Pokémon in Showdown.

<img width="1886" height="718" alt="Pokémon Showdown / PokéPaste export" src="https://github.com/user-attachments/assets/517f7980-c9f8-48f9-b081-60656a28c1a6" />

### Backups and local data

PokeCompanion stores local browser data and helps manage useful run information.

<img width="1886" height="558" alt="Backup" src="https://github.com/user-attachments/assets/11f7630c-f437-4ebe-af9e-a7cd6b9f075c" />

---

## Compatibility

| Game | Status |
|---|---|
| Pokémon Ruby | Supported |
| Pokémon Sapphire | Supported |
| Pokémon Emerald | Supported |
| Pokémon FireRed | Supported |
| Pokémon LeafGreen | Supported |

Version 2.0 has been validated with full reading of party, bag, Trainer Card, money, badges, cemetery/Box 14, checklist, and manual per-profile data.

---

## Installation and usage

### Requirements

- Windows 10/11.
- Node.js installed.
- mGBA with Lua support.
- Compatible Pokémon GEN3 ROM.
- Working save file.
- Modern browser: Chrome, Edge, Firefox, or equivalent.

> PokeCompanion does not include ROMs, BIOS files, commercial saves, or official Pokémon files. Use your own legal copies.

### Steps

1. Download the latest version from:

   [GitHub Releases](https://github.com/vngnzz/Lockeweb-Companion/releases)

2. Extract the ZIP into a local folder.

3. Open a terminal in the project folder and install dependencies:

```bash
npm install
```

4. Start the companion:

```bash
npm start
```

5. Open the local web app shown in the console, usually:

```text
http://localhost:3000
```

6. Open your ROM in mGBA and load the matching Lua script:

```text
lua/pokeconnect_ruby_sender.lua
lua/pokeconnect_sapphire_sender.lua
lua/pokeconnect_emerald_sender.lua
lua/pokeconnect_firered_sender.lua
lua/pokeconnect_leafgreen_sender.lua
```

Always use the dedicated script for the game you are running.

---

## Local data and profiles

Since v2.0, PokeCompanion separates data by game to prevent cross-profile contamination.

This applies to:

- Checklist.
- Encounters.
- Captures.
- Roster.
- Latest live data.
- Manual snapshots.
- Auxiliary run data.

---

## Troubleshooting

If the web app is not receiving data:

- Check that the local server is running.
- Check that mGBA has loaded the correct Lua script.
- Make sure you are not using a script from another game.
- Check the mGBA console for Lua errors.
- Verify that the local port is not blocked.

If the cemetery does not appear:

- Make sure the Pokémon are placed in **Box 14** in the in-game PC.

If the checklist shows old data:

- Some legacy browser data may remain if you are upgrading from an older version. Export your data if needed and clear the affected profile.

---

## Open Source

PokeCompanion GEN3 is an **Open Source** project.

You can review the code, modify it, adapt it to your needs, and propose improvements through GitHub issues or pull requests.

---

## Credits

- Created and maintained by **vngnzz**.
- Thanks to **mGBA** for the emulator and Lua support.
- Thanks to **PokeAPI / sprites** for community resources and visual references.
- Thanks to **Pokémon Showdown** for the team format that inspires the Showdown / PokéPaste-compatible export.
- Thanks to the Pokémon GEN3 research, save research, RAM mapping, decompilation, and ROM hacking communities.

---

## Legal notice

PokeCompanion GEN3 is an unofficial fan-made project.

It is not affiliated with, sponsored by, or endorsed by Nintendo, Game Freak, Creatures Inc., The Pokémon Company, or any entity that owns the Pokémon brand.

Pokémon and all related names, sprites, trademarks, and assets belong to their respective owners.

This repository does not include ROMs, BIOS files, commercial saves, or official Pokémon files.

</details>
