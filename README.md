# KioskoControl · Lector inteligente de productos

Incluye lector de códigos de barras para iOS y Android, reconocimiento automático por código local y consulta a **Open Food Facts** para intentar recuperar nombre, marca, categoría, tipo de producto y fotografía. La consulta requiere Internet y depende de la cobertura del catálogo; no siempre existe una coincidencia.

## Flujos

- En **Venta rápida**, al leer un código que ya existe, se añade directamente al carrito.
- En **Inventario → Escanear mercadería**, si el producto existe, se abre su registro de ingreso de stock con el producto seleccionado. Solo debes registrar cantidad, lote, ubicación y costo.
- Si un código nuevo coincide de forma segura con un producto existente (misma familia, variante y presentación), se asocia el nuevo código al producto existente, sin duplicarlo.
- Para artículos nuevos, la ficha se autocompleta si Open Food Facts reconoce el código; **no inventa los precios de venta, costos de compra, lote ni cantidad**.
- Si la búsqueda falla, permite registrar manualmente.

## Publicación

Sube **index.html** a la raíz de tu repositorio GitHub `KiosKoControlCL`, reemplazando el archivo anterior. GitHub Pages actualiza la aplicación tras publicar `main`. Usa Safari o Chrome directamente en el celular y concede el permiso de cámara.

## Sobre los códigos de prueba

Los códigos EAN-13 que creamos para pruebas (`7801234567894`, etc.) son ficticios y están contemplados como **datos de demostración**. No representan identificadores comerciales reales. El primero se asocia a la Coca-Cola 500 ml de la demo.

## Datos

Todos los registros siguen guardándose en el navegador de cada dispositivo y no se sincronizan entre teléfonos. Exporta un respaldo antes de reemplazar los datos reales.
