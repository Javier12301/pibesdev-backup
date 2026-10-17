# PibesDev Backups — Página de información OAuth

Sitio web estático para describir la integración privada Rclone + Google Drive API usada para almacenar respaldos cifrados de la infraestructura.

## Archivos

- `index.html`: presentación de la aplicación
- `privacidad.html`: política de privacidad y uso de datos de Google
- `styles.css`: estilos básicos

No contiene claves OAuth, tokens, contraseñas ni datos de usuarios.

## Publicación mediante GitHub Pages

1. Crear el repositorio **público** `Javier12301/pibesdev-backup` con rama `main`.
2. Subir los archivos a la raíz de `main`.
3. Ir a **Settings → Pages → Build and deployment**.
4. Seleccionar **Deploy from a branch**, `main`, `/(root)` y guardar.
5. Verificar que la página y la política de privacidad abren públicamente.

URLs esperadas (una vez publicadas):

- Página principal: `https://javier12301.github.io/pibesdev-backup/`
- Política de privacidad: `https://javier12301.github.io/pibesdev-backup/privacidad.html`

## Nota sobre Google OAuth

Google podría exigir verificación de dominio en Search Console para autorizar un proyecto OAuth externo. Un subdominio de `github.io` no garantiza que Google acepte la titularidad en su proceso de verificación. Si eso sucede, hay que usar un dominio propio verificable o evaluar las opciones autorizadas por Google, sin inventar dominios.

**Antes de automatizar los backups:** completar y verificar el cifrado Rclone Crypt, pruebas de restauración y retención; mantener la política alineada con el tratamiento real de datos.
