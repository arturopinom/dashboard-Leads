# 🚀 Guía Rápida - Actualización Mensual

## 📅 Cada mes, sigue estos pasos (toma 2 minutos):

### 1. Ve a tu repositorio en GitHub
```
https://github.com/TU-USUARIO/dashboard-leads
```

### 2. Abre el archivo data.json
- Click en `data.json`
- Click en el ícono del lápiz ✏️ (arriba a la derecha)

### 3. Ubica el año actual (2025 por ejemplo)

Busca esta sección:
```json
"2025": {
  "months": ["Ene", "Feb", "Mar", "Abr", "May", "Jun", "Jul", "Ago", "Sep", "Oct", "Nov", "Dic"],
```

### 4. Actualiza los números

#### Ejemplo: Agregar datos de Noviembre 2025

**ANTES:**
```json
"1 DÍA GRATIS (WEB)": [4154, 3336, 3598, 2494, 2916, 3035, 3973, 3384, 2970, 3520, 0, 0],
```

**DESPUÉS:** (Suponiendo que Noviembre tuvo 4500 leads)
```json
"1 DÍA GRATIS (WEB)": [4154, 3336, 3598, 2494, 2916, 3035, 3973, 3384, 2970, 3520, 4500, 0],
```

### 5. Actualiza TODOS los canales

Repite el paso 4 para:
- 1 DÍA GRATIS (WEB)
- FORMULARIO META
- SEMÁFORO NUTRICIONAL
- PRE LEADS MAILING PT
- MANYCHAT

### 6. Actualiza el TOTAL

**MUY IMPORTANTE:** El total debe ser la suma de todos los canales.

Si tus canales sumaron 15,000 en Noviembre:

**ANTES:**
```json
"total": [9855, 9276, 11502, 8716, 9580, 12639, 13926, 17286, 13392, 5364, 0, 0]
```

**DESPUÉS:**
```json
"total": [9855, 9276, 11502, 8716, 9580, 12639, 13926, 17286, 13392, 5364, 15000, 0]
```

### 7. Guarda los cambios

- Scroll hasta abajo
- En "Commit message" escribe: "Actualización Noviembre 2025"
- Click en **"Commit changes"**

### 8. ¡Listo! 🎉

Espera 2-3 minutos y tu dashboard en:
```
https://TU-USUARIO.github.io/dashboard-leads/
```
Ya estará actualizado con los nuevos datos.

---

## 🎯 Checklist Mensual

Usa esta lista cada mes:

- [ ] Abrir data.json en GitHub
- [ ] Actualizar canal "1 DÍA GRATIS (WEB)"
- [ ] Actualizar canal "FORMULARIO META"
- [ ] Actualizar canal "SEMÁFORO NUTRICIONAL"
- [ ] Actualizar canal "PRE LEADS MAILING PT"
- [ ] Actualizar canal "MANYCHAT"
- [ ] Actualizar array "total"
- [ ] Verificar que la suma coincida
- [ ] Commit con mensaje descriptivo
- [ ] Esperar 2-3 minutos
- [ ] Verificar dashboard actualizado

---

## 🆘 Errores Comunes

### Error: "Invalid JSON"
**Problema:** Olvidaste una coma o corchete
**Solución:** Copia tu JSON y pégalo en [jsonlint.com](https://jsonlint.com) para ver el error

### Error: Los números no suman
**Problema:** El total no coincide con la suma de canales
**Solución:** Usa una calculadora y verifica la suma

### Error: El dashboard no se actualiza
**Problema:** GitHub Pages toma unos minutos
**Solución:** Espera 5 minutos y refresca con Ctrl+F5

---

## 💡 Tips

1. **Copia de seguridad**: Antes de editar, copia todo el contenido del archivo por si algo sale mal
2. **Doble verificación**: Revisa los números antes de hacer commit
3. **Historial**: Si algo sale mal, GitHub guarda todas las versiones anteriores

---

**¿Dudas?** Lee el README.md completo para más detalles.
