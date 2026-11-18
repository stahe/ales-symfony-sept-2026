# Introducción paso a paso al framework web [Symfony]

**El curso está disponible en línea aquí: [https://stahe.github.io/ales-symfony-sept-2026/](https://stahe.github.io/ales-symfony-sept-2026/)**

## Autor

El curso y todo su código fueron escritos por **Claude**, la IA de Anthropic, **único autor**, a petición de Serge Tahé (septiembre de 2026).

## Descripción general

Este curso ofrece una guía paso a paso para construir una aplicación web MVC con el framework **Symfony 8.1** y el lenguaje **PHP 8.4**. Las páginas HTML las genera el servidor mediante vistas **Twig**, sin un framework JavaScript del lado del cliente. El acceso a datos se realiza mediante el ORM **Doctrine**.

Adapta el curso [Introducción paso a paso al framework web [Laravel]](https://stahe.github.io/ales-laravel-sept-2026/), que a su vez se basa en los cursos de [Flask](https://stahe.github.io/ales-flask-sept-2026/), [Spring MVC](https://stahe.github.io/ales-springmvc-sept-2026/), [ASP.NET Core MVC](https://stahe.github.io/ales-aspnetcoremvc-sept-2026/) y [NestJS](https://stahe.github.io/ales-nestjs-html-sept-2026/). Los ejemplos tienen los mismos números y abarcan los mismos temas: puede comparar los frameworks ejemplo por ejemplo.

## Contenido

| Capítulo | Temas | Ejemplos |
|---|---|---|
| Acciones, enrutamiento, respuestas | rutas (`#[Route]`), controladores, respuestas, redirecciones, contenedor de servicios | 01 a 06 |
| El modelo de la acción | parámetros de la solicitud, resolutores de argumentos, restricciones de validación, solicitudes POST | 07–12 |
| La vista y su modelo | Twig, plantillas, macros, extensiones, componente Form, validación, Post/Redirect/Get, protección CSRF | 13–21 |
| Internacionalización | una aplicación en francés e inglés (diccionarios YAML, mensajes ICU) | 22 |
| Ámbitos de datos | solicitud, sesión, caché, cookies | 23 |
| El ciclo de vida de la solicitud | eventos del núcleo, listeners, resolutores de argumentos, páginas de error | 24 |
| Autenticación y autorización | firewall, autenticador JWT en una cookie, roles, CAPTCHA, limitación de tasa | 25–27 |
| Arquitectura en capas | web / lógica de negocio / DAO con Doctrine y MySQL | 28 |
| Caso de estudio | **RdvMedecins**, una aplicación de programación de citas médicas, explicada archivo por archivo | - |

El caso de estudio `rdvmedecins2-symfony` administra tres roles (administrador, médicos, pacientes): calendarios, reservas, administración de médicos y clientes, creación de cuentas protegida por CAPTCHA y una interfaz en francés/inglés. Utiliza la misma base de datos `dbrdvmedecins2` que las demás versiones de la aplicación.

## Requisitos previos

- PHP 8.4 o superior (extensiones `intl`, `mbstring`, `openssl`, `pdo_mysql`);
- Composer 2;
- MySQL 8 o MariaDB (Laragon en Windows);
- Visual Studio Code con las extensiones PHP Intelephense, Twig Language 2 y YAML;
- curl.

El código fuente se puede descargar desde el sitio web del curso. Las carpetas `vendor` no se incluyen allí: `composer install` las crea, una en la carpeta `exemples` y otra en la carpeta `rdvmedecins2-symfony`.
