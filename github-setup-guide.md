# Guía: Crear repo en GitHub con portal-supabase.html

## PASO 1: Prepara el archivo para GitHub
El archivo HTML necesita estar en una carpeta con estructura correcta para Vercel.

## PASO 2: Crea la carpeta del proyecto localmente (en tu PC)
1. Abre tu PC
2. Crea una carpeta llamada `acercobalt-portal` en un lugar fácil de encontrar (ej: tu Desktop o Documentos)

## PASO 3: Crea los archivos necesarios

Dentro de la carpeta `acercobalt-portal`, crea estos archivos:

### 3a) Archivo `index.html`
Copia todo el contenido de `portal-supabase.html` y guárdalo como `index.html` en esa carpeta.

(Descargar: portal-supabase.html de aquí ↓)

### 3b) Archivo `vercel.json` (IMPORTANTE)
Crea un archivo de texto llamado `vercel.json` con este contenido exacto:

```json
{
  "buildCommand": null,
  "installCommand": null,
  "devCommand": null,
  "framework": null,
  "public": true,
  "cleanUrls": true,
  "trailingSlash": false
}
```

### 3c) Archivo `.gitignore` (opcional pero recomendado)
Crea un archivo de texto llamado `.gitignore` con:

```
node_modules/
.DS_Store
*.log
.env
```

### 3d) Archivo `README.md` (opcional)
Crea un archivo de texto llamado `README.md` con:

```markdown
# Portal de Seguimiento Acercobalt

Portal de cliente para seguimiento de obras en tiempo real.

Conectado a Supabase para autenticación y gestión de datos.

## Despliegue
Alojado en Vercel en https://portal.acercobalt.com
```

## Estructura final en tu carpeta:
```
acercobalt-portal/
├── index.html
├── vercel.json
├── .gitignore
└── README.md
```

---

# PASO 4: Git en tu PC (Windows/Mac)

### 4a) Instala Git (si no lo tienes)
- Windows: https://git-scm.com/download/win
- Mac: https://git-scm.com/download/mac
- Linux: `sudo apt install git`

### 4b) Abre Terminal/CMD en la carpeta `acercobalt-portal`

**Windows (PowerShell/CMD):**
- Click derecho en la carpeta → "Abrir PowerShell aquí" o "Abrir terminal aquí"

**Mac/Linux:**
- Abre Terminal → `cd ~/ruta/a/acercobalt-portal`

### 4c) Inicia Git en la carpeta

```bash
git init
git config user.name "Tu Nombre"
git config user.email "tu.email@gmail.com"
git add .
git commit -m "Initial commit: Portal Acercobalt"
```

---

# PASO 5: Crea repo en GitHub

### 5a) Ve a https://github.com
- Si no tienes cuenta, crea una gratis

### 5b) Click en "+" (arriba a la derecha) → "New repository"

### 5c) Rellena así:
- **Repository name:** `acercobalt-portal`
- **Description:** "Portal de seguimiento de obras Acercobalt"
- **Public:** ✓ Seleccionado
- **README:** Deja NO seleccionado (tú ya creaste uno)
- **gitignore:** Deja "None"
- **License:** Deja "None"

### 5d) Click en "Create repository"

---

# PASO 6: Sube tu código a GitHub

GitHub te mostrará instrucciones. En tu Terminal/CMD, copia y ejecuta:

```bash
git remote add origin https://github.com/TU_USUARIO/acercobalt-portal.git
git branch -M main
git push -u origin main
```

(Cambia `TU_USUARIO` por tu nombre de usuario de GitHub)

Si te pide usuario/contraseña:
- Usuario: Tu nombre de GitHub
- Contraseña: Usa un "Personal Access Token" (no la contraseña real)
  - Ve a GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
  - Click "Generate new token (classic)"
  - Marca "repo" y copia el token
  - Usa ese token como contraseña en Terminal

---

# ✅ Listo en GitHub

Tu repo ahora está en: `https://github.com/TU_USUARIO/acercobalt-portal`

Puedes verlo público, clonar, etc.

---

# PASO 7: Conectar a Vercel (siguiente paso)

Una vez que confirmes que el repo está en GitHub, conectamos Vercel.
