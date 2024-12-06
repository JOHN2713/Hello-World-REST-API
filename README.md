# Hola Mundo REST API

¡Bienvenido! Este es un proyecto básico que implementa una REST API usando Node.js, Express.js y está dockerizado para facilitar su despliegue.

## Descripción

Esta API expone un único endpoint `GET /` que responde con un mensaje de bienvenida: `¡Hola Mundo desde una REST API!`. Es ideal como punto de partida para aprender sobre REST APIs, contenedores Docker y despliegue en sistemas modernos.

## Características

- Implementado en **Node.js** con **Express.js**
- Respuesta en formato texto
- **Dockerizado** para facilitar el despliegue
- Compatible con cualquier sistema operativo que soporte Docker

## Instalación

### Requisitos previos

Asegúrate de tener instalado:
- Node.js (versión 18 o superior)
- Docker
- Opcional: Docker Compose

### Configuración local

1. Clona este repositorio:
   ```bash
   git clone https://github.com/JOHN2713/Hello-World-REST-API.git
   cd Hello-World-REST-API
   ```

2. Instala las dependencias:
   ```bash
   npm install
   ```

3. Ejecuta el servidor:
   ```bash
   node index.js
   ```

4. Accede a la API en http://localhost:3000

## Docker

### Construcción de la imagen

1. Construye la imagen Docker:
   ```bash
   docker build -t hola-mundo-rest .
   ```

2. Ejecuta el contenedor:
   ```bash
   docker run -p 3000:3000 --name hola-mundo-rest-container hola-mundo-rest
   ```

### Usando Docker Compose

1. Ejecuta con Docker Compose:
   ```bash
   docker-compose up
   ```

2. Detén la aplicación:
   ```bash
   docker-compose down
   ```

## Uso

### Endpoint disponible

- **GET /**: Devuelve un mensaje de bienvenida
  - Respuesta:
    ```
    ¡Hola Mundo desde una REST API!
    ```

## Prueba

Puedes probarlo directamente en tu navegador o con herramientas como **Postman** o `curl`:

```bash
curl http://localhost:3000
```
