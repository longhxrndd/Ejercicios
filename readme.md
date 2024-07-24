# 🏁 Ejercicios Completados

## Ejercicio 1

### ✔ Instalación de Visual Studio Code y Git completadas.

---

## Ejercicio 2

1. **Un servidor HTTP** 🌐: Es un software que procesa solicitudes de clientes (navegadores web) y devuelve los recursos solicitados, como páginas web, imágenes o videos.

2. **Los verbos HTTP**: Son comandos para indicarle al servidor que ejecute acciones con los recursos solicitados, ya sea mostrarlos, agregarlos, cambiarlos o eliminarlos. Los más conocidos son:

   - `GET`
   - `POST`
   - `PUT`
   - `PATCH`
   - `DELETE`

3. **Componentes del Protocolo HTTP**:

   - **Request** 📩: Es una solicitud que un cliente envía a un servidor para un recurso. Esto incluye una URL, headers y, a veces, un body.
   - **Response** 📤: Es el mensaje enviado al cliente por el servidor respondiendo a una solicitud. Incluye un `responseCode`, headers y un body con el recurso solicitado.
   - **Headers** 📝: Son partes del request y response que contienen información adicional, pueden incluir, por ejemplo, información del tipo de contenido, tamaño del contenido o cookies.

4. **QueryString**: Es la parte de una URL que contiene datos que se envían a una aplicación web. Es usado para referirse a las interacciones con bases de datos.

5. **ResponseCode**: Es un número que el servidor devuelve al cliente indicando el resultado de su solicitud. Los números o códigos más comunes son:

   - `200 OK`: Solicitud procesada con éxito.
   - `404 Not Found`: No se encontró el recurso solicitado.
   - `500 Internal Server Error`: Indica un error del servidor.
   - `301 Moved Permanently`: El recurso solicitado fue movido a una nueva URL.
   - `403 Forbidden`: Acceso denegado.

6. **Métodos de Envío de Datos**:

   - **GET**: Los datos se envían como parte de la URL a través del queryString.
   - **POST**: Los datos se envían en el body de la solicitud, permite enviar grandes cantidades de datos más complejos.

7. **Verbo Utilizado por el Navegador** 🌐: El navegador utiliza el verbo `GET` para solicitar la página web.

8. **Formatos de Intercambio de Datos**:

   - **JSON** 📄: Es un formato de intercambio de datos ligero, es derivado de la sintaxis de JavaScript. Por ejemplo:
     ```json
     {
       "nombre": "Diana",
       "edad": 20,
       "pais": "Colombia"
     }
     ```
   - **XML** 📄: Es un formato de marcado basado en texto para organizar la información de manera estructurada. Por ejemplo:
     ```xml
     <persona>
       <nombre>Diana</nombre>
       <edad>20</edad>
       <pais>Colombia</pais>
     </persona>
     ```

9. **SOAP** 🧼: Es un protocolo para intercambiar información basado en XML, utiliza verbos HTTP.

10. **REST**: Es un estilo de arquitectura de software para diseñar servicios web. Utiliza verbos HTTP y se basa en recursos identificados por URLs.

11. **Headers en una Solicitud** 📋: Son campos adicionales enviados con solicitudes HTTP que ofrecen información sobre la solicitud o el cliente. El header `Content-type` indica el tipo de contenido enviado al servidor.

## Ejercicio 3

📁 **Se puede observar la modificación del archivo JSON con mis datos, después de realizar el POST request.**

![Postman request](/imagenes/Postman.png)

## Ejercicio 4

🔗 [**Perfil de trailhead**](https://www.salesforce.com/trailblazer/ifj9uz34hz9kfduc4v)


---

## Ejercicio 5

1. **Lead**: Es un potencial cliente que ha mostrado interés en los productos o servicios de la empresa.

   - **Datos que almacena**:
     - Nombre y apellido
     - Empresa
     - Correo electrónico
     - Teléfono
   - **Relaciones**: Un lead puede convertirse en una cuenta, contacto y en una potencial oportunidad.

2. **Account** 🏢: Una cuenta es una empresa, organización o individuo con la que tu empresa tiene una relación comercial.

   - **Datos que almacena**:
     - Nombre de la cuenta
     - Dirección
     - Teléfono
     - Industria
     - Número de empleados
     - Sitio web
   - **Relaciones**: Una cuenta puede tener contactos asociados, oportunidades relacionadas y estar relacionada con casos, activos y contratos.

3. **Contact** 📇: Un contacto se refiere a una persona asociada a una cuenta con la que la empresa interactúa.

   - **Datos que almacena**:
     - Nombre y apellido
     - Correo electrónico
     - Teléfono
     - Título
     - Departamento
   - **Relaciones**: Un contacto está relacionado con una cuenta, puede estar relacionado con oportunidades, casos y campañas.

4. **Opportunity** 💼: Una oportunidad significa una venta potencial o una transacción que la empresa está gestionando.

   - **Datos que almacena**:
     - Nombre de la oportunidad
     - Etapa de la venta
     - Monto estimado
     - Fecha de cierre
     - Probabilidad de cierre
   - **Relaciones**: Una cuenta y uno o más contactos, puede tener productos y cotizaciones asociados.

5. **Product** 📦: Un producto son los bienes o servicios que la empresa ofrece.

   - **Datos que almacena**:
     - Nombre del producto
     - Código del producto
     - Descripción
     - Precio estándar
     - Familia de productos
   - **Relaciones**: Se asocia con oportunidades y cotizaciones, puede estar incluido en uno o más libros de precios.

6. **PriceBook** 📚: Un libro de precios es una lista de productos y sus precios asociados.

   - **Datos que almacena**:
     - Nombre del libro de precios
     - Activo (sí/no)
     - Productos y sus precios específicos
   - **Relaciones**: Productos y oportunidades. Un libro de precios puede tener múltiples productos y cada producto puede estar en múltiples libros de precios.

7. **Quote** 💬: Una cotización es una oferta de productos o servicios a un potencial cliente con precios y condiciones.

   - **Datos que almacena**:
     - Nombre de la cotización
     - Fecha de la cotización
     - Estado de la cotización
     - Productos y precios
   - **Relaciones**: Puede estar relacionado a una oportunidad, incluir varios productos y ser convertido en un pedido.

8. **Asset** 🏷: Un activo se refiere a un producto que un cliente ha comprado y posee.

   - **Datos que almacena**:
     - Nombre del activo
     - Número de serie
     - Fecha de compra
     - Estado del activo
   - **Relaciones**: Una cuenta o un contacto. Puede estar asociado con casos para soporte técnico.

9. **Case** 📁: Un caso significa un problema, pregunta o solicitud de servicio de un cliente.

   - **Datos que almacena**:
     - Número de caso
     - Estado del caso (nuevo, en proceso, cerrado)
     - Prioridad
     - Descripción del problema
   - **Relaciones**: Relacionado con una cuenta y contacto, podría estar asociado con activos, contratos o estar vinculado a artículos.

10. **Article** 📜: Un artículo representa un documento o contenido en la base de conocimientos que proporciona información sobre productos, servicios, procesos o soluciones a problemas comunes.

    - **Datos que almacena**:
      - Título del artículo
      - Contenido
      - Categoría
      - Palabras clave
      - Fecha de publicación
    - **Relaciones**: Asociado con casos como parte de la resolución de problemas.

### Ejemplo de Diagrama

![Ejemplo de Diagrama](/imagenes/Diagrama.png)

## Ejercicio 6

### Soluciones de Salesforce

A. **¿Qué es Salesforce?**: Es una plataforma de gestión de relaciones con clientes (CRM) que permite a las empresas gestionar sus ventas, marketing, servicio al cliente y otras operaciones comerciales.

B. **¿Qué es Sales Cloud?** ☁️: Es una app de Salesforce diseñada para mejorar ventas. Ayuda a gestionar cuentas, contactos, oportunidades de ventas y automatizar procesos de ventas.

C. **¿Qué es Service Cloud?** ☁️: Es una solución de Salesforce enfocada en el servicio al cliente. Ofrece herramientas para gestionar casos y ayuda a otorgar un servicio al cliente eficiente y personalizado.

D. **¿Qué es Health Cloud?** 🏥: Una solución de Salesforce diseñada para el sector de salud. Permite a las organizaciones de salud gestionar las relaciones con los pacientes, coordinar la atención y ofrecer un cuidado más específico.

E. **¿Qué es Marketing Cloud?** 📈: Es una plataforma de Salesforce para la automatización de marketing. Permite gestionar campañas de marketing, interactuar con los clientes y analizar datos de marketing.

### Funcionalidades de Salesforce

A. **¿Qué es un RecordType?**: Un RecordType permite a los usuarios ofrecer diferentes procesos de negocio y diseños de página para diferentes usuarios en función de su perfil o requisitos.

B. **¿Qué es un ReportType?**: Define la estructura y los objetos que pueden ser utilizados en un informe. Establece las relaciones entre los objetos y determina qué campos están disponibles para la creación de informes.

C. **¿Qué es un Page Layout?**: Un Page Layout en Salesforce controla los campos, secciones, botones y enlaces en la página de un objeto. Permite personalizar la visualización de la información para diferentes perfiles de usuario.

D. **¿Qué es un Compact Layout?**: Un Compact Layout define los campos que se muestran en el encabezado del registro y en las vistas de detalles de registros en la interfaz móvil y en la aplicación de Salesforce.

E. **¿Qué es un Perfil?**: Es una colección de permisos y configuraciones que determina qué usuarios pueden hacer dentro de la plataforma. Controla el acceso a objetos, campos y otras funciones.

F. **¿Qué es un Rol?**: Un Rol define el nivel de acceso a datos de un usuario en función de su cargo o posición. Ayuda a compartir registros con otros usuarios.

G. **¿Qué es un Validation Rule?** ✔: Es una regla que verifica que los datos ingresados en un registro cumplen con ciertos criterios antes de que se puedan guardar. Ayuda a mantener la integridad de los datos.

H. **¿Qué diferencia hay entre una relación Master Detail y Lookup?**:

- **Master-Detail**: Es una relación donde el registro secundario (detail) depende del registro primario (master).
- **Lookup**: Es una relación más flexible que no tiene una fuerte dependencia entre los registros.

I. **¿Qué es un Sandbox?**: Es un entorno de prueba aislado que permite realizar pruebas y desarrollos sin afectar los datos ni la configuración en el entorno de producción.

J. **¿Qué es un ChangeSet?** 🛠: Es una colección de componentes personalizados que se pueden mover de un entorno de Salesforce a otro.

K. **¿Para qué sirve el import Wizard de Salesforce?**: Permite a los usuarios importar datos en masa desde archivos CSV a objetos estándar y personalizados de Salesforce.

L. **¿Para qué sirve la funcionalidad Web to Lead?** 🌐: Permite crear leads automáticamente en Salesforce a partir de formularios web que los visitantes del sitio completan.

M. **¿Para qué sirve la funcionalidad Web to Case?**: Permite crear casos automáticamente en Salesforce a partir de formularios web completados por los clientes en el sitio web de una empresa.

N. **¿Para qué sirve la funcionalidad Omnichannel?** 🌍: Distribuye automáticamente trabajos y casos a los agentes adecuados en función de su disponibilidad y habilidades, mejorando la eficiencia y el servicio al cliente.

O. **¿Para qué sirve la funcionalidad Chatter?** 💬: Chatter es una red social corporativa integrada en Salesforce que permite a los empleados colaborar, compartir información y trabajar juntos a tiempo real.

### Conceptos Generales

A. **¿Qué significa SaaS?**: (Software as a Service) es un modelo de distribución de software donde el software y los datos se alojan en servidores de un tercero y se accede a ellos a través de Internet.

B. **¿Salesforce es Saas?** ✅: Sí, debido a que los usuarios acceden a la plataforma a través de Internet, sin necesidad de instalar el software.

C. **¿Qué significa que una solución sea Cloud?** ☁️: Significa que se entrega y accede a través de Internet, y los datos y aplicaciones se almacenan en servidores remotos gestionados por proveedores de servicios en la nube.

D. **¿Qué significa que una solución sea On-Premise?** 🏢: Significa que se instala y ejecuta en los servidores locales de la empresa, y la empresa es responsable del mantenimiento y la gestión de la infraestructura.

E. **¿Qué es un pipeline de ventas?**: Es una visualización de las etapas que atraviesan las oportunidades de ventas desde el primer contacto con un potencial cliente hasta el cierre de la venta.

F. **¿Qué es un funnel de ventas?**: Es una representación gráfica que muestra la reducción progresiva de oportunidades de ventas a medida que avanzan a través de diferentes etapas del proceso de ventas, desde leads hasta clientes cerrados.

G. **¿Qué significa Customer Experience?** 😊: Significa la percepción total que tiene un cliente sobre su interacción con una empresa a lo largo de todas las etapas del ciclo de vida del cliente.

H. **¿Qué significa omnicanalidad?**: Significa una estrategia de marketing y ventas en la que una empresa ofrece una experiencia de cliente integrada a través de canales de comunicación y puntos de contacto.

I. **¿Qué significa que un negocio sea B2B? ¿Qué significa que un negocio sea B2C?**:

- **B2B (Business to Business)**: Un negocio que vende productos o servicios a otras empresas.
- **B2C (Business to Consumer)**: Un negocio que vende productos o servicios directamente a los consumidores finales.

J. **¿Qué es un KPI?** 📈: Un KPI (en inglés “Key Performance Indicator”) es una métrica utilizada para medir el rendimiento de una organización o de una actividad específica en función de objetivos establecidos.

K. **¿Qué es una API y en qué se diferencia de una Rest API?**:

- **API (Application Programming Interface)**: Un conjunto de reglas y protocolos que permiten a las aplicaciones comunicarse entre sí.
- **REST API**: Un tipo de API que sigue los principios de la arquitectura REST (Representational State Transfer) y utiliza métodos HTTP para realizar operaciones.

L. **¿Qué es un Proceso Batch?**: Es una ejecución de un programa o script que procesa varios datos en lote sin intervención del usuario, en lugar de procesar los datos uno por uno en tiempo real.

M. **¿Qué es Kanban?**: Es un método de gestión visual para tareas y proyectos que utiliza tarjetas en un tablero para representar el trabajo en diferentes etapas del proceso de producción.

N. **¿Qué es un ERP?** 🏢: Un ERP (Enterprise Resource Planning) es un sistema integrado de gestión empresarial que automatiza procesos de negocio, como la contabilidad, gestión de inventarios, compras y ventas.

O. **¿Salesforce es un ERP?** ❌: No es un ERP, es un CRM (Customer Relationship Management). Aun así, puede integrarse con sistemas ERP para asegurar una visión más completa de las operaciones empresariales.

## Ejercicio 7

📁 **El código y la clase se encuentran en el repositorio.**
