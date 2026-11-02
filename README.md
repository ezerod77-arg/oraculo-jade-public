# Oráculo de Jade — sitio público

Este repositorio es **exclusivamente público** y contiene las páginas institucionales y legales necesarias para identificar la aplicación OAuth que automatiza la publicación de videos del canal Oráculo de Jade.

**Arquitectura / separación obligatoria**

- **Repositorio privado `ezerod77-arg/Youtube`:** pipelines, código, recursos, automatizaciones, configuración técnica y cualquier información no pública.
- **Repositorio público `ezerod77-arg/oraculo-jade-public`:** únicamente contenido publicado para Google OAuth / YouTube: presentación, privacidad, condiciones y documentación pública no sensible.
- Jamás incluir credenciales, `client_secret.json`, `token.json`, refresh tokens, variables de entorno, materiales de producción, logs privados ni recursos internos. Los cambios de comportamiento operativo se realizan en el repositorio privado.
- Antes de hacer `git push`, revisar los archivos y confirmar que su publicación no expone datos privados. Mantener la URL permanente siempre que sea posible.

## Enlaces públicos

- **Página principal:** https://ezerod77-arg.github.io/oraculo-jade-public/
- **Política de privacidad:** https://ezerod77-arg.github.io/oraculo-jade-public/privacy.html
- **Condiciones de uso:** https://ezerod77-arg.github.io/oraculo-jade-public/terms.html

GitHub Pages publica la rama `main` desde `/`.

## Uso con Google Cloud

En Google Auth Platform → Información de la marca, copiar los enlaces anteriores a los campos respectivos. En `Público`, revisar los requisitos de publicación de la aplicación; publicar el sitio no cambia el estado OAuth. Luego renovar la autorización y validar permisos del canal. Un refresh token no es literalmente permanente y se puede revocar.

## Historial

Consultar [CHANGELOG.md](CHANGELOG.md) para modificaciones del sitio. El historial operativo de los videos se conserva **solo** en el proyecto privado.
