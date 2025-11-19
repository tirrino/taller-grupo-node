# Conceptos de Seguridad Explicados

## 1. Rate–Limit
Rate-limit es una técnica que consiste en limitar la cantidad de requests que un cliente puede hacer dentro de un tiempo.
Esto ayuda a prevenir ataques como fuerza bruta (brute force) y abusos del sistema.
En esta API, se implementa la técnica para proteger el endpoint de login y reducir intentos repetidos desde la misma IP.

## 2. CORS
CORS (Cross-Origin Resource Sharing) es una seguridad que controla qué orígenes son capaces de hacer requests a la API.
Esto sirve para evitar que navegadores puedan hacer requests desde dominios que no tienen permitidos.
Aquí se utiliza para prevenir que páginas no autorizadas hagan uso de nuestra API.

## 3. Autenticación con JWT
JWT (JSON Web Token) es una forma de autenticación sin estado.
Es decir, el servidor genera un token firmado que el cliente tiene la obligación de incluir en cada petición que sea protegida.
En esta API, al iniciar sesión, el usuario recibe el JWT.
Más adelante este se envía en los headers tal como:
