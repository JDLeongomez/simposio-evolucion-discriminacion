# Simposio — Pensamiento evolutivo en la psicología

Presentación en Quarto revealjs. Incluye la apertura del simposio (breve) y
la charla "Evolución y discursos discriminatorios".

## Estructura

```
.
├── index.qmd            # la presentación completa (apertura + charla)
├── theme/
│   └── poster.scss       # tema revealjs con la paleta del póster
├── img/
│   ├── simposio/          # logos institucionales, recorte del póster
│   └── charla/             # imágenes reutilizables de la charla 2025
│                           # (https://github.com/JDLeongomez/evolucion-y-psicologia)
├── references.bib        # citas (Turkheimer 2000, Polderman et al. 2015, etc.)
└── README.md
```

## Paleta de colores (extraída del póster)

Muestreada directamente de la imagen del póster. Si tienes el SVG original,
sería mejor sacar los valores exactos de ahí (probablemente estén definidos
como variables de color en el archivo) y actualizar `theme/poster.scss`.

| Uso                          | Hex       |
|-------------------------------|-----------|
| Fondo (cream)                  | `#FAF6EB` |
| Árbol decorativo (cream oscuro)| `#F3EDE0` |
| Texto principal (ink)          | `#262420` |
| Acento naranja                 | `#F08C00` |
| Franja inferior (charcoal)     | `#333333` |

## Pendientes

- [ ] Reemplazar `img/simposio/logo_ubosque.svg` (y agregar logos de EvoCo /
      LabPsiExp / Especialización) con los archivos SVG reales.
- [ ] Copiar a `img/charla/` las imágenes que quieras reciclar de la charla
      2025.
- [ ] Completar `references.bib`: Lynn & Vanhanen 2002, Lynn & Becker 2019,
      Cell 2024, Al-Shawaf 2025, Vasquez-Amézquita et al. 2025.
- [ ] Si quieres formato APA en las citas en pantalla, descarga un `.csl`
      (p. ej. desde <https://www.zotero.org/styles>) y colócalo en la raíz
      del proyecto como `apa.csl`, o borra esa línea del YAML si prefieres
      el formato por defecto de Pandoc.
- [ ] Ir llenando cada sección de `index.qmd` (los comentarios `<!-- -->`
      indican qué va en cada diapositiva) con imágenes y el texto mínimo
      que quieras dejar en pantalla.

## Renderizar

```bash
quarto render index.qmd
# o, para vista previa en vivo mientras editas:
quarto preview index.qmd
```
