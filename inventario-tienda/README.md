# Inventario de la Tienda

App web de inventario compartido, publicada como artifact de Claude.

- **Link:** https://claude.ai/artifact/HpbsZtLv2vMY4vnrpmc6Bg
- **Código:** `index.html`

## Qué hace
- Admins (Editor): agregan productos (nombre, precio, stock, mínimo, foto), registran ventas y entradas, editan y eliminan.
- Familia (Viewer): solo ve, en vivo, desde el celular.
- Alertas: urgente (se acaba un producto muy vendido), stock bajo (mínimo o ≤7 días), sin movimiento (30 días sin ventas).
- Las fotos se comprimen antes de subirlas.

## Cómo compartir
1. En la app: Compartir → agregar cada correo (familia = Viewer, co-admin = Editor).
2. Cada persona crea su cuenta gratis en claude.ai con ESE correo.
3. Enviarles el link. No activar el link público.
4. En el celular: "Agregar a pantalla de inicio".

## Costos
Usar la app no gasta tokens. Solo se gastan al pedir cambios a Claude o con avisos programados.

## Pendiente (opcional)
- Avisos por correo programados (Gmail) a la familia.
- Versión independiente con Firebase + bot de Telegram para avisos al instante.

## Prompt reutilizable
```
Crea una app web compartida como artifact de Claude para [TEMA].
Usuarios: [N] admins (Editor) editan; [N] personas (Viewer) solo ven en vivo. Uso solo en celular.
Datos por registro: [campos, ej. nombre, precio, cantidad, foto].
Alertas: [reglas, ej. stock bajo, sin movimiento X días].
Usa capacidades db (escritura solo admin), user y assets (fotos comprimidas).
Interfaz en español, simple, modo claro/oscuro. Respuestas cortas, pocos tokens.
Al final explica cómo compartirla por correo.
```
