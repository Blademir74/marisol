# Sitio Oficial — Diputada Marisol Bazán Fernández
**Distrito 04 Acapulco · LXIV Legislatura · Congreso de Guerrero**

## Estructura del proyecto

```
marisol-bazan-site/
├── public/
│   └── index.html       ← El sitio completo (one-page)
├── vercel.json          ← Configuración de despliegue
├── package.json
└── .gitignore
```

---

## 🚀 Despliegue en Vercel

### Opción A — Desde GitHub (recomendado)

1. Sube este proyecto a un repositorio de GitHub:
   ```bash
   git init
   git add .
   git commit -m "Sitio Marisol Bazán - versión inicial"
   git remote add origin https://github.com/tu-usuario/marisol-bazan-site.git
   git push -u origin main
   ```

2. Ve a [vercel.com](https://vercel.com) → **New Project** → Importa el repositorio.

3. Vercel detecta automáticamente la configuración. Haz clic en **Deploy**.

4. En segundos tendrás una URL tipo `marisol-bazan-site.vercel.app`.

### Opción B — Desde la CLI de Vercel

```bash
# 1. Instala la CLI (solo la primera vez)
npm install -g vercel

# 2. Dentro de la carpeta del proyecto
cd marisol-bazan-site
vercel

# 3. Sigue las instrucciones del asistente de Vercel
# Cuando pregunte "In which directory is your code located?" → responde: ./public
```

### Dominio personalizado (opcional)

Desde el panel de Vercel:  
**Settings → Domains → Add** → escribe tu dominio, ej: `marisolbazan.com`

Luego configura los DNS con tu proveedor de dominio apuntando a Vercel:
- Registro **A** → `76.76.21.21`
- Registro **CNAME** → `cname.vercel-dns.com`

---

## ✏️ Personalización antes de publicar

Abre `public/index.html` y actualiza estos datos:

| Línea | Qué cambiar |
|-------|-------------|
| `wa.me/527441234567` | Número real de WhatsApp (x3 veces en el archivo) |
| Links de Facebook, YouTube, Instagram | URLs reales de las redes oficiales |
| `congresoguerrero.gob.mx` | Verificar que sea la URL correcta |
| Fotos hero/quién/collage | Reemplazar URLs de ibb.co por hosting propio si se desea |

---

## 📸 Sobre las imágenes

Las imágenes se cargan desde URLs externas (ibb.co). Para producción se recomienda:
1. Subir las fotos a la carpeta `public/images/`
2. Actualizar las rutas en el HTML: `src="images/marisol-hero.jpg"`
3. Esto mejora velocidad de carga y evitar dependencia de terceros.

---

© 2025 · Diputada Local Marisol Bazán Fernández · Distrito 04, Acapulco, Guerrero
