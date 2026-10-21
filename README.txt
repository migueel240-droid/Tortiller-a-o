# Tortillería Obregón — aplicación web instalable

## Archivos
- `index.html`: aplicación de ventas, devoluciones, inventario y catálogo.
- `manifest.json`: configuración para instalarla como aplicación.
- `sw.js`: caché básica para abrir la aplicación sin conexión después de cargarla en línea.

## Publicar desde Android en GitHub Pages
1. Abre el repositorio `TortilleriaObregon`.
2. Sube estos tres archivos a la raíz del repositorio. Si ya hay archivos con el mismo nombre, reemplázalos únicamente si deseas sustituir la versión anterior.
3. En Settings → Pages, configura la publicación desde la rama principal (`main`) y la carpeta raíz (`/root`), si no está configurado.
4. Abre la URL de GitHub Pages en Chrome y deja que cargue una vez con internet.
5. En el menú de Chrome, elige “Instalar aplicación” o “Agregar a pantalla principal”.

## Funciones incluidas
- Ventas con múltiples productos por ticket, contado o crédito.
- Cantidades editables con teclado numérico y botones + / −.
- Catálogo con agregar, editar, activar/desactivar, precio, unidad, tipo de inventario y foto desde cámara/galería.
- Inventario editable por producto.
- Devoluciones; las tortillas de maíz se envían al inventario de “Tortillas frías”.
- Historial de movimientos y exportación/importación de respaldo.
- Almacenamiento local del navegador.

## Importante: límites de esta primera versión
- Los datos se guardan en el dispositivo/navegador que los registra. **No hay sincronización automática entre teléfonos ni una base de datos en la nube configurada.** Para compartir cambios entre administrador y repartidores hace falta integrar un backend (por ejemplo, Firebase/Supabase) y reglas de usuarios.
- El modo offline funciona para la interfaz después de haberla cargado con internet al menos una vez; no se garantiza que el primer acceso sea offline.
- Las fotos se comprimen antes de guardarse, pero el almacenamiento del navegador es limitado. Exporta respaldos con regularidad.
- Las cantidades de inventario iniciales son cero; edítalas en Inventario antes de vender.
- El ejemplo de producto con precio de $15 no se agrega automáticamente: el precio $15 aparece como valor inicial del formulario para crear un producto, con nombre vacío.
- Esta es una base funcional inicial; prueba ventas, devoluciones y respaldos con datos de prueba antes de usarla para la operación real.
