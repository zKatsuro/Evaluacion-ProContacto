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
   Un servidor HTTP es un software o sistema que procesa solicitudes HTTP (protocolo utilizado para transferir información en la web) y envía respuestas al cliente, como un navegador web. Su función principal es servir contenido, como páginas HTML, archivos o datos en formato JSON.

2. **¿Qué son los verbos HTTP?**  
   Los verbos HTTP (o métodos) son acciones que se pueden realizar sobre un recurso. Los más conocidos son:
   - GET: Solicitar datos del servidor.
   - POST: Enviar datos al servidor (crear recursos).
   - PUT: Actualizar datos existentes.
   - DELETE: Eliminar recursos.
   - PATCH: Actualizar parcialmente un recurso

3. **¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?**  
   - Request: Es la solicitud que un cliente (por ejemplo, un navegador) envía al servidor, incluyendo método HTTP, URL y headers. 
   - Response: Es la respuesta del servidor que incluye un código de estado, headers y, opcionalmente, datos en el cuerpo.
   - Headers: Son metadatos que acompañan a las solicitudes y respuestas HTTP, proporcionando información como el formato del contenido o la autenticación requerida.

4. **¿Qué es un queryString? (En el contexto de una URL)**  
   Un queryString es la parte de la URL que contiene parámetros para enviar datos al servidor. Se encuentra después del signo ? y consiste en pares clave-valor separados por &.
   Ejemplo: https://example.com/search?query=libros&categoria=ficcion
   

5. **¿Qué es el responseCode? ¿Qué significado tienen los posibles valores devueltos?**  
  Es el código de estado que devuelve un servidor indicando el resultado de la solicitud. Ejemplos:
   - **200**: Éxito.
   - **404**: Recurso no encontrado.
   - **500**: Error interno del servidor.
   - **301**: Redirección permanente.
   - **401**: No autorizado.
  
6. **¿Cómo se envía la data en un GET y cómo en un POST?**  
   - **GET**: Los datos se envían como parte de la URL, generalmente en el queryString. 
   - **POST**: Los datos se envían en el cuerpo de la solicitud, lo que permite mayor seguridad y soporte para grandes volúmenes de datos.
  
7. **¿Qué verbo HTTP utiliza el navegador cuando accedemos a una página?**  
   El navegador utiliza el verbo **GET**.
  
8. **Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.**  REVISAR
   - **JSON**: Es un formato ligero basado en texto para estructurar datos. Utiliza llaves {} y pares clave-valor.
     Ejemplo:
     {
  "nombre": "Juan",
  "edad": 30,
  "activo": true
}
      
   - **XML**: Es un formato más rígido y estructurado para datos que utiliza etiquetas <></>.
     Ejemplo:
     <persona>
  <nombre>Juan</nombre>
  <edad>30</edad>
  <activo>true</activo>
</persona>

9. **Explicar brevemente el estándar SOAP.**  
   SOAP (Simple Object Access Protocol) es un protocolo basado en XML para intercambiar información estructurada en redes. Es más estricto que REST y define un conjunto de reglas estándar, generalmente usado en sistemas empresariales.
  
10. **Explicar brevemente el estándar REST Full.**  
   REST (Representational State Transfer) es un estilo arquitectónico para desarrollar servicios web. Utiliza verbos HTTP (GET, POST, PUT, DELETE), URL para identificar recursos, y formatos como JSON o XML para enviar datos.
  
11. **¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?**  
   - Los headers son campos de metadatos en las solicitudes y respuestas HTTP que proporcionan información adicional, como tipo de contenido, autenticación, etc. 
   - **Content-Type** especifica el formato del cuerpo de la solicitud o respuesta (ejemplo: application/json o text/html). Esto permite al cliente/servidor saber cómo interpretar los datos.
---

## Ejercicio 3: Uso de Postman
   - [Descargar Postman](https://www.postman.com/downloads/).![image](https://github.com/user-attachments/assets/747d6a06-c080-419a-adb4-7e57bb445271)

### Resoluciones
1. **Request GET inicial**  
   URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json  
   Screenshot: ![image](https://github.com/user-attachments/assets/ae11d124-c9f3-4d39-9985-e357ed05b222)


2. **Request POST**  
   URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json
   Body enviado:  
   ```json
   {
       "name": "Federico",
       "email": "Federico.Gomez@procontacto.com.mx"
   }
   ```
   Screenshot: ![image](https://github.com/user-attachments/assets/f8e01277-c480-4de7-b118-a93122360e81)

4. **Request GET final** 
   URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json
   Diferencia observada: El nuevo contacto aparece en los resultados.
   Screenshot:![image](https://github.com/user-attachments/assets/b324692d-bf91-4977-ac54-9bc6bd054d9b)

