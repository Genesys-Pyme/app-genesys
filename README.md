# Genesys App — Landing Page

Landing page para `app.genesys.com.ar`.

## Estructura

```
genesys-app-landing/
├── index.html       ← página principal
├── css/
│   └── style.css    ← estilos custom
├── js/
│   └── main.js      ← scripts
└── README.md
```

## Deploy en Netlify desde GitHub

1. Subí esta carpeta como repositorio en GitHub
2. En Netlify → "Add new site" → "Import from Git"
3. Conectá el repositorio
4. Build settings:
   - Build command: (vacío, no hay build)
   - Publish directory: `.` (punto, raíz del repo)
5. Deploy

## Configurar subdominio app.genesys.com.ar

### En Netlify:
1. Site settings → Domain management → Add custom domain
2. Escribí `app.genesys.com.ar`
3. Copiá el valor CNAME que te da Netlify

### En Don Web:
1. Panel → Dominios → genesys.com.ar → DNS
2. Agregar registro:
   - Tipo: CNAME
   - Nombre: app
   - Valor: (el que te dio Netlify)
   - TTL: 3600
3. Guardar y esperar 15-30 minutos

## Personalización

Antes de publicar, actualizá en `index.html`:
- Los precios en la sección #precios
- El número de WhatsApp (buscar `2604104160`)
- El link de demo (buscar `exodocell.netlify.app`)
