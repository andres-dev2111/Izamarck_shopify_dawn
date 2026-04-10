# IZAMARCK SHOPIFY THEME
## Migración completa de React a Shopify Liquid

Este tema es una migración fiel del diseño original de Izamarck (React + Tailwind) a Shopify Dawn.

---

## 📦 CONTENIDO DEL TEMA

### ✅ Componentes Migrados

1. **Header & Navigation**
   - Announcement Bar con carrusel de anuncios
   - Navbar sticky con menú desktop y móvil
   - Logo centrado con navegación de género

2. **Homepage**
   - Hero Banner con CTAs
   - Categories Section (grid 2x2/4 columnas)
   - Featured Products
   - Lookbook masonry grid

3. **Collection Page**
   - Grid de productos responsive
   - Ordenamiento por precio/nombre/fecha
   - Paginación

4. **Product Page**
   - Galería de imágenes
   - Selector de variantes
   - Cantidad ajustable
   - Descripción del producto

5. **Footer**
   - Ticker animado
   - Logo y redes sociales
   - 3 columnas de links
   - Newsletter signup

---

## 🎨 ARCHIVOS CSS CREADOS

```
assets/
├── izamarck-theme.css           # Variables, utilidades, estilos base
├── izamarck-header.css          # Estilos del header/navbar
├── izamarck-announcement.css    # Announcement bar
├── izamarck-hero.css            # Hero banner
├── izamarck-categories.css      # Sección de categorías
├── izamarck-footer.css          # Footer completo
├── izamarck-products.css        # Grid de productos
├── izamarck-lookbook.css        # Lookbook masonry
├── izamarck-collection.css      # Página de colección
└── izamarck-product-page.css    # Página de producto
```

---

## 📄 SECCIONES LIQUID CREADAS

```
sections/
├── izamarck-announcement-bar.liquid
├── izamarck-header.liquid
├── izamarck-hero-banner.liquid
├── izamarck-categories.liquid
├── izamarck-footer.liquid
├── izamarck-featured-products.liquid
├── izamarck-lookbook.liquid
├── main-collection-product-grid-izm.liquid
├── main-product-izm.liquid
├── header-group.json
└── footer-group.json
```

---

## 🚀 INSTALACIÓN

### Opción 1: Shopify CLI (Recomendado)

1. Instala Shopify CLI:
```bash
npm install -g @shopify/cli @shopify/theme
```

2. Navega a la carpeta del tema:
```bash
cd izamarck-shopify-migrated
```

3. Conecta a tu tienda:
```bash
shopify theme dev --store=tu-tienda.myshopify.com
```

4. Sube el tema:
```bash
shopify theme push
```

### Opción 2: Upload Manual

1. Comprime toda la carpeta `izamarck-shopify-migrated` en un archivo .zip

2. Ve a tu Admin de Shopify → Online Store → Themes

3. Haz clic en "Add theme" → "Upload zip file"

4. Selecciona el archivo .zip y sube

5. Una vez subido, haz clic en "Customize" para configurar

---

## ⚙️ CONFIGURACIÓN POST-INSTALACIÓN

### 1. Configurar Menú de Navegación

1. Ve a **Navigation** en tu Admin
2. Crea un menú llamado `main-menu`
3. Añade los siguientes links:
   - Hombre → `/collections/hombre`
   - Mujer → `/collections/mujer`
   - Accesorios → `/collections/accesorios`

### 2. Configurar Homepage

1. Ve a **Online Store → Themes → Customize**
2. Selecciona la homepage
3. Configura las secciones:
   - **Announcement Bar**: Edita los 3 anuncios
   - **Hero Banner**: Sube imagen, edita textos y links
   - **Categories**: Sube 4 imágenes de categorías
   - **Lookbook**: Añade imágenes de looks

### 3. Configurar Footer

1. En el editor del tema, selecciona el Footer
2. Configura:
   - Redes sociales (Instagram, Facebook, Twitter, etc.)
   - 3 columnas de links
   - Newsletter
   - Copyright

### 4. Crear Colecciones

Crea las siguientes colecciones en Products → Collections:
- `hombre`
- `mujer`
- `accesorios`

---

## 🎨 COLORES Y VARIABLES

Los colores principales del tema están definidos en `izamarck-theme.css`:

```css
--izm-gold: #D4A843;         /* Dorado principal */
--izm-gold-hover: #c49730;   /* Dorado hover */
--izm-black: #030213;        /* Negro principal */
--izm-dark: #111;            /* Fondo oscuro */
--izm-white: #ffffff;        /* Blanco */
```

Para cambiar colores, edita estas variables en el archivo CSS.

---

## 📱 RESPONSIVE

El tema es completamente responsive:
- **Mobile**: Grid 2 columnas, menú hamburguesa
- **Tablet**: Grid 3 columnas
- **Desktop**: Grid 4 columnas, navegación completa

---

## ✨ CARACTERÍSTICAS

- ✅ Diseño fiel al original en React
- ✅ Completamente responsive
- ✅ Quick Add al carrito desde grid
- ✅ Paginación de productos
- ✅ Galería de imágenes en producto
- ✅ Selector de variantes
- ✅ Newsletter signup
- ✅ Redes sociales integradas
- ✅ Lookbook masonry grid
- ✅ Animaciones suaves

---

## 🔧 PERSONALIZACIÓN

### Cambiar Fuentes

Edita en el Theme Editor → Theme Settings → Typography

### Añadir Secciones

Todas las secciones de Izamarck están disponibles en el Theme Editor para añadir a cualquier página.

### Modificar Layout

Los templates JSON en `templates/` controlan qué secciones aparecen en cada tipo de página.

---

## 📞 SOPORTE

Para preguntas o problemas con la migración, contacta al desarrollador.

---

## 📝 NOTAS TÉCNICAS

### Diferencias con el Original React

1. **No hay estado global**: Shopify maneja el carrito del lado del servidor
2. **Sin búsqueda overlay**: Se puede añadir usando Ajax API de Shopify
3. **Sin sidebar de perfil**: Se redirecciona a la página de cuenta
4. **Quick Add simplificado**: Añade la primera variante disponible

### Mejoras Futuras Posibles

- [ ] Cart Drawer Ajax
- [ ] Search Overlay
- [ ] Profile Sidebar
- [ ] Filtros de colección avanzados
- [ ] Wishlist/Favoritos
- [ ] Quick View modal

---

## 🏆 CRÉDITOS

Diseño original: Izamarck (React/Tailwind)
Migración a Shopify: Claude
Fecha: Abril 2026

---

**¡Tema listo para usar!** 🎉
