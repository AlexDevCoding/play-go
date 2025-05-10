# 🛍️ Tienda Virtual - Documentación de Carpetas

Este proyecto es una tienda virtual desarrollada con **HTML**, **Tailwind CSS**, **PHP**, **JavaScript** y **PostgreSQL**, con dos niveles de usuario: **Administrador** y **Cliente**.

---

## 📁 Estructura de Carpetas

### `assets/`
Contiene recursos estáticos del proyecto.
- `css/`: Estilos personalizados con Tailwind (`tailwind.css`).
- `js/`: Scripts JavaScript generales y del carrito.
- `img/`: Imágenes del sitio (productos, íconos, etc.).

---

### `includes/`
Fragmentos PHP reutilizables en diferentes vistas.
- `header.php`: Cabecera HTML común.
- `footer.php`: Pie de página.
- `navbar.php`: Menú de navegación (varía según el rol del usuario).

---

### `admin/`
Panel de control para el administrador.
- `dashboard.php`: Resumen general.
- `productos.php`: Gestión de productos.
- `pedidos.php`: Gestión de pedidos.
- `usuarios.php`: Administración de usuarios.
- `perfil.php`: Perfil del administrador.

---

### `cliente/`
Páginas accesibles para usuarios registrados (clientes).
- `inicio.php`: Página de inicio o catálogo.
- `producto.php`: Detalles de un producto.
- `carrito.php`: Carrito de compras.
- `historial.php`: Historial de pedidos del cliente.
- `perfil.php`: Gestión del perfil del cliente.

---

### `auth/`
Manejo de autenticación.
- `login.php`: Inicio de sesión.
- `registro.php`: Registro de nuevos clientes.
- `logout.php`: Cierre de sesión.
- `validar_login.php`: Lógica para validar el acceso.

---

### `config/`
Configuración general del proyecto.
- `config.php`: Conexión a la base de datos PostgreSQL y constantes globales.

---

### `controllers/`
Controladores con la lógica del sistema (MVC).
- `productoController.php`: Operaciones de productos.
- `pedidoController.php`: Lógica de pedidos.
- `usuarioController.php`: Manejo de usuarios.

---

### `database/`
Archivos relacionados con la base de datos.
- `estructura.sql`: Script para crear las tablas necesarias en PostgreSQL.

---

### `middleware/`
Verificaciones de acceso y control de roles.
- `auth.php`: Protege rutas restringidas según si el usuario está logueado y su tipo.

---

### Archivos raíz
- `index.php`: Página principal de la tienda.
- `404.php`: Página de error personalizada.
- `.htaccess`: Reglas de redirección, URLs limpias, etc.

---

## ✅ Roles de usuario

- **Administrador:** Puede gestionar productos, usuarios y pedidos.
- **Cliente:** Puede navegar, comprar productos y ver su historial.

---

## 💡 Recomendaciones

- Usa sesiones PHP para manejar el login y los roles.
- Protege rutas sensibles con el middleware.
- Mantén separados los archivos de lógica (`controllers/`) de las vistas (`admin/`, `cliente/`).
