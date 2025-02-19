# Media Address

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Estado: En Progreso](https://img.shields.io/badge/estado-En%20progreso-yellow.svg)
![Flutter](https://img.shields.io/badge/Flutter-3.24.3-blue.svg)

Media Address es una aplicación Flutter para el registro de ubicaciones, en la cual se almacena toda la información de manera local. El objetivo es facilitar la captura y gestión de ubicaciones asociadas a los metadatos de fotos, evitando duplicidades y asegurando que cada ubicación tenga detalles únicos y bien estructurados.

---

## Descripción

La aplicación permite:

- **Captura de Ubicaciones:** Al tomar una foto, se registra automáticamente la ubicación (latitud y longitud) donde fue capturada mediante los metadatos.
- **Gestión de Ubicaciones:**  
  - Cada ubicación debe tener un nombre único y puede incluir hasta 3 fotos.
  - Se muestra un detalle para cada ubicación, con sus fotos y una descripción.
  - No se podrá crear una ubicación con el mismo nombre y posición.
  - No se permitirá crear una ubicación dentro de un radio de 500 metros de otra ya registrada.
- **Administración de Amigos:**  
  - Cada usuario puede tener una lista de hasta 5 amigos.
  - Cada amigo incluye información como nombre, apellido, email, número de celular y foto.
  - A un amigo se le podrán asignar ubicaciones, con un máximo de 5 por amigo.

Además, el proyecto sigue una arquitectura limpia (Clean Architecture) que separa correctamente las capas de datos, dominio y presentación, e implementa navegación entre las distintas pantallas (lista de usuarios, detalle de usuarios, creación y detalle de ubicaciones, y ubicaciones favoritas). El manejo del estado se realiza de forma reactiva mediante MobX.

### Extras (Opcionales)

- **Búsqueda:** Funcionalidad de búsqueda por usuario o ubicación.
- **Test Unitarios:** Pruebas unitarias utilizando 'flutter_test' y 'mockito'.

---

## Tecnologías Utilizadas

- **Flutter (Dart):** Framework para el desarrollo de aplicaciones multiplataforma (versión 3.24.3).
- **MobX:** Para el manejo del estado de forma reactiva.
- **Clean Architecture:** Organización del código en capas (datos, dominio y presentación).

---

## Requisitos

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (versión 3.24.3 o superior).

---

## Instalación

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/DanielAndresClavijo/media_address.git
   cd media_address
   ```

2. **Instalar las dependencias:**

   ```bash
   flutter pub get
   ```

3. **Ejecutar la aplicación:**

   ```bash
   flutter run
   ```

---

## Notas

- **Implementación Nativa:**  
  Por el momento no se ha implementado ninguna lógica especial en el lado nativo. Si las carpetas de las plataformas (Android, iOS, Windows, Web y Linux) no se encuentran en el proyecto, deberás generarlas ejecutando:
  
  ```bash
  flutter create .
  ```
  
  Esto asegurará que la aplicación cuente con la configuración nativa necesaria para compilar y ejecutar el cliente en cada plataforma.

- **Estado del Proyecto:**  
  Este proyecto se encuentra en una etapa temprana de desarrollo. Se planifican futuras actualizaciones y mejoras en la funcionalidad.

- **Arquitectura y Estado:**  
  Se utiliza Clean Architecture para garantizar una separación clara entre las capas de datos, dominio y presentación, y MobX para una gestión del estado reactiva.

---

## Contribución

¡Las contribuciones son bienvenidas! Para contribuir:

1. Realiza un fork del repositorio.
2. Crea una rama para tu funcionalidad o corrección:

   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```

3. Realiza tus cambios y haz commit:

   ```bash
   git commit -m "Añadida nueva funcionalidad X"
   ```

4. Envía tu pull request.

Por favor, sigue las buenas prácticas de desarrollo y documenta tus cambios adecuadamente.

---

## Licencia

Este proyecto está licenciado bajo la **Licencia MIT**.

``` 
MIT License

Copyright (c) 2025 Daniel Andrés Clavijo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## Contacto

Si tienes alguna pregunta o sugerencia, no dudes en contactar al autor:

- **Daniel Andrés Clavijo**
- [Perfil de GitHub](https://github.com/DanielAndresClavijo)
