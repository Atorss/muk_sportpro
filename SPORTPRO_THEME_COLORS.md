# SportPro Theme - Paleta de Colores Actualizada

## 📋 Resumen

Este documento describe la paleta de colores del tema de backend MuK personalizado para **SportPro**, diseñado para complementar y hacer contraste con los colores del sitio web.

---

## 🎨 PALETA DE COLORES

### Sitio Web Frontend (sportpro_website)

| Color | Hex | Uso |
|-------|-----|-----|
| **Verde Principal** | `#1a7f37` | Botones, headers, elementos principales |
| **Verde Oscuro** | `#0f5323` | Hover, degradados, fondos |
| **Naranja Acento** | `#ff6b35` | CTAs, highlights, elementos de acción |
| **Gris Claro** | `#f1f5f9` | Backgrounds, secciones |
| **Azul Oscuro** | `#0f172a` | Textos, footer |

---

### Backend Theme - Modo Claro (Light Mode)

Archivo: `muk_web_colors/static/src/scss/colors_light.scss`

| Variable | Color | Hex | Uso |
|----------|-------|-----|-----|
| `$mk_color_brand` | Verde Oscuro | `#0f5323` | Color de marca principal |
| `$mk_color_primary` | Verde Principal | `#1a7f37` | Color primario de acciones |
| `$mk_color_success` | Verde Principal | `#1a7f37` | Mensajes de éxito |
| `$mk_color_info` | Cyan | `#17A2B8` | Mensajes informativos |
| `$mk_color_warning` | Naranja Acento | `#ff6b35` | Advertencias |
| `$mk_color_danger` | Rojo | `#DC3545` | Errores y peligros |

---

### Backend Theme - Modo Oscuro (Dark Mode)

Archivo: `muk_web_colors/static/src/scss/colors_dark.scss`

| Variable | Color | Hex | Uso |
|----------|-------|-----|-----|
| `$mk_color_brand` | Verde Brillante | `#1fa855` | Color de marca (versión clara) |
| `$mk_color_primary` | Verde Brillante | `#2ecc71` | Color primario brillante |
| `$mk_color_success` | Verde Brillante | `#2ecc71` | Mensajes de éxito |
| `$mk_color_info` | Cyan Brillante | `#6AB5FB` | Mensajes informativos |
| `$mk_color_warning` | Naranja Brillante | `#ff8c5a` | Advertencias |
| `$mk_color_danger` | Rojo Brillante | `#FF5757` | Errores y peligros |

---

### Appsbar & Menú

Archivo: `muk_web_theme/static/src/scss/colors.scss`

| Variable | Color | Hex | Uso |
|----------|-------|-----|-----|
| `$mk_color_appbar_active` | Verde Principal | `#1a7f37` | Items activos en la barra lateral |
| `$mk_color_appbar_background` | Gris Oscuro | `#111827` | Fondo de la barra lateral |
| `$mk_color_appbar_text` | Gris Claro | `#DEE2E6` | Texto de la barra lateral |
| `$mk_color_appsmenu_text` | Blanco Roto | `#F8F9FA` | Texto del menú de apps |

---

## 🎯 FILOSOFÍA DEL DISEÑO

### Coherencia Visual
Los colores del backend complementan perfectamente el sitio web:
- **Verde** como color corporativo principal (unifica frontend y backend)
- **Naranja** como acento energético deportivo
- **Consistencia** en toda la experiencia del usuario

### Contraste y Accesibilidad
- ✅ **Alto contraste** para legibilidad
- ✅ **Colores diferenciados** para estados (success, warning, danger)
- ✅ **Modo oscuro optimizado** con colores brillantes
- ✅ **Accesibilidad WCAG AA** en combinaciones de colores

### Identidad Deportiva
- Verde = Naturaleza, deporte, crecimiento, vitalidad
- Naranja = Energía, acción, dinamismo
- Paleta moderna y profesional para una academia deportiva

---

## 📂 ARCHIVOS MODIFICADOS

```
muk_sportpro/
├── muk_web_colors/
│   └── static/src/scss/
│       ├── colors_light.scss       ✅ Actualizado - Paleta modo claro
│       └── colors_dark.scss        ✅ Actualizado - Paleta modo oscuro
└── muk_web_theme/
    └── static/src/scss/
        └── colors.scss              ✅ Actualizado - Color appbar activo
```

---

## 🚀 APLICACIÓN DE CAMBIOS

### Para ver los cambios:

1. **Actualizar el módulo:**
   ```bash
   cd /home/altorresp/Proyectos/nuevo_18/odoo-docker-build
   docker compose restart odoo18
   ```

2. **Limpiar caché del navegador:**
   - `Ctrl + Shift + R` (Windows/Linux)
   - `Cmd + Shift + R` (Mac)

3. **Forzar actualización de assets (si es necesario):**
   - Ir a: Configuración > Activar modo desarrollador
   - Ir a: Configuración > Técnico > Assets
   - Clic en: Regenerar Assets

### Verificación:

- ✅ Botones primarios deben ser verde `#1a7f37`
- ✅ Items activos en sidebar deben ser verde
- ✅ Badges de éxito deben ser verde
- ✅ Badges de advertencia deben ser naranja `#ff6b35`
- ✅ En modo oscuro, los verdes deben ser más brillantes

---

## 🎨 EJEMPLOS DE USO

### Botones
```html
<!-- Botón principal (verde) -->
<button class="btn btn-primary">Guardar</button>

<!-- Botón de éxito (verde) -->
<button class="btn btn-success">Confirmar</button>

<!-- Botón de advertencia (naranja) -->
<button class="btn btn-warning">Atención</button>

<!-- Botón de peligro (rojo) -->
<button class="btn btn-danger">Eliminar</button>
```

### Badges
```html
<span class="badge bg-success">Activo</span>
<span class="badge bg-warning">Pendiente</span>
<span class="badge bg-danger">Inactivo</span>
```

### Alertas
```html
<div class="alert alert-success">Operación exitosa</div>
<div class="alert alert-warning">Advertencia importante</div>
<div class="alert alert-danger">Error crítico</div>
```

---

## 📊 MAPEO DE COLORES

### Frontend → Backend

| Elemento Frontend | Color Frontend | Elemento Backend | Color Backend |
|-------------------|----------------|------------------|---------------|
| Botón CTA Hero | Verde `#1a7f37` | Botón Primary | Verde `#1a7f37` |
| Cards Hover | Verde `#0f5323` | Brand Color | Verde `#0f5323` |
| Acento Warning | Naranja `#ff6b35` | Warning Badge | Naranja `#ff6b35` |
| Footer Dark | Azul `#0f172a` | Appbar BG | Gris `#111827` |

---

## 🔄 COMPATIBILIDAD

- ✅ **Odoo 18.0**
- ✅ **MuK Web Theme v18.0.1.2.4**
- ✅ **MuK Web Colors v18.0.1.0.6**
- ✅ **Responsive Design**
- ✅ **Modo Claro y Oscuro**

---

## 📝 NOTAS PARA DESARROLLADORES

### Sobrescribir Colores
Si necesitas personalizar colores específicos, edita:
```scss
// muk_web_colors/static/src/scss/colors_light.scss
$mk_color_primary: #TU_COLOR_AQUI;
```

### Agregar Nuevos Colores
```scss
// Define tu color
$mk_color_custom: #123456;

// Agrégalo al mapa de colores
$o-theme-text-colors: (
    "primary": $mk-color-brand,
    "custom": $mk-color-custom,  // ← Nuevo color
);
```

### Testing
```bash
# Ver logs durante actualización
docker logs -f odoo18

# Reiniciar contenedor
docker compose restart odoo18
```

---

## 🎯 RESULTADO ESPERADO

**Antes (Tema Original MuK):**
- Azul oscuro `#243742` como color principal
- Azul claro `#5D8DA8` como primario
- Sin coherencia con el sitio web

**Después (Tema SportPro):**
- ✅ Verde oscuro `#0f5323` como marca
- ✅ Verde principal `#1a7f37` como primario
- ✅ Naranja `#ff6b35` como acento
- ✅ **100% coherente** con el sitio web
- ✅ **Identidad deportiva** clara
- ✅ **Contraste profesional**

---

**Última actualización:** 2026-04-09
**Versión:** 1.0.0
**Autor:** SportPro Development Team
