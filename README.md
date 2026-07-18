# Angular Apps

Sitio web estático para Angular Apps, preparado para publicarse con GitHub Pages. No utiliza frameworks, backend, cookies propias ni analítica.

## Personalización rápida

### Reemplazar `angular.apps14@gmail.com`

Busca `angular.apps14@gmail.com` en `privacidad.html` y `contacto.html` y reemplázalo por el correo real de soporte. Actualiza tanto el texto visible como el valor de los enlaces `mailto:`.

### Agregar nuevas aplicaciones

1. Duplica `apps/defensa-del-evangelio.html` y cambia el nombre del archivo.
2. Actualiza el contenido, las funciones y los enlaces relativos.
3. Añade una nueva tarjeta en la sección `Aplicaciones` de `index.html` con un enlace a la nueva página.
4. Mantén el enlace a `../styles.css` y `../script.js` desde cualquier página dentro de `apps/`.

### Agregar capturas

Guarda las imágenes en `assets/defensa-del-evangelio/` (por ejemplo, `inicio.webp`). En `apps/defensa-del-evangelio.html`, reemplaza cada bloque `.screenshot-placeholder` por un elemento como `<img src="../assets/defensa-del-evangelio/inicio.webp" alt="Pantalla principal de Defensa del Evangelio">`. Usa imágenes optimizadas para web.

### Publicar con GitHub Pages

1. Crea un repositorio en GitHub y sube el contenido de esta carpeta a la rama principal.
2. En el repositorio, abre **Settings → Pages**.
3. En **Build and deployment**, selecciona **Deploy from a branch**, la rama principal y la carpeta `/ (root)`.
4. Guarda los cambios y espera a que GitHub Pages publique el sitio.
5. Si usas un dominio propio, configúralo en la misma sección y añade el registro DNS que indique GitHub.

### Actualizar Google Play y App Store

Cuando las aplicaciones estén publicadas, abre `apps/defensa-del-evangelio.html` y reemplaza los `href="#proximamente"` de los botones por las URLs reales de Google Play y App Store. Cambia también los textos `Próximamente` si corresponde.

## Estructura

`index.html` es la portada; `privacidad.html` y `contacto.html` son páginas informativas; `apps/` contiene las fichas individuales; `assets/` está reservado para logos y capturas; `styles.css` contiene el diseño responsive y `script.js` únicamente controla el menú móvil.
