# Dorilab · Página de pedidos

Página web de Dorilab (Dorilocos, Cartagena). El cliente arma su Dorilocos (tamaño, toppings, salsas y cantidad) y el pedido llega ya escrito a WhatsApp.

## Archivos
- `index.html`: toda la página (diseño, menú y lógica de pedidos)
- `cup.jpg`, `ring.jpg`, `pour.jpg`: fotos de la marca (déjalas en la misma carpeta que `index.html`)

## Publicar gratis con GitHub Pages
1. En GitHub: **New repository**, nombre `dorilab` (público) y **Create**.
2. **Add file → Upload files** y sube los 5 archivos (también funciona desde el celular).
3. **Commit changes**.
4. Ve a **Settings → Pages**. En *Branch* elige `main` y carpeta `/ (root)`, y guarda.
5. En 1 o 2 minutos tu página queda en `https://TU-USUARIO.github.io/dorilab/`.

Con Git en la terminal:
```bash
git init && git add . && git commit -m "Dorilab web"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/dorilab.git
git push -u origin main
```

## Qué editar (busca estas líneas dentro de `index.html`)
| Qué | Línea a buscar |
|---|---|
| Número de WhatsApp | `var WHATSAPP="573181418725"` (código de país + número, sin + ni espacios) |
| Precios Mini y Maxi | `var PR={Mini:12000,Maxi:20000}` (**son de ejemplo, cámbialos**) |
| Toppings | `var TP=[` |
| Salsas y sus nombres | `var SA=[` (la tercera se llama "La secreta" por ahora) |

## Dominio propio (opcional)
En **Settings → Pages → Custom domain** escribe tu dominio y crea en tu proveedor un registro CNAME hacia `TU-USUARIO.github.io`.

## Cómo llegan los pedidos
Al confirmar, se abre WhatsApp con el pedido completo y un número único (DL-fecha-número). El cliente solo toca enviar. WhatsApp no permite enviarlo automáticamente.

## Siguiente paso sugerido
Conectar una hoja de Google Sheets para registrar cada pedido solo y recibir un correo de aviso.
