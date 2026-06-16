# Portfolio — Pablo

Sitio estático de una sola página (`index.html`), sin frameworks ni build step. Listo para GitHub Pages o Vercel tal cual.

## Antes de publicar — sustituye estos placeholders

- **Apellido**: el `<h1>` solo dice "Pablo", añade tu apellido si quieres.
- **Email**: busca `tu-email@ejemplo.com` y cámbialo por el tuyo.
- **GitHub / LinkedIn**: busca `tu-usuario` (aparece dos veces) y pon tus URLs reales.
- **Proyectos**: las 3 tarjetas con borde discontinuo en la sección "Proyectos" son plantillas de ejemplo — sustitúyelas por tus repositorios reales (nombre, descripción de 1-2 líneas, y enlace al repo).
- **Estado de certificaciones**: ahora todas aparecen en la hoja de ruta como plan. Si ya tienes alguna conseguida, puedes añadir algo como `<span style="color:var(--teal)"> · Conseguida</span>` justo después del `cert__id` correspondiente.

## Opción A — GitHub Pages

1. Crea un repositorio nuevo en GitHub (puede llamarse como quieras, o `tu-usuario.github.io` si quieres que sea tu dominio raíz).
2. Sube `index.html` a la raíz del repositorio (arrastrarlo en la web de GitHub funciona, o por terminal):
   ```bash
   git init
   git add index.html README.md
   git commit -m "Primer portfolio"
   git branch -M main
   git remote add origin https://github.com/tu-usuario/tu-repo.git
   git push -u origin main
   ```
3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main / (root)**.
4. Espera 1-2 minutos. Tu URL será `https://tu-usuario.github.io/tu-repo/` (o `https://tu-usuario.github.io/` si el repo se llama así).

## Opción B — Vercel

1. Sube el mismo repositorio a GitHub (pasos 1-2 de arriba).
2. Entra en [vercel.com](https://vercel.com), **Add New → Project**, e importa el repositorio.
3. Como es HTML puro, Vercel no necesita build command ni output directory — déjalo en blanco y pulsa **Deploy**.
4. Te da una URL al instante (`tu-repo.vercel.app`). Cada `git push` futuro se despliega solo.

## Dominio propio (opcional, para ambas opciones)

1. Compra un dominio (Namecheap, Cloudflare).
2. En GitHub Pages: **Settings → Pages → Custom domain**, escribe tu dominio y sigue las instrucciones de DNS (CNAME).
3. En Vercel: **Project → Settings → Domains**, añade tu dominio y configura el registro que te indique.
