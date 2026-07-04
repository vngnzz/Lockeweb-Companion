<p align="center">
  <img width="192" height="192" alt="LockeWeb Companion icon" src="https://github.com/user-attachments/assets/400bd182-2c9c-442b-9551-9f2a0d7da62d" />
</p>

<h1 align="center">LockeWeb Companion</h1>

<p align="center">
  <strong>Local companion app for Pokémon Emerald RandomLocke/Nuzlocke runs in mGBA.</strong><br>
  <strong>Companion app local para RandomLocke/Nuzlocke de Pokémon Esmeralda en mGBA.</strong>
</p>

<p align="center">
  <img width="1920" height="1369" alt="LockeWeb Companion banner" src="https://github.com/user-attachments/assets/8881649d-0cc4-4d83-be28-ee51b43160b6" />
</p>

---

<p align="center">
  <strong>Latest stable version / Última versión estable:</strong><br>
  <code>v1.18.3 — HelloWorld Update ESP/ENG Public NPM Fix</code>
</p>

<p align="center">
  <a href="https://github.com/vngnzz/Lockeweb-Companion/releases/tag/1.18.3">
    <strong>Download latest release / Descargar última versión</strong>
  </a>
</p>

<p align="center">
  <strong>Languages / Idiomas:</strong> 🇪🇸 Español · 🇬🇧 English
</p>

---

<details open>
<summary><strong>🇪🇸 README — Español</strong></summary>

<br>

<details open>
<summary><strong>Qué es LockeWeb Companion</strong></summary>

<br>

LockeWeb Companion es una webapp local pensada para usarse como **segunda pantalla** mientras juegas una run de **Pokémon Esmeralda RandomLocke/Nuzlocke** en **mGBA**.

Lee información en directo desde mGBA mediante un script Lua y un pequeño bridge local en Node.js.

La idea es simple: tú juegas en mGBA, y LockeWeb te muestra en el navegador el equipo, mochila, ficha de entrenador, medallas, cementerio y checklist de capturas.

</details>

---

<details open>
<summary><strong>Estado actual</strong></summary>

<br>

**Última versión estable:** `v1.18.3 — HelloWorld Update ESP/ENG Public NPM Fix`

**Descarga de la última versión:**

```text
https://github.com/vngnzz/Lockeweb-Companion/releases/tag/1.18.3
```

Esta edición está pensada para que cualquier persona pueda usarla de forma sencilla:

- selector de idioma español/inglés integrado en la app;
- un único archivo `.bat`;
- instalación automática de dependencias internas si faltan;
- apertura automática del navegador;
- servidor local incluido;
- enlace directo al GitHub del proyecto dentro de la app;
- corrección del registry público de npm para evitar errores de instalación en otros PCs;
- sin `package-lock.json` con URLs internas;
- archivo `.npmrc` local incluido para forzar `https://registry.npmjs.org/`;
- `abrir_lockeweb.bat` instala dependencias usando el registry público oficial;
- sin login;
- sin servicios externos obligatorios;
- sin tocar la ROM ni el save.

</details>

---

<details>
<summary><strong>Qué hace</strong></summary>

<br>

<details>
<summary><strong>Equipo en directo</strong></summary>

<br>

LockeWeb lee automáticamente desde la memoria de mGBA:

- Pokémon actuales del equipo;
- mote;
- especie real;
- sprite;
- nivel;
- PS actuales y máximos;
- stats;
- ataques;
- PP;
- estado del Pokémon.

El **Equipo en directo** es solo de lectura.  
No se edita manualmente desde la web.

</details>

<details>
<summary><strong>Selector de idioma</strong></summary>

<br>

La app incluye selector de idioma en la parte superior derecha:

```text
🇪🇸 ES
🇬🇧 EN
```

El idioma elegido se guarda localmente en el navegador mediante `localStorage`.

La interfaz puede mostrarse en:

- español;
- inglés.

También se adaptan por idioma:

- textos de interfaz;
- estados de captura;
- estados de equipo/caja;
- filtros;
- tipos Pokémon;
- stats;
- nombres de movimientos e ítems cuando están disponibles.

</details>

<details>
<summary><strong>Ficha de entrenador</strong></summary>

<br>

Muestra automáticamente:

- nombre del entrenador;
- ID;
- dinero;
- medallas.

</details>

<details>
<summary><strong>Mochila</strong></summary>

<br>

Lee la mochila desde mGBA y la organiza por bolsillos:

- Objetos;
- Objetos clave;
- Poké Balls;
- MT/MO;
- Bayas.

</details>

<details>
<summary><strong>Registro rápido de capturas</strong></summary>

<br>

Permite actualizar la checklist de la run rápidamente.

Puedes registrar:

- ruta o sitio;
- estado de la captura;
- Pokémon capturado;
- mote;
- nivel;
- notas.

Estados disponibles:

- Capturado;
- Perdido;
- Dupe / Species;
- Regalo;
- Estático;
- Saltado.

También incluye una opción para rellenar datos desde un Pokémon actual del equipo live.

</details>

<details>
<summary><strong>Buscador de Pokémon</strong></summary>

<br>

Incluye un buscador con tolerancia a pequeños errores de escritura.

Ejemplo:

```text
chimchou
```

puede encontrar:

```text
Chinchou
```

El catálogo local incluye Pokémon de:

- Generación 1;
- Generación 2;
- Generación 3.

Hasta **Deoxys #386**.

El catálogo está preparado con estructura bilingüe:

```text
name_es
name_en
search
```

En Pokémon Esmeralda, la mayoría de nombres oficiales de Pokémon de Generación 1, 2 y 3 son iguales en español e inglés.  
Aun así, la estructura ya permite añadir diferencias de idioma, aliases y variantes comunes en futuras versiones.

</details>

<details>
<summary><strong>Checklist de Hoenn</strong></summary>

<br>

Incluye una checklist de rutas y zonas de Hoenn para llevar el control de capturas durante la run.

</details>

<details>
<summary><strong>Cementerio automático</strong></summary>

<br>

La app usa la **Caja 14 del PC** como cementerio automático.

```text
Caja 14 = Pokémon muertos
```

Cuando un Pokémon muere en la run, muévelo a la Caja 14 del PC y LockeWeb lo mostrará automáticamente en el cementerio.

</details>

<details>
<summary><strong>Backup</strong></summary>

<br>

LockeWeb permite:

- guardar progreso localmente en el navegador;
- exportar backup JSON;
- importar backup JSON.

</details>

</details>

---

<details open>
<summary><strong>Instalación rápida</strong></summary>

<br>

<details open>
<summary><strong>Requisitos</strong></summary>

<br>

Para usar LockeWeb Companion necesitas:

- Windows;
- Node.js instalado;
- mGBA con soporte de scripting Lua;
- una copia legal de Pokémon Esmeralda;
- la ROM cargada en mGBA.

Node.js solo hay que instalarlo una vez en el ordenador.

</details>

<details open>
<summary><strong>1. Instalar Node.js</strong></summary>

<br>

Instala **Node.js LTS** desde su web oficial:

```text
https://nodejs.org/
```

Solo tienes que hacerlo una vez.

Si ya tienes Node.js instalado, puedes saltar este paso.

</details>

<details open>
<summary><strong>2. Descargar LockeWeb Companion</strong></summary>

<br>

Descarga el ZIP desde la sección **Releases** del repositorio.

Última versión:

```text
https://github.com/vngnzz/Lockeweb-Companion/releases/tag/1.18.3
```

Archivo recomendado:

```text
LockeWeb-Companion-v1.18.3-HelloWorld-Update-ESP-ENG-Public-NPM-Fix.zip
```

Extrae la carpeta en cualquier ubicación de tu ordenador.

Ejemplo:

```text
Escritorio/LockeWeb-Companion-v1.18.3-HelloWorld-Update-ESP-ENG-Public-NPM-Fix/
```

</details>

<details open>
<summary><strong>3. Abrir LockeWeb Companion</strong></summary>

<br>

Dentro de la carpeta extraída, ejecuta:

```text
abrir_lockeweb.bat
```

En condiciones normales, basta con doble clic.

Si Windows bloquea permisos o la app no arranca correctamente, prueba:

```text
Clic derecho → Ejecutar como administrador
```

</details>

</details>

---

<details open>
<summary><strong>Uso con mGBA</strong></summary>

<br>

<details open>
<summary><strong>1. Abrir el juego</strong></summary>

<br>

Abre Pokémon Esmeralda en mGBA y carga tu partida.

</details>

<details open>
<summary><strong>2. Cargar el script Lua</strong></summary>

<br>

En mGBA, ve a:

```text
Tools → Scripting → Load Script
```

Selecciona el archivo:

```text
lua/emerald_party_sender.lua
```

</details>

<details open>
<summary><strong>3. Comprobar conexión</strong></summary>

<br>

Cuando todo esté funcionando correctamente, la web mostrará:

```text
Bridge conectado
```

A partir de ese momento, LockeWeb empezará a recibir datos desde mGBA.

</details>

<details open>
<summary><strong>Uso diario recomendado</strong></summary>

<br>

Después de tener Node.js instalado, el flujo normal es:

```text
1. Ejecutar abrir_lockeweb.bat.
2. Abrir Pokémon Esmeralda en mGBA.
3. Cargar lua/emerald_party_sender.lua.
4. Jugar con LockeWeb abierto como segunda pantalla.
```

Mantén abierta la ventana negra de `abrir_lockeweb.bat` mientras juegas.

Para cerrar LockeWeb:

```text
CTRL + C
```

y confirma con `S` si Windows lo pregunta.

</details>

</details>

---

<details>
<summary><strong>Qué hace abrir_lockeweb.bat</strong></summary>

<br>

`abrir_lockeweb.bat` es el único archivo necesario para iniciar LockeWeb Companion.

Hace automáticamente:

```text
1. Comprueba si Node.js está instalado.
2. Comprueba si npm está disponible.
3. Comprueba si faltan dependencias internas.
4. Ejecuta npm install solo si hace falta.
5. Abre el navegador.
6. Arranca el servidor local.
```

Importante:

```text
El BAT no instala Node.js.
```

Node.js debe instalarse manualmente una sola vez desde su web oficial.

### Corrección npm de la v1.18.3

La v1.18.3 corrige un problema detectado en instalaciones desde otros PCs.

La release pública ya no incluye `package-lock.json`, para evitar que npm use rutas internas de empaquetado.

Además, se incluye un archivo `.npmrc` local:

```text
registry=https://registry.npmjs.org/
audit=false
fund=false
```

Y el BAT fuerza la instalación con el registry público oficial:

```bat
npm install --registry=https://registry.npmjs.org/ --no-audit --no-fund
```

Si existe un `package-lock.json` antiguo con un registry interno incorrecto, el BAT lo detecta y lo elimina antes de instalar dependencias.

</details>

---

<details>
<summary><strong>Estructura del proyecto</strong></summary>

<br>

```text
LockeWeb-Companion/
├─ public/
│  ├─ index.html
│  ├─ app.js
│  ├─ styles.css
│  ├─ manifest.webmanifest
│  ├─ service-worker.js
│  ├─ data/
│  │  └─ pokemon_catalog_gen3.json
│  └─ iconos web
├─ lua/
│  └─ emerald_party_sender.lua
├─ server.js
├─ package.json
├─ package-lock.json
├─ abrir_lockeweb.bat
├─ INICIO_RAPIDO_WINDOWS.md
└─ README.md
```

</details>

---

<details>
<summary><strong>Problemas comunes</strong></summary>

<br>

<details>
<summary><strong>La web abre, pero no muestra datos</strong></summary>

<br>

Revisa:

- que `abrir_lockeweb.bat` siga abierto;
- que mGBA tenga cargado `lua/emerald_party_sender.lua`;
- que la web muestre `Bridge conectado`;
- que hayas cargado el script Lua de la carpeta correcta.

</details>

<details>
<summary><strong>El BAT dice que falta Node.js</strong></summary>

<br>

Instala Node.js LTS desde:

```text
https://nodejs.org/
```

Luego cierra la ventana y vuelve a ejecutar:

```text
abrir_lockeweb.bat
```

</details>

<details>
<summary><strong>Aparece un error relacionado con ws, npm, node_modules o ETIMEDOUT</strong></summary>

<br>

Si estás usando la v1.18.3 o superior, normalmente basta con usar una carpeta limpia y ejecutar:

```text
abrir_lockeweb.bat
```

Si vienes de una versión anterior o has mezclado archivos, cierra LockeWeb y borra:

```text
node_modules/
package-lock.json
```

Luego vuelve a ejecutar:

```text
abrir_lockeweb.bat
```

La v1.18.3 fuerza el registry público oficial de npm y evita el problema de URLs internas en `package-lock.json`.

</details>

<details>
<summary><strong>Windows bloquea el BAT</strong></summary>

<br>

Prueba:

```text
Clic derecho → Ejecutar como administrador
```

</details>

</details>

---

<details>
<summary><strong>Notas técnicas</strong></summary>

<br>

LockeWeb Companion funciona con esta arquitectura:

```text
mGBA
└─ Script Lua
   └─ TCP local
      └─ Node.js local bridge
         └─ Webapp en navegador
```

Todo funciona en local.

No requiere servidor externo, cuenta de usuario ni conexión permanente a internet, salvo para instalar dependencias la primera vez y para algunos recursos externos si no están cacheados.

</details>

---

<details>
<summary><strong>Seguridad y privacidad</strong></summary>

<br>

LockeWeb Companion:

- funciona en local;
- no sube tus datos a ningún servidor;
- no requiere login;
- guarda el progreso en el navegador;
- permite exportar/importar backup JSON.

</details>

---

<details>
<summary><strong>Qué NO incluye este proyecto</strong></summary>

<br>

Este proyecto no incluye:

- ROMs;
- BIOS;
- saves;
- archivos oficiales de Pokémon;
- assets propietarios del juego.

Cada usuario debe usar sus propias copias legales.

</details>

---

<details>
<summary><strong>Disclaimer</strong></summary>

<br>

Este proyecto es una herramienta **fan-made no oficial**.

No está afiliado, asociado ni respaldado por Nintendo, Game Freak, Creatures Inc. ni The Pokémon Company.

Pokémon y sus marcas relacionadas pertenecen a sus respectivos propietarios.

El proyecto no incluye ROMs, BIOS ni archivos protegidos.

</details>

---

<details>
<summary><strong>Licencia</strong></summary>

<br>

MIT.

</details>

</details>

---

<details>
<summary><strong>🇬🇧 README — English</strong></summary>

<br>

<details open>
<summary><strong>What is LockeWeb Companion?</strong></summary>

<br>

LockeWeb Companion is a local webapp designed to be used as a **second screen** while playing a **Pokémon Emerald RandomLocke/Nuzlocke** run in **mGBA**.

It reads live information from mGBA through a Lua script and a small local Node.js bridge.

The idea is simple: you play in mGBA, and LockeWeb shows your team, bag, trainer card, badges, graveyard and encounter checklist in your browser.

</details>

---

<details open>
<summary><strong>Current status</strong></summary>

<br>

**Latest stable version:** `v1.18.3 — HelloWorld Update ESP/ENG Public NPM Fix`

**Download latest release:**

```text
https://github.com/vngnzz/Lockeweb-Companion/releases/tag/1.18.3
```

This edition is designed to be easy to use:

- built-in Spanish/English language selector;
- single `.bat` file;
- automatic internal dependency installation if needed;
- automatic browser launch;
- local server included;
- direct GitHub link inside the app;
- public npm registry fix to avoid dependency installation errors on other PCs;
- no `package-lock.json` with internal URLs;
- local `.npmrc` file included to force `https://registry.npmjs.org/`;
- `abrir_lockeweb.bat` installs dependencies using the official public npm registry;
- no login;
- no required external service;
- no ROM or save modification.

</details>

---

<details>
<summary><strong>What it does</strong></summary>

<br>

<details>
<summary><strong>Live team</strong></summary>

<br>

LockeWeb automatically reads from mGBA memory:

- current party Pokémon;
- nickname;
- real species;
- sprite;
- level;
- current and maximum HP;
- stats;
- moves;
- PP;
- Pokémon status.

The **Live team** section is read-only.  
It is not edited manually from the webapp.

</details>

<details>
<summary><strong>Language selector</strong></summary>

<br>

The app includes a language selector in the top-right area:

```text
🇪🇸 ES
🇬🇧 EN
```

The selected language is saved locally in the browser using `localStorage`.

The interface can be displayed in:

- Spanish;
- English.

The following elements are also adapted per language:

- UI texts;
- capture statuses;
- team/box statuses;
- filters;
- Pokémon types;
- stats;
- move and item names when available.

</details>

<details>
<summary><strong>Trainer card</strong></summary>

<br>

Automatically displays:

- trainer name;
- ID;
- money;
- badges.

</details>

<details>
<summary><strong>Bag</strong></summary>

<br>

Reads the bag from mGBA and organizes it by pockets:

- Items;
- Key Items;
- Poké Balls;
- TM/HM;
- Berries.

</details>

<details>
<summary><strong>Quick capture registration</strong></summary>

<br>

Lets you quickly update the run checklist.

You can register:

- route or location;
- capture status;
- captured Pokémon;
- nickname;
- level;
- notes.

Available statuses:

- Caught;
- Missed;
- Dupe / Species;
- Gift;
- Static;
- Skipped.

It also includes an option to fill capture data from a current live team Pokémon.

</details>

<details>
<summary><strong>Pokémon search</strong></summary>

<br>

Includes typo-tolerant Pokémon search.

Example:

```text
chimchou
```

can find:

```text
Chinchou
```

The local catalog includes Pokémon from:

- Generation 1;
- Generation 2;
- Generation 3.

Up to **Deoxys #386**.

The catalog is prepared with bilingual structure:

```text
name_es
name_en
search
```

In Pokémon Emerald, most official Generation 1, 2 and 3 Pokémon species names are the same in Spanish and English.  
Even so, the structure already supports future language differences, aliases and common variants.

</details>

<details>
<summary><strong>Hoenn checklist</strong></summary>

<br>

Includes a checklist of Hoenn routes and locations to track captures during the run.

</details>

<details>
<summary><strong>Automatic graveyard</strong></summary>

<br>

The app uses **PC Box 14** as the automatic graveyard.

```text
Box 14 = dead Pokémon
```

When a Pokémon dies in the run, move it to PC Box 14 and LockeWeb will automatically show it in the graveyard section.

</details>

<details>
<summary><strong>Backup</strong></summary>

<br>

LockeWeb allows you to:

- save progress locally in the browser;
- export JSON backup;
- import JSON backup.

</details>

</details>

---

<details open>
<summary><strong>Quick setup</strong></summary>

<br>

<details open>
<summary><strong>Requirements</strong></summary>

<br>

To use LockeWeb Companion you need:

- Windows;
- Node.js installed;
- mGBA with Lua scripting support;
- a legal copy of Pokémon Emerald;
- the ROM loaded in mGBA.

Node.js only needs to be installed once on the computer.

</details>

<details open>
<summary><strong>1. Install Node.js</strong></summary>

<br>

Install **Node.js LTS** from the official website:

```text
https://nodejs.org/
```

You only need to do this once.

If Node.js is already installed, you can skip this step.

</details>

<details open>
<summary><strong>2. Download LockeWeb Companion</strong></summary>

<br>

Download the ZIP from the repository **Releases** section.

Latest release:

```text
https://github.com/vngnzz/Lockeweb-Companion/releases/tag/1.18.3
```

Recommended file:

```text
LockeWeb-Companion-v1.18.3-HelloWorld-Update-ESP-ENG-Public-NPM-Fix.zip
```

Extract the folder anywhere on your computer.

Example:

```text
Desktop/LockeWeb-Companion-v1.18.3-HelloWorld-Update-ESP-ENG-Public-NPM-Fix/
```

</details>

<details open>
<summary><strong>3. Open LockeWeb Companion</strong></summary>

<br>

Inside the extracted folder, run:

```text
abrir_lockeweb.bat
```

Normally, a double click is enough.

If Windows blocks permissions or the app does not start correctly, try:

```text
Right click → Run as administrator
```

</details>

</details>

---

<details open>
<summary><strong>Usage with mGBA</strong></summary>

<br>

<details open>
<summary><strong>1. Open the game</strong></summary>

<br>

Open Pokémon Emerald in mGBA and load your save.

</details>

<details open>
<summary><strong>2. Load the Lua script</strong></summary>

<br>

In mGBA, go to:

```text
Tools → Scripting → Load Script
```

Select the file:

```text
lua/emerald_party_sender.lua
```

</details>

<details open>
<summary><strong>3. Check connection</strong></summary>

<br>

When everything is working correctly, the webapp will show:

```text
Bridge connected
```

From that moment, LockeWeb will start receiving data from mGBA.

</details>

<details open>
<summary><strong>Recommended daily usage</strong></summary>

<br>

After Node.js is installed, the normal flow is:

```text
1. Run abrir_lockeweb.bat.
2. Open Pokémon Emerald in mGBA.
3. Load lua/emerald_party_sender.lua.
4. Play with LockeWeb open as a second screen.
```

Keep the black `abrir_lockeweb.bat` window open while playing.

To close LockeWeb:

```text
CTRL + C
```

and confirm with `Y` if Windows asks.

</details>

</details>

---

<details>
<summary><strong>What abrir_lockeweb.bat does</strong></summary>

<br>

`abrir_lockeweb.bat` is the only file needed to start LockeWeb Companion.

It automatically:

```text
1. Checks if Node.js is installed.
2. Checks if npm is available.
3. Checks if internal dependencies are missing.
4. Runs npm install only if needed.
5. Opens the browser.
6. Starts the local server.
```

Important:

```text
The BAT does not install Node.js.
```

Node.js must be installed manually once from the official website.

### v1.18.3 npm fix

v1.18.3 fixes an issue detected when installing dependencies on external PCs.

The public release no longer includes `package-lock.json`, so npm does not use internal packaging registry URLs.

A local `.npmrc` file is also included:

```text
registry=https://registry.npmjs.org/
audit=false
fund=false
```

And the BAT forces dependency installation through the official public registry:

```bat
npm install --registry=https://registry.npmjs.org/ --no-audit --no-fund
```

If an old `package-lock.json` exists with a wrong internal registry, the BAT detects it and deletes it before installing dependencies.

</details>

---

<details>
<summary><strong>Project structure</strong></summary>

<br>

```text
LockeWeb-Companion/
├─ public/
│  ├─ index.html
│  ├─ app.js
│  ├─ styles.css
│  ├─ manifest.webmanifest
│  ├─ service-worker.js
│  ├─ data/
│  │  └─ pokemon_catalog_gen3.json
│  └─ web icons
├─ lua/
│  └─ emerald_party_sender.lua
├─ server.js
├─ package.json
├─ package-lock.json
├─ abrir_lockeweb.bat
├─ INICIO_RAPIDO_WINDOWS.md
└─ README.md
```

</details>

---

<details>
<summary><strong>Common problems</strong></summary>

<br>

<details>
<summary><strong>The webapp opens, but does not show data</strong></summary>

<br>

Check:

- that `abrir_lockeweb.bat` is still open;
- that mGBA has loaded `lua/emerald_party_sender.lua`;
- that the webapp shows `Bridge connected`;
- that you loaded the Lua script from the correct folder.

</details>

<details>
<summary><strong>The BAT says Node.js is missing</strong></summary>

<br>

Install Node.js LTS from:

```text
https://nodejs.org/
```

Then close the window and run again:

```text
abrir_lockeweb.bat
```

</details>

<details>
<summary><strong>An error appears related to ws, npm, node_modules or ETIMEDOUT</strong></summary>

<br>

If you are using v1.18.3 or newer, using a clean folder and running this should normally be enough:

```text
abrir_lockeweb.bat
```

If you came from an older version or mixed files, close LockeWeb and delete:

```text
node_modules/
package-lock.json
```

Then run again:

```text
abrir_lockeweb.bat
```

v1.18.3 forces the official public npm registry and avoids the internal `package-lock.json` URL issue.

</details>

<details>
<summary><strong>Windows blocks the BAT</strong></summary>

<br>

Try:

```text
Right click → Run as administrator
```

</details>

</details>

---

<details>
<summary><strong>Technical notes</strong></summary>

<br>

LockeWeb Companion works with this architecture:

```text
mGBA
└─ Lua Script
   └─ Local TCP
      └─ Node.js local bridge
         └─ Browser webapp
```

Everything runs locally.

It does not require an external server, user account or permanent internet connection, except for first dependency installation and some external resources if they are not cached yet.

</details>

---

<details>
<summary><strong>Security and privacy</strong></summary>

<br>

LockeWeb Companion:

- runs locally;
- does not upload your data to any server;
- does not require login;
- stores progress in the browser;
- allows JSON backup export/import.

</details>

---

<details>
<summary><strong>What this project does NOT include</strong></summary>

<br>

This project does not include:

- ROMs;
- BIOS files;
- saves;
- official Pokémon files;
- proprietary game assets.

Each user must use their own legal copies.

</details>

---

<details>
<summary><strong>Disclaimer</strong></summary>

<br>

This project is an **unofficial fan-made tool**.

It is not affiliated with, associated with, or endorsed by Nintendo, Game Freak, Creatures Inc. or The Pokémon Company.

Pokémon and related trademarks belong to their respective owners.

This project does not include ROMs, BIOS files or protected files.

</details>

---

<details>
<summary><strong>License</strong></summary>

<br>

MIT.

</details>

</details>
