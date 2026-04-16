## BUG-01 - [Checkout permite avanzar con código postal inválido]

**Entorno:**
Chrome - Windows

**Pasos para reproducir:**
1. Ir a la pagina de login
2. Ingresar usuario válido y contraseña válida
4. Click en login
5. Añadir un producto al carrito de compras
6. Ir al carrito de compras
7. Hacer clic en Checkout
8. Ingresar first name
9. Ingresar last name
10. Ingresar un código postal inválido
11. Click en continue

**Resultado esperado:**
- El sistema debe validar el código postal
- No se debe permitir avanzar con datos inválidos
- Se debe mostrar un mensaje de error indicando que el zip/code postal es inválido
- El usuario permanece en la página de Checkout: Your Information

**Resultado actual:**
- No se muestra ningún mensaje de error
- EEl sistema permite avanzar al siguiente paso del checkout

**Severidad:**
Alta
