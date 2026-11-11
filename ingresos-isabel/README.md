# Ingresos Isabel

Web de control de pensionistas y de todo el dinero que entra al restaurante, publicada como artifact de Claude.

- **Link:** https://claude.ai/artifact/QNGGmDq7fkmwZvrHcbCaRW
- **Código:** `index.html`
- **Acceso:** solo administradores (Editor). No activar el enlace público.

## Pestañas
- **Hoy:** anota platos de pensionistas (desayuno, almuerzo, cena; S/ 10 en local, S/ 11 para llevar) o sus productos (lista oculta con buscador y cantidad por toque).
- **Pensionistas:** deuda de cada uno, detalle por día y periodo, pagos parciales (efectivo o Yape), archivar.
- **Ventas:** ventas de menú y de productos, anotadas por comida y método; registro rápido de un toque.
- **Caja:** cuadre por desayuno, almuerzo y cena (efectivo y Yape esperado vs. contado).
- **Resumen:** dinero que entró por periodo, platos totales y mejor/peor día de la semana.

## Datos (base de datos del artifact)
`pensionistas`, `comidas` (por pensionista y mes), `extras` (productos a cuenta), `pagos`, `ventas` (por día), `cajas` (por día), `productos`.

## Notas
- Los precios se guardan con cada registro: cambiarlos no altera lo anterior.
- No se conecta con la web Inventario Isabel: el stock se resta allí.
- Los platos de pensionistas no entran a la caja el día que comen; entran cuando pagan.
