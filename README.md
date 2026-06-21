# Portal de Seguimiento Acercobalt

Portal de cliente para seguimiento de obras en tiempo real.

## Características

- ✅ Autenticación por PIN
- ✅ Visualización de obras en progreso
- ✅ Tracking de fases por obra
- ✅ Seguimiento de entregas 2026
- ✅ Filtros y búsqueda
- ✅ Responsivo (mobile-first)

## Tecnología

- **Frontend:** HTML5 + CSS3 + JavaScript vanilla
- **Backend:** Supabase (PostgreSQL + Edge Functions)
- **Hosting:** Vercel
- **Dominio:** portal.acercobalt.com

## Estructura

```
acercobalt-portal/
├── index.html          # Portal completo (HTML + CSS + JS)
├── vercel.json         # Configuración de Vercel
├── .gitignore          # Archivos a excluir de Git
└── README.md           # Este archivo
```

## Despliegue

1. Hacer push a GitHub
2. Conectar en Vercel
3. Configurar dominio personalizado: `portal.acercobalt.com`
4. Listo ✓

## Variables de conexión

El portal se conecta a Supabase vía:
- URL: `https://kzjhymovdatnontzvkum.supabase.co`
- ANON_KEY: `sb_publishable_SiBFvz-ruZTZzPTXshhjgg_CTDGDusD`
- Edge Function: `/functions/v1/rapid-handler`

## Desarrollo local

Para probar el portal sin Vercel, abre `index.html` directamente en el navegador.

## Contacto

Acercobalt - facturas@acercobalt.com
