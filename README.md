# PeterosMC-Assets

Repositorio de assets remotos para **Peteros Launcher**.

Aquí se almacenan todos los archivos que el launcher descarga y sincroniza automáticamente:

- `launcher.json` — configuración pública del launcher (versiones, servidor, noticias)
- `manifest.json` — inventario de archivos a sincronizar (mods, configs, etc.)
- `mods/` — mods del modpack
- `configs/` — archivos de configuración
- `resourcepacks/` — resource packs
- `shaderpacks/` — shader packs
- `images/` — imágenes y recursos visuales
- `news/` — contenido adicional de noticias

## Consumo

Peteros Launcher obtiene estos archivos desde la URL pública del repositorio (o CDN asociado) mediante `ConfigService` y `ManifestService`.

No edites `manifest.json` a mano de forma permanente: en el futuro un **Manifest Builder** lo generará a partir del contenido de estas carpetas (hashes, tamaños y URLs), sin cambiar la estructura del repositorio.
