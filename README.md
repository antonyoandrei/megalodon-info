# Megalodon · información pública

Sitio estático de presentación y privacidad para configurar el cliente OAuth personal de Google Drive. No contiene el reproductor, credenciales, una biblioteca multimedia ni datos de usuarios. No necesita Node, dependencias ni compilación.

## Publicar en GitHub Pages

1. Sube estos archivos a la rama `main` de `antonyoandrei/megalodon-info`.
2. En GitHub: **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Selecciona **main**, carpeta **/(root)**, y guarda.
4. Espera a que GitHub confirme el despliegue y abre ambas páginas antes de usarlas en Google.

Con GitHub Free, este repositorio informativo debe ser público para usar Pages. El repositorio de la aplicación Megalodon permanece separado y privado. No copies su `.env`, configuración de rclone, tokens, bases de datos ni archivos multimedia aquí.

## Direcciones para Google Auth Platform

Una vez publicado correctamente:

| Campo | Valor |
|---|---|
| Nombre de la aplicación | Megalodon |
| Página principal | https://antonyoandrei.github.io/megalodon-info/ |
| Política de privacidad | https://antonyoandrei.github.io/megalodon-info/privacy.html |
| Dominio autorizado | antonyoandrei.github.io |
| Condiciones del servicio | Opcional; dejar vacío |
| Contacto | antonyoandrei@gmail.com |

El cliente OAuth de rclone es de tipo **Aplicación de escritorio**. Estas páginas son enlaces informativos, no sus direcciones de redirección. Si Google solicita acreditar la propiedad del sitio, utiliza el procedimiento de Google Search Console correspondiente al sitio de GitHub Pages. Publicar estas páginas no garantiza por sí solo la aprobación de Google.

La política describe una conexión con permiso **drive.readonly**, caché local de rclone y una instalación privada de Jellyfin/Megalodon. Actualízala antes de cambiar los permisos o el tratamiento de datos.

Ambas páginas incluyen `noindex, nofollow` para solicitar que no aparezcan en buscadores. Eso no restringe el acceso: las páginas informativas son públicas y deben ser legibles sin iniciar sesión.

## Archivos

- `index.html`: presentación del proyecto y contacto.
- `privacy.html`: política de privacidad y revocación del acceso.
- `styles.css`: estilos responsive, sin fuentes ni recursos externos.
- `assets/megalodon.png`: imagen de marca.
- `.nojekyll`: publicación directa de archivos estáticos.

Para revisar localmente, abre `index.html` en un navegador. Todos los enlaces internos son relativos y funcionan bajo la subruta de GitHub Pages.
