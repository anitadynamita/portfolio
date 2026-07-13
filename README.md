# Portfolio Ana Muros — cómo ponerlo en marcha

## 1. Añade tus vídeos
Crea (ya existe) la carpeta `videos/` junto a `index.html` y suelta dentro tus MP4 con estos nombres exactos:

| Archivo | Qué es |
|---|---|
| `hero.mp4` | Fondo abstracto full-bleed (incluido — [CONFIRMAR autoría: si es stock, sustituir por pieza propia en v1.1]) |
| `wall-01.mp4` … `wall-08.mp4` (ya incluidos) | Los creativos de Welltech, SOLO 9:16 |
| `sephora.mp4` | Too Faced Ribbon Wrap — thumbnail card (incluido) |
| `primark.mp4` + `primark-b.mp4` | Rutas A y B de X-Mas (incluidos, lightbox) |
| `case-*.mp4` | Piezas de los case studies (incluidas) |
| `banners/` e `images/` | Banners HTML5 en vivo y fotogramas fijos (incluidos) |
| `samsung.mp4` | Mejor pieza Samsung |
| `compeed.mp4` | El FOOH |
| `lab.mp4` | Pieza de motion puro o experimento AI |

Mientras un vídeo no exista, su hueco muestra una etiqueta gris con el nombre esperado — así ves qué falta.

**Compresión (obligatoria):** MP4 H.264, máx. 1080px de lado mayor, < 5 MB por vídeo (< 8 MB el hero). HandBrake preset "Vimeo YouTube 1080p" o Media Encoder a 2–4 Mbps. Recorta cada loop a sus mejores 4–8 segundos.

## 2. Pruébalo en local
Doble clic en `index.html` y se abre en el navegador. (Algunos navegadores bloquean autoplay en local: si no arrancan los vídeos, prueba tras subirlo a Netlify.)

## 3. Publícalo gratis en Netlify
1. Ve a https://app.netlify.com/drop
2. Arrastra la carpeta completa `anamuros-site` (con `index.html` y `videos/` dentro)
3. Netlify te da una URL en segundos. Cada vez que cambies algo, vuelve a arrastrar.

## 4. Conecta tu dominio
En Netlify: Site settings → Domain management → Add custom domain → sigue las instrucciones de DNS de tu registrador (Namecheap/Porkbun/Cloudflare). HTTPS automático incluido.

## 5. Personaliza el contenido
Todo el texto está en `index.html`, buscable a simple vista:
- Testimonials: sustituye los `[Quote pending…]` por citas reales (con permiso).
- LinkedIn: pon tu URL real en el footer (busca `linkedin.com`).
- CV: añade tu `cv.pdf` junto a `index.html`.
- Bio del About: tres párrafos, edítalos a tu voz.

## 5.b Sección "Same script, different bets"
Suelta en `videos/` las variaciones del mismo voiceover como `var-01.mp4` … `var-04.mp4` (ya incluidos) (9:16). Si tienes más o menos de 6, dímelo y ajusto el número en un minuto. La etiqueta V01–V06 se genera sola.

## 6. Pendiente para v1.1
- `case-sephora.html` y `case-samsung.html` (las cards ya enlazan a esos nombres — pídeme las páginas cuando tengas el material ordenado).
- Banners HTML5 de Samsung: súbelos a Netlify Drop por separado y los embebemos por iframe en la página de case.
- Creative Factory Demo cuando la produzcas.

## Reglas de oro del diseño (no las rompas)
- El vídeo es el único color y el único movimiento. La UI no se anima.
- El acento violeta (#5B4EE0) solo en métricas, flechas y hovers.
- Nada de preloaders, cursores custom ni parallax.
