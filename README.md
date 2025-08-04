# Helmets Pro 🛡️🛒 – Tienda de Cascos (v2.0)

## Descripción del Proyecto
Helmets Pro es una tienda virtual especializada en la venta de cascos para motociclistas, desarrollada con tecnologías web tradicionales (PHP, MySQL, Bootstrap). Este proyecto busca ofrecer una plataforma sólida, escalable y segura, enfocada en la experiencia de usuario y en las buenas prácticas de desarrollo web.

## Tecnologías Utilizadas
- **Backend**: PHP 8.2.4 (PDO para conexión segura)
- **Base de Datos**: MySQL (MariaDB 10.4.28)
- **Frontend**: Bootstrap 4.3.1, HTML5, CSS3
- **Servidor Local**: XAMPP (Apache + MySQL)
- **Control de Versiones**: Git & GitHub

## Estructura de Carpetas
```
sitioweb/
├── index.php
├── productos.php
├── nosotros.php
├── carrito.php
├── login.php
├── registro.php
├── pedido_confirmado.php
├── template/
│   ├── cabecera.php
│   └── pie.php
├── administrador/
│   ├── index.php
│   ├── inicio.php
│   ├── estadisticas.php
│   ├── config/
│   │   └── bd.php
│   └── seccion/
│       └── productos.php
├── clases/
│   ├── DB.php
│   ├── Carrito.php
│   ├── Pedido.php
│   └── Usuario.php
├── bd/
│   └── sitio.sql
├── img/
├── css/
├── js/
├── uploads/
└── .env
```

## Instrucciones para Clonar y Correr el Proyecto (Localhost XAMPP)

1. **Clona el repositorio desde GitHub:**
```bash
git clone https://github.com/jhans11/helmetspro.git
```

2. **Coloca la carpeta en el directorio de XAMPP:**
```
C:/xampp/htdocs/sitioweb
```

3. **Importa la base de datos:**
- Abre phpMyAdmin.
- Crea una base de datos llamada `sitioweb`.
- Importa el archivo `bd/sitio.sql`.

4. **Configura las credenciales en `.env` o `config/bd.php`:**
```php
$host = 'localhost';
$db = 'sitioweb';
$user = 'root';
$password = '';
```

5. **Accede al proyecto desde tu navegador:**
- Tienda: `http://localhost/sitioweb/`
- Panel Admin: `http://localhost/sitioweb/administrador/`

## Créditos y Licencia
**Desarrollador**: Jhans Jiménez
**Licencia**: MIT License

---

# 📁 /docs – Documentación Técnica

## Arquitectura.md
- Explicación del flujo de datos MVC (Modelo: clases/ | Vista: template/ | Controlador: *.php raíz)
- Separación de lógica y presentación (includes y clases)
- Flujo: Navegación → Productos → Carrito → Pedido

## Seguridad.md
- Hash de contraseñas con `password_hash()`
- Validación de formularios con `filter_input()`
- Protección CSRF con tokens únicos en sesiones
- Uso de PDO + Prepared Statements para evitar SQL Injection
- Control de sesiones seguras (regeneración de ID)

## Funcionalidades.md
- Carrito de compras con PHP Sessions
- CRUD de productos para administrador
- Sistema de usuarios (clientes)
- Gestión de pedidos (estado, historial)
- Integración de PayPal Sandbox para pagos

## Roadmap.md
### Helmets Pro v3.0 (Futuras Mejoras)
- API RESTful para integración móvil
- Sistema de recomendaciones IA
- Dashboard avanzado con analíticas
- Optimización SEO y Lighthouse
- Sistema de notificaciones (email + WhatsApp)
- Migración progresiva a Laravel (Microservicios)

---

# 🚀 Siguiente Paso
1. Crear la rama `dev-v2` en GitHub.
2. Subir este README.md y carpeta /docs.
3. Empezar implementación técnica desde la rama dev-v2.

---

**Versión:** 2.0 IA Copilot Ready
**Autor:** Jhans Jiménez
