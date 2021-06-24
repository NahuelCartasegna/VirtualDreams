# VirtualDreams
Ejercicio 2
1.	¿Qué es un servidor HTTP?

Es un programa informático que procesa una aplicación del lado del servidor, realizando conexiones bidireccionales o unidireccionales y síncronas o asíncronas con el cliente y generando o cediendo una respuesta en cualquier lenguaje o aplicación del lado del cliente. El código recibido por el cliente es renderizado por un navegador web. Para la transmisión de todos estos datos suele utilizarse algún protocolo. Generalmente se usa el protocolo HTTP para estas comunicaciones, perteneciente a la capa de aplicación del modelo OSI. El término también se emplea para referirse al ordenador.

2.	¿Qué son los verbos HTTP? Mencionar los más conocidos?

HTTP define un conjunto de métodos de petición para indicar la acción que se desea realizar para un recurso determinado. Aunque estos también pueden ser sustantivos, estos métodos de solicitud a veces son llamados HTTP verbs. Cada uno de ellos implementan una semántica diferente, pero algunas características similares son compartidas por un grupo de ellos
Get, head, post, put, delete, connect, options, trace, patch

3.	¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers? 

El comando HTTP Request permite enviar todo tipo de petición HTTP a un URL específico y procesar la respuesta del servidor HTTP.
La respuesta o HTTP response es el mensaje que envía el servidor al cliente tras haber recibido una petición o HTTP request
Los HTTP headers son la parte central de los HTTP requests y responses, y transmiten información acerca del navegador del cliente, de la página solicitada, del servidor, etc.

4.	¿Qué es un queryString? (En el contexto de una url)

Las Query String o cadenas de consultas es un término que se utiliza para hacer referencia a una interacción con una base de datos. Además, es la parte de una URL que contiene los datos que deben pasar a las aplicaciones web.

5.	¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?

Los códigos de estado de respuesta HTTP indican si se ha completado satisfactoriamente una solicitud HTTP específica. Las respuestas se agrupan en cinco clases:
Respuestas informativas (100–199),
Respuestas satisfactorias (200–299),
Redirecciones (300–399),
Errores de los clientes (400–499),
y errores de los servidores (500–599).

100 Continue
Esta respuesta provisional indica que todo hasta ahora está bien y que el cliente debe continuar con la solicitud o ignorarla si ya está terminada.

101 Switching Protocol
Este código se envía en respuesta a un encabezado de solicitud Upgrade (en-US) por el cliente e indica que el servidor acepta el cambio de protocolo propuesto por el agente de usuario.

200 OK
La solicitud ha tenido éxito. El significado de un éxito varía dependiendo del método HTTP:

201 Created
La solicitud ha tenido éxito y se ha creado un nuevo recurso como resultado de ello. Ésta es típicamente la respuesta enviada después de una petición PUT.

300 Multiple Choice (en-US)
Esta solicitud tiene más de una posible respuesta. User-Agent o el usuario debe escoger uno de ellos. No hay forma estandarizada de seleccionar una de las respuestas.

301 Moved Permanently
Este código de respuesta significa que la URI  del recurso solicitado ha sido cambiado. Probablemente una nueva URI sea devuelta en la respuesta.

404 Not Found
El servidor no pudo encontrar el contenido solicitado. Este código de respuesta es uno de los más famosos dada su alta ocurrencia en la web.

405 Method Not Allowed (en-US)
El método solicitado es conocido por el servidor pero ha sido deshabilitado y no puede ser utilizado. Los dos métodos obligatorios, GET y HEAD, nunca deben ser deshabilitados y no deberían retornar este código de error.

6.	¿Cómo se envía data en un Get y cómo en un POST?

GET lleva los datos de forma "visible" al cliente (navegador web). El medio de envío es la URL. Los datos los puede ver cualquiera.

POST consiste en datos "ocultos" (porque el cliente no los ve) enviados por un formulario cuyo método de envío es post. Es adecuado para formularios. Los datos no son visibles.

7.	¿Qué verbo http utiliza el navegador cuando accedemos a una página?

El verbo que utiliza el navegador cuando accedemos a una pagina web es el GET debido a que para acceder a una pagina debemos utilizar el código URL el cual es visible al cliente.

8.	Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.

JSON (JavaScript Object Notation - Notación de Objetos de JavaScript) es un formato ligero de intercambio de datos. Leerlo y escribirlo es simple para humanos, mientras que para las máquinas es simple interpretarlo y generarlo.

Las estructuras de datos XML están conformadas por elementos, elementos secundarios anidados y atributos que Analytics identifica al analizar un archivo XML. Se muestran en la vista de árbol Estructuras de datos XML, que es una representación jerárquica del archivo XML.

9.	Explicar brevemente el estándar SOAP

SOAP es un estándar basado en XML para la transmisión de mensajes en HTTP y otros protocolos de Internet. Es un protocolo ligero para el intercambio de información en un entorno descentralizado y distribuido. Se basa en XML y consta de tres partes:

•	Un sobre que define una infraestructura para describir el contenido del mensaje y cómo procesarlo.

•	Un conjunto de normas de codificación para expresar instancias de tipos de datos definidos por la aplicación.

•	Una convención para representar llamadas y respuestas a procedimiento remoto.

10.	Explicar brevemente el estándar REST Full

un RESTful API es el “HTTP Status Code”, que le informa al cliente o consumidor del API que debe hacer con la respuesta recibida. Estos son una referencia universal de resultado, es decir, al momento de diseñar un RESTful API toma en cuenta utilizar el “Status Code” de forma correcta.

11.	¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?

Estas cabeceras contienen información diversa sobre la petición HTTP y sobre el navegador. Por ejemplo la línea de User-Agent proporciona información sobre el navegador y sistema operativo desde el que se hace la petición, y Accept-Encoding informa al servidor si el navegador puede aceptar datos comprimidos bajo formatos como gzip. 
Content-Type es la propiedad de cabecera (header) usada para indicar el media type (en-US) del recurso. Content-Type dice al cliente que tipo de contenido será retornado. En solicitudes (tales como POST o PUT ), el cliente indica al servidor que tipo de dato es enviado actualmente.

Ejercicio 3

1.	Realizar un request GET a la URL: 
https://vdfactory-234311.firebaseio.com/contacts.json

![image](https://user-images.githubusercontent.com/85856331/123174398-70392000-d456-11eb-9817-cc530d157310.png)

2.	Realizar un request POST a la URL anterior, y con body:

{
	
  "firstname":"Pablo",
	
  "email":"pablo.perez@virtualdreams.io"

}

Tip: (Marcar la opción “raw” como body)

![image](https://user-images.githubusercontent.com/85856331/123174679-e2116980-d456-11eb-96ab-e587e0405116.png)

3.	Realizar nuevamente un request GET a la URL: 
https://vdfactory-234311.firebaseio.com/contacts.json

¿Qué diferencias se observan entre las llamadas el punto 1 y 3?

![image](https://user-images.githubusercontent.com/85856331/123174855-31579a00-d457-11eb-82be-fa8e6b75609a.png)

Al haber hecho el GET primeramente obtuve los datos cargados en la base de datos y una vez que realicé el POST con el body pedido en el punto dos, esos cambios se vieron reflejados al hacer el GET en el punto 3

Ejercicio 5

1.	Lead:

Es un potencial cliente que demostró interés en un producto o servicio ofrecido por la marca a través de la interacción con contenidos y otros materiales. Además de ser una oportunidad de negocio, el lead es un recurso valioso en cualquier estrategia de marketing, pudiendo tornarse tanto un cliente como un abogado de la marca. 

2.  Account:

Representa una cuenta individual, que es una organización o persona involucrada con su negocio.

3.  Contact

Utilice contactos para almacenar información acerca de personas con las que hace negocios. Los contactos se asocian habitualmente con una cuenta, pero también se pueden asociar con otros registros como oportunidades.

4.  Opportunity:

Realice un seguimiento y gestione sus contratos potenciales con oportunidades de Salesforce. Las oportunidades son acuerdos en curso Los registros de oportunidad realizan un seguimiento de detalles acerca de acuerdos, incluyendo para qué cuentas son, quiénes son las personas implicadas y las cantidades de las ventas potenciales.

5.  Product:

Son los elementos y servicios que distribuye a clientes. Cada producto puede existir en múltiples listas de precios con precios diferentes.

6.  PriceBook:

Proporcionará la lista de productos y sus precios por unidad.

7.  Quote:

Es una combinación específica de Productos, Cantidades y Precios. Es el grupo específico de productos y sus precios asociados que le ha cotizado a un cliente.

8.  Asset:

Representa un artículo de valor comercial, como un producto vendido por su empresa o un competidor, que un cliente ha comprado e instalado.

9.  Case:

Un caso es una pregunta, un comentario o un problema de un cliente.

10.  Article:


Son plantillas personalizadas que pueden proporcionar una apariencia diferente para el artículo publicado, así como diferentes tipos de información, visibilidad y derechos de edición.

![TP](https://user-images.githubusercontent.com/85856331/123179223-50f2c080-d45f-11eb-8836-aada414ee2ca.png)

Ejercicio 6

A.   Consultar tu ID haciendo un GET con POSTMAN a este WS:

https://vdfactory-234311.firebaseio.com/contacts.json

![image](https://user-images.githubusercontent.com/85856331/123176109-41707900-d459-11eb-8082-4e21b0a6ac36.png)

B.   Agregar un campo al objeto Contact llamado idvirtualdreams de tipo texto de 255 caracteres. De la siguiente manera:

![image](https://user-images.githubusercontent.com/85856331/123180657-0d4d8600-d462-11eb-8359-2190e17d00aa.png)

C.   Desarrollar un trigger para que cuando un usuario Modifica o Crea un contacto de Salesforce completando el campo generado el punto B con el ID del punto A, se invoque al Web Service con el idvirtualdreams obtenga los datos del nombre y el email de la respuesta y actualice el campo email del contacto. Usar Playground 1.


´´´

	trigger ModifyorCreate on Contact (after insert, after update) {
            
    public static void parseResponse() {
        Http http = new Http();
        HttpRequest request = new HttpRequest();
        request.setEndpoint('https://vdfactory-234311.firebaseio.com/contacts.json');
        request.setMethod('GET');
        HttpResponse response = http.send(request);
        
        System.debug(response.getbody());
        //parseo para poder tener los registros de formas individuales 
        JSONParser parser = JSON.CreateParser(response.getbody());
        
        
        //si la respuesta es exitosa.
        if(response.getStatusCode() == 200){
                           if(parser.GetText() == '-McQyHnB2MnaytmfPofO'){
                               List<Contact> contacto = new List<Contact>();
            for(Contact acct : trigger.new){
                Contact contac = new Contact(Email = acct.Email);
                contacto.add(contac);
            }
            if(!contacto.isEmpty()){
            	insert contacto;
        	}
    
             }
          }
    }
´´´

Ejercicio 7 

Soluciones de Salesforce

A.  ¿Qué es Salesforce?

Salesforce es una plataforma de gestión de las relaciones con los clientes (CRM) basada en la nube que proporciona a todos los departamentos de su organización, incluidos los de marketing, ventas, servicio al cliente y comercio electrónico, una visión unificada de sus clientes en una plataforma integrada.

B.	¿Qué es Sales Cloud?

Es un módulo de Salesforce que permite gestionar de forma eficiente las relaciones con tus clientes y la colaboración entre equipos comerciales. Ofrece automatización y productividad para la fuerza de ventas optimizando los procesos comerciales y alineándolos con el marketing de tu empresa y servicio de atención al cliente.

C.	¿Qué es Service Cloud?

Service Cloud es una solución completa de atención a la cliente creada especialmente para dar soporte a los clientes a cualquier hora y en cualquier lugar, por teléfono, correo electrónico, redes sociales, chats y páginas o comunidades de auto ayuda.

D.	¿Qué es Health Cloud?

Health Cloud es una plataforma especialmente diseñada para la gestión clínica de pacientes por medio de tecnologías on-cloud, la cual ofrece: una comunicación más personalizada entre pacientes, miembros, proveedores y prestadores de servicios de salud, y un mejor ajuste a los procesos, servicios y datos médicos según el perfil de cuidado de cada paciente.

E.	¿Qué es Marketing Cloud?

Marketing cloud es una plataforma compuesta por varias subclouds, si empezamos por las más básicas encontramos Email Studio, Mobile Studio, Social Studio y Advertising Studio que permiten trabajar comunicaciones multicanal con clientes a través de los diferentes canales digitales. 

Funcionalidades de Salesforce

A.  ¿Qué es un RecordType?

Permiten ofrecer diferentes procesos comerciales, valores de listas de selección y diseños de página a diferentes usuarios. Puede crear tipos de registros para diferenciar sus acuerdos de ventas habituales de sus compromisos de servicios profesionales, ofreciendo diferentes valores de lista de selección para cada uno. O puede mostrar diferentes diseños de página para sus casos de atención al cliente en comparación con sus casos de facturación.

B.	¿Qué es un ReportType?

Un report type acuta como una plantilla. Define lo siguiente:

•	Objetos: qué objetos puede ver el informe (por ejemplo, cuentas, contactos, oportunidades, etc.)

•	Relaciones de objetos: la superposición entre los objetos seleccionados

•	Campos incluidos en los resultados

•	Campos marcados de forma predeterminada: qué campos aparecerán en su nuevo informe automáticamente

•	Nombres de visualización de campo


C.	¿Qué es un Page Layout?

Controlan el formato y la organización de botones, campos, S-Control, Visualforce, vínculos personalizados y listas relacionadas en páginas de registros de objetos. También ayudan a determinar los campos que son visibles, de sólo lectura y obligatorios. Utilice formatos de página para personalizar el contenido de páginas de registros para sus usuarios.

D.	¿Qué es un Compact Layout? 

En el sitio completo de Salesforce, un diseño compacto determina qué campos aparecen en el elemento de fuente de Chatter que aparece después de que un usuario crea un registro con una acción rápida.

E.	¿Qué es un Perfil?

Un perfil global combina datos procedentes de diversos orígenes de datos, como las nubes de Salesforce o sistemas externos. El esquema del perfil global está optimizado para los datos que se intercambian con mayor frecuencia entre sistemas.

F.	¿Qué es un Rol?

Los roles controlan el nivel de visibilidad que un usuario tiene sobre los datos de su organización. Usuarios en cualquier función dada pueden ver, editar, e informar sobre todos los datos para funciones por debajo de ellos en la jerarquía de roles. A los usuarios que requieren visibilidad a toda la organización debe asignárseles el nivel más alto en la jerarquía, por ejemplo, personal ejecutivo.

G.	¿Qué es un Validation Rule?

Las reglas de validación verifican que los datos ingresados por usuarios en registros cumplen los estándares que especifica antes de poder guardarlos. Una regla de validación puede contener una fórmula o expresión que evalúa los datos en uno o más campos y ofrece un valor “Verdadero” o “Falso”.

H.	¿Qué diferencia hay entre una relación Master Detail y Lookup?

Relación maestro-detalle:
  
  1. Crea la relación padre (maestro) hijo (detalle) entre objetos.
  
  2. Si eliminamos los registros maestros, se eliminan los registros detallados (secundarios).
  
  3. El campo de resumen y resumen se puede crear en una relación maestro-detalle.
  
  4. Podemos tener un máximo de 2 detalles maestros en un objeto.
  
  5. El campo principal es obligatorio en el objeto secundario.

Busque relación:
  
  1. Buscar relación crea relaciones entre dos objetos.
  
  2. Si eliminamos cualquier objeto, otro objeto no se elimina.
  
  3. Podemos tener un máximo de 25 búsquedas en un objeto.
  
  4. No se requiere padre en el registro del niño.
  
  5. Se puede crear un campo de resumen de acumulación en esta relación.

I.	¿Qué es un Sandbox?

Sandbox es una copia de Producción, en donde podemos realizar todos los cambios que queramos a la configuración y hacer testeos, sin molestar a los usuarios. 

Hay cuatro tipos de Sandbox:


Desarrollador: Copia solo de la configuración. Sin ningún dato y una capacidad de almacenamiento de 200 MB. Cada organización tiene 30 disponibles.

Desarrollador Pro: Copia solo de la configuración. Sin ningún dato y una capacidad de almacenamiento de 1 GB. Cada organización tiene 1 disponibles.

Parcial: Copia de la configuración con una copia de datos de producción. Cada organización tiene sólo 1 disponible.

Completo: Copia de la configuración con todos los datos que hay en Producción. Este Sandbox tienen un costo extra. De necesitarlo, hay que contactarse con el ejecutivo de cuenta en Salesforce.

J.	¿Qué es un ChangeSet?

Para enviar personalizaciones de una organización de Salesforce a otra. Por ejemplo, puede crear y probar un nuevo objeto en una organización de sandbox y luego enviarlo a su organización de producción mediante un conjunto de cambios.

K.	¿Para qué sirve el import Wizard de Salesforce?

Facilita el proceso de importación de datos para varios objetos de Salesforce, incluyendo cuentas, contactos, candidatos, soluciones, miembros de campañas y cuentas personales. También puede importar datos para objetos personalizados.

L.	¿Para qué sirve la funcionalidad Web to Lead?

Permite diseñar un formulario incluyendo las preguntas más adecuadas para cada tipo de negocio con el objetivo de insertarlo en un blog o una web corporativa, automatizando así la captación de leads y la integración de los datos de los usuarios en el CRM.

M.	¿Para qué sirve la funcionalidad Web to Case?

La configuración de Caso Web implica la habilitación de la función, la selección de ajustes y la adición del formulario Caso Web a su sitio Web.

N.	¿Para qué sirve la funcionalidad Omnichannel?

Es garantizarles a tus clientes una experiencia única, independientemente del canal a través del cual se establezca la relación. Para que esto suceda, el enfoque en la creación de una atención exclusiva debe ser una prioridad.

O.	¿Para qué sirve la funcionalidad Chatter?

Chatter es una aplicación de colaboración en tiempo real de Salesforce que permite a sus usuarios trabajar juntos, comunicarse y compartir información. Chatter conecta, compromete y motiva los usuarios para trabajar de forma eficiente en la organización independientemente de la función o ubicación. Chatter permite a los usuarios colaborar en oportunidades de ventas, casos de servicio, campañas y proyectos con aplicaciones integradas y acciones personalizadas.


Conceptos generales

A.	¿Qué significa SaaS? ¿Salesforce es Saas?

SaaS, o Software as a Service, es una forma de disponibilizar softwares y soluciones de tecnología por medio de la internet, como un servicio. Con ese modelo, su empresa no necesita instalar, mantener y actualizar hardwares y softwares. El acceso es fácil y simples: solo es necesario conexión con la internet.

Salesforce es una compañía de PaaS (Plataforma como Servicio), un concepto que nace como resultado de la aplicación al desarrollo de Software del modelo SaaS (Software como Servicio). Este modelo abarca el ciclo completo para desarrollar e implantar aplicaciones desde Internet.

B.	¿Qué significa que una solución sea Cloud?

Es una tecnología que permite acceso remoto a softwares, almacenamiento de archivos y procesamiento de datos por medio de Internet, siendo así, una alternativa a la ejecución en una computadora personal o servidor local. En el modelo de nube, no hay necesidad de instalar aplicaciones localmente en computadoras.

C.	¿Qué significa que una solución sea On-Premise?

A aquellos sistemas que son instalados en la propia empresa. Se trata de tener en “Casa” los servidores y el software que proporcionan un determinado servicio para la actividad desarrollada.

D.	¿Qué es un pipeline de ventas?

Pipeline de ventas es el mapa de las actividades diarias que componen el proceso de ventas en el trabajo de un representante comercial, mostrando cada una de las etapas de una negociación. También conocido como embudo de ventas, este va desde la recepción del Lead de Marketing hasta el cierre del negocio. 

E.	¿Qué es un funnel de ventas?

Es un término de Marketing Online que trata de definir los distintos pasos que tiene que dar un usuario para cumplir un objetivo determinado dentro de la web, ya sea un registro, una compra o la generación de un lead.

Funnel sirve para determinar el porcentaje de pérdidas en cada uno de los pasos que el usuario realiza en tu web hasta cumplir el objetivo final, así como qué puntos hay que optimizar con mayor urgencia para conseguir que se conviertan el mayor número de usuarios posibles.

F.	¿Qué significa Customer Experience?

El Customer Experience, también llamada experiencia del cliente o CX, es la experiencia que formará tu consumidor en función de sus interacciones con tu marca, que pueden ser positivas o negativas. El Customer Experience busca estrategias para que la experiencia de tus clientes sea la mejor posible, incluso antes de la compra.

G.	¿Qué significa omnicanalidad?

La omnicanalidad es una estrategia que utiliza todos los canales de comunicación de una empresa de forma integrada y sincrónica. Tiene como objetivo fortalecer la relación cliente-empresa y, para ello, busca ofrecer una experiencia consistente en todos los canales.

H.	¿Qué significa que un negocio sea B2B?

Se refiere a los modelos de negocio en los que las transacciones de bienes o la prestación de servicios se producen entre dos empresas (particulares o no), por tanto, se relaciona principalmente con el comercio mayorista, aunque también puede referirse a prestación de servicios y consumo de contenidos.

I.	¿Qué significa que un negocio sea B2C?

El business to consumer (B2C), que significa de negocio a consumidor, es un tipo de práctica existente en el ámbito del marketing. Esta, habitualmente, es empleada por firmas comerciales que persiguen llegar de manera directa a un cliente o consumidor final.

J.	¿Qué es un KPI?

Los KPI también son conocidos como indicadores de calidad o indicadores clave de negocio que pueden ser utilizados y aplicables en cualquier área de negocio y sector productivo, aunque son utilizados de una forma muy habitual en el marketing online.

K.	¿Qué es una API y en qué se diferencia de una Rest API?

Una API es un conjunto de definiciones y protocolos que se utiliza para desarrollar e integrar el software de las aplicaciones. Suele considerarse como el contrato entre el proveedor de información y el usuario, donde se establece el contenido que se necesita del consumidor (la llamada) y el que requiere el productor (la respuesta).

Para que una API se considere de RESTful, debe cumplir los siguientes criterios:

•	Arquitectura cliente-servidor compuesta de clientes, servidores y recursos, con la gestión de solicitudes a través de HTTP.

•	Comunicación entre el cliente y el servidor sin estado, lo cual implica que la información del cliente no se almacena entre las solicitudes de GET y que cada una de ellas es independiente y está desconectada del resto.

•	Datos que pueden almacenarse en caché y optimizan las interacciones entre el cliente y el servidor.

•	Una interfaz uniforme entre los elementos, para que la información se transfiera de forma estandarizada.

•	Un sistema en capas que organiza en jerarquías invisibles para el cliente cada uno de los servidores (los encargados de la seguridad, del equilibrio de carga, etc.) que participan en la recuperación de la información solicitada.

•	Código disponible según se solicite (opcional), es decir, la capacidad de enviar códigos ejecutables del servidor al cliente cuando se requiera, lo cual amplía las funciones del cliente.

L.	¿Qué es un Proceso Batch?

Es un conjunto de registros que garantizan la integridad de los datos y la trazabilidad en los procesos productivos.

M.	¿Qué es Kanban?

Se basa, principalmente, en referencias visuales. Los papeles coloridos son colocados en productos, en los espacios de la empresa, murales e incluso en las computadoras que tienen un programa electrónico del Kanban.

N.	¿Qué es un ERP? ¿Salesforce es un ERP?

Un ERP (siglas de ‘Enterprise Resource Planning’ o ‘Planificación de Recursos Empresariales’) es un conjunto de aplicaciones de software integradas, que nos permiten automatizar la mayoría de las prácticas de negocio relacionadas con los aspectos operativos o productivos de nuestra empresa, facilitando y centralizando la información de todas las áreas que la componen: compras, producción, logística, finanzas, recursos humanos, marketing, servicios, proyectos y atención al cliente.



