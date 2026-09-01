# Proyecto 8 - Pruebas de API de Urban Grocers

Este proyecto contiene la automatización de pruebas de API para la aplicación Urban Grocers, enfocándose en la validación del endpoint para la creación de kits de productos.

## Tecnologías utilizadas
- Python 3
- Pytest
- Librería `requests`

## Estructura del proyecto
- `configuration.py`: Almacena la URL base del servidor y las rutas (endpoints) de la API.
- `data.py`: Contiene los cuerpos de las peticiones (JSON) y los encabezados (headers) necesarios.
- `sender_stand_request.py`: Contiene las funciones que realizan las peticiones HTTP (POST) para crear usuarios y kits.
- `create_kit_name_kit_test.py`: Contiene los casos de prueba automatizados (positivos y negativos) para validar las restricciones del campo `name` al crear un kit.

## Cómo ejecutar las pruebas
1. Asegúrate de tener instalados los paquetes necesarios (`pytest` y `requests`).
2. Inicia un servidor de Urban Grocers y actualiza la variable `URL_SERVICE` en el archivo `configuration.py` con la URL generada.
3. Abre una terminal en la raíz del proyecto y ejecuta el siguiente comando:
   ```bash
   pytest create_kit_name_kit_test.py
