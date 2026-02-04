# 🚀 Guía de Despliegue - Portfolio

Esta guía te ayudará a subir tu portfolio a GitHub y desplegarlo en Vercel o Netlify.

## 📋 Requisitos Previos

- [ ] Cuenta en [GitHub](https://github.com)
- [ ] [Git](https://git-scm.com/downloads) instalado en tu computadora
- [ ] Cuenta en [Vercel](https://vercel.com) o [Netlify](https://netlify.com)

## 📤 Paso 1: Subir a GitHub

### Opción A: Usando GitHub Desktop (Más fácil)

1. **Descarga GitHub Desktop**
   - Ve a https://desktop.github.com
   - Descarga e instala

2. **Crea un nuevo repositorio**
   - Abre GitHub Desktop
   - File → New Repository
   - Name: `portfolio` (o el nombre que prefieras)
   - Local Path: Selecciona la carpeta donde están tus archivos
   - Click en "Create Repository"

3. **Sube los archivos**
   - Arrastra tus archivos (index.html, styles.css, script.js, README.md) a la carpeta del repositorio
   - En GitHub Desktop verás los cambios
   - Escribe un mensaje: "Initial commit - Portfolio website"
   - Click en "Commit to main"
   - Click en "Publish repository"
   - Marca "Public" si quieres que sea público
   - Click en "Publish Repository"

### Opción B: Usando la Terminal/Línea de comandos

1. **Abre la terminal** en la carpeta de tu portfolio

2. **Ejecuta estos comandos uno por uno:**

```bash
# Inicializar Git
git init

# Agregar todos los archivos
git add .

# Crear el primer commit
git commit -m "Initial commit - Portfolio website"

# Crear el repositorio en GitHub (ve a github.com/new primero y copia la URL)
git remote add origin https://github.com/TU-USUARIO/portfolio.git

# Subir los archivos
git branch -M main
git push -u origin main
```

**Nota:** Reemplaza `TU-USUARIO` con tu nombre de usuario de GitHub

## 🌐 Paso 2: Desplegar en Vercel (Recomendado)

### ¿Por qué Vercel?
- ✅ Despliegue automático
- ✅ HTTPS gratis
- ✅ Dominio personalizado gratis (.vercel.app)
- ✅ Muy rápido

### Pasos:

1. **Ve a Vercel**
   - Abre https://vercel.com
   - Click en "Sign Up" o "Log In"
   - Usa tu cuenta de GitHub para iniciar sesión

2. **Importa tu proyecto**
   - Click en "Add New..." → "Project"
   - Busca tu repositorio "portfolio"
   - Click en "Import"

3. **Configura el proyecto**
   - Project Name: `portfolio` (o el que prefieras)
   - Framework Preset: selecciona "Other" o déjalo vacío
   - Root Directory: `./` (déjalo como está)
   - **NO necesitas cambiar nada más**

4. **Despliega**
   - Click en "Deploy"
   - Espera 30-60 segundos ⏳
   - ¡Listo! 🎉

5. **Tu sitio estará disponible en:**
   ```
   https://tu-proyecto.vercel.app
   ```

### Configurar dominio personalizado (Opcional)

1. En Vercel, ve a tu proyecto
2. Settings → Domains
3. Agrega tu dominio personalizado
4. Sigue las instrucciones para configurar DNS

## 🌐 Alternativa: Desplegar en Netlify

### Pasos:

1. **Ve a Netlify**
   - Abre https://app.netlify.com
   - Click en "Sign Up" o "Log In"
   - Usa tu cuenta de GitHub

2. **Importa tu proyecto**
   - Click en "Add new site" → "Import an existing project"
   - Selecciona "Deploy with GitHub"
   - Autoriza a Netlify si es necesario
   - Busca y selecciona tu repositorio "portfolio"

3. **Configura el despliegue**
   - Site name: elige un nombre único
   - Build command: déjalo vacío
   - Publish directory: déjalo vacío o pon `./`

4. **Despliega**
   - Click en "Deploy site"
   - Espera un momento ⏳
   - ¡Listo! 🎉

5. **Tu sitio estará disponible en:**
   ```
   https://tu-nombre.netlify.app
   ```

## 🔄 Actualizaciones Futuras

Cada vez que hagas cambios:

### Con GitHub Desktop:
1. Guarda tus cambios en los archivos
2. Abre GitHub Desktop
3. Verás los cambios listados
4. Escribe un mensaje describiendo los cambios
5. Click en "Commit to main"
6. Click en "Push origin"
7. Vercel/Netlify automáticamente actualizará tu sitio

### Con Terminal:
```bash
git add .
git commit -m "Descripción de los cambios"
git push
```

## 🎨 Personalización Adicional

### Cambiar colores:
Abre `styles.css` y modifica las variables en `:root`:

```css
:root {
    --color-primary: #1a1a2e;      /* Color principal */
    --color-highlight: #e94560;     /* Color de acento */
    /* ... más colores */
}
```

### Agregar más secciones:
1. Agrega la sección en `index.html`
2. Estiliza en `styles.css`
3. Actualiza la navegación si es necesario

## 📱 Verificar Responsive

Prueba tu sitio en:
- Chrome DevTools (F12 → Toggle device toolbar)
- Tu teléfono móvil
- Tablet
- Diferentes navegadores

## 🐛 Solución de Problemas

### El sitio no se ve bien:
- Verifica que todos los archivos estén en la misma carpeta
- Revisa la consola del navegador (F12) por errores
- Asegúrate de que los nombres de archivos coincidan exactamente

### No puedo hacer push a GitHub:
- Verifica tu conexión a internet
- Asegúrate de estar autenticado en Git
- Revisa que la URL del repositorio sea correcta

### El despliegue falló:
- Verifica que todos los archivos estén en GitHub
- Revisa los logs de error en Vercel/Netlify
- Asegúrate de que no haya errores en el código

## 📞 ¿Necesitas Ayuda?

Si tienes problemas:
1. Revisa los logs de error
2. Busca el error en Google
3. Consulta la documentación:
   - [GitHub Docs](https://docs.github.com)
   - [Vercel Docs](https://vercel.com/docs)
   - [Netlify Docs](https://docs.netlify.com)

## ✅ Checklist Final

- [ ] Archivos subidos a GitHub
- [ ] Repositorio público (si quieres compartirlo)
- [ ] Sitio desplegado en Vercel o Netlify
- [ ] Probado en diferentes dispositivos
- [ ] Información personal actualizada
- [ ] Enlaces de contacto funcionando

¡Felicidades! 🎉 Tu portfolio está en línea.

---

**Próximos pasos sugeridos:**
- Agregar más proyectos a medida que los completes
- Personalizar los colores a tu gusto
- Agregar un blog o sección de artículos
- Conectar con Google Analytics (opcional)
- Configurar un dominio personalizado
