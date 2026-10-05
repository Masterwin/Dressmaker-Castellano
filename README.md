# Dressmaker en Castellano

Traducción al español de **Dressmaker** (Cozy Lives / Free Lives, Steam 4019220).
*Spanish translation for Dressmaker — English summary at the end.*

![Opciones > Idioma](captura.png)

Añade el español como **un idioma más** en *Opciones > Idioma*, junto a English, 中文 y 日本語.
Se cambia de uno a otro al momento, sin tocar los archivos del juego y sin pisar el inglés.

El botón se llama **«Para mi hija Emma»**, porque este mod se hizo para ella. Si lo quieres de
otra manera, se cambia en `BepInEx\config\masterwin.dressmaker.es.cfg` (`NombreEnMenu`).

## Descargar

**[Última versión](../../releases/latest)** · también en [Nexus Mods](https://www.nexusmods.com/dressmaker/mods/185).

## Instalar

La carpeta del juego se abre en Steam: clic derecho en Dressmaker > *Administrar > Explorar archivos locales*.

### Windows

1. Descomprime `BepInEx_win_x64_5.4.23.5.zip` ([BepInEx](https://github.com/BepInEx/BepInEx/releases))
   en la carpeta del juego, no en una subcarpeta: `winhttp.dll` y `BepInEx` deben quedar junto a `Dressmaker.exe`.
2. Abre el juego una vez y ciérralo.
3. Descomprime el zip del mod en esa misma carpeta (se crea `BepInEx\plugins\DressmakerES`).
4. En el juego: *Opciones > Idioma > Para mi hija Emma*.

### Mac (sin probar)

1. Descomprime `BepInEx_macos_universal_5.4.23.5.zip` ([BepInEx](https://github.com/BepInEx/BepInEx/releases))
   en la carpeta del juego, junto a la app.
2. Abre `run_bepinex.sh` con TextEdit y cambia:
   - `executable_name=""` → `executable_name="Dressmaker.app"` (el nombre de la app del juego).
   - **Solo en Mac con chip Apple (M1, M2…):** `export ARCHPREFERENCE="arm64,x86_64"` →
     `export ARCHPREFERENCE="x86_64,arm64"`. Sin esto el mod no carga y no avisa.
3. En Terminal, escribe `cd ` (con espacio), arrastra la carpeta del juego, pulsa Intro y ejecuta:
   ```
   chmod +x run_bepinex.sh
   xattr -dr com.apple.quarantine .
   ```
4. En Steam: Dressmaker > *Propiedades > Opciones de lanzamiento*:
   `"/ruta/completa/a/run_bepinex.sh" %command%` (arrastra el archivo a la casilla para la ruta).
5. Abre el juego desde Steam una vez y ciérralo (debe aparecer `BepInEx/plugins`).
6. Descomprime el zip del mod en la carpeta del juego (se crea `BepInEx/plugins/DressmakerES`).
7. En el juego: *Opciones > Idioma > Para mi hija Emma*.

En Mac con chip Apple el juego va en modo Intel (Rosetta): los cambios de pantalla pueden tardar un poco más.

Si tienes **Dress Maker ESP** instalado, quítalo (borra `BepInEx/plugins/DressMakerSpanish`): escribe
el español encima del inglés y los dos a la vez se pisan.

## Qué traduce

| Tabla | Traducido |
|---|---|
| Telas, accesorios, patrones, piezas, encargos, colores… | 1 909 de 1 930 |
| Diálogos | 3 578 de 3 677 (lo que falta son «…», «Oh.», «Hmm.») |
| Interfaz | 208 de 208 |
| Tutorial | 71 de 71 |

También los dos avisos que el juego tiene fijos en inglés: «Desbloqueado: …» y «¡No tienes telas!».
Se quedan en inglés los nombres de las clientas y las 5 imágenes con texto (cartel de la tienda,
folleto de prestigio, periódico y título).

## Versión del juego

Probado en la build **410.44874e6** (24/09/2026) con BepInEx 5.4.23.5 x64. Si un parche añade
textos nuevos, salen en inglés hasta que se traduzcan: nunca en blanco.

¿Ves un texto cortado, montado o mal traducido? Abre un [issue](../../issues) con una captura.

## Créditos y licencia

- Plugin y textos de objetos rehechos desde las tablas del juego: **Masterwin**.
- Base de los diálogos, la interfaz y el tutorial: [Dress Maker ESP](https://www.nexusmods.com/dressmaker/mods/32)
  de **Gabssby**, revisada y corregida, con su permiso. ¡Gracias, Gabssby!

Plugin: [MIT](LICENSE). Nuestras traducciones: CC BY 4.0 (detalle en el zip, `LICENSE-traduccion.md`).
Dressmaker es de Cozy Lives; este mod no es oficial.

---

### English

Adds **Spanish** as one more language in *Options > Language* (the button reads «Para mi hija
Emma», "For my daughter Emma"; rename it in `BepInEx\config\masterwin.dressmaker.es.cfg`).
Install [BepInEx 5 x64](https://github.com/BepInEx/BepInEx/releases) next to `Dressmaker.exe`,
run the game once, then unzip the [latest release](../../releases/latest) into the same folder.
**Mac** (untested): use `BepInEx_macos_universal`, set `executable_name="Dressmaker.app"` in
`run_bepinex.sh`, on Apple Silicon change `ARCHPREFERENCE` to `"x86_64,arm64"` (plugins won't load
natively), then launch with `"/path/to/run_bepinex.sh" %command%` in Steam's launch options.
Tested on build 410.44874e6. MIT (plugin) · CC BY 4.0 (our translations).
