# Cómo publicar un nuevo release

La plantilla [`RELEASE_TEMPLATE.md`](RELEASE_TEMPLATE.md) se usa como cuerpo del release en GitHub. Contiene placeholders que hay que reemplazar antes de publicar.

## Placeholders

| Placeholder       | Qué va ahí                                                                                              |
|-------------------|----------------------------------------------------------------------------------------------------------|
| `{{VERSION}}`     | Versión semántica sin la `v`, ej. `3.4.2`                                                                |
| `{{BUTTON_URL}}`  | URL de la imagen del botón. Usar `https://raw.githubusercontent.com/wco/launcher/main/.github/assets/descargar-launcher.png` |

## Flujo manual

```bash
VERSION=3.4.2
BUTTON_URL="https://raw.githubusercontent.com/wco/launcher/main/.github/assets/descargar-launcher.png"

sed -e "s|{{VERSION}}|$VERSION|g" \
    -e "s|{{BUTTON_URL}}|$BUTTON_URL|g" \
    .github/RELEASE_TEMPLATE.md > /tmp/release-notes.md

gh release create v$VERSION \
  wow-colombia.exe wow-colombia.zip wow-colombia-pack.zip \
  --title "v$VERSION" \
  --notes-file /tmp/release-notes.md \
  --repo wco/launcher
```

## Editar un release existente

```bash
gh release edit vX.Y.Z --notes-file /tmp/release-notes.md --repo wco/launcher
```
