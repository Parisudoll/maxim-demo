# Maxim — demo

Demo interactivo con cristal negro → ámbar, transición al logo Maxim charol negro, y frosted glass sobre video de fondo que se revela en **30 segundos**.

## Cómo verlo

**Importante:** no se puede abrir el `index.html` con doble clic — el navegador bloquea la carga de los `.glb` por seguridad. Hay dos formas de correrlo:

### Opción A — Local (para probar rápido)

En la terminal, parada/o dentro de la carpeta `maxim-demo`:

```
python3 -m http.server 8000
```

Después abrí en el navegador: `http://localhost:8000`

### Opción B — GitHub Pages (para compartir con el inversor)

Igual que hiciste con `tarjetadan`:

1. Creá un repo nuevo (por ejemplo `maxim-demo`) en tu cuenta `parisudoll`
2. Subí todos los archivos de esta carpeta al repo
3. Activá GitHub Pages en Settings → Pages → Source: `main` branch
4. Compartí el link `https://parisudoll.github.io/maxim-demo/`

## Cómo funciona la demo

1. Aparece el cristal levitando y rotando sobre fondo negro
2. Al pasar el cursor (o tocar en mobile), el cristal se vuelve ámbar
3. Al hacer clic o tocar el cristal, transiciona al logo Maxim
4. El logo tiene brillo que se mueve siguiendo el cursor
5. Detrás del logo aparece el video del photoshoot, cubierto por frosted glass negro
6. Empieza un conteo de 30 segundos en la esquina
7. El frosted glass va de negro → ámbar → transparente, revelando el video

## Cambiar la duración de la demo

En `index.html`, buscá esta línea (cerca del comentario "Countdown"):

```js
const DEMO_SECONDS = 30;
```

Cambiala al número de segundos que quieras.

## Para la versión real (con fecha de lanzamiento)

Cuando tengas la fecha exacta, se reemplaza esa lógica por una que compare con `new Date('2026-XX-XX')` y muestre días restantes en vez de segundos. Se hace en 5 minutos.
