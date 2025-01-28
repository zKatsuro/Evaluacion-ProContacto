# Trabajo Práctico - Desarrollo de Aplicaciones Web y Móviles

Este repositorio contiene las resoluciones del trabajo práctico asignado. Se incluye la instalación del ambiente, preguntas teóricas, ejercicios prácticos con herramientas como Postman y Salesforce, y otros conceptos relacionados.

---

## Tabla de Contenidos

1. [Ejercicio 1: Instalación del Ambiente](#ejercicio-1-instalación-del-ambiente)
2. [Ejercicio 2: Preguntas sobre el protocolo HTTP](#ejercicio-2-preguntas-sobre-el-protocolo-http)
3. [Ejercicio 3: Uso de Postman](#ejercicio-3-uso-de-postman)
4. [Ejercicio 4: Trailhead](#ejercicio-4-trailhead)
5. [Ejercicio 5: Objetos de Salesforce](#ejercicio-5-objetos-de-salesforce)
6. [Ejercicio 6: Salesforce y conceptos relacionados](#ejercicio-6-salesforce-y-conceptos-relacionados)
7. [Ejercicio 7: Importación de datos con DataLoader](#ejercicio-7-importación-de-datos-con-dataloader)

---

## Ejercicio 1: Instalación del Ambiente

Para este ejercicio, se realizaron las siguientes instalaciones requeridas para el desarrollo del trabajo práctico:

### Herramientas Instaladas
1. **Visual Studio Code**  
   - IDE utilizado para desarrollar aplicaciones web y móviles.  
   - Soporte para HTML, CSS, C#, Javascript, Node.js, Angular, React, etc.

2. **Git y Git Bash**  
   - Control de versiones para gestionar los cambios en los archivos.  
   - Permite realizar backups automáticos y trabajar desde cualquier lugar con acceso a internet.

### Referencias de instalación
- [Descargar Visual Studio Code](https://code.visualstudio.com/)
- [Descargar Git](https://git-scm.com/)
- Acceso a recursos adicionales:  
  [Platzi](https://platzi.com/)  
  **Usuario**: virtualdreamsfactory  
  **Contraseña**: VDFactory

---

## Ejercicio 2: Preguntas sobre el protocolo HTTP

### Respuestas
1. **¿Qué es un servidor HTTP?**  
   Es un software o hardware que recibe solicitudes (requests) del cliente y devuelve respuestas (responses), generalmente en formato HTML o JSON.

2. **¿Qué son los verbos HTTP?**  
   Son métodos que indican la acción a realizar. Ejemplos: `GET`, `POST`, `PUT`, `DELETE`.

3. **¿Qué es un request y un response en una comunicación HTTP?**  
   - Request: Solicitud enviada por el cliente al servidor.  
   - Response: Respuesta que el servidor envía al cliente. Incluye los headers y el cuerpo.

...

(Continúa enumerando las respuestas con subtítulos para cada pregunta).

---

## Ejercicio 3: Uso de Postman

### Resoluciones
1. **Request GET inicial**  
   URL: [https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json](https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json)  
   Screenshot: ![GET Inicial](screenshots/get-inicial.png)

2. **Request POST**  
   Body enviado:  
   ```json
   {
       "name": "Tu Nombre",
       "email": "tunombre.tuapellido@procontacto.com.mx"
   }
