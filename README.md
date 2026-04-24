# Nuestra historia

Una página personal, hecha a mano, para recordar lo que fuimos.

## Cómo abrirla

Doble click en `index.html` y se abre en tu navegador. No necesita nada más.

Si quieres verla como si ya estuviera en internet (mejor para probar):

```
cd /home/user/personal/nuestra-historia
python3 -m http.server 8000
```

Luego abre `http://localhost:8000` en tu navegador.

## Cómo editarla

Todo está en **`index.html`**. No necesitas saber programar — cualquier editor de texto sirve (VS Code, Sublime, hasta el Bloc de notas).

- **Carta**: busca `Para ti, Valeria` y reemplaza los tres párrafos `[entre corchetes]`.
- **Línea de tiempo**: busca `<div class="timeline">` y cambia los años, títulos y descripciones de cada `<div class="hito">`.
- **Sección del hijo**: busca `Y llegó él` y edita los párrafos debajo.
- **Frase de cierre**: busca `Gracias por cada día.` y cámbiala si quieres.
- **Nombres y año**: en el `<h1>` del hero y el `<div class="anios">`.

## Cómo poner fotos reales

1. Guarda tus fotos en la carpeta `fotos/` (ya existe, vacía).
2. En `index.html`, busca un placeholder tipo `<div class="foto" data-n="1">Foto 1</div>` y reemplázalo por:
   ```html
   <div class="foto"><img src="fotos/nombre-de-tu-foto.jpg" alt="Descripción"></div>
   ```
3. Lo mismo con la foto del hero (`<div class="foto-hero">`), las mini-fotos de la línea de tiempo, y la foto del hijo.

## Cómo publicarla gratis

Cuando estés lista/listo para tener un link público, tienes tres opciones:

### 1. Netlify Drop (la más fácil — 30 segundos)

1. Entra a https://app.netlify.com/drop
2. Arrastra la carpeta `nuestra-historia` entera a la pantalla
3. Listo. Te dan un link tipo `https://tu-sitio-aleatorio.netlify.app`
4. Gratis, sin cuenta necesaria al inicio.

### 2. Vercel

```
cd /home/user/personal/nuestra-historia
npx vercel
```

Sigue las instrucciones. Gratis.

### 3. GitHub Pages

1. Sube esta carpeta a un repo de GitHub (privado o público — tú decides).
2. En Settings → Pages, activa Pages desde la rama `main`.
3. Tu link queda en `https://tu-usuario.github.io/nombre-del-repo/`.

## Privacidad

Esta carpeta vive solo en tu computadora hasta que tú decidas publicarla. No se sube a ningún lado automáticamente.
