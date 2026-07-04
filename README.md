<p align="center">
  <img width="192" height="192" alt="LockeWeb Companion icon" src="https://github.com/user-attachments/assets/400bd182-2c9c-442b-9551-9f2a0d7da62d" />
</p>

<h1 align="center">LockeWeb Companion</h1>

<p align="center">
  <strong>Companion app local para RandomLocke/Nuzlocke de Pokémon Esmeralda en mGBA.</strong>
</p>

<p align="center">
  LockeWeb Companion es una webapp pensada para usarse como <strong>segunda pantalla</strong> mientras juegas una run de Pokémon Esmeralda.
</p>

---

LockeWeb Companion lee información en directo desde mGBA mediante un script Lua y un pequeño bridge local en Node.js.

La idea es simple: tú juegas en mGBA, y LockeWeb te muestra en el navegador el equipo, mochila, ficha de entrenador, medallas, cementerio y checklist de capturas.

---

<details open>
<summary><strong>Estado actual</strong></summary>

<br>

**Última versión estable:** `v1.17.2 — Easy Start Edition`

Esta edición está pensada para que cualquier persona pueda usarla de forma sencilla:

- un único archivo `.bat`;
- instalación automática de dependencias internas si faltan;
- apertura automática del navegador;
- servidor local incluido;
- sin login;
- sin servicios externos obligatorios;
- sin tocar la ROM ni el save.

</details>

---

<details>
<summary><strong>Qué hace</strong></summary>

<br>

### Equipo en directo

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

---

### Ficha de entrenador

Muestra automáticamente:

- nombre del entrenador;
- ID;
- dinero;
- medallas.

---

### Mochila

Lee la mochila desde mGBA y la organiza por bolsillos:

- Objetos;
- Objetos clave;
- Poké Balls;
- MT/MO;
- Bayas.

---

### Registro rápido de capturas

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

---

### Buscador de Pokémon

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

---

### Checklist de Hoenn

Incluye una checklist de rutas y zonas de Hoenn para llevar el control de capturas durante la run.

---

### Cementerio automático

La app usa la **Caja 14 del PC** como cementerio automático.

```text
Caja 14 = Pokémon muertos
```

Cuando un Pokémon muere en la run, muévelo a la Caja 14 del PC y LockeWeb lo mostrará automáticamente en el cementerio.

---

### Backup

LockeWeb permite:

- guardar progreso localmente en el navegador;
- exportar backup JSON;
- importar backup JSON.

</details>

---

<details open>
<summary><strong>Instalación rápida</strong></summary>

<br>

## Requisitos

Para usar LockeWeb Companion necesitas:

- Windows;
- Node.js instalado;
- mGBA con soporte de scripting Lua;
- una copia legal de Pokémon Esmeralda;
- la ROM cargada en mGBA.

Node.js solo hay que instalarlo una vez en el ordenador.

---

### 1. Instalar Node.js

Instala **Node.js LTS** desde su web oficial:

```text
https://nodejs.org/
```

Solo tienes que hacerlo una vez.

Si ya tienes Node.js instalado, puedes saltar este paso.

---

### 2. Descargar LockeWeb Companion

Descarga el ZIP desde la sección **Releases** del repositorio.

Archivo recomendado:

```text
LockeWeb-Companion-v1.17.2-Easy-Start.zip
```

Extrae la carpeta en cualquier ubicación de tu ordenador.

Ejemplo:

```text
Escritorio/LockeWeb-Companion-v1.17.2-Easy-Start/
```

---

### 3. Abrir LockeWeb Companion

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

---

<details open>
<summary><strong>Uso con mGBA</strong></summary>

<br>

### 1. Abrir el juego

Abre Pokémon Esmeralda en mGBA y carga tu partida.

---

### 2. Cargar el script Lua

En mGBA, ve a:

```text
Tools → Scripting → Load Script
```

Selecciona el archivo:

```text
lua/emerald_party_sender.lua
```

---

### 3. Comprobar conexión

Cuando todo esté funcionando correctamente, la web mostrará:

```text
Bridge conectado
```

A partir de ese momento, LockeWeb empezará a recibir datos desde mGBA.

---

## Uso diario recomendado

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

### La web abre, pero no muestra datos

Revisa:

- que `abrir_lockeweb.bat` siga abierto;
- que mGBA tenga cargado `lua/emerald_party_sender.lua`;
- que la web muestre `Bridge conectado`;
- que hayas cargado el script Lua de la carpeta correcta.

---

### El BAT dice que falta Node.js

Instala Node.js LTS desde:

```text
https://nodejs.org/
```

Luego cierra la ventana y vuelve a ejecutar:

```text
abrir_lockeweb.bat
```

---

### Aparece un error relacionado con `ws` o `node_modules`

Cierra LockeWeb, borra la carpeta:

```text
node_modules/
```

y vuelve a ejecutar:

```text
abrir_lockeweb.bat
```

El BAT volverá a instalar las dependencias necesarias.

---

### Windows bloquea el BAT

Prueba:

```text
Clic derecho → Ejecutar como administrador
```

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
