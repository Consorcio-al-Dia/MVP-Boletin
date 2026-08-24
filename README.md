# Código Civil y Comercial de la Nación — Libro Digital

Visor flipbook del Código Civil y Comercial de la Nación (Argentina), con efecto de paso de página, navegación por teclado, ir a página y pantalla completa.

Construido con [StPageFlip](https://github.com/Nodlik/StPageFlip) (`page-flip@2.0.7`, incluido localmente en `js/`, sin depender de CDNs).

## Estructura

```
├── index.html    # visor
├── js/           # librería page-flip (UMD para navegador)
├── pages/        # 517 imágenes JPG de las páginas
└── pdf/          # PDF original descargable
```

## Uso local

Por cómo carga las imágenes, hace falta un servidor HTTP (no alcanza con abrir el archivo directamente):

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Publicar en GitHub Pages

1. Creá un repositorio en GitHub y subé este contenido a la rama `main`.
2. En el repo: **Settings → Pages**.
3. En **Source**: *Deploy from a branch* → rama `main`, carpeta `/ (root)` → **Save**.
4. El sitio queda disponible en `https://<usuario>.github.io/<repo>/`.

## Controles

| Acción | Control |
|---|---|
| Pasar hoja | Clic cerca del borde · Flechas ←/→ |
| Ir a página | Número en la barra superior |
| Pantalla completa | Botón ⛶ o `F11` |
| Descargar PDF | Botón ⭳ |
