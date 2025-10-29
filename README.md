# Sorteo Selección Argentina

Landing estática para el sorteo de Revista Matices.

## Deploy en Vercel

1. Requisitos
   - Tener una cuenta en Vercel (`https://vercel.com`)
   - Tener este repo en GitHub (ya configurado)

2. Conectar el repo a Vercel
   - Entra a Vercel → `New Project` → Importa `IgnacioDiaz757/SeleccionArgentinaSorteo`
   - Framework Preset: `Other`
   - Build & Output Settings:
     - Build Command: vacío
     - Output Directory: `./` (raíz)
     - Root Directory: `./` (si te lo pide)
   - Variables de entorno: no necesarias
   - Clic en `Deploy`

3. Opcional: Vercel CLI
```bash
npm i -g vercel
vercel login
vercel --prod
```

## Configuración necesaria antes del lanzamiento
- Editar URLs reales del post de Instagram y Bases en `Index.html` (ver comentarios de CONFIGURACIÓN)
- Ajustar la fecha del contador en `Index.html`
- Subir `favicon.ico` si aún no lo agregaste

## Estructura
- `Index.html`: landing responsive con contador, confeti y SEO
- `vercel.json`: configuración de headers y limpieza de URLs
- `README.md`: este archivo
- `.gitignore`: ignores comunes

## Notas
- Imágenes cacheadas agresivamente (1 año) via `vercel.json`
- Respeta `prefers-reduced-motion` para accesibilidad
