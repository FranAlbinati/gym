# Iron · Gym Tracker

Web app single-file para seguir rutinas de gimnasio, cambiar ejercicios sobre la marcha y anotar pesos. Multi-usuario (vos y tu novia, cada uno con su rutina), guardado en tu dispositivo.

## Cómo usarla

Opción rápida — abrirla local:
```bash
# desde la carpeta del repo
python3 -m http.server 8000
# luego abrí http://localhost:8000 en el celu o la compu
```

Opción recomendada — GitHub Pages:
1. Settings → Pages → Deploy from branch → `main` / root.
2. Al minuto tenés una URL pública que podés agregar al home del celular como app.

## Qué trae

- **Multi-usuario**: cambio rápido entre personas desde el header. Cada una con su propio color, emoji, unidad (kg/lb) y rutina.
- **Rutina editable**: días (Empuje/Tirón/Pierna precargados para vos; Glúteo/Superior/Full body para ella). Agregá, editá o borrá días y ejercicios.
- **Sesión en vivo**: tocás *Empezar*, cargás peso y reps por set, marcás ✓. Se autocompleta con el peso de la última vez.
- **Cambiar ejercicio**: botón ⇄ en cada ejercicio. Podés cambiarlo solo para hoy o guardarlo en la rutina.
- **Historial**: cada sesión terminada queda con fecha, volumen total y detalle. PR por ejercicio.
- **Persistencia**: todo en `localStorage` del navegador. Sin cuentas, sin servidor.

## Stack

- HTML + Tailwind (CDN) + JS vanilla. Un solo archivo (`index.html`).
- Mobile-first, dark mode nativo, sin dependencias que instalar.
