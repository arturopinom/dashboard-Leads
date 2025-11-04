# 🚀 Dashboard de Leads - GitHub Pages

Dashboard interactivo para análisis de leads con actualización automática desde GitHub.

## 📋 ¿Qué incluye este dashboard?

- ✅ Métricas clave (Total, Promedio, Tendencia, Riesgo)
- 📊 Gráficos interactivos con Chart.js
- 🔄 Comparación 2024 vs 2025
- 🎯 Proyecciones automáticas
- ⚡ Análisis de concentración de riesgo
- 💡 Insights y recomendaciones inteligentes

## 🎯 Configuración en GitHub Pages (5 minutos)

### Paso 1: Crear Repositorio en GitHub

1. Ve a [github.com](https://github.com) y haz login
2. Click en el botón **"+"** arriba a la derecha → **"New repository"**
3. Nombra tu repositorio: `dashboard-leads` (o el nombre que prefieras)
4. Marca como **"Public"**
5. Click en **"Create repository"**

### Paso 2: Subir los archivos

Tienes 2 opciones:

#### Opción A: Subir por la web (más fácil)

1. En tu repositorio recién creado, click en **"uploading an existing file"**
2. Arrastra estos 3 archivos:
   - `index.html`
   - `data.json`
   - `README.md`
3. Escribe un mensaje: "Initial commit - Dashboard de Leads"
4. Click en **"Commit changes"**

#### Opción B: Usar Git (si ya lo tienes)

```bash
git init
git add index.html data.json README.md
git commit -m "Initial commit - Dashboard de Leads"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/dashboard-leads.git
git push -u origin main
```

### Paso 3: Activar GitHub Pages

1. En tu repositorio, ve a **"Settings"** (arriba)
2. En el menú izquierdo, click en **"Pages"**
3. En **"Branch"**, selecciona **"main"** y carpeta **"/ (root)"**
4. Click en **"Save"**
5. ¡Listo! En 1-2 minutos tu dashboard estará en:
   ```
   https://TU-USUARIO.github.io/dashboard-leads/
   ```

## 📝 Cómo actualizar los datos

### Actualización Directa en GitHub (Recomendado)

1. Ve a tu repositorio en GitHub
2. Click en el archivo **`data.json`**
3. Click en el ícono del lápiz ✏️ (Edit this file)
4. Actualiza los números que necesites
5. Scroll abajo y click en **"Commit changes"**
6. ¡Tu dashboard se actualiza automáticamente en 1-2 minutos!

### Estructura del archivo data.json

```json
{
  "2025": {
    "months": ["Ene", "Feb", "Mar", "Abr", "May", "Jun", "Jul", "Ago", "Sep", "Oct", "Nov", "Dic"],
    "categories": {
      "1 DÍA GRATIS (WEB)": [4154, 3336, 3598, 2494, 2916, 3035, 3973, 3384, 2970, 3520, 0, 0],
      "FORMULARIO META": [513, 3759, 5601, 5637, 4681, 6311, 4164, 10572, 4887, 0, 0, 0]
    },
    "total": [9855, 9276, 11502, 8716, 9580, 12639, 13926, 17286, 13392, 5364, 0, 0]
  }
}
```

### ⚠️ Importante al actualizar:

1. **Meses con datos en 0**: Deja en `0` los meses sin datos aún
2. **Total mensual**: Debe ser la suma de todos los canales de ese mes
3. **Formato JSON**: Respeta las comas y corchetes (usa un validador JSON si tienes dudas)

### Ejemplo: Agregar datos de Noviembre 2025

Si Noviembre tuvo 5,000 leads totales, actualiza así:

```json
"total": [9855, 9276, 11502, 8716, 9580, 12639, 13926, 17286, 13392, 5364, 5000, 0]
```

Y actualiza cada canal con sus números respectivos.

## 🎨 Personalización

### Cambiar el título

Edita el archivo `index.html`, línea 229:
```html
<h1>Dashboard de Leads</h1>
```

### Agregar un nuevo canal

En `data.json`, agrega una nueva línea en `categories`:
```json
"categories": {
  "1 DÍA GRATIS (WEB)": [...],
  "TU NUEVO CANAL": [100, 200, 300, ...]
}
```

### Cambiar colores

En `index.html`, busca la línea con `colors` (alrededor de línea 650):
```javascript
const colors = ['#667eea', '#764ba2', '#f093fb', '#4facfe', '#43e97b'];
```

Cambia los códigos de color hexadecimales a tu gusto.

## 🔧 Solución de problemas

### El dashboard muestra "Error al cargar datos"
- Verifica que `data.json` esté en la misma carpeta que `index.html`
- Revisa que el JSON no tenga errores de sintaxis (usa [jsonlint.com](https://jsonlint.com))

### Los datos no se actualizan
- Espera 2-3 minutos después de hacer commit
- Refresca con Ctrl+F5 (o Cmd+Shift+R en Mac) para limpiar caché
- Verifica que el archivo se actualizó en GitHub

### El gráfico se ve raro
- Asegúrate que el `total` coincida con la suma de los canales
- Verifica que todos los arrays tengan la misma longitud (12 elementos)

## 📱 Compartir el Dashboard

Una vez configurado, comparte tu link:
```
https://TU-USUARIO.github.io/dashboard-leads/
```

El dashboard es:
- ✅ Responsive (se ve bien en móvil y tablet)
- ✅ Público (cualquiera con el link puede verlo)
- ✅ Actualizable en tiempo real

## 🎯 Tips Pro

1. **Actualización mensual**: Marca un recordatorio el día 1 de cada mes para actualizar los datos
2. **Backup**: GitHub guarda todas las versiones anteriores, nunca pierdes datos
3. **Colaboración**: Puedes agregar colaboradores que también pueden editar los datos
4. **Analytics**: Agrega Google Analytics para ver cuántas personas consultan el dashboard

## 📞 Soporte

¿Problemas o dudas? Revisa:
- [Documentación de GitHub Pages](https://docs.github.com/es/pages)
- [Validador JSON](https://jsonlint.com)

---

**¡Tu dashboard está listo! 🎉**

Desarrollado con ❤️ por Claude
