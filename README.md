## RPC Hello World
**Description / Descripción**
This is a simple Python project that implements an XML-RPC server and client communication. The server listens for requests on a specific port, and the client sends a message ("Hello, World") to the server, which responds accordingly.

Este es un proyecto simple en Python que implementa un servidor y cliente utilizando XML-RPC. El servidor escucha solicitudes en un puerto específico, y el cliente envía un mensaje ("Hola, Mundo") al servidor, el cual responde en consecuencia.

**Technologies / Tecnologías**
Python: Version 3.11 or higher
XML-RPC: Built-in Python library for remote procedure calls.
Docker: To containerize and run the project.
**Requirements / Requisitos**
Python installed (version 3.11 or higher).
Docker installed and running.
**How to Clone the Project / Cómo Clonar el Proyecto**
Run the following command to clone the repository:
Ejecuta el siguiente comando para clonar el repositorio:

```bash
git clone <repository-url>
cd hola_mundo_rpc
```
Replace <repository-url> with the actual GitHub or GitLab repository URL.
Reemplaza <repository-url> con la URL real del repositorio.

**How to Run / Cómo Ejecutar**
**Run the Server / Ejecutar el Servidor**
To start the XML-RPC server, run:
Para iniciar el servidor XML-RPC, ejecuta:

```bash
python server.py
```
You should see:
Deberías ver:

```bash
Servidor RPC iniciado y escuchando en puerto 8000...
```
**Run the Client / Ejecutar el Cliente**
To run the client and connect to the server, run:
Para ejecutar el cliente y conectarse al servidor, ejecuta:

```bash
python client.py
```
Expected output:
Salida esperada:

```bash
Respuesta del servidor: Hola, Mundo
```
**How to Dockerize / Cómo Dockerizar**
Build the Docker image:
Construye la imagen de Docker:

```bash
docker build -t rpc-hello-world .
```
Run the Server in a Container:
Ejecuta el servidor en un contenedor:

```bash
docker run -d -p 8000:8000 --name rpc-server rpc-hello-world
```
Run the Client in a Container:
Ejecuta el cliente en un contenedor:

```bash
docker run --rm --name rpc-client rpc-hello-world python client.py
```
**Docker Hub Link / Enlace de Docker Hub**
Replace <docker-hub-link> with your actual Docker Hub repository link.
Reemplaza <docker-hub-link> con el enlace real de tu repositorio en Docker Hub.

**Docker Hub Repository / Repositorio de Docker Hub**

