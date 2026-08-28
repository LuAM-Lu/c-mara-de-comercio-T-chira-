# Propuesta de convenio · Electro Shop Morandin × CCIET

Documento web de una sola página dirigido a la Junta Directiva de la Cámara de
Comercio e Industria del Estado Táchira, en respuesta al **Plan Integral de
Blindaje Comercial y Fortalecimiento de los Cuadrantes de Paz** presentado por
PoliTáchira el 25 de agosto de 2026.

**Ref. ESM-CCIET-01**

---

## Cómo se publica

`index.html` es autocontenido: todo el CSS, el JavaScript, el catálogo de 263
productos y los logotipos van dentro del archivo, codificados en base64. No
depende de ningún recurso externo salvo las tipografías de Google Fonts.

- **Abrir en local:** doble clic sobre `index.html`
- **Publicar:** subir el archivo a cualquier hosting, o activar GitHub Pages
  sobre la rama `main` con la carpeta raíz

---

## Cómo se edita

Todo lo que cambia con frecuencia vive en un solo bloque, al inicio del
`<script>`, marcado como `███ CONFIGURACIÓN — EDITAR SOLO ESTE BLOQUE ███`.

| Qué | Dónde |
|---|---|
| Teléfono, correo, RIF, dirección, sitio web | `CONFIG` · datos de contacto |
| Tasa de cambio Bs./USD | `CONFIG.tasaBs` |
| Descuento por pago de contado | `CONFIG.descuentoContado` |
| Calendario de pago a 45 días | `CONFIG.calendario` |
| Mínimo de locales por jornada | `CONFIG.minimoJornada` |
| Tarifas de instalación | `CONFIG.tabulador` |
| Composición de los paquetes | `CONFIG.paquetes` |

Los paquetes se arman por **código de producto**: el precio se calcula solo a
partir del catálogo incrustado. Cambiar un paquete es editar su lista de
códigos y sus renglones de mano de obra.

---

## Estructura del documento

1. **Resumen ejecutivo** — la propuesta en cuatro puntos
2. **El convenio** — mecánica y aporte de cada parte
3. **Alcance** — familias de producto, marcas, tabulador de instalación y catálogo
4. **Paquetes y pago** — tres configuraciones, calculadora y comparador
5. **Cómo se ejecuta** — modelo de jornada por corredor comercial
6. **Condiciones** — articulado propuesto

---

## Archivos

```
index.html              El documento completo, autocontenido
ElectroShop_Logo.png    Marca del emisor
Tachira.png             Emblema CCIET (destinatario)
marca-*.png             Logotipos de las marcas representadas
```

---

## Advertencia sobre datos internos

El repositorio **no incluye** el catálogo maestro en CSV ni la carta de
PoliTáchira, y así debe permanecer:

- El CSV lleva la columna de **precio de costo** de cada producto. Publicarlo
  deja a la vista el margen de la operación.
- El PDF es una comunicación oficial de un organismo público dirigida a un
  tercero.

Ambos están declarados en `.gitignore`. El sitio publica únicamente precios de
venta ya calculados; en ningún punto del HTML aparece información de costos.

---

## Pendiente de definir

- Modalidad de financiamiento a discutir en la reunión con la Junta
- Tarifas de instalación de sistemas solares y de redes
- Cerradura electromagnética para el terminal biométrico (falta en el catálogo)
