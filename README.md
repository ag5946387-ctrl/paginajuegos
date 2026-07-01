# Juegos educativos

Colección de juegos educativos interactivos (anagrama, rueda aleatoria, parejas con fotos propias, cuestionario, etc.) en un solo archivo HTML, sin dependencias ni build.

## Cómo publicarlo en GitHub Pages

1. **Crea un repositorio nuevo** en GitHub (público, para poder usar Pages gratis).
2. **Sube estos archivos** a la raíz del repositorio:
   - `index.html`
   - `.nojekyll`
   - `README.md`

   Opción A — desde la web de GitHub:
   - Entra al repo → botón **"Add file" → "Upload files"** → arrastra los archivos → **Commit changes**.

   Opción B — desde tu computadora con git:
   ```bash
   git init
   git add .
   git commit -m "Primera versión de juegos educativos"
   git branch -M main
   git remote add origin https://github.com/TU-USUARIO/TU-REPO.git
   git push -u origin main
   ```

3. **Activa GitHub Pages:**
   - Ve a **Settings → Pages** en el repositorio.
   - En **"Build and deployment" → Source**, elige **"Deploy from a branch"**.
   - En **Branch**, selecciona `main` y la carpeta `/ (root)`.
   - Guarda.

4. **Espera 1-2 minutos.** GitHub te dará una URL como:
   ```
   https://TU-USUARIO.github.io/TU-REPO/
   ```
   Ahí ya queda publicado y accesible para cualquiera.

## Notas importantes

- Todo el contenido editable (palabras, preguntas, fotos del juego de Parejas, etc.) se guarda en el **almacenamiento local del navegador** (`localStorage`) de cada visitante. Esto significa:
  - Cada persona que entre ve/edita **su propia copia** de los datos; no hay una base de datos compartida.
  - Si el visitante borra el caché/datos del navegador, o entra desde otro dispositivo, no verá los cambios guardados anteriormente.
- No requiere backend, servidor ni build: es un único `index.html` autocontenido.
- Cualquier cambio futuro: edita `index.html` y vuelve a subir (commit + push) los cambios; GitHub Pages se actualiza solo.
