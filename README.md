# Trabajo Práctico - ProContacto
Este repositorio contiene las resoluciones del trabajo práctico asignado. Se incluye la instalación del ambiente, preguntas teóricas, ejercicios prácticos con herramientas como: Postman, Salesforce y otros conceptos relacionados.

## Tabla de contenidos

1. [Ejercicio 1: Instalación del entorno](#ejercicio-1-instalación-del-entorno)
2. [Ejercicio 2: Preguntas sobre el protocolo HTTP](#ejercicio-2-preguntas-sobre-el-protocolo-http)
3. [Ejercicio 3: Uso de Postman](#ejercicio-3-uso-de-postman)
4. [Ejercicio 4: Trailhead](#ejercicio-4-trailhead)
5. [Ejercicio 5: Objetos de Salesforce](#ejercicio-5-objetos-de-salesforce)
6. [Ejercicio 6: Salesforce y conceptos relacionados](#ejercicio-6-salesforce-y-conceptos-relacionados)
7. [Ejercicio 7: Importación de datos con DataLoader](#ejercicio-7-importación-de-datos-con-dataloader)


## Ejercicio 1: Instalación del entorno

Para este ejercicio, se realizaron las siguientes instalaciones necesarias para el desarrollo del trabajo práctico:

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
  Acceso a recursos adicionales:  
- [Platzi](https://platzi.com/)  
  **Usuario**: virtualdreamsfactory  
  **Contraseña**: VDFactory

---

## Ejercicio 2: Preguntas sobre el protocolo HTTP

### Respuestas
1. **¿Qué es un servidor HTTP?**
   
   Un servidor HTTP es un software o sistema que procesa solicitudes HTTP (protocolo utilizado para transferir información en la web) y envía respuestas al cliente, como un navegador web. Su función principal es servir contenido, como páginas HTML, archivos o datos en formato JSON.

2. **¿Qué son los verbos HTTP?**

   Los verbos HTTP (o métodos) son acciones que se pueden realizar sobre un recurso. Los más conocidos son:
   - **GET:** Solicitar datos del servidor.
   - **POST:** Enviar datos al servidor (crear recursos).
   - **PUT:** Actualizar datos existentes.
   - **DELETE:** Eliminar recursos.
   - **PATCH:** Actualizar parcialmente un recurso

3. **¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?**

   - **Request:** Es la solicitud que un cliente (por ejemplo, un navegador) envía al servidor, incluyendo método HTTP, URL y headers. 
   - **Response:** Es la respuesta del servidor que incluye un código de estado, headers y, opcionalmente, datos en el cuerpo.
   - **Headers:** Son metadatos que acompañan a las solicitudes y respuestas HTTP, proporcionando información como el formato del contenido o la autenticación requerida.

4. **¿Qué es un queryString? (En el contexto de una URL)**

   Un queryString es la parte de la URL que contiene parámetros para enviar datos al servidor. Se encuentra después del signo ? y consiste en pares clave-valor separados por &.

   **Ejemplo:** https://example.com/search?query=libros&categoria=ficcion
   

6. **¿Qué es el responseCode? ¿Qué significado tienen los posibles valores devueltos?**

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
  
8. **Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.**
   - **JSON**: Es un formato ligero basado en texto para estructurar datos. Utiliza llaves {} y pares clave-valor.
     Ejemplo:

   ``` json
   {
       "nombre": "Juan",
       "edad": 30,
       "activo": true
   }
   ```
      
   - **XML**: Es un formato más rígido y estructurado para datos que utiliza etiquetas <></>.
     Ejemplo:

     ```xml
     <persona>
        <nombre>Juan</nombre>
        <edad>30</edad>
        <activo>true</activo>
     </persona>
     ```

9. **Explicar brevemente el estándar SOAP.**
 
   SOAP (Simple Object Access Protocol) es un protocolo basado en XML para intercambiar información estructurada en redes. Es más estricto que REST y define un conjunto de reglas estándar, generalmente usado en sistemas empresariales.
  
10. **Explicar brevemente el estándar REST Full.**
 
    REST (Representational State Transfer) es un estilo arquitectónico para desarrollar servicios web. Utiliza verbos HTTP (GET, POST, PUT, DELETE), URL para identificar recursos, y formatos como JSON o XML para enviar datos.
  
11. **¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?**
 
   - Los **headers** son campos de metadatos en las solicitudes y respuestas HTTP que proporcionan información adicional, como tipo de contenido, autenticación, etc. 
   - **Content-Type** especifica el formato del cuerpo de la solicitud o respuesta (ejemplo: application/json o text/html). Esto permite al cliente/servidor saber cómo interpretar los datos.


## Ejercicio 3: Uso de Postman
   - [Descargar Postman](https://www.postman.com/downloads/).![image](https://github.com/user-attachments/assets/747d6a06-c080-419a-adb4-7e57bb445271)

### Resoluciones
1. **Request GET inicial**  
   **URL:** https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json  
   Screenshot: ![image](https://github.com/user-attachments/assets/ae11d124-c9f3-4d39-9985-e357ed05b222)


2. **Request POST**  
   **URL:** https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

   Body enviado:  
   ```json
   {
       "name": "Federico",
       "email": "Federico.Gomez@procontacto.com.mx"
   }
   ```
   Screenshot:
![image](https://github.com/user-attachments/assets/f8e01277-c480-4de7-b118-a93122360e81)

4. **Request GET final**

   **URL:** https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json

   **Diferencia observada:** El nuevo contacto aparece en los resultados.

   Screenshot:
![image](https://github.com/user-attachments/assets/b324692d-bf91-4977-ac54-9bc6bd054d9b)


## Ejercicio 4: Trailhead
**1. Creación de usuario**
   - URL: https://trailhead.salesforce.com/
   - Screenshot:
![image](https://github.com/user-attachments/assets/01138d58-5221-4a2e-9b23-d343c405d179)

**2. Cambio de idioma a ingles:** 
![image](https://github.com/user-attachments/assets/0193f7b8-6d68-48ee-91a7-c3c33967a23d)


## Ejercicio 5: Objetos de Salesforce
**1. Lead**
   
   **Concepto:** Un Lead representa un posible cliente o prospecto interesado en los productos o servicios de una empresa. Es el primer paso en el ciclo de ventas.
   
   **Datos que almacena:**
   - Nombre
   - Empresa
   - Teléfono
   - Correo electrónico
   - Estado del Lead (Abierto, Contactado, Convertido, etc.)

   **Relaciones:** Un Lead puede convertirse en una Account, Contact y Opportunity mediante el proceso de conversión.

**2. Account**
   
   **Concepto:** Una Account representa una organización o empresa con la que la empresa tiene o puede tener una relación comercial.
   
   **Datos que almacena:**
   - Nombre de la cuenta
   - Dirección
   - Industria
   - Teléfono
   - Sitio web

   **Relaciones:** 
   - Una Account puede tener muchos Contacts.
   - Una Account puede estar relacionada con varias Opportunities.
   - Puede tener Assets y Cases asociados.
  
**3. Contact**
   
   **Concepto:** Un Contact representa a una persona vinculada a una Account con la que la empresa tiene una relación.
   
   **Datos que almacena:**
   - Nombre
   - Apellido
   - Teléfono
   - Correo electrónico
   - Puesto de trabajo

   **Relaciones:**
   - Un Contact está vinculado a una Account.
   - Puede estar relacionado con Cases y Opportunities.

**4. Opportunity**
   
   **Concepto:** Una Opportunity representa un posible negocio o venta en curso.
   
   **Datos que almacena:**
   - Nombre de la oportunidad
   - Fase de ventas
   - Fecha de cierre
   - Monto esperado
   - Account asociada

   **Relaciones:** 
   - Una Opportunity está asociada a una Account.
   - Puede tener Products relacionados.
   - Puede generar Quotes.

**5. Product**
   
   **Concepto:** Un Product representa un bien o servicio que la empresa ofrece a sus clientes.
   
   **Datos que almacena:**
   - Nombre del producto
   - Código de producto
   - Precio
   - Descripción

   **Relaciones:** 
   - Los Products se incluyen en PriceBooks.
   - Se relacionan con Opportunities mediante OpportunityLineItems.

**6. PriceBook**
   
   **Concepto:** Un PriceBook es un conjunto de precios para un grupo de Products.
   
   **Datos que almacena:**
   - Nombre del PriceBook
   - Activo (Sí/No)
   - Description

   **Relaciones:**
   - Contiene Products con precios específicos.
   - Asociado a Opportunities a través de los OpportunityLineItems.

**7. Quote**
   
   **Concepto:** Un Quote representa una propuesta de precios que se envía a un cliente potencial.
   
   **Datos que almacena:**
   - Nombre
   - Precio total
   - Fecha de vencimiento

   **Relaciones:** Asociado a una Opportunity.

**8. Asset**
   
   **Concepto:** Un Asset representa un producto adquirido por un cliente.
   
   **Datos que almacena:**
   - Nombre del asset
   - Account asociada
   - Estado (Activo, Inactivo)

   **Relaciones:** Relacionado con Accounts y Cases.

**9. Case**
   
   **Concepto:** Un Case representa un problema o solicitud del cliente.
   
   **Datos que almacena:**
   - Asunto
   - Descripción
   - Estado (Abierto, Cerrado)
   - Prioridad

   **Relaciones:** Asociado a Accounts y Contacts.

**10. Article**
   
   **Concepto:** Un Article es una pieza de conocimiento utilizada para responder preguntas o resolver problemas.
   
   **Datos que almacena:**
   - Título
   - Contenido
   - Categoría

   **Relaciones:** No tiene relaciones directas con los demás objetos enumerados.

**Diagrama de Drawio:**

![Relaciones entre objetos Salesforce](https://github.com/user-attachments/assets/7ad71001-8e37-4a46-9c9b-368a385d9303)



## Ejercicio 6: Salesforce y conceptos relacionados

### Soluciones Salesforce
**A. ¿Qué es Salesforce?**

   Es un CRM que funciona en la nube. Es una herramienta que te ayuda a gestionar clientes, ventas, soporte y más, todo desde un solo lugar. Es muy popular porque se adapta a muchas industrias, tiene diversas funciones y permite una amplia personalización.

**B. ¿Qué es Sales Cloud?**

   Es la parte de Salesforce que está enfocada en ventas. Permite llevar un control de los clientes potenciales, oportunidades, cuentas y todo lo relacionado con cerrar negocios.

**C. ¿Qué es Service Cloud?**

   Es una solución diseñada para el servicio al cliente. Con ella se pueden gestionar casos, hacer seguimiento de problemas, ofrecer soporte en varios canales y asegurar la satisfacción de los clientes.

**D. ¿Qué es Health Cloud?**

   Es una versión de Salesforce pensada para el sector de la salud. Ayuda a los profesionales a gestionar pacientes, coordinar atención médica y mantener todo organizado.

**E. ¿Qué es Marketing Cloud?**

   Es una solución de automatización de marketing que ayuda a crear campañas personalizadas, enviar correos electrónicos masivos, gestionar redes sociales y analizar el impacto de las acciones de marketing.

### Funcionalidades de Salesforce
**A. ¿Qué es un RecordType?**

   Es una funcionalidad que permite diferenciar tipos de registros dentro de un mismo objeto para manejar distintas vistas, layouts y procesos de negocio.

**B. ¿Qué es un ReportType?**

   Es la plantilla que define qué objetos y relaciones están disponibles para crear un informe en Salesforce.

**C. ¿Qué es un Page Layout?**

   Es la configuración que define qué campos, botones y secciones son visibles para los usuarios en la interfaz de un registro.

**D. ¿Qué es un Compact Layout?**

   Es una versión resumida del Page Layout que define los campos visibles en vistas compactas como la aplicación móvil o resúmenes rápidos.

**E. ¿Qué es un Perfil?**

   Define los permisos y accesos de un usuario, como objetos, campos, aplicaciones y pestañas.

**F. ¿Qué es un Rol?**

   Es una jerarquía que define la visibilidad de datos en función de la estructura organizacional.

**G. ¿Qué es un Validation Rule?**

   Es una regla que verifica si los datos ingresados cumplen ciertos criterios antes de guardar un registro.

**H. ¿Qué diferencia hay entre una relación Master Detail y Lookup?**

   - Master Detail: Relación estrecha donde el registro hijo depende completamente del padre. Si el padre se elimina, el hijo también.
   - Lookup: Relación más flexible y opcional. Los registros hijo pueden existir sin un padre.

**I. ¿Qué es un Sandbox?**

   Es un entorno aislado que permite realizar pruebas y desarrollo sin afectar los datos en producción.

**J. ¿Qué es un ChangeSet?**

   Es una herramienta para migrar cambios configurados en Salesforce (como objetos, campos o reglas) de un entorno a otro.

**K. ¿Para qué sirve el import Wizard de Salesforce?**

   Permite importar datos (como cuentas, contactos o leads) de forma sencilla a través de un asistente.

**L. ¿Para qué sirve la funcionalidad Web to Lead?**

   Crea leads automáticamente en Salesforce a partir de formularios en línea.

**M. ¿Para qué sirve la funcionalidad Web to Case?**

   Genera casos de soporte automáticamente desde formularios web enviados por los clientes.

**N. ¿Para qué sirve la funcionalidad Omnichannel?**

   Permite distribuir automáticamente trabajos o casos entre los agentes disponibles en múltiples canales (chat, email, teléfono, etc.).

**O. ¿Para qué sirve la funcionalidad Chatter?**

   Es una herramienta de colaboración interna que permite a los usuarios interactuar, compartir archivos y trabajar en equipo.

### Conceptos Generales
**A. ¿Qué significa SaaS?**

   "Software as a Service": Modelo donde el software se proporciona a través de internet como un servicio, sin necesidad de instalación local.

**B. ¿Salesforce es SaaS?**

   Sí, Salesforce opera bajo el modelo SaaS, proporcionando sus servicios en la nube.

**C. ¿Qué significa que una solución sea Cloud?**

   Significa que opera en servidores remotos accesibles a través de internet, en lugar de estar instalado localmente.

**D. ¿Qué significa que una solución sea On-Premise?**

   Implica que el software se instala y opera en servidores locales dentro de la organización.

**E. ¿Qué es un pipeline de ventas?**

   Es el conjunto de etapas que atraviesa un cliente potencial desde el primer contacto hasta el cierre de la venta.

**F. ¿Qué es un funnel de ventas?**

   Es una representación visual que muestra cómo los prospectos pasan por diferentes fases del proceso de ventas.

**G. ¿Qué significa Customer Experience?**

   Es la percepción general del cliente sobre su interacción con una empresa, abarcando todos los puntos de contacto.

**H. ¿Qué significa omnicanalidad?**

   Es la capacidad de integrar y coordinar múltiples canales de comunicación para ofrecer una experiencia uniforme al cliente.

**I. ¿Qué significa que un negocio sea B2B? ¿Qué significa que un negocio sea B2C?**
   - B2B (Business to Business): Una empresa vende a otras empresas.
   - B2C (Business to Consumer): Una empresa vende directamente a consumidores finales.

**J. ¿Qué es un KPI?**

   "Key Performance Indicator": Indicador clave de rendimiento que mide el éxito de una acción o estrategia.

**K. ¿Qué es una API y en qué se diferencia de una Rest API?**
   - API: Interfaz de Programación de Aplicaciones, permite que diferentes sistemas se comuniquen entre sí.
   - REST API: Tipo de API que sigue el estilo arquitectónico REST, utilizando HTTP y recursos representados como URLs.

**L. ¿Qué es un Proceso Batch?**

   Es un proceso que ejecuta operaciones en grandes volúmenes de datos en segundo plano, generalmente de forma programada.

**M. ¿Qué es Kanban?**

   Es un sistema visual de gestión de tareas que organiza el trabajo en columnas (como "Pendiente", "En Proceso", "Completado").

**N. ¿Qué es un ERP?**

   "Enterprise Resource Planning": Software que gestiona procesos centrales de una empresa como finanzas, inventario y recursos humanos.

**O. ¿Salesforce es un ERP?**

   No, Salesforce es un CRM, pero se puede integrar con ERPs para gestionar procesos complementarios.


## Ejercicio 7: Importación de datos con DataLoader
   ### Importación
   **1. Instalación de DataLoader:** [URL](https://developer.salesforce.com/docs/atlas.en-us.dataLoader.meta/dataLoader/loader_install_mac.htm)
   
   **2. Adaptación del archivo a subir:** Se deben revisar los formatos de la data a cargarse, ejemplos: formato de date que coincidad con sf, cantidad de caracteres, si las picklist son restricted, columnas sin header, etc.

   Referencia: https://developer.salesforce.com/docs/atlas.en-us.dataLoader.meta/dataLoader/supported_data_types.htm

   **3. Abrir DataLoader**
   
![image](https://github.com/user-attachments/assets/d7c935f5-1c72-48ae-9347-19cc7750a9f7)

   **4. Autenticar org:**
   
![image](https://github.com/user-attachments/assets/482a48d0-ab6b-4e07-9c98-9992f3bf0823)

   **5. Seleccionamos el objeto en el cual cargaramos los registros asi como el archivo a importar:**
   
![image](https://github.com/user-attachments/assets/ee6d0634-f388-4cc5-b923-f529681202d0)

   **6. Omitimos en este caso para relacionar los lookup**
   
![image](https://github.com/user-attachments/assets/95ded01b-d5b1-4717-926d-affd118a2b5a)

   **7. Creamos un mapeo de fields**
   
![image](https://github.com/user-attachments/assets/c09aab17-6c8b-42c1-ba5a-53959bf6f18d)
![image](https://github.com/user-attachments/assets/89253844-a3c7-4809-85fc-47d01e403c50)
![image](https://github.com/user-attachments/assets/a8331f6e-a429-48c1-9da6-d8fa1cd5d43c)

   **8. Elegimos donde guardar los archivos con los resultados de la importación**
   
![image](https://github.com/user-attachments/assets/d0e33a92-6f40-4af6-8684-8989a3df2a0c)
![image](https://github.com/user-attachments/assets/3b6e75a1-d2db-460c-8ab1-ff3dcbc2285c)

   ### List View 
   **1.** Creamos el list view con los filters necesarios, en este caso utilizamos "Created Date" equals TODAY y añadimos los fields a mostrar (omitimos webside y owner ya que estaban vacios en el archivo a cargar y el limite de fields a mostrar en list view es de 15):

![image](https://github.com/user-attachments/assets/2b7edbc0-0416-4bd3-8af6-a7b75720e3da)
