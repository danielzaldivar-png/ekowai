# DWA Hydraulik-Rechner

Aplicación web para cálculos hidráulicos conforme a normas DWA alemanas.

## Estructura

```
dwa-app/
├── server.js        ← Entry point (Hostinger lo detecta automáticamente)
├── package.json
├── .gitignore
└── public/
    └── index.html   ← La app completa
```

## Deploy en Hostinger

1. Sube este proyecto a GitHub (repo privado o público)
2. En hPanel → Websites → Add Website → Node.js Apps
3. Conecta tu repositorio GitHub
4. Hostinger detecta automáticamente:
   - Framework: **Express / Other**
   - Entry file: **server.js**
   - Build command: `npm install`
   - Start command: `npm start`
5. Clic en Deploy

## Variables de entorno (no requeridas por ahora)
Las credenciales de Supabase están en el HTML directamente.
En producción avanzada puedes moverlas a variables de entorno.

## Base de datos
- Supabase PostgreSQL (Frankfurt)
- Tablas: `projects`, `calculations`
