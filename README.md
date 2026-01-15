# Catálogo digital con WhatsApp

Catálogo web completo con:
- ✅ Catálogo de productos dinámico
- ✅ Botones de contacto por WhatsApp para cada producto
- ✅ Formulario de pedidos que envía a WhatsApp
- ✅ Panel de administrador para editar productos sin código
- ✅ Almacenamiento local (LocalStorage) — sin necesidad de servidor

## Uso rápido

### 1️⃣ Personalizar el número de WhatsApp

Abre `index.html` o `admin.html` y busca la línea:
```javascript
const PHONE = '1234567890';
```

Reemplázalo con tu número en formato internacional sin `+` ni espacios:
- España: `34` + tu número (ej: `34123456789`)
- Colombia: `57` + tu número (ej: `573001234567`)
- México: `52` + tu número (ej: `525512345678`)

### 2️⃣ Panel de administrador

Abre `admin.html` en el navegador. Desde aquí puedes:
- ➕ Agregar nuevos productos
- ✏️ Editar productos existentes
- 🗑️ Eliminar productos
- 💾 Los cambios se guardan automáticamente en el navegador

### 3️⃣ Formulario de pedidos

En `index.html` hay un formulario donde los clientes pueden:
- Escribir su nombre y email
- Describir qué desean pedir
- Enviar directamente a WhatsApp con un click

### 4️⃣ Probar localmente

Simplemente abre `index.html` en el navegador (doble clic).
- En **móvil**: abrirá la app de WhatsApp
- En **desktop**: abrirá WhatsApp Web (si está disponible)

## Características técnicas

- **LocalStorage**: Los productos se guardan en el navegador del cliente (no necesita servidor)
- **Sin dependencias**: Solo HTML, CSS y JavaScript vanilla
- **Responsivo**: Se ve bien en celular, tablet y escritorio
- **Fácil de personalizar**: Edita el `admin.html` para cambiar productos sin tocar código

## Despliegue

### Opción 1: GitHub Pages (gratis)
1. Crea un repositorio en GitHub
2. Sube estos archivos
3. Ve a Settings > Pages > Source y selecciona la rama `main`
4. ¡Listo! Tu catálogo estará en `https://tu-usuario.github.io/nombre-repo`

### Opción 2: Netlify (gratis)
1. Ve a [netlify.com](https://netlify.com)
2. Conecta tu repositorio de GitHub o sube los archivos directamente
3. ¡Se despliega automáticamente!

### Opción 3: Vercel (gratis)
Similar a Netlify, ve a [vercel.com](https://vercel.com) y conecta tu repo.

### Opción 4: Hosting estático tradicional
Sube los archivos a cualquier hosting (Hostinger, GoDaddy, etc.) vía FTP.

## Personalización avanzada

**Cambiar colores:**
En `style.css`, busca `:root` y modifica las variables:
```css
:root{
  --bg:#f7f7f8;        /* Fondo general */
  --card:#ffffff;      /* Color de tarjetas */
  --accent:#25D366;    /* Color verde WhatsApp */
}
```

**Cambiar mensajes:**
En `index.html` o `admin.html`, busca la función `makeMessage()` y personalízala.

## Estructura de archivos

```
proyecto/
├── index.html          # Catálogo principal + formulario pedidos
├── admin.html          # Panel de administrador
├── style.css           # Estilos compartidos
└── README.md           # Este archivo
```

## Notas importantes

- Los productos se guardan en **LocalStorage del navegador** (cada navegador tiene su propia copia)
- Si borras datos del navegador, se restablecen los productos por defecto
- Para sincronizar productos entre navegadores, necesitarías un servidor (backend con base de datos)
- El número de WhatsApp se personaliza en el código, no es configurable desde la UI (para seguridad)

## Soporte

¿Necesitas ayuda? Puedo:
- Cambiar diseño o colores
- Agregar más funciones
- Optimizar SEO
- Integrar con servicios (email, pagos, etc.)

---
**Hecho con ❤️ — Listo para personalizar y subir a la web.**

