# Dominio 1: Desarrollo con servicios de AWS (32 %)

Preguntas de práctica AWS Certified Developer Associate (DVA-C02) — 132 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [¿Cuáles de los siguientes servicios son almacenes clave-valor? (Elija 3 respuestas)](#cuáles-de-los-siguientes-servicios-son-almacenes-clave-valor-elija-3-respuestas) |
| 2 | [Un desarrollador desea enviar encabezados multivalor (multi-value headers) a una función de AWS Lambda registrada como destino (target) de un Application Load Balancer (ALB). ¿Qué debe hacer el desarrollador para lograrlo?](#un-desarrollador-desea-enviar-encabezados-multivalor-multi-value-headers-a-una-función-de-aws-lambda-registrada-como-destino-target-de-un-application-load-balancer-alb-qué-debe-hacer-el-desarrollador-para-lograrlo) |
| 3 | [El sitio web de comercio electrónico de una empresa experimenta picos masivos de tráfico que causan problemas de rendimiento en la base de datos de la empresa. Los usuarios reportan que acceder al sitio web toma mucho tiempo. Un desarrollador desea implementar una capa de caché con Amazon ElastiCache. El sitio web debe ser receptivo sin importar qué producto vea un usuario, y las actualizaciones de la información y los precios de los productos deben ser fuertemente consistentes. ¿Qué política de escritura en caché cumplirá con estos requisitos?](#el-sitio-web-de-comercio-electrónico-de-una-empresa-experimenta-picos-masivos-de-tráfico-que-causan-problemas-de-rendimiento-en-la-base-de-datos-de-la-empresa-los-usuarios-reportan-que-acceder-al-sitio-web-toma-mucho-tiempo-un-desarrollador-desea-implementar-una-capa-de-caché-con-amazon-elasticache-el-sitio-web-debe-ser-receptivo-sin-importar-qué-producto-vea-un-usuario-y-las-actualizaciones-de-la-información-y-los-precios-de-los-productos-deben-ser-fuertemente-consistentes-qué-política-de-escritura-en-caché-cumplirá-con-estos-requisitos) |
| 4 | [La Empresa D ejecuta su sitio web corporativo en Amazon S3, al que se accede desde `http://www.companyd.com`. Su equipo de marketing publicó nuevas fuentes web en un bucket de S3 separado, al que se accede mediante el endpoint de S3 `https://s3-us-west-1.amazonaws.com/cdfonts`. Al probar las nuevas fuentes web, la Empresa D notó que el navegador las está bloqueando. ¿Qué debe hacer la Empresa D para evitar que el navegador bloquee las fuentes web?](#la-empresa-d-ejecuta-su-sitio-web-corporativo-en-amazon-s3-al-que-se-accede-desde-httpwwwcompanydcom-su-equipo-de-marketing-publicó-nuevas-fuentes-web-en-un-bucket-de-s3-separado-al-que-se-accede-mediante-el-endpoint-de-s3-httpss3-us-west-1amazonawscomcdfonts-al-probar-las-nuevas-fuentes-web-la-empresa-d-notó-que-el-navegador-las-está-bloqueando-qué-debe-hacer-la-empresa-d-para-evitar-que-el-navegador-bloquee-las-fuentes-web) |
| 5 | [Un desarrollador está creando una aplicación que necesita localizar la dirección IPv4 pública de la instancia de Amazon EC2 en la que se ejecuta. ¿Cómo puede la aplicación obtener esta información?](#un-desarrollador-está-creando-una-aplicación-que-necesita-localizar-la-dirección-ipv4-pública-de-la-instancia-de-amazon-ec2-en-la-que-se-ejecuta-cómo-puede-la-aplicación-obtener-esta-información) |
| 6 | [Un desarrollador necesita modificar la arquitectura de una aplicación para cumplir con nuevos requisitos funcionales. Los datos de la aplicación se almacenan en Amazon DynamoDB y se procesan para su análisis en un lote nocturno. Los analistas del sistema no quieren esperar hasta el día siguiente para ver los datos procesados y han solicitado que estén disponibles casi en tiempo real. ¿Qué patrón de arquitectura de aplicación permitiría que los datos se procesen a medida que se reciben?](#un-desarrollador-necesita-modificar-la-arquitectura-de-una-aplicación-para-cumplir-con-nuevos-requisitos-funcionales-los-datos-de-la-aplicación-se-almacenan-en-amazon-dynamodb-y-se-procesan-para-su-análisis-en-un-lote-nocturno-los-analistas-del-sistema-no-quieren-esperar-hasta-el-día-siguiente-para-ver-los-datos-procesados-y-han-solicitado-que-estén-disponibles-casi-en-tiempo-real-qué-patrón-de-arquitectura-de-aplicación-permitiría-que-los-datos-se-procesen-a-medida-que-se-reciben) |
| 7 | [Una aplicación utiliza Amazon Kinesis Data Streams para ingerir y procesar grandes flujos de registros de datos en tiempo real. Las instancias de Amazon EC2 consumen y procesan los datos de los shards del flujo de datos de Kinesis mediante Amazon Kinesis Client Library (KCL). La aplicación maneja los escenarios de falla y no requiere workers en espera. La aplicación reporta que un shard específico está recibiendo más datos de lo esperado. Para adaptarse a los cambios en la tasa de flujo de datos, se realiza un resharding del shard `hot`. Suponiendo que el número inicial de shards en el flujo de datos de Kinesis es 4 y que después del resharding el número de shards aumentó a 6, ¿cuál es el número máximo de instancias EC2 que se pueden implementar para procesar los datos de todos los shards?](#una-aplicación-utiliza-amazon-kinesis-data-streams-para-ingerir-y-procesar-grandes-flujos-de-registros-de-datos-en-tiempo-real-las-instancias-de-amazon-ec2-consumen-y-procesan-los-datos-de-los-shards-del-flujo-de-datos-de-kinesis-mediante-amazon-kinesis-client-library-kcl-la-aplicación-maneja-los-escenarios-de-falla-y-no-requiere-workers-en-espera-la-aplicación-reporta-que-un-shard-específico-está-recibiendo-más-datos-de-lo-esperado-para-adaptarse-a-los-cambios-en-la-tasa-de-flujo-de-datos-se-realiza-un-resharding-del-shard-hot-suponiendo-que-el-número-inicial-de-shards-en-el-flujo-de-datos-de-kinesis-es-4-y-que-después-del-resharding-el-número-de-shards-aumentó-a-6-cuál-es-el-número-máximo-de-instancias-ec2-que-se-pueden-implementar-para-procesar-los-datos-de-todos-los-shards) |
| 8 | [Una empresa de videojuegos está desarrollando una aplicación de juego móvil para las plataformas iOS® y Android®. Este juego móvil almacena de forma segura los datos del usuario localmente en el dispositivo. La empresa desea permitir que los usuarios utilicen varios dispositivos para el juego, lo que requiere la sincronización de los datos del usuario entre dispositivos. ¿Qué servicio se debe utilizar para sincronizar los datos del usuario entre dispositivos sin necesidad de crear una aplicación backend?](#una-empresa-de-videojuegos-está-desarrollando-una-aplicación-de-juego-móvil-para-las-plataformas-ios-y-android-este-juego-móvil-almacena-de-forma-segura-los-datos-del-usuario-localmente-en-el-dispositivo-la-empresa-desea-permitir-que-los-usuarios-utilicen-varios-dispositivos-para-el-juego-lo-que-requiere-la-sincronización-de-los-datos-del-usuario-entre-dispositivos-qué-servicio-se-debe-utilizar-para-sincronizar-los-datos-del-usuario-entre-dispositivos-sin-necesidad-de-crear-una-aplicación-backend) |
| 9 | [Un desarrollador está escribiendo un servicio REST que agregará elementos a una lista de compras. El servicio está construido sobre Amazon API Gateway con integraciones de AWS Lambda. Los elementos de la lista de compras se envían como parámetros de cadena de consulta (query string) en la solicitud del método. ¿Cómo debe el desarrollador convertir los parámetros de cadena de consulta en argumentos para la función Lambda?](#un-desarrollador-está-escribiendo-un-servicio-rest-que-agregará-elementos-a-una-lista-de-compras-el-servicio-está-construido-sobre-amazon-api-gateway-con-integraciones-de-aws-lambda-los-elementos-de-la-lista-de-compras-se-envían-como-parámetros-de-cadena-de-consulta-query-string-en-la-solicitud-del-método-cómo-debe-el-desarrollador-convertir-los-parámetros-de-cadena-de-consulta-en-argumentos-para-la-función-lambda) |
| 10 | [¿Cómo se ve afectado el rendimiento aprovisionado (provisioned throughput) por el modelo de consistencia elegido al leer datos de una tabla de DynamoDB?](#cómo-se-ve-afectado-el-rendimiento-aprovisionado-provisioned-throughput-por-el-modelo-de-consistencia-elegido-al-leer-datos-de-una-tabla-de-dynamodb) |
| 11 | [Un proveedor está escribiendo una nueva API RESTful para que los clientes consulten el estado de los pedidos. Los clientes solicitaron el siguiente endpoint de API `http://www.supplierdomain.com/status/customerID`. ¿Cuáles de los siguientes diseños de aplicación cumplen con los requisitos? (Seleccione DOS)](#un-proveedor-está-escribiendo-una-nueva-api-restful-para-que-los-clientes-consulten-el-estado-de-los-pedidos-los-clientes-solicitaron-el-siguiente-endpoint-de-api-httpwwwsupplierdomaincomstatuscustomerid-cuáles-de-los-siguientes-diseños-de-aplicación-cumplen-con-los-requisitos-seleccione-dos) |
| 12 | [Un desarrollador está diseñando una función de AWS Lambda que crea archivos temporales de menos de 10 MB durante su ejecución. Los archivos temporales se accederán y modificarán varias veces durante la ejecución. El desarrollador no necesita guardar ni recuperar estos archivos en el futuro. ¿Dónde se deben almacenar los archivos temporales?](#un-desarrollador-está-diseñando-una-función-de-aws-lambda-que-crea-archivos-temporales-de-menos-de-10-mb-durante-su-ejecución-los-archivos-temporales-se-accederán-y-modificarán-varias-veces-durante-la-ejecución-el-desarrollador-no-necesita-guardar-ni-recuperar-estos-archivos-en-el-futuro-dónde-se-deben-almacenar-los-archivos-temporales) |
| 13 | [Una empresa está desarrollando una aplicación web de comercio electrónico sin servidor. La aplicación necesita realizar cambios coordinados de tipo todo o nada en varios elementos de la tabla de inventario de la empresa en Amazon DynamoDB. ¿Qué solución cumplirá con estos requisitos?](#una-empresa-está-desarrollando-una-aplicación-web-de-comercio-electrónico-sin-servidor-la-aplicación-necesita-realizar-cambios-coordinados-de-tipo-todo-o-nada-en-varios-elementos-de-la-tabla-de-inventario-de-la-empresa-en-amazon-dynamodb-qué-solución-cumplirá-con-estos-requisitos) |
| 14 | [Un desarrollador necesita diseñar una aplicación que se ejecuta en AWS y que se usará para consumir mensajes de Amazon SQS con tamaños que van desde 1 KB hasta 1 GB. ¿Cómo se deben administrar los mensajes de Amazon SQS?](#un-desarrollador-necesita-diseñar-una-aplicación-que-se-ejecuta-en-aws-y-que-se-usará-para-consumir-mensajes-de-amazon-sqs-con-tamaños-que-van-desde-1-kb-hasta-1-gb-cómo-se-deben-administrar-los-mensajes-de-amazon-sqs) |
| 15 | [Se le pide a un desarrollador implementar una capa de caché delante de Amazon RDS. El contenido en caché es costoso de regenerar en caso de una falla del servicio. ¿Qué implementación de las siguientes funcionaría manteniendo el máximo tiempo de actividad?](#se-le-pide-a-un-desarrollador-implementar-una-capa-de-caché-delante-de-amazon-rds-el-contenido-en-caché-es-costoso-de-regenerar-en-caso-de-una-falla-del-servicio-qué-implementación-de-las-siguientes-funcionaría-manteniendo-el-máximo-tiempo-de-actividad) |
| 16 | [Una aplicación sin servidor utiliza un API Gateway y AWS Lambda. ¿Dónde debería almacenar la función Lambda su información de sesión entre invocaciones de la función?](#una-aplicación-sin-servidor-utiliza-un-api-gateway-y-aws-lambda-dónde-debería-almacenar-la-función-lambda-su-información-de-sesión-entre-invocaciones-de-la-función) |
| 17 | [Una arquitectura actual utiliza muchas funciones Lambda que se invocan entre sí como una máquina de estados grande. La coordinación de esta máquina de estados es código personalizado heredado que se rompe con facilidad. ¿Qué servicio de AWS puede ayudar a refactorizar y administrar la máquina de estados?](#una-arquitectura-actual-utiliza-muchas-funciones-lambda-que-se-invocan-entre-sí-como-una-máquina-de-estados-grande-la-coordinación-de-esta-máquina-de-estados-es-código-personalizado-heredado-que-se-rompe-con-facilidad-qué-servicio-de-aws-puede-ayudar-a-refactorizar-y-administrar-la-máquina-de-estados) |
| 18 | [Un desarrollador debe volver a implementar la lógica de negocio de un sistema de cumplimiento de pedidos. La lógica de negocio tiene que realizar solicitudes a varios proveedores para decidir dónde comprar un artículo. Todo el proceso puede tardar hasta una semana en completarse. ¿Cuál es la forma MÁS eficiente y MÁS SIMPLE de implementar un sistema que cumpla con estos requisitos?](#un-desarrollador-debe-volver-a-implementar-la-lógica-de-negocio-de-un-sistema-de-cumplimiento-de-pedidos-la-lógica-de-negocio-tiene-que-realizar-solicitudes-a-varios-proveedores-para-decidir-dónde-comprar-un-artículo-todo-el-proceso-puede-tardar-hasta-una-semana-en-completarse-cuál-es-la-forma-más-eficiente-y-más-simple-de-implementar-un-sistema-que-cumpla-con-estos-requisitos) |
| 19 | [Una aplicación móvil almacena publicaciones de blog en una tabla de Amazon DynamoDB. Se agregan millones de publicaciones cada día y cada publicación representa un único elemento de la tabla. La aplicación móvil solo requiere las publicaciones recientes. Cualquier publicación con más de 48 horas de antigüedad puede eliminarse. ¿Cuál es la forma MÁS rentable de eliminar las publicaciones con más de 48 horas de antigüedad?](#una-aplicación-móvil-almacena-publicaciones-de-blog-en-una-tabla-de-amazon-dynamodb-se-agregan-millones-de-publicaciones-cada-día-y-cada-publicación-representa-un-único-elemento-de-la-tabla-la-aplicación-móvil-solo-requiere-las-publicaciones-recientes-cualquier-publicación-con-más-de-48-horas-de-antigüedad-puede-eliminarse-cuál-es-la-forma-más-rentable-de-eliminar-las-publicaciones-con-más-de-48-horas-de-antigüedad) |
| 20 | [Una aplicación procesa en tiempo real millones de eventos que se reciben a través de una API. ¿Qué servicio podría utilizarse para permitir que varios consumidores procesen los datos de forma concurrente y de la manera MÁS rentable?](#una-aplicación-procesa-en-tiempo-real-millones-de-eventos-que-se-reciben-a-través-de-una-api-qué-servicio-podría-utilizarse-para-permitir-que-varios-consumidores-procesen-los-datos-de-forma-concurrente-y-de-la-manera-más-rentable) |
| 21 | [Una aplicación ingerirá datos a muy alto rendimiento desde muchas fuentes y debe almacenar los datos en un bucket de Amazon S3. ¿Qué servicio cumpliría MEJOR con esta tarea?](#una-aplicación-ingerirá-datos-a-muy-alto-rendimiento-desde-muchas-fuentes-y-debe-almacenar-los-datos-en-un-bucket-de-amazon-s3-qué-servicio-cumpliría-mejor-con-esta-tarea) |
| 22 | [Un servicio heredado tiene una interfaz SOAP basada en XML. El desarrollador quiere exponer la funcionalidad del servicio a clientes externos con Amazon API Gateway. ¿Qué técnica logrará esto?](#un-servicio-heredado-tiene-una-interfaz-soap-basada-en-xml-el-desarrollador-quiere-exponer-la-funcionalidad-del-servicio-a-clientes-externos-con-amazon-api-gateway-qué-técnica-logrará-esto) |
| 23 | [Un desarrollador ha configurado un Amazon Kinesis Stream con 4 shards para ingerir un máximo de 2500 registros por segundo. Se ha configurado una función Lambda para procesar estos registros. ¿En qué orden se procesarán estos registros?](#un-desarrollador-ha-configurado-un-amazon-kinesis-stream-con-4-shards-para-ingerir-un-máximo-de-2500-registros-por-segundo-se-ha-configurado-una-función-lambda-para-procesar-estos-registros-en-qué-orden-se-procesarán-estos-registros) |
| 24 | [Una aplicación está diseñada para usar Amazon SQS para administrar mensajes de muchos remitentes independientes. Los mensajes de cada remitente deben procesarse en el orden en que se reciben. ¿Qué característica de SQS debe implementar el desarrollador?](#una-aplicación-está-diseñada-para-usar-amazon-sqs-para-administrar-mensajes-de-muchos-remitentes-independientes-los-mensajes-de-cada-remitente-deben-procesarse-en-el-orden-en-que-se-reciben-qué-característica-de-sqs-debe-implementar-el-desarrollador) |
| 25 | [Un desarrollador está trabajando en una aplicación que registra cientos de millones de reseñas de productos en una tabla de Amazon DynamoDB. Los registros incluyen los elementos de datos que se muestran en la tabla. ¿Qué campo, al usarse como clave de partición, produciría el rendimiento MÁS consistente con DynamoDB?](#un-desarrollador-está-trabajando-en-una-aplicación-que-registra-cientos-de-millones-de-reseñas-de-productos-en-una-tabla-de-amazon-dynamodb-los-registros-incluyen-los-elementos-de-datos-que-se-muestran-en-la-tabla-qué-campo-al-usarse-como-clave-de-partición-produciría-el-rendimiento-más-consistente-con-dynamodb) |
| 26 | [Una aplicación tarda 40 segundos en procesar las instrucciones recibidas en un mensaje de Amazon SQS. Suponiendo que la cola de SQS está configurada con el valor predeterminado de `VisibilityTimeout`, ¿cuál es la MEJOR manera, al recibir un mensaje, de asegurar que ninguna otra instancia pueda recuperar un mensaje que ya ha sido procesado o que se está procesando actualmente?](#una-aplicación-tarda-40-segundos-en-procesar-las-instrucciones-recibidas-en-un-mensaje-de-amazon-sqs-suponiendo-que-la-cola-de-sqs-está-configurada-con-el-valor-predeterminado-de-visibilitytimeout-cuál-es-la-mejor-manera-al-recibir-un-mensaje-de-asegurar-que-ninguna-otra-instancia-pueda-recuperar-un-mensaje-que-ya-ha-sido-procesado-o-que-se-está-procesando-actualmente) |
| 27 | [Un desarrollador está escribiendo transacciones en una tabla de DynamoDB llamada `SystemUpdates` que tiene 5 unidades de capacidad de escritura. ¿Qué opción tiene el mayor rendimiento de lectura?](#un-desarrollador-está-escribiendo-transacciones-en-una-tabla-de-dynamodb-llamada-systemupdates-que-tiene-5-unidades-de-capacidad-de-escritura-qué-opción-tiene-el-mayor-rendimiento-de-lectura) |
| 28 | [Una aplicación almacena imágenes en un bucket de S3. Las notificaciones de eventos de Amazon S3 se usan para activar una función Lambda que cambia el tamaño de las imágenes. Procesar cada imagen toma menos de un segundo. ¿Cómo manejará AWS Lambda el tráfico adicional?](#una-aplicación-almacena-imágenes-en-un-bucket-de-s3-las-notificaciones-de-eventos-de-amazon-s3-se-usan-para-activar-una-función-lambda-que-cambia-el-tamaño-de-las-imágenes-procesar-cada-imagen-toma-menos-de-un-segundo-cómo-manejará-aws-lambda-el-tráfico-adicional) |
| 29 | [Una aplicación sobrescribe un objeto en Amazon S3 y luego lee inmediatamente el mismo objeto. ¿Por qué la aplicación a veces recuperaría la versión anterior del objeto?](#una-aplicación-sobrescribe-un-objeto-en-amazon-s3-y-luego-lee-inmediatamente-el-mismo-objeto-por-qué-la-aplicación-a-veces-recuperaría-la-versión-anterior-del-objeto) |
| 30 | [Un desarrollador está configurando Amazon API Gateway para los productos de su empresa. La API será utilizada por desarrolladores registrados para consultar y actualizar sus entornos. La empresa quiere limitar la cantidad de solicitudes que los usuarios finales pueden enviar, tanto por razones de costo como de seguridad. La dirección quiere ofrecer a los desarrolladores registrados la opción de comprar paquetes más grandes que permitan más solicitudes. ¿Cómo puede el desarrollador lograr esto con la MENOR cantidad de sobrecarga de administración?](#un-desarrollador-está-configurando-amazon-api-gateway-para-los-productos-de-su-empresa-la-api-será-utilizada-por-desarrolladores-registrados-para-consultar-y-actualizar-sus-entornos-la-empresa-quiere-limitar-la-cantidad-de-solicitudes-que-los-usuarios-finales-pueden-enviar-tanto-por-razones-de-costo-como-de-seguridad-la-dirección-quiere-ofrecer-a-los-desarrolladores-registrados-la-opción-de-comprar-paquetes-más-grandes-que-permitan-más-solicitudes-cómo-puede-el-desarrollador-lograr-esto-con-la-menor-cantidad-de-sobrecarga-de-administración) |
| 31 | [Un desarrollador está refactorizando una aplicación monolítica. La aplicación recibe una solicitud POST y realiza varias operaciones. Algunas de las operaciones se ejecutan en paralelo, mientras que otras se ejecutan secuencialmente. Estas operaciones han sido refactorizadas en funciones individuales de AWS Lambda. La solicitud POST será procesada por Amazon API Gateway. ¿Cómo debería el desarrollador invocar las funciones Lambda en la misma secuencia usando API Gateway?](#un-desarrollador-está-refactorizando-una-aplicación-monolítica-la-aplicación-recibe-una-solicitud-post-y-realiza-varias-operaciones-algunas-de-las-operaciones-se-ejecutan-en-paralelo-mientras-que-otras-se-ejecutan-secuencialmente-estas-operaciones-han-sido-refactorizadas-en-funciones-individuales-de-aws-lambda-la-solicitud-post-será-procesada-por-amazon-api-gateway-cómo-debería-el-desarrollador-invocar-las-funciones-lambda-en-la-misma-secuencia-usando-api-gateway) |
| 32 | [Una empresa está agregando la capacidad de valor almacenado (o tarjeta de regalo) a su popular sitio web de juegos casuales. Los usuarios necesitan poder intercambiar este valor por artículos de otros usuarios en la plataforma. Esto requeriría que los registros de ambos usuarios se actualicen como una sola transacción, o que los registros de ambos usuarios se reviertan por completo. ¿Qué opciones de base de datos de AWS pueden proporcionar la capacidad transaccional requerida para esta nueva funcionalidad? (Elija DOS)](#una-empresa-está-agregando-la-capacidad-de-valor-almacenado-o-tarjeta-de-regalo-a-su-popular-sitio-web-de-juegos-casuales-los-usuarios-necesitan-poder-intercambiar-este-valor-por-artículos-de-otros-usuarios-en-la-plataforma-esto-requeriría-que-los-registros-de-ambos-usuarios-se-actualicen-como-una-sola-transacción-o-que-los-registros-de-ambos-usuarios-se-reviertan-por-completo-qué-opciones-de-base-de-datos-de-aws-pueden-proporcionar-la-capacidad-transaccional-requerida-para-esta-nueva-funcionalidad-elija-dos) |
| 33 | [Un desarrollador está creando una función de AWS Lambda que genera un nuevo archivo cada vez que se ejecuta. Cada nuevo archivo debe registrarse (check in) en un repositorio de AWS CodeCommit alojado en la misma cuenta de AWS. ¿Cómo debería el desarrollador lograr esto?](#un-desarrollador-está-creando-una-función-de-aws-lambda-que-genera-un-nuevo-archivo-cada-vez-que-se-ejecuta-cada-nuevo-archivo-debe-registrarse-check-in-en-un-repositorio-de-aws-codecommit-alojado-en-la-misma-cuenta-de-aws-cómo-debería-el-desarrollador-lograr-esto) |
| 34 | [Un equipo de desarrollo está trabajando en una aplicación móvil que permite a los usuarios cargar fotos en Amazon S3. El equipo espera que la aplicación sea utilizada simultáneamente por cientos de miles de usuarios durante un solo evento. Una vez cargadas las fotos, el servicio de backend las analizará y procesará para detectar contenido inapropiado. ¿Qué enfoque es la forma MÁS resiliente de lograr este objetivo y que además suaviza los picos temporales de volumen para el servicio de backend?](#un-equipo-de-desarrollo-está-trabajando-en-una-aplicación-móvil-que-permite-a-los-usuarios-cargar-fotos-en-amazon-s3-el-equipo-espera-que-la-aplicación-sea-utilizada-simultáneamente-por-cientos-de-miles-de-usuarios-durante-un-solo-evento-una-vez-cargadas-las-fotos-el-servicio-de-backend-las-analizará-y-procesará-para-detectar-contenido-inapropiado-qué-enfoque-es-la-forma-más-resiliente-de-lograr-este-objetivo-y-que-además-suaviza-los-picos-temporales-de-volumen-para-el-servicio-de-backend) |
| 35 | [Un equipo de desarrollo quiere ejecutar sus cargas de trabajo de contenedores en Amazon ECS. Cada contenedor de aplicación necesita compartir datos con otro contenedor para recopilar logs y métricas. ¿Qué debe hacer el equipo de desarrollo para cumplir con estos requisitos?](#un-equipo-de-desarrollo-quiere-ejecutar-sus-cargas-de-trabajo-de-contenedores-en-amazon-ecs-cada-contenedor-de-aplicación-necesita-compartir-datos-con-otro-contenedor-para-recopilar-logs-y-métricas-qué-debe-hacer-el-equipo-de-desarrollo-para-cumplir-con-estos-requisitos) |
| 36 | [Un desarrollador está escribiendo una aplicación web que debe compartir documentos seguros con los usuarios finales. Los documentos se almacenan en un bucket privado de Amazon S3. La aplicación debe permitir que solo los usuarios autenticados descarguen documentos específicos cuando se soliciten, y únicamente durante un período de 15 minutos. ¿Cómo puede el desarrollador cumplir con estos requisitos?](#un-desarrollador-está-escribiendo-una-aplicación-web-que-debe-compartir-documentos-seguros-con-los-usuarios-finales-los-documentos-se-almacenan-en-un-bucket-privado-de-amazon-s3-la-aplicación-debe-permitir-que-solo-los-usuarios-autenticados-descarguen-documentos-específicos-cuando-se-soliciten-y-únicamente-durante-un-período-de-15-minutos-cómo-puede-el-desarrollador-cumplir-con-estos-requisitos) |
| 37 | [Una empresa está desarrollando un reporte ejecutado por AWS Step Functions; Amazon CloudWatch muestra errores en la máquina de estados de tareas de Step Functions. Para solucionar los problemas de cada tarea, la entrada del estado debe incluirse junto con el mensaje de error en la salida del estado. ¿Qué práctica de codificación puede conservar tanto la entrada original como el error para el estado?](#una-empresa-está-desarrollando-un-reporte-ejecutado-por-aws-step-functions-amazon-cloudwatch-muestra-errores-en-la-máquina-de-estados-de-tareas-de-step-functions-para-solucionar-los-problemas-de-cada-tarea-la-entrada-del-estado-debe-incluirse-junto-con-el-mensaje-de-error-en-la-salida-del-estado-qué-práctica-de-codificación-puede-conservar-tanto-la-entrada-original-como-el-error-para-el-estado) |
| 38 | [Un desarrollador ha creado una aplicación de mercado que almacena datos de precios en Amazon DynamoDB con Amazon ElastiCache al frente. Los precios de los artículos en el mercado cambian con frecuencia. Los vendedores han comenzado a quejarse de que, después de actualizar el precio de un artículo, el precio en realidad no cambia en el listado del producto. ¿Qué podría estar causando este problema?](#un-desarrollador-ha-creado-una-aplicación-de-mercado-que-almacena-datos-de-precios-en-amazon-dynamodb-con-amazon-elasticache-al-frente-los-precios-de-los-artículos-en-el-mercado-cambian-con-frecuencia-los-vendedores-han-comenzado-a-quejarse-de-que-después-de-actualizar-el-precio-de-un-artículo-el-precio-en-realidad-no-cambia-en-el-listado-del-producto-qué-podría-estar-causando-este-problema) |
| 39 | [La flota de instancias de Amazon EC2 de una empresa recibe datos de millones de usuarios a través de una API. Los servidores agrupan los datos por lotes, agregan un objeto por cada usuario y cargan los objetos en un bucket de S3 para garantizar altas tasas de acceso. Los atributos del objeto son `Customer ID`, `Server ID`, `TS-Server` (`TimeStamp` y `Server ID`), el tamaño del objeto y una marca de tiempo. Un desarrollador quiere encontrar todos los objetos de un usuario determinado recopilados durante un intervalo de tiempo específico. Después de crear un evento de creación de objeto de S3, ¿cómo puede el desarrollador cumplir con este requisito?](#la-flota-de-instancias-de-amazon-ec2-de-una-empresa-recibe-datos-de-millones-de-usuarios-a-través-de-una-api-los-servidores-agrupan-los-datos-por-lotes-agregan-un-objeto-por-cada-usuario-y-cargan-los-objetos-en-un-bucket-de-s3-para-garantizar-altas-tasas-de-acceso-los-atributos-del-objeto-son-customer-id-server-id-ts-server-timestamp-y-server-id-el-tamaño-del-objeto-y-una-marca-de-tiempo-un-desarrollador-quiere-encontrar-todos-los-objetos-de-un-usuario-determinado-recopilados-durante-un-intervalo-de-tiempo-específico-después-de-crear-un-evento-de-creación-de-objeto-de-s3-cómo-puede-el-desarrollador-cumplir-con-este-requisito) |
| 40 | [Una empresa administra una base de datos NoSQL local (on-premises) que aloja un componente crítico de una aplicación y que está comenzando a tener problemas de escalado. La empresa quiere migrar la aplicación a Amazon DynamoDB con las siguientes consideraciones: optimizar las consultas frecuentes, reducir las latencias de lectura y planificar consultas frecuentes sobre ciertos atributos clave de la tabla. ¿Qué solución ayudaría a lograr estos objetivos?](#una-empresa-administra-una-base-de-datos-nosql-local-on-premises-que-aloja-un-componente-crítico-de-una-aplicación-y-que-está-comenzando-a-tener-problemas-de-escalado-la-empresa-quiere-migrar-la-aplicación-a-amazon-dynamodb-con-las-siguientes-consideraciones-optimizar-las-consultas-frecuentes-reducir-las-latencias-de-lectura-y-planificar-consultas-frecuentes-sobre-ciertos-atributos-clave-de-la-tabla-qué-solución-ayudaría-a-lograr-estos-objetivos) |
| 41 | [Un desarrollador está escribiendo una aplicación que procesará datos entregados en un bucket de Amazon S3. Los datos se entregan aproximadamente 10 veces al día, y el desarrollador espera que los datos se procesen en menos de 1 minuto, en promedio. ¿Cómo puede el desarrollador desplegar e invocar la aplicación con el menor costo y la menor latencia?](#un-desarrollador-está-escribiendo-una-aplicación-que-procesará-datos-entregados-en-un-bucket-de-amazon-s3-los-datos-se-entregan-aproximadamente-10-veces-al-día-y-el-desarrollador-espera-que-los-datos-se-procesen-en-menos-de-1-minuto-en-promedio-cómo-puede-el-desarrollador-desplegar-e-invocar-la-aplicación-con-el-menor-costo-y-la-menor-latencia) |
| 42 | [Un desarrollador está migrando aplicaciones existentes a AWS. Estas aplicaciones usan MongoDB como su almacén de datos principal y se desplegarán en instancias de Amazon EC2. La gerencia requiere que el desarrollador minimice los cambios en las aplicaciones mientras usa servicios de AWS. ¿Qué solución debería usar el desarrollador para alojar MongoDB en AWS?](#un-desarrollador-está-migrando-aplicaciones-existentes-a-aws-estas-aplicaciones-usan-mongodb-como-su-almacén-de-datos-principal-y-se-desplegarán-en-instancias-de-amazon-ec2-la-gerencia-requiere-que-el-desarrollador-minimice-los-cambios-en-las-aplicaciones-mientras-usa-servicios-de-aws-qué-solución-debería-usar-el-desarrollador-para-alojar-mongodb-en-aws) |
| 43 | [Un desarrollador está escribiendo una aplicación que se ejecuta en instancias de Amazon EC2 en un Auto Scaling group. Los datos de la aplicación se almacenan en una tabla de Amazon DynamoDB y todas las instancias actualizan constantemente los registros. En ocasiones, una instancia recupera datos antiguos. El desarrollador quiere corregir esto asegurándose de que las lecturas sean fuertemente consistentes. ¿Cómo puede el desarrollador lograrlo?](#un-desarrollador-está-escribiendo-una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-en-un-auto-scaling-group-los-datos-de-la-aplicación-se-almacenan-en-una-tabla-de-amazon-dynamodb-y-todas-las-instancias-actualizan-constantemente-los-registros-en-ocasiones-una-instancia-recupera-datos-antiguos-el-desarrollador-quiere-corregir-esto-asegurándose-de-que-las-lecturas-sean-fuertemente-consistentes-cómo-puede-el-desarrollador-lograrlo) |
| 44 | [Un desarrollador tiene una aplicación que debe aceptar una gran cantidad de flujos de datos entrantes y procesar los datos antes de enviarlos a muchos usuarios posteriores (downstream). ¿Qué solución sin servidor debería usar el desarrollador para cumplir estos requisitos?](#un-desarrollador-tiene-una-aplicación-que-debe-aceptar-una-gran-cantidad-de-flujos-de-datos-entrantes-y-procesar-los-datos-antes-de-enviarlos-a-muchos-usuarios-posteriores-downstream-qué-solución-sin-servidor-debería-usar-el-desarrollador-para-cumplir-estos-requisitos) |
| 45 | [Un desarrollador tiene una tabla de Amazon DynamoDB que debe estar en modo aprovisionado (provisioned) para cumplir con los requisitos del usuario. La aplicación necesita admitir lo siguiente: tamaño promedio de ítem: 10 KB. Lecturas de ítems por segundo: 10 fuertemente consistentes. Escrituras de ítems por segundo: 2 transaccionales. ¿Qué capacidad de lectura y escritura cumple estos requisitos de forma rentable?](#un-desarrollador-tiene-una-tabla-de-amazon-dynamodb-que-debe-estar-en-modo-aprovisionado-provisioned-para-cumplir-con-los-requisitos-del-usuario-la-aplicación-necesita-admitir-lo-siguiente-tamaño-promedio-de-ítem-10-kb-lecturas-de-ítems-por-segundo-10-fuertemente-consistentes-escrituras-de-ítems-por-segundo-2-transaccionales-qué-capacidad-de-lectura-y-escritura-cumple-estos-requisitos-de-forma-rentable) |
| 46 | [Una empresa quiere contenerizar una aplicación web existente de tres capas y desplegarla en Amazon ECS Fargate. La aplicación usa datos de sesión para llevar el seguimiento de las actividades de los usuarios. ¿Qué enfoque proporcionaría la MEJOR experiencia de usuario?](#una-empresa-quiere-contenerizar-una-aplicación-web-existente-de-tres-capas-y-desplegarla-en-amazon-ecs-fargate-la-aplicación-usa-datos-de-sesión-para-llevar-el-seguimiento-de-las-actividades-de-los-usuarios-qué-enfoque-proporcionaría-la-mejor-experiencia-de-usuario) |
| 47 | [Una aplicación tiene los siguientes requisitos: eficiencia de rendimiento de segundos con hasta un minuto de latencia. El tamaño de almacenamiento de datos puede crecer hasta miles de terabytes. El tamaño por mensaje puede variar entre 100 KB y 100 MB. Los datos pueden almacenarse como almacenes clave/valor que admitan consistencia eventual. ¿Cuál es el servicio de AWS MÁS rentable para cumplir estos requisitos?](#una-aplicación-tiene-los-siguientes-requisitos-eficiencia-de-rendimiento-de-segundos-con-hasta-un-minuto-de-latencia-el-tamaño-de-almacenamiento-de-datos-puede-crecer-hasta-miles-de-terabytes-el-tamaño-por-mensaje-puede-variar-entre-100-kb-y-100-mb-los-datos-pueden-almacenarse-como-almacenes-clavevalor-que-admitan-consistencia-eventual-cuál-es-el-servicio-de-aws-más-rentable-para-cumplir-estos-requisitos) |
| 48 | [Un desarrollador ha descubierto que una aplicación responsable de procesar mensajes de una cola de Amazon SQS se está retrasando de forma rutinaria. La aplicación es capaz de procesar varios mensajes en una ejecución, pero solo recibe un mensaje a la vez. ¿Qué debería hacer el desarrollador para aumentar el número de mensajes que recibe la aplicación?](#un-desarrollador-ha-descubierto-que-una-aplicación-responsable-de-procesar-mensajes-de-una-cola-de-amazon-sqs-se-está-retrasando-de-forma-rutinaria-la-aplicación-es-capaz-de-procesar-varios-mensajes-en-una-ejecución-pero-solo-recibe-un-mensaje-a-la-vez-qué-debería-hacer-el-desarrollador-para-aumentar-el-número-de-mensajes-que-recibe-la-aplicación) |
| 49 | [Una empresa ofrece APIs como servicio y se compromete con un acuerdo de nivel de servicio (SLA) con todos sus usuarios. Para cumplir con cada SLA, ¿qué debería hacer la empresa?](#una-empresa-ofrece-apis-como-servicio-y-se-compromete-con-un-acuerdo-de-nivel-de-servicio-sla-con-todos-sus-usuarios-para-cumplir-con-cada-sla-qué-debería-hacer-la-empresa) |
| 50 | [Un desarrollador está creando una aplicación sin servidor con AWS Lambda y debe crear una API REST que use un método HTTP GET. ¿Qué se debe definir para cumplir este requisito? (Elija DOS)](#un-desarrollador-está-creando-una-aplicación-sin-servidor-con-aws-lambda-y-debe-crear-una-api-rest-que-use-un-método-http-get-qué-se-debe-definir-para-cumplir-este-requisito-elija-dos) |
| 51 | [Un desarrollador está migrando una aplicación local (on-premises) a AWS. Actualmente la aplicación recibe cargas de los usuarios y las guarda en un directorio local del servidor. Todas las cargas deben guardarse y estar disponibles de inmediato para todas las instancias de un Auto Scaling group. ¿Qué enfoque cumplirá estos requisitos?](#un-desarrollador-está-migrando-una-aplicación-local-on-premises-a-aws-actualmente-la-aplicación-recibe-cargas-de-los-usuarios-y-las-guarda-en-un-directorio-local-del-servidor-todas-las-cargas-deben-guardarse-y-estar-disponibles-de-inmediato-para-todas-las-instancias-de-un-auto-scaling-group-qué-enfoque-cumplirá-estos-requisitos) |
| 52 | [Un desarrollador implementó un sitio web estático alojado en Amazon S3 que realiza solicitudes a servicios web alojados en Amazon API Gateway y AWS Lambda. El sitio muestra un error que dice: `No Access-Control-Allow-Origin` header is present on the requested resource. Origin `null` is therefore not allowed access.' ¿Qué debería hacer el desarrollador para resolver este problema?](#un-desarrollador-implementó-un-sitio-web-estático-alojado-en-amazon-s3-que-realiza-solicitudes-a-servicios-web-alojados-en-amazon-api-gateway-y-aws-lambda-el-sitio-muestra-un-error-que-dice-no-access-control-allow-origin-header-is-present-on-the-requested-resource-origin-null-is-therefore-not-allowed-access-qué-debería-hacer-el-desarrollador-para-resolver-este-problema) |
| 53 | [Un Developer migró una aplicación web a AWS. Como parte de la migración, el Developer implementó un proceso automatizado de integración continua/mejora continua (CI/CD) mediante un despliegue blue/green. El despliegue aprovisiona nuevas instancias de Amazon EC2 en un Auto Scaling group detrás de un nuevo Application Load Balancer. Una vez completada la migración, el Developer comenzó a recibir quejas de usuarios que eran expulsados del sistema. Además, el sistema requiere que los usuarios inicien sesión después de cada nuevo despliegue. ¿Cómo se pueden resolver estos problemas?](#un-developer-migró-una-aplicación-web-a-aws-como-parte-de-la-migración-el-developer-implementó-un-proceso-automatizado-de-integración-continuamejora-continua-cicd-mediante-un-despliegue-bluegreen-el-despliegue-aprovisiona-nuevas-instancias-de-amazon-ec2-en-un-auto-scaling-group-detrás-de-un-nuevo-application-load-balancer-una-vez-completada-la-migración-el-developer-comenzó-a-recibir-quejas-de-usuarios-que-eran-expulsados-del-sistema-además-el-sistema-requiere-que-los-usuarios-inicien-sesión-después-de-cada-nuevo-despliegue-cómo-se-pueden-resolver-estos-problemas) |
| 54 | [Un Developer quiere insertar un registro en una tabla de Amazon DynamoDB en cuanto se agregue un nuevo archivo a un bucket de Amazon S3. ¿Qué conjunto de pasos sería necesario para lograrlo?](#un-developer-quiere-insertar-un-registro-en-una-tabla-de-amazon-dynamodb-en-cuanto-se-agregue-un-nuevo-archivo-a-un-bucket-de-amazon-s3-qué-conjunto-de-pasos-sería-necesario-para-lograrlo) |
| 55 | [Una aplicación ingiere una gran cantidad de mensajes pequeños y los almacena en una base de datos. La aplicación usa AWS Lambda. Un equipo de desarrollo está realizando cambios en la lógica de procesamiento de la aplicación. En las pruebas, procesar cada mensaje toma más de 15 minutos. Al equipo le preocupa que el backend actual pueda agotar el tiempo de espera. ¿Qué cambios se deben hacer en el sistema backend para asegurar que cada mensaje se procese de la forma MÁS escalable?](#una-aplicación-ingiere-una-gran-cantidad-de-mensajes-pequeños-y-los-almacena-en-una-base-de-datos-la-aplicación-usa-aws-lambda-un-equipo-de-desarrollo-está-realizando-cambios-en-la-lógica-de-procesamiento-de-la-aplicación-en-las-pruebas-procesar-cada-mensaje-toma-más-de-15-minutos-al-equipo-le-preocupa-que-el-backend-actual-pueda-agotar-el-tiempo-de-espera-qué-cambios-se-deben-hacer-en-el-sistema-backend-para-asegurar-que-cada-mensaje-se-procese-de-la-forma-más-escalable) |
| 56 | [Un Developer está escribiendo una aplicación que se ejecutará en instancias de Amazon EC2 en un Auto Scaling group. El Developer quiere externalizar el estado de sesión para dar soporte a la aplicación. ¿Qué servicios cumplirán estas necesidades? (Elija DOS)](#un-developer-está-escribiendo-una-aplicación-que-se-ejecutará-en-instancias-de-amazon-ec2-en-un-auto-scaling-group-el-developer-quiere-externalizar-el-estado-de-sesión-para-dar-soporte-a-la-aplicación-qué-servicios-cumplirán-estas-necesidades-elija-dos) |
| 57 | [Una empresa está desarrollando una aplicación web que permite a sus empleados cargar una foto de perfil a un bucket privado de Amazon S3. No hay límite de tamaño para las fotos de perfil, que deben mostrarse cada vez que un empleado inicia sesión. Por razones de seguridad, las fotos no pueden ser de acceso público. ¿Cuál es una solución viable a largo plazo para este escenario?](#una-empresa-está-desarrollando-una-aplicación-web-que-permite-a-sus-empleados-cargar-una-foto-de-perfil-a-un-bucket-privado-de-amazon-s3-no-hay-límite-de-tamaño-para-las-fotos-de-perfil-que-deben-mostrarse-cada-vez-que-un-empleado-inicia-sesión-por-razones-de-seguridad-las-fotos-no-pueden-ser-de-acceso-público-cuál-es-una-solución-viable-a-largo-plazo-para-este-escenario) |
| 58 | [Una empresa tiene una aplicación heredada que fue migrada a una flota de instancias de Amazon EC2. La aplicación almacena datos en una base de datos MySQL que actualmente está instalada en una única instancia de EC2. La empresa ha decidido migrar la base de datos de la instancia de EC2 a MySQL en Amazon RDS. ¿Qué debe hacer el Developer para actualizar la aplicación de modo que soporte el almacenamiento de datos en Amazon RDS?](#una-empresa-tiene-una-aplicación-heredada-que-fue-migrada-a-una-flota-de-instancias-de-amazon-ec2-la-aplicación-almacena-datos-en-una-base-de-datos-mysql-que-actualmente-está-instalada-en-una-única-instancia-de-ec2-la-empresa-ha-decidido-migrar-la-base-de-datos-de-la-instancia-de-ec2-a-mysql-en-amazon-rds-qué-debe-hacer-el-developer-para-actualizar-la-aplicación-de-modo-que-soporte-el-almacenamiento-de-datos-en-amazon-rds) |
| 59 | [Una empresa quiere implementar autenticación para su nuevo servicio REST usando Amazon API Gateway. Para autenticar las llamadas, cada solicitud debe incluir encabezados HTTP con un ID de cliente y un ID de usuario. Estas credenciales deben compararse con los datos de autenticación de una tabla de Amazon DynamoDB. ¿Qué DEBE hacer la empresa para implementar esta autenticación en API Gateway?](#una-empresa-quiere-implementar-autenticación-para-su-nuevo-servicio-rest-usando-amazon-api-gateway-para-autenticar-las-llamadas-cada-solicitud-debe-incluir-encabezados-http-con-un-id-de-cliente-y-un-id-de-usuario-estas-credenciales-deben-compararse-con-los-datos-de-autenticación-de-una-tabla-de-amazon-dynamodb-qué-debe-hacer-la-empresa-para-implementar-esta-autenticación-en-api-gateway) |
| 60 | [Al desarrollar una función de AWS Lambda que procesa Amazon Kinesis Data Streams, los administradores de la empresa deben recibir una notificación que incluya los datos procesados. ¿Cómo debe escribir el Desarrollador la función para enviar los datos procesados a los administradores?](#al-desarrollar-una-función-de-aws-lambda-que-procesa-amazon-kinesis-data-streams-los-administradores-de-la-empresa-deben-recibir-una-notificación-que-incluya-los-datos-procesados-cómo-debe-escribir-el-desarrollador-la-función-para-enviar-los-datos-procesados-a-los-administradores) |
| 61 | [¿Qué operación de elementos permite la recuperación de múltiples elementos de una tabla de DynamoDB en una sola llamada a la API?](#qué-operación-de-elementos-permite-la-recuperación-de-múltiples-elementos-de-una-tabla-de-dynamodb-en-una-sola-llamada-a-la-api) |
| 62 | [Usted intenta almacenar un objeto en la región `US-STANDARD` de Amazon S3 y recibe una confirmación de que se almacenó correctamente. Luego realiza inmediatamente otra llamada a la API e intenta leer este objeto. S3 le indica que el objeto no existe. ¿Qué podría explicar este comportamiento?](#usted-intenta-almacenar-un-objeto-en-la-región-us-standard-de-amazon-s3-y-recibe-una-confirmación-de-que-se-almacenó-correctamente-luego-realiza-inmediatamente-otra-llamada-a-la-api-e-intenta-leer-este-objeto-s3-le-indica-que-el-objeto-no-existe-qué-podría-explicar-este-comportamiento) |
| 63 | [¿Cuál es el número máximo de buckets de S3 disponibles por cuenta de AWS?](#cuál-es-el-número-máximo-de-buckets-de-s3-disponibles-por-cuenta-de-aws) |
| 64 | [Si un mensaje se recupera de una cola en Amazon SQS, ¿durante cuánto tiempo permanece inaccesible para otros usuarios por defecto?](#si-un-mensaje-se-recupera-de-una-cola-en-amazon-sqs-durante-cuánto-tiempo-permanece-inaccesible-para-otros-usuarios-por-defecto) |
| 65 | [¿Cuál es el formato de los mensajes de notificación estructurados enviados por Amazon SNS?](#cuál-es-el-formato-de-los-mensajes-de-notificación-estructurados-enviados-por-amazon-sns) |
| 66 | [¿Cuáles de los siguientes son argumentos válidos para una solicitud Publish de SNS? (Elija TRES)](#cuáles-de-los-siguientes-son-argumentos-válidos-para-una-solicitud-publish-de-sns-elija-tres) |
| 67 | [¿Cómo puede un software determinar las direcciones IP públicas y privadas de la instancia de Amazon EC2 en la que se está ejecutando?](#cómo-puede-un-software-determinar-las-direcciones-ip-públicas-y-privadas-de-la-instancia-de-amazon-ec2-en-la-que-se-está-ejecutando) |
| 68 | [¿Qué llamada a la API de EC2 usaría para recuperar una lista de Amazon Machine Images (AMIs)?](#qué-llamada-a-la-api-de-ec2-usaría-para-recuperar-una-lista-de-amazon-machine-images-amis) |
| 69 | [¿Cuál de las siguientes se elige como la región predeterminada al realizar una llamada a la API con un AWS SDK?](#cuál-de-las-siguientes-se-elige-como-la-región-predeterminada-al-realizar-una-llamada-a-la-api-con-un-aws-sdk) |
| 70 | [¿Cuáles de las siguientes afirmaciones sobre SWF son verdaderas? (Elija TRES)](#cuáles-de-las-siguientes-afirmaciones-sobre-swf-son-verdaderas-elija-tres) |
| 71 | [¿Cuáles de los siguientes son transportes de entrega válidos de SNS? (Elija DOS)](#cuáles-de-los-siguientes-son-transportes-de-entrega-válidos-de-sns-elija-dos) |
| 72 | [La Empresa C ha lanzado recientemente un sitio de comercio en línea de bicicletas en AWS. Tienen una tabla de DynamoDB `Product` que almacena los detalles de cada bicicleta, como fabricante, color, precio, cantidad y talla, para mostrarlos en la tienda en línea. Debido a la demanda de los clientes, quieren incluir una imagen de cada bicicleta junto con los detalles existentes. ¿Cuál de los siguientes enfoques provoca el menor impacto en el throughput aprovisionado de la tabla `Product`?](#la-empresa-c-ha-lanzado-recientemente-un-sitio-de-comercio-en-línea-de-bicicletas-en-aws-tienen-una-tabla-de-dynamodb-product-que-almacena-los-detalles-de-cada-bicicleta-como-fabricante-color-precio-cantidad-y-talla-para-mostrarlos-en-la-tienda-en-línea-debido-a-la-demanda-de-los-clientes-quieren-incluir-una-imagen-de-cada-bicicleta-junto-con-los-detalles-existentes-cuál-de-los-siguientes-enfoques-provoca-el-menor-impacto-en-el-throughput-aprovisionado-de-la-tabla-product) |
| 73 | [¿Qué límites de DynamoDB pueden aumentarse contactando al soporte de AWS? (Elija DOS)](#qué-límites-de-dynamodb-pueden-aumentarse-contactando-al-soporte-de-aws-elija-dos) |
| 74 | [Cuando un mensaje de Simple Queue Service desencadena una tarea que tarda 5 minutos en completarse, ¿cuál de los siguientes procesos dará como resultado el procesamiento exitoso del mensaje y su eliminación de la cola, minimizando al mismo tiempo las posibilidades de procesamiento duplicado?](#cuando-un-mensaje-de-simple-queue-service-desencadena-una-tarea-que-tarda-5-minutos-en-completarse-cuál-de-los-siguientes-procesos-dará-como-resultado-el-procesamiento-exitoso-del-mensaje-y-su-eliminación-de-la-cola-minimizando-al-mismo-tiempo-las-posibilidades-de-procesamiento-duplicado) |
| 75 | [La Empresa A tiene un bucket de S3 con contenido premium que pretende poner a disposición únicamente de los suscriptores de pago de su sitio web. Actualmente el bucket de S3 tiene permisos predeterminados en los que todos los objetos son privados, para evitar la exposición inadvertida del contenido premium a visitantes que no pagan. ¿Cómo puede la Empresa A permitir que solo los suscriptores de pago descarguen un archivo de contenido premium del bucket de S3?](#la-empresa-a-tiene-un-bucket-de-s3-con-contenido-premium-que-pretende-poner-a-disposición-únicamente-de-los-suscriptores-de-pago-de-su-sitio-web-actualmente-el-bucket-de-s3-tiene-permisos-predeterminados-en-los-que-todos-los-objetos-son-privados-para-evitar-la-exposición-inadvertida-del-contenido-premium-a-visitantes-que-no-pagan-cómo-puede-la-empresa-a-permitir-que-solo-los-suscriptores-de-pago-descarguen-un-archivo-de-contenido-premium-del-bucket-de-s3) |
| 76 | [¿Cuál de los siguientes es un ejemplo de un buen esquema de hash key de DynamoDB para lograr eficiencia en el throughput aprovisionado?](#cuál-de-los-siguientes-es-un-ejemplo-de-un-buen-esquema-de-hash-key-de-dynamodb-para-lograr-eficiencia-en-el-throughput-aprovisionado) |
| 77 | [Una aplicación almacena cada noche la información de nómina en DynamoDB para una gran cantidad de empleados de cientos de oficinas. Los atributos de cada elemento consisten en el nombre de la persona, el identificador de la oficina y las horas diarias acumuladas. Los gerentes ejecutan informes para rangos de nombres que trabajan en su oficina. Una consulta es: `Return all Items in this office for names starting with A through E`. ¿Qué configuración de tabla producirá el menor impacto en el throughput aprovisionado para esta consulta?](#una-aplicación-almacena-cada-noche-la-información-de-nómina-en-dynamodb-para-una-gran-cantidad-de-empleados-de-cientos-de-oficinas-los-atributos-de-cada-elemento-consisten-en-el-nombre-de-la-persona-el-identificador-de-la-oficina-y-las-horas-diarias-acumuladas-los-gerentes-ejecutan-informes-para-rangos-de-nombres-que-trabajan-en-su-oficina-una-consulta-es-return-all-items-in-this-office-for-names-starting-with-a-through-e-qué-configuración-de-tabla-producirá-el-menor-impacto-en-el-throughput-aprovisionado-para-esta-consulta) |
| 78 | [¿Cuál es una diferencia clave entre una instancia respaldada por Amazon EBS y una respaldada por instance store?](#cuál-es-una-diferencia-clave-entre-una-instancia-respaldada-por-amazon-ebs-y-una-respaldada-por-instance-store) |
| 79 | [Su aplicación intenta cargar un archivo de 6 GB a Simple Storage Service y recibe el mensaje de error `Your proposed upload exceeds the maximum allowed object size.`. ¿Cuál es una posible solución?](#su-aplicación-intenta-cargar-un-archivo-de-6-gb-a-simple-storage-service-y-recibe-el-mensaje-de-error-your-proposed-upload-exceeds-the-maximum-allowed-object-size-cuál-es-una-posible-solución) |
| 80 | [¿Cuáles de los siguientes lenguajes de programación tienen un SDK de AWS con soporte oficial? (Elija DOS)](#cuáles-de-los-siguientes-lenguajes-de-programación-tienen-un-sdk-de-aws-con-soporte-oficial-elija-dos) |
| 81 | [Un sistema meteorológico monitorea 600 sensores de temperatura, obtiene muestras de temperatura cada minuto y guarda cada muestra en una tabla de DynamoDB. Cada muestra implica escribir 1K de datos y las escrituras se distribuyen uniformemente en el tiempo. ¿Cuánto throughput de escritura se requiere para la tabla de destino?](#un-sistema-meteorológico-monitorea-600-sensores-de-temperatura-obtiene-muestras-de-temperatura-cada-minuto-y-guarda-cada-muestra-en-una-tabla-de-dynamodb-cada-muestra-implica-escribir-1k-de-datos-y-las-escrituras-se-distribuyen-uniformemente-en-el-tiempo-cuánto-throughput-de-escritura-se-requiere-para-la-tabla-de-destino) |
| 82 | [Un bucket de Amazon S3, `myawsbucket`, está configurado con hosting de sitio web en la región de Tokio. ¿Cuál es el endpoint del sitio web específico de la región?](#un-bucket-de-amazon-s3-myawsbucket-está-configurado-con-hosting-de-sitio-web-en-la-región-de-tokio-cuál-es-el-endpoint-del-sitio-web-específico-de-la-región) |
| 83 | [Usted ha escrito una aplicación que usa el servicio Elastic Load Balancing para distribuir el tráfico entre varios servidores web. Sus usuarios se quejan de que a veces se ven obligados a iniciar sesión de nuevo en medio del uso de su aplicación, después de haber iniciado sesión. Este no es un comportamiento que usted haya diseñado. ¿Cuál es una posible solución para evitar que esto ocurra?](#usted-ha-escrito-una-aplicación-que-usa-el-servicio-elastic-load-balancing-para-distribuir-el-tráfico-entre-varios-servidores-web-sus-usuarios-se-quejan-de-que-a-veces-se-ven-obligados-a-iniciar-sesión-de-nuevo-en-medio-del-uso-de-su-aplicación-después-de-haber-iniciado-sesión-este-no-es-un-comportamiento-que-usted-haya-diseñado-cuál-es-una-posible-solución-para-evitar-que-esto-ocurra) |
| 84 | [¿Qué afirmaciones sobre DynamoDB son verdaderas? (Elija DOS)](#qué-afirmaciones-sobre-dynamodb-son-verdaderas-elija-dos) |
| 85 | [Usted brinda servicios de consultoría de AWS a una empresa que desarrolla una nueva aplicación móvil que aprovechará Amazon SNS Mobile Push para las notificaciones push. Para enviar mensajes de notificación directos a dispositivos individuales, el identificador de registro o token de cada dispositivo debe registrarse en SNS; sin embargo, los desarrolladores no están seguros de la mejor manera de hacerlo. Usted les aconseja:](#usted-brinda-servicios-de-consultoría-de-aws-a-una-empresa-que-desarrolla-una-nueva-aplicación-móvil-que-aprovechará-amazon-sns-mobile-push-para-las-notificaciones-push-para-enviar-mensajes-de-notificación-directos-a-dispositivos-individuales-el-identificador-de-registro-o-token-de-cada-dispositivo-debe-registrarse-en-sns-sin-embargo-los-desarrolladores-no-están-seguros-de-la-mejor-manera-de-hacerlo-usted-les-aconseja) |
| 86 | [¿Cuál de las siguientes afirmaciones sobre SQS es verdadera?](#cuál-de-las-siguientes-afirmaciones-sobre-sqs-es-verdadera) |
| 87 | [La Empresa C actualmente aloja su sitio corporativo en un bucket de Amazon S3 con Static Website Hosting habilitado. Actualmente, cuando los visitantes van a `http://www.companyc.com` se devuelve la página `index.html`. Ahora la Empresa C desea que se devuelva una nueva página welcome.html cuando un visitante ingrese `http://www.companyc.com` en el navegador. ¿Cuáles de los siguientes pasos permitirán a la Empresa C cumplir este requisito? (Elija DOS)](#la-empresa-c-actualmente-aloja-su-sitio-corporativo-en-un-bucket-de-amazon-s3-con-static-website-hosting-habilitado-actualmente-cuando-los-visitantes-van-a-httpwwwcompanyccom-se-devuelve-la-página-indexhtml-ahora-la-empresa-c-desea-que-se-devuelva-una-nueva-página-welcomehtml-cuando-un-visitante-ingrese-httpwwwcompanyccom-en-el-navegador-cuáles-de-los-siguientes-pasos-permitirán-a-la-empresa-c-cumplir-este-requisito-elija-dos) |
| 88 | [Un desarrollador creó una nueva cuenta de AWS y debe crear una función de AWS Lambda escalable que cumpla los siguientes requisitos de ejecución concurrente: tiempo de ejecución promedio de 100 segundos y 50 solicitudes por segundo. ¿Qué paso debe realizarse antes del despliegue para evitar errores?](#un-desarrollador-creó-una-nueva-cuenta-de-aws-y-debe-crear-una-función-de-aws-lambda-escalable-que-cumpla-los-siguientes-requisitos-de-ejecución-concurrente-tiempo-de-ejecución-promedio-de-100-segundos-y-50-solicitudes-por-segundo-qué-paso-debe-realizarse-antes-del-despliegue-para-evitar-errores) |
| 89 | [Un desarrollador está construyendo una aplicación web de tres capas que debe poder manejar un mínimo de 5000 solicitudes por minuto. Los requisitos indican que la capa web debe ser completamente stateless, mientras que la aplicación mantiene el estado de sesión de los usuarios. ¿Cómo se pueden externalizar los datos de sesión manteniendo la latencia en el valor MÁS bajo posible?](#un-desarrollador-está-construyendo-una-aplicación-web-de-tres-capas-que-debe-poder-manejar-un-mínimo-de-5000-solicitudes-por-minuto-los-requisitos-indican-que-la-capa-web-debe-ser-completamente-stateless-mientras-que-la-aplicación-mantiene-el-estado-de-sesión-de-los-usuarios-cómo-se-pueden-externalizar-los-datos-de-sesión-manteniendo-la-latencia-en-el-valor-más-bajo-posible) |
| 90 | [Una empresa ejecuta un sitio web de comercio electrónico que utiliza Amazon DynamoDB, donde los precios de los artículos se actualizan dinámicamente en tiempo real. En cualquier momento, pueden ocurrir múltiples actualizaciones simultáneas de la información de precios de un producto en particular. Esto provoca que los cambios del editor original se sobrescriban sin un proceso de revisión adecuado. ¿Qué opción de escritura de DynamoDB se debe seleccionar para evitar esta sobrescritura?](#una-empresa-ejecuta-un-sitio-web-de-comercio-electrónico-que-utiliza-amazon-dynamodb-donde-los-precios-de-los-artículos-se-actualizan-dinámicamente-en-tiempo-real-en-cualquier-momento-pueden-ocurrir-múltiples-actualizaciones-simultáneas-de-la-información-de-precios-de-un-producto-en-particular-esto-provoca-que-los-cambios-del-editor-original-se-sobrescriban-sin-un-proceso-de-revisión-adecuado-qué-opción-de-escritura-de-dynamodb-se-debe-seleccionar-para-evitar-esta-sobrescritura) |
| 91 | [Se le ha pedido a un desarrollador crear una función de AWS Lambda que se active cada vez que se realicen actualizaciones en los elementos de una tabla de Amazon DynamoDB. La función ha sido creada y se han agregado los permisos apropiados al rol de ejecución de Lambda. Los streams de Amazon DynamoDB se han habilitado para la tabla, pero la función aún no se activa. ¿Qué opción permitiría que las actualizaciones de la tabla de DynamoDB activen la función de Lambda?](#se-le-ha-pedido-a-un-desarrollador-crear-una-función-de-aws-lambda-que-se-active-cada-vez-que-se-realicen-actualizaciones-en-los-elementos-de-una-tabla-de-amazon-dynamodb-la-función-ha-sido-creada-y-se-han-agregado-los-permisos-apropiados-al-rol-de-ejecución-de-lambda-los-streams-de-amazon-dynamodb-se-han-habilitado-para-la-tabla-pero-la-función-aún-no-se-activa-qué-opción-permitiría-que-las-actualizaciones-de-la-tabla-de-dynamodb-activen-la-función-de-lambda) |
| 92 | [Una empresa necesita ingerir terabytes de datos cada hora desde miles de fuentes que se entregan de forma casi continua durante todo el día. El volumen de mensajes generados varía a lo largo del día. Los mensajes deben entregarse en tiempo real para la detección de fraudes y para paneles operativos en vivo. ¿Qué enfoque cumplirá estos requisitos?](#una-empresa-necesita-ingerir-terabytes-de-datos-cada-hora-desde-miles-de-fuentes-que-se-entregan-de-forma-casi-continua-durante-todo-el-día-el-volumen-de-mensajes-generados-varía-a-lo-largo-del-día-los-mensajes-deben-entregarse-en-tiempo-real-para-la-detección-de-fraudes-y-para-paneles-operativos-en-vivo-qué-enfoque-cumplirá-estos-requisitos) |
| 93 | [Una aplicación escribe elementos en una tabla de Amazon DynamoDB. A medida que la aplicación escala a miles de instancias, las llamadas a la API de DynamoDB generan errores `ThrottlingException` ocasionales. La aplicación está codificada en un lenguaje incompatible con el AWS SDK. ¿Cómo se debe manejar el error?](#una-aplicación-escribe-elementos-en-una-tabla-de-amazon-dynamodb-a-medida-que-la-aplicación-escala-a-miles-de-instancias-las-llamadas-a-la-api-de-dynamodb-generan-errores-throttlingexception-ocasionales-la-aplicación-está-codificada-en-un-lenguaje-incompatible-con-el-aws-sdk-cómo-se-debe-manejar-el-error) |
| 94 | [Una aplicación web de comercio electrónico que comparte el estado de sesión de forma local (on-premises) se está migrando a AWS. La aplicación debe ser tolerante a fallos, altamente escalable de forma nativa, y cualquier interrupción del servicio no debe afectar la experiencia del usuario. ¿Cuál es la mejor opción para almacenar el estado de sesión?](#una-aplicación-web-de-comercio-electrónico-que-comparte-el-estado-de-sesión-de-forma-local-on-premises-se-está-migrando-a-aws-la-aplicación-debe-ser-tolerante-a-fallos-altamente-escalable-de-forma-nativa-y-cualquier-interrupción-del-servicio-no-debe-afectar-la-experiencia-del-usuario-cuál-es-la-mejor-opción-para-almacenar-el-estado-de-sesión) |
| 95 | [Un desarrollador tiene un servidor web con estado (stateful) on-premises que se está migrando a AWS. El desarrollador debe tener mayor elasticidad en el nuevo diseño. ¿Cómo debe el desarrollador refactorizar la aplicación para hacerla más elástica? (Elija DOS)](#un-desarrollador-tiene-un-servidor-web-con-estado-stateful-on-premises-que-se-está-migrando-a-aws-el-desarrollador-debe-tener-mayor-elasticidad-en-el-nuevo-diseño-cómo-debe-el-desarrollador-refactorizar-la-aplicación-para-hacerla-más-elástica-elija-dos) |
| 96 | [Una empresa está migrando una aplicación web on-premises de un solo servidor a AWS. La empresa pretende usar múltiples servidores detrás de un Elastic Load Balancer (ELB) para balancear la carga, y también almacenará los datos de sesión en memoria en el servidor web. La empresa no quiere perder esos datos de sesión si un servidor falla o queda fuera de línea, y quiere minimizar el tiempo de inactividad de los usuarios. ¿Dónde debe la empresa mover los datos de sesión para reducir de la forma MÁS efectiva el tiempo de inactividad y hacer que los datos de sesión de los usuarios sean más tolerantes a fallos?](#una-empresa-está-migrando-una-aplicación-web-on-premises-de-un-solo-servidor-a-aws-la-empresa-pretende-usar-múltiples-servidores-detrás-de-un-elastic-load-balancer-elb-para-balancear-la-carga-y-también-almacenará-los-datos-de-sesión-en-memoria-en-el-servidor-web-la-empresa-no-quiere-perder-esos-datos-de-sesión-si-un-servidor-falla-o-queda-fuera-de-línea-y-quiere-minimizar-el-tiempo-de-inactividad-de-los-usuarios-dónde-debe-la-empresa-mover-los-datos-de-sesión-para-reducir-de-la-forma-más-efectiva-el-tiempo-de-inactividad-y-hacer-que-los-datos-de-sesión-de-los-usuarios-sean-más-tolerantes-a-fallos) |
| 97 | [Un desarrollador está construyendo una aplicación móvil y necesita que cualquier actualización de los datos del perfil de usuario se envíe a todos los dispositivos que accedan a la identidad específica. El desarrollador no quiere administrar un back end para mantener los datos del perfil de usuario. ¿Cuál es la forma MÁS eficiente para que el desarrollador logre estos requisitos usando Amazon Cognito?](#un-desarrollador-está-construyendo-una-aplicación-móvil-y-necesita-que-cualquier-actualización-de-los-datos-del-perfil-de-usuario-se-envíe-a-todos-los-dispositivos-que-accedan-a-la-identidad-específica-el-desarrollador-no-quiere-administrar-un-back-end-para-mantener-los-datos-del-perfil-de-usuario-cuál-es-la-forma-más-eficiente-para-que-el-desarrollador-logre-estos-requisitos-usando-amazon-cognito) |
| 98 | [Una empresa mantiene un servicio REST que usa Amazon API Gateway y la validación de claves de API nativa de API Gateway. Recientemente la empresa lanzó una nueva página de registro que permite a los usuarios inscribirse en el servicio. La página de registro crea una nueva clave de API mediante `CreateApiKey` y envía la nueva clave al usuario. Cuando el usuario intenta llamar a la API con esta clave, recibe un error `403 Forbidden`. Los usuarios existentes no se ven afectados y aún pueden llamar a la API. ¿Qué actualizaciones de código otorgarán acceso a la API a estos nuevos usuarios?](#una-empresa-mantiene-un-servicio-rest-que-usa-amazon-api-gateway-y-la-validación-de-claves-de-api-nativa-de-api-gateway-recientemente-la-empresa-lanzó-una-nueva-página-de-registro-que-permite-a-los-usuarios-inscribirse-en-el-servicio-la-página-de-registro-crea-una-nueva-clave-de-api-mediante-createapikey-y-envía-la-nueva-clave-al-usuario-cuando-el-usuario-intenta-llamar-a-la-api-con-esta-clave-recibe-un-error-403-forbidden-los-usuarios-existentes-no-se-ven-afectados-y-aún-pueden-llamar-a-la-api-qué-actualizaciones-de-código-otorgarán-acceso-a-la-api-a-estos-nuevos-usuarios) |
| 99 | [Un trabajo por lotes nocturno carga 1 millón de registros nuevos en una tabla de DynamoDB. Los registros solo se necesitan durante una hora y la tabla debe estar vacía para el trabajo por lotes de la noche siguiente. ¿Cuál es el método MÁS eficiente y rentable para disponer de una tabla vacía?](#un-trabajo-por-lotes-nocturno-carga-1-millón-de-registros-nuevos-en-una-tabla-de-dynamodb-los-registros-solo-se-necesitan-durante-una-hora-y-la-tabla-debe-estar-vacía-para-el-trabajo-por-lotes-de-la-noche-siguiente-cuál-es-el-método-más-eficiente-y-rentable-para-disponer-de-una-tabla-vacía) |
| 100 | [Una empresa presta servicios a muchos consumidores downstream. Cada consumidor puede conectarse a uno o más servicios. Esto ha dado lugar a una arquitectura compleja que es difícil de administrar y no escala bien. La empresa necesita una única interfaz para administrar estos servicios para los consumidores. ¿Qué servicio de AWS se debe usar para refactorizar esta arquitectura?](#una-empresa-presta-servicios-a-muchos-consumidores-downstream-cada-consumidor-puede-conectarse-a-uno-o-más-servicios-esto-ha-dado-lugar-a-una-arquitectura-compleja-que-es-difícil-de-administrar-y-no-escala-bien-la-empresa-necesita-una-única-interfaz-para-administrar-estos-servicios-para-los-consumidores-qué-servicio-de-aws-se-debe-usar-para-refactorizar-esta-arquitectura) |
| 101 | [Un desarrollador está creando un sitio web sin servidor con contenido que incluye archivos HTML, imágenes, videos y JavaScript (scripts del lado del cliente). ¿Qué combinación de servicios debe usar el desarrollador para crear el sitio web?](#un-desarrollador-está-creando-un-sitio-web-sin-servidor-con-contenido-que-incluye-archivos-html-imágenes-videos-y-javascript-scripts-del-lado-del-cliente-qué-combinación-de-servicios-debe-usar-el-desarrollador-para-crear-el-sitio-web) |
| 102 | [Un equipo de desarrollo mantiene actualmente una aplicación que usa un almacén en memoria para guardar los resultados acumulados de juegos. Los resultados individuales se almacenan en una base de datos. Como parte de la migración a AWS, el equipo necesita usar escalado automático. El equipo sabe que esto producirá resultados inconsistentes. ¿Dónde debe almacenar el equipo estos resultados acumulados de juegos para permitir MEJOR resultados consistentes sin afectar el rendimiento?](#un-equipo-de-desarrollo-mantiene-actualmente-una-aplicación-que-usa-un-almacén-en-memoria-para-guardar-los-resultados-acumulados-de-juegos-los-resultados-individuales-se-almacenan-en-una-base-de-datos-como-parte-de-la-migración-a-aws-el-equipo-necesita-usar-escalado-automático-el-equipo-sabe-que-esto-producirá-resultados-inconsistentes-dónde-debe-almacenar-el-equipo-estos-resultados-acumulados-de-juegos-para-permitir-mejor-resultados-consistentes-sin-afectar-el-rendimiento) |
| 103 | [Un desarrollador debe crear una aplicación que usa Amazon DynamoDB. Los requisitos indican que los elementos almacenados en la tabla de DynamoDB tendrán un tamaño de 7 KB y que las lecturas deben ser fuertemente consistentes. La tasa máxima de lectura es de 3 elementos por segundo y la tasa máxima de escritura es de 10 elementos por segundo. ¿Cómo debe dimensionar el desarrollador la tabla de DynamoDB para cumplir estos requisitos?](#un-desarrollador-debe-crear-una-aplicación-que-usa-amazon-dynamodb-los-requisitos-indican-que-los-elementos-almacenados-en-la-tabla-de-dynamodb-tendrán-un-tamaño-de-7-kb-y-que-las-lecturas-deben-ser-fuertemente-consistentes-la-tasa-máxima-de-lectura-es-de-3-elementos-por-segundo-y-la-tasa-máxima-de-escritura-es-de-10-elementos-por-segundo-cómo-debe-dimensionar-el-desarrollador-la-tabla-de-dynamodb-para-cumplir-estos-requisitos) |
| 104 | [Una función de AWS Lambda debe leer datos de una base de datos Amazon RDS MySQL en una VPC y también alcanzar un endpoint público a través de internet para obtener datos adicionales. ¿Qué pasos se deben seguir para permitir que la función acceda tanto al recurso de RDS como al endpoint público? (Seleccione DOS)](#una-función-de-aws-lambda-debe-leer-datos-de-una-base-de-datos-amazon-rds-mysql-en-una-vpc-y-también-alcanzar-un-endpoint-público-a-través-de-internet-para-obtener-datos-adicionales-qué-pasos-se-deben-seguir-para-permitir-que-la-función-acceda-tanto-al-recurso-de-rds-como-al-endpoint-público-seleccione-dos) |
| 105 | [Un desarrollador quiere obtener una lista de elementos de un índice secundario global de una tabla de Amazon DynamoDB. ¿Qué llamada a la API de DynamoDB puede usar el desarrollador para consumir la MENOR cantidad de unidades de capacidad de lectura?](#un-desarrollador-quiere-obtener-una-lista-de-elementos-de-un-índice-secundario-global-de-una-tabla-de-amazon-dynamodb-qué-llamada-a-la-api-de-dynamodb-puede-usar-el-desarrollador-para-consumir-la-menor-cantidad-de-unidades-de-capacidad-de-lectura) |
| 106 | [Un desarrollador está diseñando un entorno tolerante a fallos donde se guardarán las sesiones de los clientes. ¿Cómo puede el desarrollador asegurarse de que no se pierda ninguna sesión si falla una instancia de Amazon EC2?](#un-desarrollador-está-diseñando-un-entorno-tolerante-a-fallos-donde-se-guardarán-las-sesiones-de-los-clientes-cómo-puede-el-desarrollador-asegurarse-de-que-no-se-pierda-ninguna-sesión-si-falla-una-instancia-de-amazon-ec2) |
| 107 | [En un movimiento hacia el uso de microservicios, el equipo de Administración de una empresa ha pedido a todos los equipos de desarrollo que construyan sus servicios de modo que las solicitudes de API dependan únicamente del almacén de datos de ese servicio. Un equipo está construyendo un servicio de Pagos que tiene su propia base de datos; el servicio necesita datos que se originan en la base de datos de Cuentas. Ambas usan Amazon DynamoDB. ¿Qué enfoque dará como resultado el método más simple, desacoplado y confiable para obtener actualizaciones casi en tiempo real desde la base de datos de Cuentas?](#en-un-movimiento-hacia-el-uso-de-microservicios-el-equipo-de-administración-de-una-empresa-ha-pedido-a-todos-los-equipos-de-desarrollo-que-construyan-sus-servicios-de-modo-que-las-solicitudes-de-api-dependan-únicamente-del-almacén-de-datos-de-ese-servicio-un-equipo-está-construyendo-un-servicio-de-pagos-que-tiene-su-propia-base-de-datos-el-servicio-necesita-datos-que-se-originan-en-la-base-de-datos-de-cuentas-ambas-usan-amazon-dynamodb-qué-enfoque-dará-como-resultado-el-método-más-simple-desacoplado-y-confiable-para-obtener-actualizaciones-casi-en-tiempo-real-desde-la-base-de-datos-de-cuentas) |
| 108 | [Un desarrollador está escribiendo una aplicación sin servidor que requiere que una función de AWS Lambda se invoque cada 10 minutos. ¿Cuál es una forma automatizada y sin servidor de activar la función?](#un-desarrollador-está-escribiendo-una-aplicación-sin-servidor-que-requiere-que-una-función-de-aws-lambda-se-invoque-cada-10-minutos-cuál-es-una-forma-automatizada-y-sin-servidor-de-activar-la-función) |
| 109 | [Una empresa está construyendo una aplicación para dar seguimiento al rendimiento de atletas usando una tabla de Amazon DynamoDB. Cada elemento de la tabla se identifica mediante una clave de partición (`user_id`) y una clave de ordenación (`sport_name`). El diseño de la tabla se muestra a continuación. (Nota: no se muestran todos los atributos de la tabla) Se le pide a un desarrollador que escriba una aplicación de tabla de posiciones para mostrar a los mejores competidores (`user_id`) según la puntuación para cada `sport_name`. ¿Qué proceso permitirá al desarrollador extraer los resultados de la tabla de DynamoDB de la manera MÁS eficiente?](#una-empresa-está-construyendo-una-aplicación-para-dar-seguimiento-al-rendimiento-de-atletas-usando-una-tabla-de-amazon-dynamodb-cada-elemento-de-la-tabla-se-identifica-mediante-una-clave-de-partición-user_id-y-una-clave-de-ordenación-sport_name-el-diseño-de-la-tabla-se-muestra-a-continuación-nota-no-se-muestran-todos-los-atributos-de-la-tabla-se-le-pide-a-un-desarrollador-que-escriba-una-aplicación-de-tabla-de-posiciones-para-mostrar-a-los-mejores-competidores-user_id-según-la-puntuación-para-cada-sport_name-qué-proceso-permitirá-al-desarrollador-extraer-los-resultados-de-la-tabla-de-dynamodb-de-la-manera-más-eficiente) |
| 110 | [¿Qué logra una cola de retraso (delay queue) de Amazon SQS?](#qué-logra-una-cola-de-retraso-delay-queue-de-amazon-sqs) |
| 111 | [Un desarrollador está usando la AWS CLI, pero al ejecutar comandos de listado sobre una gran cantidad de recursos, se agota el tiempo de espera. ¿Qué se puede hacer para evitar este tiempo de espera agotado?](#un-desarrollador-está-usando-la-aws-cli-pero-al-ejecutar-comandos-de-listado-sobre-una-gran-cantidad-de-recursos-se-agota-el-tiempo-de-espera-qué-se-puede-hacer-para-evitar-este-tiempo-de-espera-agotado) |
| 112 | [¿Dónde se puede definir PortMapping al lanzar contenedores en Amazon ECS?](#dónde-se-puede-definir-portmapping-al-lanzar-contenedores-en-amazon-ecs) |
| 113 | [Una organización almacena archivos grandes en Amazon S3 y está escribiendo una aplicación web para mostrar metadatos sobre los archivos a los usuarios finales. Según los metadatos, un usuario selecciona un objeto para descargar. La organización necesita un mecanismo para indexar los archivos y proporcionar una recuperación de los metadatos con latencia de un solo dígito en milisegundos. ¿Qué servicio de AWS se debe usar para lograrlo?](#una-organización-almacena-archivos-grandes-en-amazon-s3-y-está-escribiendo-una-aplicación-web-para-mostrar-metadatos-sobre-los-archivos-a-los-usuarios-finales-según-los-metadatos-un-usuario-selecciona-un-objeto-para-descargar-la-organización-necesita-un-mecanismo-para-indexar-los-archivos-y-proporcionar-una-recuperación-de-los-metadatos-con-latencia-de-un-solo-dígito-en-milisegundos-qué-servicio-de-aws-se-debe-usar-para-lograrlo) |
| 114 | [Una aplicación local (on-premises) realiza llamadas repetidas para almacenar archivos en Amazon S3. A medida que ha aumentado el uso de la aplicación, se están registrando errores `LimitExceeded`. ¿Qué se debe cambiar para corregir este error?](#una-aplicación-local-on-premises-realiza-llamadas-repetidas-para-almacenar-archivos-en-amazon-s3-a-medida-que-ha-aumentado-el-uso-de-la-aplicación-se-están-registrando-errores-limitexceeded-qué-se-debe-cambiar-para-corregir-este-error) |
| 115 | [Una empresa almacena en caché la información de sesión de una aplicación web en una tabla de Amazon DynamoDB. La empresa quiere una forma automatizada de eliminar los elementos antiguos de la tabla. ¿Cuál es la forma más simple de hacerlo?](#una-empresa-almacena-en-caché-la-información-de-sesión-de-una-aplicación-web-en-una-tabla-de-amazon-dynamodb-la-empresa-quiere-una-forma-automatizada-de-eliminar-los-elementos-antiguos-de-la-tabla-cuál-es-la-forma-más-simple-de-hacerlo) |
| 116 | [Se espera que una aplicación procese muchos archivos. Cada archivo tarda cuatro minutos en procesarse en cada invocación de AWS Lambda. La función Lambda no devuelve ningún dato importante. ¿Cuál es la forma más rápida de procesar todos los archivos?](#se-espera-que-una-aplicación-procese-muchos-archivos-cada-archivo-tarda-cuatro-minutos-en-procesarse-en-cada-invocación-de-aws-lambda-la-función-lambda-no-devuelve-ningún-dato-importante-cuál-es-la-forma-más-rápida-de-procesar-todos-los-archivos) |
| 117 | [Falla la carga de un objeto de 15 GB a Amazon S3. El mensaje de error dice: `Your proposed upload exceeds the maximum allowed object size.`. ¿Qué técnica permitirá al desarrollador cargar este objeto?](#falla-la-carga-de-un-objeto-de-15-gb-a-amazon-s3-el-mensaje-de-error-dice-your-proposed-upload-exceeds-the-maximum-allowed-object-size-qué-técnica-permitirá-al-desarrollador-cargar-este-objeto) |
| 118 | [Una aplicación usa Amazon DynamoDB como almacén de datos y debe poder leer 100 elementos por segundo como lecturas de consistencia fuerte. Cada elemento tiene un tamaño de 5 KB. ¿A qué valor se debe establecer el rendimiento de lectura aprovisionado de la tabla?](#una-aplicación-usa-amazon-dynamodb-como-almacén-de-datos-y-debe-poder-leer-100-elementos-por-segundo-como-lecturas-de-consistencia-fuerte-cada-elemento-tiene-un-tamaño-de-5-kb-a-qué-valor-se-debe-establecer-el-rendimiento-de-lectura-aprovisionado-de-la-tabla) |
| 119 | [Un desarrollador está creando una función de Lambda que generará y exportará un archivo. La función requiere 100 MB de almacenamiento temporal para archivos temporales durante su ejecución. Estos archivos no serán necesarios después de que la función termine. ¿Cómo puede el desarrollador manejar de la manera MÁS eficiente los archivos temporales?](#un-desarrollador-está-creando-una-función-de-lambda-que-generará-y-exportará-un-archivo-la-función-requiere-100-mb-de-almacenamiento-temporal-para-archivos-temporales-durante-su-ejecución-estos-archivos-no-serán-necesarios-después-de-que-la-función-termine-cómo-puede-el-desarrollador-manejar-de-la-manera-más-eficiente-los-archivos-temporales) |
| 120 | [Una aplicación se ejecuta en múltiples instancias EC2 detrás de un ELB. ¿Dónde es mejor escribir los datos de sesión para que puedan servirse de manera confiable a través de múltiples solicitudes?](#una-aplicación-se-ejecuta-en-múltiples-instancias-ec2-detrás-de-un-elb-dónde-es-mejor-escribir-los-datos-de-sesión-para-que-puedan-servirse-de-manera-confiable-a-través-de-múltiples-solicitudes) |
| 121 | [Una empresa está migrando de una arquitectura monolítica a una arquitectura basada en microservicios. Los desarrolladores necesitan refactorizar la aplicación para que los numerosos microservicios puedan comunicarse de forma asíncrona entre sí sin afectar el rendimiento. ¿El uso de cuáles servicios administrados de AWS permitirá el paso de mensajes asíncrono? (Elija DOS)](#una-empresa-está-migrando-de-una-arquitectura-monolítica-a-una-arquitectura-basada-en-microservicios-los-desarrolladores-necesitan-refactorizar-la-aplicación-para-que-los-numerosos-microservicios-puedan-comunicarse-de-forma-asíncrona-entre-sí-sin-afectar-el-rendimiento-el-uso-de-cuáles-servicios-administrados-de-aws-permitirá-el-paso-de-mensajes-asíncrono-elija-dos) |
| 122 | [Una aplicación necesita usar la dirección IP del cliente en su procesamiento. La aplicación se ha movido a AWS y se ha colocado detrás de un Application Load Balancer (ALB). Sin embargo, ahora todas las direcciones IP de los clientes parecen ser la misma. La aplicación debe mantener la capacidad de escalar horizontalmente. Según este escenario, ¿cuál es la solución MÁS rentable a este problema?](#una-aplicación-necesita-usar-la-dirección-ip-del-cliente-en-su-procesamiento-la-aplicación-se-ha-movido-a-aws-y-se-ha-colocado-detrás-de-un-application-load-balancer-alb-sin-embargo-ahora-todas-las-direcciones-ip-de-los-clientes-parecen-ser-la-misma-la-aplicación-debe-mantener-la-capacidad-de-escalar-horizontalmente-según-este-escenario-cuál-es-la-solución-más-rentable-a-este-problema) |
| 123 | [Una aplicación local (on-premises) está implementada usando una pila Linux, Apache, MySQL y PHP (LAMP). El desarrollador quiere ejecutar esta aplicación en AWS. ¿Cuál de los siguientes conjuntos de servicios de AWS puede usarse para ejecutar esta pila?](#una-aplicación-local-on-premises-está-implementada-usando-una-pila-linux-apache-mysql-y-php-lamp-el-desarrollador-quiere-ejecutar-esta-aplicación-en-aws-cuál-de-los-siguientes-conjuntos-de-servicios-de-aws-puede-usarse-para-ejecutar-esta-pila) |
| 124 | [Una aplicación muestra un panel de estado. El estado se actualiza mediante mensajes de 1 KB provenientes de una cola de SQS. Aunque el estado cambia con poca frecuencia, el desarrollador debe minimizar el tiempo entre la llegada del mensaje a la cola y la actualización del panel. ¿Qué técnica proporciona el menor retraso en la actualización del panel?](#una-aplicación-muestra-un-panel-de-estado-el-estado-se-actualiza-mediante-mensajes-de-1-kb-provenientes-de-una-cola-de-sqs-aunque-el-estado-cambia-con-poca-frecuencia-el-desarrollador-debe-minimizar-el-tiempo-entre-la-llegada-del-mensaje-a-la-cola-y-la-actualización-del-panel-qué-técnica-proporciona-el-menor-retraso-en-la-actualización-del-panel) |
| 125 | [Una aplicación heredada local (on-premises) almacena en caché archivos de datos localmente y escribe imágenes compartidas en discos locales. ¿Qué es necesario para permitir el escalado horizontal al migrar la aplicación a AWS?](#una-aplicación-heredada-local-on-premises-almacena-en-caché-archivos-de-datos-localmente-y-escribe-imágenes-compartidas-en-discos-locales-qué-es-necesario-para-permitir-el-escalado-horizontal-al-migrar-la-aplicación-a-aws) |
| 126 | [Un desarrollador debe activar una función de AWS Lambda basándose en la actividad del ciclo de vida de los elementos en una tabla de Amazon DynamoDB. ¿Cómo puede el desarrollador crear la solución?](#un-desarrollador-debe-activar-una-función-de-aws-lambda-basándose-en-la-actividad-del-ciclo-de-vida-de-los-elementos-en-una-tabla-de-amazon-dynamodb-cómo-puede-el-desarrollador-crear-la-solución) |
| 127 | [Después de instalar el AWS CLI, un desarrollador intenta ejecutar el comando `aws configure` pero recibe el siguiente error: `Error: aws: command not found`. ¿Cuál es la causa más probable de este error?](#después-de-instalar-el-aws-cli-un-desarrollador-intenta-ejecutar-el-comando-aws-configure-pero-recibe-el-siguiente-error-error-aws-command-not-found-cuál-es-la-causa-más-probable-de-este-error) |
| 128 | [El desarrollador de una empresa minorista debe integrar una solución de detección de fraude en la solución de procesamiento de pedidos. La solución de detección de fraude tarda entre diez y treinta minutos en verificar un pedido. En horas pico, el sitio web puede recibir cien pedidos por minuto. ¿Cuál es el método más escalable para agregar la solución de detección de fraude a la canalización de procesamiento de pedidos?](#el-desarrollador-de-una-empresa-minorista-debe-integrar-una-solución-de-detección-de-fraude-en-la-solución-de-procesamiento-de-pedidos-la-solución-de-detección-de-fraude-tarda-entre-diez-y-treinta-minutos-en-verificar-un-pedido-en-horas-pico-el-sitio-web-puede-recibir-cien-pedidos-por-minuto-cuál-es-el-método-más-escalable-para-agregar-la-solución-de-detección-de-fraude-a-la-canalización-de-procesamiento-de-pedidos) |
| 129 | [Un conjunto de APIs se expone a los clientes mediante Amazon API Gateway. Estas APIs tienen el almacenamiento en caché habilitado en API Gateway. Los clientes han solicitado una opción para invalidar esta caché para cada una de las APIs. ¿Qué acción se puede tomar para permitir que los clientes de la API invaliden la caché de la API?](#un-conjunto-de-apis-se-expone-a-los-clientes-mediante-amazon-api-gateway-estas-apis-tienen-el-almacenamiento-en-caché-habilitado-en-api-gateway-los-clientes-han-solicitado-una-opción-para-invalidar-esta-caché-para-cada-una-de-las-apis-qué-acción-se-puede-tomar-para-permitir-que-los-clientes-de-la-api-invaliden-la-caché-de-la-api) |
| 130 | [Se ha pedido a un desarrollador que construya una aplicación web de panel en tiempo real para visualizar los prefijos de clave y el tamaño de almacenamiento de los objetos en buckets de Amazon S3. Se usará Amazon DynamoDB para almacenar los metadatos de Amazon S3. ¿Cuál es el diseño óptimo y MÁS rentable para asegurar que el panel en tiempo real se mantenga actualizado con el estado de los objetos en los buckets de Amazon S3?](#se-ha-pedido-a-un-desarrollador-que-construya-una-aplicación-web-de-panel-en-tiempo-real-para-visualizar-los-prefijos-de-clave-y-el-tamaño-de-almacenamiento-de-los-objetos-en-buckets-de-amazon-s3-se-usará-amazon-dynamodb-para-almacenar-los-metadatos-de-amazon-s3-cuál-es-el-diseño-óptimo-y-más-rentable-para-asegurar-que-el-panel-en-tiempo-real-se-mantenga-actualizado-con-el-estado-de-los-objetos-en-los-buckets-de-amazon-s3) |
| 131 | [Una aplicación sin servidor existente procesa archivos de imagen cargados. El proceso actualmente usa una única función Lambda que toma un archivo de imagen, realiza el procesamiento y almacena el archivo en Amazon S3. Los usuarios de la aplicación ahora requieren la generación de miniaturas de las imágenes. Los usuarios quieren evitar cualquier impacto en el tiempo que toma realizar las cargas de imágenes. ¿Cómo se puede agregar la generación de miniaturas a la aplicación, cumpliendo los requisitos de los usuarios y minimizando los cambios al código existente?](#una-aplicación-sin-servidor-existente-procesa-archivos-de-imagen-cargados-el-proceso-actualmente-usa-una-única-función-lambda-que-toma-un-archivo-de-imagen-realiza-el-procesamiento-y-almacena-el-archivo-en-amazon-s3-los-usuarios-de-la-aplicación-ahora-requieren-la-generación-de-miniaturas-de-las-imágenes-los-usuarios-quieren-evitar-cualquier-impacto-en-el-tiempo-que-toma-realizar-las-cargas-de-imágenes-cómo-se-puede-agregar-la-generación-de-miniaturas-a-la-aplicación-cumpliendo-los-requisitos-de-los-usuarios-y-minimizando-los-cambios-al-código-existente) |
| 132 | [Un sitio web estático está alojado en un bucket de Amazon S3. Varias páginas HTML del sitio usan JavaScript para descargar imágenes desde otro bucket de Amazon S3. Estas imágenes no se muestran cuando los usuarios navegan por el sitio. ¿Cuál es la posible causa del problema?](#un-sitio-web-estático-está-alojado-en-un-bucket-de-amazon-s3-varias-páginas-html-del-sitio-usan-javascript-para-descargar-imágenes-desde-otro-bucket-de-amazon-s3-estas-imágenes-no-se-muestran-cuando-los-usuarios-navegan-por-el-sitio-cuál-es-la-posible-causa-del-problema) |

### ¿Cuáles de los siguientes servicios son almacenes clave-valor? (Elija 3 respuestas)

- [x] Amazon ElastiCache.
- [ ] Simple Notification Service.
- [x] DynamoDB.
- [ ] Simple Workflow Service.
- [x] Simple Storage Service.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador desea enviar encabezados multivalor (multi-value headers) a una función de AWS Lambda registrada como destino (target) de un Application Load Balancer (ALB). ¿Qué debe hacer el desarrollador para lograrlo?

- [ ] Colocar la función Lambda y el target group en la misma cuenta.
- [ ] Enviar el cuerpo de la solicitud a la función Lambda con un tamaño menor a 1 MB 0.
- [ ] Incluir el estado de codificación Base64, el código de estado, la descripción del estado y los encabezados en la función Lambda.
- [x] Habilitar los encabezados multivalor (multi-value headers) en el ALB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### El sitio web de comercio electrónico de una empresa experimenta picos masivos de tráfico que causan problemas de rendimiento en la base de datos de la empresa. Los usuarios reportan que acceder al sitio web toma mucho tiempo. Un desarrollador desea implementar una capa de caché con Amazon ElastiCache. El sitio web debe ser receptivo sin importar qué producto vea un usuario, y las actualizaciones de la información y los precios de los productos deben ser fuertemente consistentes. ¿Qué política de escritura en caché cumplirá con estos requisitos?

- [ ] Escribir directamente en la caché y sincronizar el backend más tarde.
- [ ] Escribir primero en el backend y esperar a que la caché expire.
- [ ] Escribir en la caché y en el backend al mismo tiempo.
- [x] Escribir primero en el backend e invalidar la caché.

**[⬆ Back to Top](#tabla-de-contenidos)**

### La Empresa D ejecuta su sitio web corporativo en Amazon S3, al que se accede desde `http://www.companyd.com`. Su equipo de marketing publicó nuevas fuentes web en un bucket de S3 separado, al que se accede mediante el endpoint de S3 `https://s3-us-west-1.amazonaws.com/cdfonts`. Al probar las nuevas fuentes web, la Empresa D notó que el navegador las está bloqueando. ¿Qué debe hacer la Empresa D para evitar que el navegador bloquee las fuentes web?

- [ ] Habilitar el versionado en el bucket cdfonts para cada fuente web.
- [ ] Crear una política en el bucket cdfonts para habilitar el acceso a todos.
- [ ] Agregar el encabezado `Content-MD5` a la solicitud de las fuentes web en el bucket cdfonts desde el sitio web.
- [x] Configurar el bucket cdfonts para permitir solicitudes de origen cruzado (cross-origin) creando una configuración de CORS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación que necesita localizar la dirección IPv4 pública de la instancia de Amazon EC2 en la que se ejecuta. ¿Cómo puede la aplicación obtener esta información?

- [x] Obtener los metadatos de la instancia consultando `http://169.254.169.254/latest/metadata/`.
- [ ] Obtener los datos de usuario de la instancia consultando `http://169.254.169.254/latest/userdata/`.
- [ ] Hacer que la aplicación ejecute `IFCONFIG` para obtener la dirección IP pública.
- [ ] Hacer que la aplicación ejecute `IPCONFIG` para obtener la dirección IP pública.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita modificar la arquitectura de una aplicación para cumplir con nuevos requisitos funcionales. Los datos de la aplicación se almacenan en Amazon DynamoDB y se procesan para su análisis en un lote nocturno. Los analistas del sistema no quieren esperar hasta el día siguiente para ver los datos procesados y han solicitado que estén disponibles casi en tiempo real. ¿Qué patrón de arquitectura de aplicación permitiría que los datos se procesen a medida que se reciben?

- [x] Dirigido por eventos (Event driven).
- [ ] Dirigido por el cliente (Client served driven).
- [ ] Dirigido por abanico (Fan-out driven).
- [ ] Dirigido por programación (Schedule driven).

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación utiliza Amazon Kinesis Data Streams para ingerir y procesar grandes flujos de registros de datos en tiempo real. Las instancias de Amazon EC2 consumen y procesan los datos de los shards del flujo de datos de Kinesis mediante Amazon Kinesis Client Library (KCL). La aplicación maneja los escenarios de falla y no requiere workers en espera. La aplicación reporta que un shard específico está recibiendo más datos de lo esperado. Para adaptarse a los cambios en la tasa de flujo de datos, se realiza un resharding del shard `hot`. Suponiendo que el número inicial de shards en el flujo de datos de Kinesis es 4 y que después del resharding el número de shards aumentó a 6, ¿cuál es el número máximo de instancias EC2 que se pueden implementar para procesar los datos de todos los shards?

- [ ] 12.
- [x] 6.
- [ ] 4.
- [ ] 1.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa de videojuegos está desarrollando una aplicación de juego móvil para las plataformas iOS® y Android®. Este juego móvil almacena de forma segura los datos del usuario localmente en el dispositivo. La empresa desea permitir que los usuarios utilicen varios dispositivos para el juego, lo que requiere la sincronización de los datos del usuario entre dispositivos. ¿Qué servicio se debe utilizar para sincronizar los datos del usuario entre dispositivos sin necesidad de crear una aplicación backend?

- [ ] AWS Lambda.
- [ ] Amazon S3.
- [ ] Amazon DynamoDB.
- [x] Amazon Cognito.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo un servicio REST que agregará elementos a una lista de compras. El servicio está construido sobre Amazon API Gateway con integraciones de AWS Lambda. Los elementos de la lista de compras se envían como parámetros de cadena de consulta (query string) en la solicitud del método. ¿Cómo debe el desarrollador convertir los parámetros de cadena de consulta en argumentos para la función Lambda?

- [ ] Habilitar la validación de solicitudes.
- [ ] Incluir el Amazon Resource Name (ARN) de la función Lambda.
- [ ] Cambiar el tipo de integración.
- [x] Crear una plantilla de mapeo (mapping template).

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cómo se ve afectado el rendimiento aprovisionado (provisioned throughput) por el modelo de consistencia elegido al leer datos de una tabla de DynamoDB?

- [ ] Las lecturas fuertemente consistentes usan la misma cantidad de rendimiento que las lecturas eventualmente consistentes.
- [x] Las lecturas fuertemente consistentes usan más rendimiento que las lecturas eventualmente consistentes.
- [ ] Las lecturas fuertemente consistentes usan menos rendimiento que las lecturas eventualmente consistentes.
- [ ] Las lecturas fuertemente consistentes usan un rendimiento variable según la actividad de lectura.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un proveedor está escribiendo una nueva API RESTful para que los clientes consulten el estado de los pedidos. Los clientes solicitaron el siguiente endpoint de API `http://www.supplierdomain.com/status/customerID`. ¿Cuáles de los siguientes diseños de aplicación cumplen con los requisitos? (Seleccione DOS)

- [ ] Amazon SQS; Amazon SNS.
- [x] Elastic Load Balancing; Amazon EC2.
- [ ] Amazon ElastiCache; Amazon Elacticsearch Service.
- [x] Amazon API Gateway; AWS Lambda.
- [ ] Amazon S3; Amazon CloudFront.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está diseñando una función de AWS Lambda que crea archivos temporales de menos de 10 MB durante su ejecución. Los archivos temporales se accederán y modificarán varias veces durante la ejecución. El desarrollador no necesita guardar ni recuperar estos archivos en el futuro. ¿Dónde se deben almacenar los archivos temporales?

- [x] El directorio `/tmp`.
- [ ] Amazon EFS.
- [ ] Amazon EBS.
- [ ] Amazon S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está desarrollando una aplicación web de comercio electrónico sin servidor. La aplicación necesita realizar cambios coordinados de tipo todo o nada en varios elementos de la tabla de inventario de la empresa en Amazon DynamoDB. ¿Qué solución cumplirá con estos requisitos?

- [ ] Habilitar las transacciones para la tabla de DynamoDB. Usar la operación `BatchWriteItem` para actualizar los elementos.
- [x] Usar la operación `TransactWriteitems` para agrupar los cambios. Actualizar los elementos de la tabla.
- [ ] Configurar una cola FIFO mediante Amazon SQS. Agrupar los cambios en la cola. Actualizar la tabla según los cambios agrupados.
- [ ] Crear una tabla de transacciones en un clúster de base de datos de Amazon Aurora para administrar las transacciones. Escribir un proceso de backend para sincronizar la tabla de Aurora y la tabla de DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita diseñar una aplicación que se ejecuta en AWS y que se usará para consumir mensajes de Amazon SQS con tamaños que van desde 1 KB hasta 1 GB. ¿Cómo se deben administrar los mensajes de Amazon SQS?

- [ ] Usar Amazon S3 y la CLI de Amazon SQS.
- [x] Usar Amazon S3 y la Amazon SQS Extended Client Library for Java.
- [ ] Usar Amazon EBS y la CLI de Amazon SQS.
- [ ] Usar Amazon EFS y la CLI de Amazon SQS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Se le pide a un desarrollador implementar una capa de caché delante de Amazon RDS. El contenido en caché es costoso de regenerar en caso de una falla del servicio. ¿Qué implementación de las siguientes funcionaría manteniendo el máximo tiempo de actividad?

- [x] Implementar Amazon ElastiCache Redis en Cluster Mode.
- [ ] Instalar Redis en una instancia de Amazon EC2.
- [ ] Implementar Amazon ElastiCache Memcached.
- [ ] Migrar la base de datos a Amazon Redshift.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación sin servidor utiliza un API Gateway y AWS Lambda. ¿Dónde debería almacenar la función Lambda su información de sesión entre invocaciones de la función?

- [x] En una tabla de Amazon DynamoDB.
- [ ] En una cola de Amazon SQS.
- [ ] En el sistema de archivos local.
- [ ] En una tabla de sesión SQLite usando `CDSQLITE_ENABLE_SESSION`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una arquitectura actual utiliza muchas funciones Lambda que se invocan entre sí como una máquina de estados grande. La coordinación de esta máquina de estados es código personalizado heredado que se rompe con facilidad. ¿Qué servicio de AWS puede ayudar a refactorizar y administrar la máquina de estados?

- [ ] AWS Data Pipeline.
- [ ] AWS SNS con AWS SQS.
- [ ] Amazon Elastic MapReduce.
- [x] AWS Step Functions.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe volver a implementar la lógica de negocio de un sistema de cumplimiento de pedidos. La lógica de negocio tiene que realizar solicitudes a varios proveedores para decidir dónde comprar un artículo. Todo el proceso puede tardar hasta una semana en completarse. ¿Cuál es la forma MÁS eficiente y MÁS SIMPLE de implementar un sistema que cumpla con estos requisitos?

- [x] Usar AWS Step Functions para ejecutar funciones Lambda en paralelo y unir los resultados.
- [ ] Crear un AWS SQS para cada proveedor, sondear la cola desde una instancia worker y unir los resultados.
- [ ] Usar AWS Lambda para invocar de forma asíncrona una función Lambda por cada proveedor y unir los resultados.
- [ ] Usar Amazon CloudWatch Events para orquestar las funciones Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación móvil almacena publicaciones de blog en una tabla de Amazon DynamoDB. Se agregan millones de publicaciones cada día y cada publicación representa un único elemento de la tabla. La aplicación móvil solo requiere las publicaciones recientes. Cualquier publicación con más de 48 horas de antigüedad puede eliminarse. ¿Cuál es la forma MÁS rentable de eliminar las publicaciones con más de 48 horas de antigüedad?

- [ ] Para cada elemento, agregar un nuevo atributo de tipo `String` que tenga una marca de tiempo establecida en el momento de creación de la publicación. Crear un script para encontrar publicaciones antiguas mediante un escaneo de la tabla y eliminar las publicaciones con más de 48 horas de antigüedad usando la operación de API `BatchWriteItem`. Programar un cron job en una instancia de Amazon EC2 una vez por hora para iniciar el script.
- [ ] Para cada elemento, agregar un nuevo atributo de tipo `String` que tenga una marca de tiempo establecida en el momento de creación de la publicación. Crear un script para encontrar publicaciones antiguas mediante un escaneo de la tabla y eliminar las publicaciones con más de 48 horas de antigüedad usando la operación de API `BatchWriteItem`. Colocar el script en una imagen de contenedor. Programar una tarea de Amazon Elastic Container Service (Amazon ECS) en AWS Fargate que invoque el contenedor cada 5 minutos.
- [ ] Para cada elemento, agregar un nuevo atributo de tipo `Date` que tenga una marca de tiempo establecida 48 horas después del momento de creación de la publicación. Crear un índice secundario global (GSI) que use el nuevo atributo como clave de ordenación. Crear una función de AWS Lambda que haga referencia al GSI y elimine los elementos expirados usando la operación de API `BatchWriteItem`. Programar la función con un evento de Amazon CloudWatch cada minuto.
- [x] Para cada elemento, agregar un nuevo atributo de tipo `Number` que tenga una marca de tiempo establecida 48 horas después del momento de creación de la publicación. Configurar la tabla de DynamoDB con un TTL que haga referencia al nuevo atributo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación procesa en tiempo real millones de eventos que se reciben a través de una API. ¿Qué servicio podría utilizarse para permitir que varios consumidores procesen los datos de forma concurrente y de la manera MÁS rentable?

- [ ] Amazon SNS con fanout a una cola SQS para cada aplicación.
- [ ] Amazon SNS con fanout a una cola SQS FIFO (first-in, first-out) para cada aplicación.
- [ ] Amazon Kinesis Firehose.
- [x] Amazon Kinesis Streams.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación ingerirá datos a muy alto rendimiento desde muchas fuentes y debe almacenar los datos en un bucket de Amazon S3. ¿Qué servicio cumpliría MEJOR con esta tarea?

- [x] Amazon Kinesis Firehose.
- [ ] Amazon S3 Acceleration Transfer.
- [ ] Amazon SQS.
- [ ] Amazon SNS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un servicio heredado tiene una interfaz SOAP basada en XML. El desarrollador quiere exponer la funcionalidad del servicio a clientes externos con Amazon API Gateway. ¿Qué técnica logrará esto?

- [x] Crear una API RESTful con API Gateway; transformar el JSON entrante en un mensaje XML válido para la interfaz SOAP usando mapping templates.
- [ ] Crear una API RESTful con API Gateway; pasar el JSON entrante a la interfaz SOAP a través de un Application Load Balancer.
- [ ] Crear una API RESTful con API Gateway; pasar el XML entrante a la interfaz SOAP a través de un Application Load Balancer.
- [ ] Crear una API RESTful con API Gateway; transformar el XML entrante en un mensaje válido para la interfaz SOAP usando mapping templates.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha configurado un Amazon Kinesis Stream con 4 shards para ingerir un máximo de 2500 registros por segundo. Se ha configurado una función Lambda para procesar estos registros. ¿En qué orden se procesarán estos registros?

- [ ] Lambda recibirá cada registro en el orden inverso al que fue colocado en el stream, siguiendo un método LIFO (last-in, first-out).
- [ ] Lambda recibirá cada registro en el orden exacto en que fue colocado en el stream, siguiendo un método FIFO (first­-in, first-out).
- [x] Lambda recibirá cada registro en el orden exacto en que fue colocado en el shard, siguiendo un método FIFO (first-in, first-out). No hay garantía de orden entre shards.
- [ ] El desarrollador puede seleccionar FIFO (first-in, first-out), LIFO (last-in, last-out), aleatorio, o solicitar un registro específico usando la API getRecords.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación está diseñada para usar Amazon SQS para administrar mensajes de muchos remitentes independientes. Los mensajes de cada remitente deben procesarse en el orden en que se reciben. ¿Qué característica de SQS debe implementar el desarrollador?

- [x] Configurar cada remitente con un MessageGroupId único.
- [ ] Habilitar MessageDeduplicationIds en la cola SQS.
- [ ] Configurar cada mensaje con MessageGroupIds únicos.
- [ ] Habilitar ContentBasedDeduplication en la cola SQS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está trabajando en una aplicación que registra cientos de millones de reseñas de productos en una tabla de Amazon DynamoDB. Los registros incluyen los elementos de datos que se muestran en la tabla. ¿Qué campo, al usarse como clave de partición, produciría el rendimiento MÁS consistente con DynamoDB?

![Question 87](images/question87.jpg)

- [ ] `starRating`.
- [x] `reviewID`.
- [ ] `comment`.
- [ ] `productID`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación tarda 40 segundos en procesar las instrucciones recibidas en un mensaje de Amazon SQS. Suponiendo que la cola de SQS está configurada con el valor predeterminado de `VisibilityTimeout`, ¿cuál es la MEJOR manera, al recibir un mensaje, de asegurar que ninguna otra instancia pueda recuperar un mensaje que ya ha sido procesado o que se está procesando actualmente?

- [x] Usar la API `ChangeMessageVisibility` para aumentar el `VisibilityTimeout` y luego usar la API `DeleteMessage` para eliminar el mensaje.
- [ ] Usar la llamada a la API `DeleteMessage` para eliminar el mensaje de la cola y luego llamar a la API `DeleteQueue` para eliminar la cola.
- [ ] Usar la API `ChangeMessageVisibility` para disminuir el valor del timeout y luego usar la API `DeleteMessage` para eliminar el mensaje.
- [ ] Usar la API `DeleteMessageVisibility` para cancelar el `VisibilityTimeout` y luego usar la API `DeleteMessage` para eliminar el mensaje.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo transacciones en una tabla de DynamoDB llamada `SystemUpdates` que tiene 5 unidades de capacidad de escritura. ¿Qué opción tiene el mayor rendimiento de lectura?

- [x] Lecturas eventualmente consistentes de 5 unidades de capacidad de lectura que leen elementos de 4 KB de tamaño.
- [ ] Lecturas fuertemente consistentes de 5 unidades de capacidad de lectura que leen elementos de 4 KB de tamaño.
- [ ] Lecturas eventualmente consistentes de 15 unidades de capacidad de lectura que leen elementos de 1 KB de tamaño.
- [ ] Lecturas fuertemente consistentes de 15 unidades de capacidad de lectura que leen elementos de 1 KB de tamaño.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación almacena imágenes en un bucket de S3. Las notificaciones de eventos de Amazon S3 se usan para activar una función Lambda que cambia el tamaño de las imágenes. Procesar cada imagen toma menos de un segundo. ¿Cómo manejará AWS Lambda el tráfico adicional?

- [x] Lambda escalará horizontalmente para ejecutar las solicitudes de forma concurrente.
- [ ] Lambda manejará las solicitudes de forma secuencial en el orden en que fueron recibidas.
- [ ] Lambda procesará múltiples imágenes en una sola ejecución.
- [ ] Lambda agregará más cómputo a cada ejecución para reducir el tiempo de procesamiento.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación sobrescribe un objeto en Amazon S3 y luego lee inmediatamente el mismo objeto. ¿Por qué la aplicación a veces recuperaría la versión anterior del objeto?

- [x] Los PUTS de sobrescritura de S3 son eventualmente consistentes, por lo que la aplicación puede leer el objeto anterior.
- [ ] La aplicación necesita agregar metadatos adicionales para etiquetar la última versión al cargar en Amazon S3.
- [ ] Todos los PUTS de S3 son eventualmente consistentes, por lo que la aplicación puede leer el objeto anterior.
- [ ] La aplicación necesita especificar explícitamente la última versión al recuperar el objeto.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está configurando Amazon API Gateway para los productos de su empresa. La API será utilizada por desarrolladores registrados para consultar y actualizar sus entornos. La empresa quiere limitar la cantidad de solicitudes que los usuarios finales pueden enviar, tanto por razones de costo como de seguridad. La dirección quiere ofrecer a los desarrolladores registrados la opción de comprar paquetes más grandes que permitan más solicitudes. ¿Cómo puede el desarrollador lograr esto con la MENOR cantidad de sobrecarga de administración?

- [ ] Habilitar el throttling para el stage de API Gateway. Establecer un valor tanto para la tasa como para la capacidad de ráfaga. Si un usuario registrado elige un paquete más grande, crear un stage para él, ajustar los valores y compartir la nueva URL con él.
- [ ] Configurar el registro de API de Amazon CloudWatch en API Gateway. Crear un filtro basado en los campos user y requestTime y crear una alarma sobre este filtro. Escribir una función de AWS Lambda para analizar los valores y la información del solicitante, y responder en consecuencia. Configurar la función como el destino de la alarma. Si un usuario registrado elige un paquete más grande, actualizar el código de Lambda con los valores.
- [ ] Habilitar las métricas de Amazon CloudWatch para el stage de API Gateway. Configurar alarmas de CloudWatch basadas en la métrica Count y las dimensiones ApiName, Method, Resource y Stage para alertar cuando las tasas de solicitudes superen el umbral. Establecer la acción de la alarma en `Deny`. Si un usuario registrado elige un paquete más grande, crear una alarma específica para el usuario y ajustar los valores.
- [x] Configurar un plan de uso predeterminado, especificar valores para la tasa y la capacidad de ráfaga y asociarlo con un stage. Si un usuario registrado elige un paquete más grande, crear un plan personalizado con los valores apropiados y asociar el plan con el usuario.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está refactorizando una aplicación monolítica. La aplicación recibe una solicitud POST y realiza varias operaciones. Algunas de las operaciones se ejecutan en paralelo, mientras que otras se ejecutan secuencialmente. Estas operaciones han sido refactorizadas en funciones individuales de AWS Lambda. La solicitud POST será procesada por Amazon API Gateway. ¿Cómo debería el desarrollador invocar las funciones Lambda en la misma secuencia usando API Gateway?

- [ ] Usar Amazon SQS para invocar las funciones Lambda.
- [ ] Usar una actividad de AWS Step Functions para ejecutar las funciones Lambda.
- [ ] Usar Amazon SNS para activar las funciones Lambda.
- [x] Usar una máquina de estados de AWS Step Functions para orquestar las funciones Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está agregando la capacidad de valor almacenado (o tarjeta de regalo) a su popular sitio web de juegos casuales. Los usuarios necesitan poder intercambiar este valor por artículos de otros usuarios en la plataforma. Esto requeriría que los registros de ambos usuarios se actualicen como una sola transacción, o que los registros de ambos usuarios se reviertan por completo. ¿Qué opciones de base de datos de AWS pueden proporcionar la capacidad transaccional requerida para esta nueva funcionalidad? (Elija DOS)

- [ ] Amazon DynamoDB con operaciones realizadas con el parámetro `ConsistentRead` establecido en `true`.
- [ ] Amazon ElastiCache for Memcached con operaciones realizadas dentro de un bloque de transacción.
- [x] Amazon Aurora MySQL con operaciones realizadas dentro de un bloque de transacción.
- [x] Amazon DynamoDB con lecturas y escrituras realizadas usando operaciones `Transact*`.
- [ ] Amazon Redshift con operaciones realizadas dentro de un bloque de transacción.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una función de AWS Lambda que genera un nuevo archivo cada vez que se ejecuta. Cada nuevo archivo debe registrarse (check in) en un repositorio de AWS CodeCommit alojado en la misma cuenta de AWS. ¿Cómo debería el desarrollador lograr esto?

- [x] Cuando la función Lambda se inicie, usar la CLI de Git para clonar el repositorio. Registrar el nuevo archivo en el repositorio clonado y hacer push del cambio.
- [ ] Después de que el nuevo archivo se cree en Lambda, usar cURL para invocar la API de CodeCommit. Enviar el archivo al repositorio.
- [ ] Usar un AWS SDK para instanciar un cliente de CodeCommit. Invocar el método `put_file` para agregar el archivo al repositorio.
- [ ] Cargar el nuevo archivo en un bucket de Amazon S3. Crear un AWS Step Function para aceptar eventos de S3. En el Step Function, agregar el nuevo archivo al repositorio.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo está trabajando en una aplicación móvil que permite a los usuarios cargar fotos en Amazon S3. El equipo espera que la aplicación sea utilizada simultáneamente por cientos de miles de usuarios durante un solo evento. Una vez cargadas las fotos, el servicio de backend las analizará y procesará para detectar contenido inapropiado. ¿Qué enfoque es la forma MÁS resiliente de lograr este objetivo y que además suaviza los picos temporales de volumen para el servicio de backend?

- [ ] Desarrollar una función de AWS Lambda que revise la carpeta de carga en el bucket de S3. Si se detectan nuevas fotos cargadas, la función Lambda las analizará y procesará.
- [x] Una vez que una foto se carga en Amazon S3, publicar el evento en una cola de Amazon SQS. Usar la cola como origen de eventos para activar una función de AWS Lambda. En la función Lambda, analizar y procesar la foto.
- [ ] Cuando el usuario carga una foto, invocar una API alojada en Amazon API Gateway. La API invocará una función de AWS Lambda para analizar y procesar la foto.
- [ ] Crear una máquina de estados en AWS Step Functions que revise la carpeta de carga en el bucket de S3. Si se detecta una nueva foto, invocar una función de AWS Lambda para analizarla y procesarla.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo quiere ejecutar sus cargas de trabajo de contenedores en Amazon ECS. Cada contenedor de aplicación necesita compartir datos con otro contenedor para recopilar logs y métricas. ¿Qué debe hacer el equipo de desarrollo para cumplir con estos requisitos?

- [ ] Crear dos especificaciones de pod. Hacer que una incluya el contenedor de la aplicación y la otra incluya el otro contenedor. Vincular los dos pods entre sí.
- [ ] Crear dos task definitions. Hacer que una incluya el contenedor de la aplicación y la otra incluya el otro contenedor. Montar un volumen compartido entre las dos tareas.
- [x] Crear una task definition. Especificar ambos contenedores en la definición. Montar un volumen compartido entre esos dos contenedores.
- [ ] Crear una única especificación de pod. Incluir ambos contenedores en la especificación. Montar un volumen persistente en ambos contenedores.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una aplicación web que debe compartir documentos seguros con los usuarios finales. Los documentos se almacenan en un bucket privado de Amazon S3. La aplicación debe permitir que solo los usuarios autenticados descarguen documentos específicos cuando se soliciten, y únicamente durante un período de 15 minutos. ¿Cómo puede el desarrollador cumplir con estos requisitos?

- [ ] Copiar los documentos a un bucket de S3 separado que tenga una política de ciclo de vida para eliminarlos después de 15 minutos.
- [x] Crear una URL prefirmada de S3 usando el AWS SDK con un tiempo de expiración de 15 minutos.
- [ ] Usar cifrado del lado del servidor con claves administradas por AWS KMS (SSE-KMS) y descargar los documentos mediante HTTPS.
- [ ] Modificar la política del bucket de S3 para permitir solo a usuarios específicos descargar los documentos. Revertir el cambio después de 15 minutos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está desarrollando un reporte ejecutado por AWS Step Functions; Amazon CloudWatch muestra errores en la máquina de estados de tareas de Step Functions. Para solucionar los problemas de cada tarea, la entrada del estado debe incluirse junto con el mensaje de error en la salida del estado. ¿Qué práctica de codificación puede conservar tanto la entrada original como el error para el estado?

- [x] Usar `ResultPath` en una instrucción `Catch` para incluir el error junto con la entrada original.
- [ ] Usar `InputPath` en una instrucción `Catch` y establecer el valor en `null`.
- [ ] Usar `Error Equals` en una instrucción `Retry` para incluir el error junto con la entrada original.
- [ ] Usar `OutputPath` en una instrucción `Retry` y establecer el valor en `$`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha creado una aplicación de mercado que almacena datos de precios en Amazon DynamoDB con Amazon ElastiCache al frente. Los precios de los artículos en el mercado cambian con frecuencia. Los vendedores han comenzado a quejarse de que, después de actualizar el precio de un artículo, el precio en realidad no cambia en el listado del producto. ¿Qué podría estar causando este problema?

- [x] La caché no se invalida cuando cambia el precio del artículo.
- [ ] El precio del artículo se obtiene usando un clúster de ElastiCache con write-through.
- [ ] La tabla de DynamoDB se aprovisionó con capacidad de lectura insuficiente.
- [ ] La tabla de DynamoDB se aprovisionó con capacidad de escritura insuficiente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### La flota de instancias de Amazon EC2 de una empresa recibe datos de millones de usuarios a través de una API. Los servidores agrupan los datos por lotes, agregan un objeto por cada usuario y cargan los objetos en un bucket de S3 para garantizar altas tasas de acceso. Los atributos del objeto son `Customer ID`, `Server ID`, `TS-Server` (`TimeStamp` y `Server ID`), el tamaño del objeto y una marca de tiempo. Un desarrollador quiere encontrar todos los objetos de un usuario determinado recopilados durante un intervalo de tiempo específico. Después de crear un evento de creación de objeto de S3, ¿cómo puede el desarrollador cumplir con este requisito?

- [ ] Ejecutar una función de AWS Lambda en respuesta a los eventos de creación de objetos de S3 que cree un registro de Amazon DynamoDB por cada objeto con el `Customer ID` como clave de partición y el `Server ID` como clave de ordenación. Recuperar todos los registros usando los atributos `Customer ID` y `Server ID`.
- [ ] Ejecutar una función de AWS Lambda en respuesta a los eventos de creación de objetos de S3 que cree un registro de Amazon Redshift por cada objeto con el `Customer ID` como clave de partición y `TS-Server` como clave de ordenación. Recuperar todos los registros usando los atributos `Customer ID` y `TS-Server`.
- [x] Ejecutar una función de AWS Lambda en respuesta a los eventos de creación de objetos de S3 que cree un registro de Amazon DynamoDB por cada objeto con el `Customer ID` como clave de partición y `TS-Server` como clave de ordenación. Recuperar todos los registros usando los atributos `Customer ID` y `TS-Server`.
- [ ] Ejecutar una función de AWS Lambda en respuesta a los eventos de creación de objetos de S3 que cree un registro de Amazon Redshift por cada objeto con el `Customer ID` como clave de partición y el `Server ID` como clave de ordenación. Recuperar todos los registros usando los atributos `Customer ID` y `Server ID`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa administra una base de datos NoSQL local (on-premises) que aloja un componente crítico de una aplicación y que está comenzando a tener problemas de escalado. La empresa quiere migrar la aplicación a Amazon DynamoDB con las siguientes consideraciones: optimizar las consultas frecuentes, reducir las latencias de lectura y planificar consultas frecuentes sobre ciertos atributos clave de la tabla. ¿Qué solución ayudaría a lograr estos objetivos?

- [x] Crear índices secundarios globales sobre las claves que se consultan con frecuencia. Agregar los atributos necesarios a los índices.
- [ ] Crear índices secundarios locales sobre las claves que se consultan con frecuencia. DynamoDB obtendrá los atributos necesarios de la tabla.
- [ ] Crear tablas globales de DynamoDB para acelerar las respuestas de las consultas. Usar un scan para obtener los datos de la tabla.
- [ ] Crear una política de AWS Auto Scaling para la tabla de DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una aplicación que procesará datos entregados en un bucket de Amazon S3. Los datos se entregan aproximadamente 10 veces al día, y el desarrollador espera que los datos se procesen en menos de 1 minuto, en promedio. ¿Cómo puede el desarrollador desplegar e invocar la aplicación con el menor costo y la menor latencia?

- [ ] Desplegar la aplicación como una función de AWS Lambda e invocarla con una alarma de Amazon CloudWatch activada por la carga de un objeto en S3.
- [x] Desplegar la aplicación como una función de AWS Lambda e invocarla con una notificación de eventos de S3.
- [ ] Desplegar la aplicación como una función de AWS Lambda e invocarla con un evento programado de Amazon CloudWatch.
- [ ] Desplegar la aplicación en una instancia de Amazon EC2 y hacer que consulte periódicamente (polling) el bucket de S3 en busca de nuevos objetos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está migrando aplicaciones existentes a AWS. Estas aplicaciones usan MongoDB como su almacén de datos principal y se desplegarán en instancias de Amazon EC2. La gerencia requiere que el desarrollador minimice los cambios en las aplicaciones mientras usa servicios de AWS. ¿Qué solución debería usar el desarrollador para alojar MongoDB en AWS?

- [ ] Instalar MongoDB en la misma instancia donde se ejecuta la aplicación.
- [x] Desplegar Amazon DocumentDB en modo de compatibilidad con MongoDB.
- [ ] Usar Amazon API Gateway para traducir las llamadas de API de MongoDB a Amazon DynamoDB.
- [ ] Replicar la carga de trabajo existente de MongoDB a Amazon DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una aplicación que se ejecuta en instancias de Amazon EC2 en un Auto Scaling group. Los datos de la aplicación se almacenan en una tabla de Amazon DynamoDB y todas las instancias actualizan constantemente los registros. En ocasiones, una instancia recupera datos antiguos. El desarrollador quiere corregir esto asegurándose de que las lecturas sean fuertemente consistentes. ¿Cómo puede el desarrollador lograrlo?

- [x] Establecer `ConsistentRead` en `true` al llamar a `GetItem`.
- [ ] Crear una nueva tabla de DynamoDB Accelerator (DAX).
- [ ] Establecer Consistency en strong al llamar a `UpdateTable`.
- [ ] Usar el comando `GetShardIterator`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador tiene una aplicación que debe aceptar una gran cantidad de flujos de datos entrantes y procesar los datos antes de enviarlos a muchos usuarios posteriores (downstream). ¿Qué solución sin servidor debería usar el desarrollador para cumplir estos requisitos?

- [ ] Un procedimiento almacenado de Amazon RDS MySQL con AWS Lambda.
- [ ] AWS Direct Connect con AWS Lambda.
- [x] Amazon Kinesis Data Streams con AWS Lambda.
- [ ] Un script bash de Amazon EC2 con AWS Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador tiene una tabla de Amazon DynamoDB que debe estar en modo aprovisionado (provisioned) para cumplir con los requisitos del usuario. La aplicación necesita admitir lo siguiente: tamaño promedio de ítem: 10 KB. Lecturas de ítems por segundo: 10 fuertemente consistentes. Escrituras de ítems por segundo: 2 transaccionales. ¿Qué capacidad de lectura y escritura cumple estos requisitos de forma rentable?

- [ ] Lectura `10`; escritura `2`.
- [x] Lectura `30`; escritura `40`.
- [ ] Usar escalado on-demand.
- [ ] Lectura `300`; escritura `400`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa quiere contenerizar una aplicación web existente de tres capas y desplegarla en Amazon ECS Fargate. La aplicación usa datos de sesión para llevar el seguimiento de las actividades de los usuarios. ¿Qué enfoque proporcionaría la MEJOR experiencia de usuario?

- [x] Aprovisionar un clúster de Redis en Amazon ElastiCache y guardar los datos de sesión en el clúster.
- [ ] Crear una tabla de sesiones en Amazon Redshift y guardar los datos de sesión en la tabla de la base de datos.
- [ ] Habilitar la persistencia de sesión (session stickiness) en el Network Load Balancer existente y administrar los datos de sesión en el contenedor.
- [ ] Usar un bucket de Amazon S3 como almacén de datos y guardar los datos de sesión en el bucket.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación tiene los siguientes requisitos: eficiencia de rendimiento de segundos con hasta un minuto de latencia. El tamaño de almacenamiento de datos puede crecer hasta miles de terabytes. El tamaño por mensaje puede variar entre 100 KB y 100 MB. Los datos pueden almacenarse como almacenes clave/valor que admitan consistencia eventual. ¿Cuál es el servicio de AWS MÁS rentable para cumplir estos requisitos?

- [x] Amazon DynamoDB.
- [ ] Amazon S3.
- [ ] Amazon RDS (con un motor MySQL).
- [ ] Amazon ElastiCache.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha descubierto que una aplicación responsable de procesar mensajes de una cola de Amazon SQS se está retrasando de forma rutinaria. La aplicación es capaz de procesar varios mensajes en una ejecución, pero solo recibe un mensaje a la vez. ¿Qué debería hacer el desarrollador para aumentar el número de mensajes que recibe la aplicación?

- [ ] Llamar a la API `ChangeMessageVisibility` de la cola y establecer `MaxNumberOfMessages` en un valor mayor que el valor predeterminado de `1`.
- [ ] Llamar a la API `AddPermission` para establecer `MaxNumberOfMessages` de la acción `ReceiveMessage` en un valor mayor que el valor predeterminado de `1`.
- [x] Llamar a la API `ReceiveMessage` para establecer `MaxNumberOfMessages` en un valor mayor que el valor predeterminado de `1`.
- [ ] Llamar a la API `SetQueueAttributes` de la cola y establecer `MaxNumberOfMessages` en un valor mayor que el valor predeterminado de `1`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ofrece APIs como servicio y se compromete con un acuerdo de nivel de servicio (SLA) con todos sus usuarios. Para cumplir con cada SLA, ¿qué debería hacer la empresa?

- [ ] Habilitar límites de limitación (throttling) para cada método en Amazon API Gateway.
- [x] Crear un usage plan para cada usuario y solicitar API keys para acceder a las APIs.
- [ ] Habilitar la limitación de tasa de la API en Amazon Cognito para cada usuario.
- [ ] Habilitar los límites de limitación (throttling) predeterminados para cada stage después de desplegar las APIs.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación sin servidor con AWS Lambda y debe crear una API REST que use un método HTTP GET. ¿Qué se debe definir para cumplir este requisito? (Elija DOS)

- [ ] Una función de Lambda@Edge.
- [x] Un Amazon API Gateway con una función de Lambda.
- [x] Un método GET expuesto en un Amazon API Gateway.
- [ ] Un método GET expuesto en la función de Lambda.
- [ ] Un método GET expuesto en Amazon Route 53.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está migrando una aplicación local (on-premises) a AWS. Actualmente la aplicación recibe cargas de los usuarios y las guarda en un directorio local del servidor. Todas las cargas deben guardarse y estar disponibles de inmediato para todas las instancias de un Auto Scaling group. ¿Qué enfoque cumplirá estos requisitos?

- [ ] Usar Amazon EBS y configurar la AMI de la aplicación para que use una instantánea de la misma instancia de EBS al arrancar.
- [x] Usar Amazon S3 y rediseñar la aplicación para que todas las cargas se coloquen en S3.
- [ ] Usar almacenamiento de instancia (instance storage) y compartirlo entre las instancias lanzadas desde la misma Amazon Machine Image (AMI).
- [ ] Usar Amazon EBS y software de sincronización de archivos para lograr consistencia eventual entre los miembros del Auto Scaling group.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador implementó un sitio web estático alojado en Amazon S3 que realiza solicitudes a servicios web alojados en Amazon API Gateway y AWS Lambda. El sitio muestra un error que dice: `No Access-Control-Allow-Origin` header is present on the requested resource. Origin `null` is therefore not allowed access.' ¿Qué debería hacer el desarrollador para resolver este problema?

- [ ] Habilitar el uso compartido de recursos de origen cruzado (CORS) en el bucket de S3.
- [x] Habilitar el uso compartido de recursos de origen cruzado (CORS) para el método en API Gateway.
- [ ] Agregar el encabezado `Access-Control-Request-Method` a la solicitud.
- [ ] Agregar el encabezado `Access-Control-Request-Headers` a la solicitud.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer migró una aplicación web a AWS. Como parte de la migración, el Developer implementó un proceso automatizado de integración continua/mejora continua (CI/CD) mediante un despliegue blue/green. El despliegue aprovisiona nuevas instancias de Amazon EC2 en un Auto Scaling group detrás de un nuevo Application Load Balancer. Una vez completada la migración, el Developer comenzó a recibir quejas de usuarios que eran expulsados del sistema. Además, el sistema requiere que los usuarios inicien sesión después de cada nuevo despliegue. ¿Cómo se pueden resolver estos problemas?

- [ ] Usar actualizaciones progresivas (rolling updates) en lugar de un despliegue blue/green.
- [x] Externalizar las sesiones de usuario a Amazon ElastiCache.
- [ ] Activar las sticky sessions en el Application Load Balancer.
- [ ] Usar multicast para replicar la información de sesión.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer quiere insertar un registro en una tabla de Amazon DynamoDB en cuanto se agregue un nuevo archivo a un bucket de Amazon S3. ¿Qué conjunto de pasos sería necesario para lograrlo?

- [ ] Crear un evento con Amazon CloudWatch Events que monitoree el bucket de S3 y luego inserte los registros en DynamoDB.
- [x] Configurar un evento de S3 para invocar una función de Lambda que inserte los registros en DynamoDB.
- [ ] Crear una función de Lambda que consulte periódicamente (poll) el bucket de S3 y luego inserte los registros en DynamoDB.
- [ ] Crear un cron job que se ejecute en un horario programado e inserte los registros en DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación ingiere una gran cantidad de mensajes pequeños y los almacena en una base de datos. La aplicación usa AWS Lambda. Un equipo de desarrollo está realizando cambios en la lógica de procesamiento de la aplicación. En las pruebas, procesar cada mensaje toma más de 15 minutos. Al equipo le preocupa que el backend actual pueda agotar el tiempo de espera. ¿Qué cambios se deben hacer en el sistema backend para asegurar que cada mensaje se procese de la forma MÁS escalable?

- [ ] Agregar los mensajes a una cola de Amazon SQS. Configurar una instancia de Amazon EC2 para consultar la cola y procesar los mensajes a medida que lleguen.
- [x] Agregar los mensajes a una cola de Amazon SQS. Configurar instancias de Amazon EC2 en un Auto Scaling group para consultar la cola y procesar los mensajes a medida que lleguen.
- [ ] Crear un ticket de soporte para aumentar el tiempo de espera de Lambda a 60 minutos y permitir un mayor tiempo de procesamiento.
- [ ] Cambiar la aplicación para que inserte directamente el cuerpo del mensaje en una base de datos de Amazon RDS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer está escribiendo una aplicación que se ejecutará en instancias de Amazon EC2 en un Auto Scaling group. El Developer quiere externalizar el estado de sesión para dar soporte a la aplicación. ¿Qué servicios cumplirán estas necesidades? (Elija DOS)

- [x] Amazon DynamoDB.
- [ ] Amazon Cognito.
- [x] Amazon ElastiCache.
- [ ] Amazon EBS.
- [ ] Amazon SQS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está desarrollando una aplicación web que permite a sus empleados cargar una foto de perfil a un bucket privado de Amazon S3. No hay límite de tamaño para las fotos de perfil, que deben mostrarse cada vez que un empleado inicia sesión. Por razones de seguridad, las fotos no pueden ser de acceso público. ¿Cuál es una solución viable a largo plazo para este escenario?

- [ ] Generar una URL prefirmada (presigned URL) cuando se cargue una foto. Guardar la URL en una tabla de Amazon DynamoDB. Devolver la URL al navegador cuando el empleado inicie sesión.
- [x] Guardar la clave S3 de la foto en una tabla de Amazon DynamoDB. Crear un VPC endpoint de Amazon S3 para permitir que los empleados descarguen las fotos una vez que inicien sesión.
- [ ] Codificar una foto usando base64. Guardar la cadena base64 en una tabla de Amazon DB. Permitir que el navegador recupere la cadena y la convierta en una foto.
- [ ] Guardar la clave S3 de la foto en una tabla de Amazon DynamoDB. Usar una función para generar una URL prefirmada (presigned URL) cada vez que un empleado inicie sesión. Devolver la URL al navegador.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene una aplicación heredada que fue migrada a una flota de instancias de Amazon EC2. La aplicación almacena datos en una base de datos MySQL que actualmente está instalada en una única instancia de EC2. La empresa ha decidido migrar la base de datos de la instancia de EC2 a MySQL en Amazon RDS. ¿Qué debe hacer el Developer para actualizar la aplicación de modo que soporte el almacenamiento de datos en Amazon RDS?

- [x] Actualizar los parámetros de conexión a la base de datos en la aplicación para que apunten a la nueva instancia de RDS.
- [ ] Agregar un script a la instancia de EC2 que implemente un AWS SDK para solicitar credenciales de la base de datos.
- [ ] Crear una nueva instancia de EC2 con un rol de IAM que permita el acceso a la nueva base de datos de RDS.
- [ ] Crear una función de AWS Lambda que enrute el tráfico desde la instancia de EC2 hacia la base de datos de RDS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa quiere implementar autenticación para su nuevo servicio REST usando Amazon API Gateway. Para autenticar las llamadas, cada solicitud debe incluir encabezados HTTP con un ID de cliente y un ID de usuario. Estas credenciales deben compararse con los datos de autenticación de una tabla de Amazon DynamoDB. ¿Qué DEBE hacer la empresa para implementar esta autenticación en API Gateway?

- [x] Implementar un Lambda authorizer de AWS Lambda que haga referencia a la tabla de autenticación de DynamoDB.
- [ ] Crear un modelo que requiera las credenciales y luego otorgar a API Gateway acceso a la tabla de autenticación.
- [ ] Modificar las integration requests para que requieran las credenciales y luego otorgar a API Gateway acceso a la tabla de autenticación.
- [ ] Implementar un Amazon Cognito authorizer que haga referencia a la tabla de autenticación de DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Al desarrollar una función de AWS Lambda que procesa Amazon Kinesis Data Streams, los administradores de la empresa deben recibir una notificación que incluya los datos procesados. ¿Cómo debe escribir el Desarrollador la función para enviar los datos procesados a los administradores?

- [ ] Separar el handler de Lambda de la lógica principal.
- [ ] Usar Amazon CloudWatch Events para enviar los datos procesados.
- [x] Publicar los datos procesados en un tema de Amazon SNS.
- [ ] Enviar los datos procesados a Amazon SQS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué operación de elementos permite la recuperación de múltiples elementos de una tabla de DynamoDB en una sola llamada a la API?

- [ ] `GetItem`.
- [x] `BatchGetItem`.
- [ ] `GetMultipleItems`.
- [ ] `GetItemRange`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Usted intenta almacenar un objeto en la región `US-STANDARD` de Amazon S3 y recibe una confirmación de que se almacenó correctamente. Luego realiza inmediatamente otra llamada a la API e intenta leer este objeto. S3 le indica que el objeto no existe. ¿Qué podría explicar este comportamiento?

- [x] `US-STANDARD` usa consistencia eventual y puede tomar tiempo para que un objeto sea legible en un bucket.
- [ ] Los objetos en Amazon S3 no se hacen visibles hasta que se replican a una segunda región.
- [ ] `US-STANDARD` impone un retraso de 1 segundo antes de que los objetos nuevos sean legibles.
- [ ] Usted excedió el límite de objetos del bucket, y una vez que se aumente este límite el objeto será visible.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuál es el número máximo de buckets de S3 disponibles por cuenta de AWS?

- [ ] 100 por región.
- [ ] no hay límite.
- [x] 1,000,000 por cuenta.
- [ ] 500 por cuenta.
- [ ] 100 por usuario de IAM.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Si un mensaje se recupera de una cola en Amazon SQS, ¿durante cuánto tiempo permanece inaccesible para otros usuarios por defecto?

- [ ] 0 segundos.
- [ ] 1 hora.
- [ ] 1 día.
- [ ] para siempre.
- [x] 30 segundos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuál es el formato de los mensajes de notificación estructurados enviados por Amazon SNS?

- [ ] Un objeto XML que contiene Messageld, UnsubscribeURL, Subject, Message y otros valores.
- [ ] Un objeto JSON que contiene Messageld, DuplicateFlag, Message y otros valores.
- [ ] Un objeto XML que contiene Messageld, DuplicateFlag, Message y otros valores.
- [x] Un objeto JSON que contiene Messageld, unsubscribeURL, Subject, Message y otros valores.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de los siguientes son argumentos válidos para una solicitud Publish de SNS? (Elija TRES)

- [x] TopicArn.
- [x] Subject.
- [ ] Destination.
- [ ] Format.
- [x] Message.
- [ ] Language.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cómo puede un software determinar las direcciones IP públicas y privadas de la instancia de Amazon EC2 en la que se está ejecutando?

- [ ] Consultar la métrica de Amazon CloudWatch correspondiente.
- [ ] Usar el comando `ipconfig` o `ifconfig`.
- [ ] Consultar el userdata local de la instancia.
- [x] Consultar los metadata locales de la instancia.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué llamada a la API de EC2 usaría para recuperar una lista de Amazon Machine Images (AMIs)?

- [ ] `DescribeInstances`.
- [ ] `DescribeAMIs`.
- [x] `DescribeImages`.
- [ ] `GetAMIs`.
- [ ] No se puede recuperar una lista de AMIs porque hay más de 10,000 AMIs.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuál de las siguientes se elige como la región predeterminada al realizar una llamada a la API con un AWS SDK?

- [ ] `ap-northeast-1`.
- [ ] `us-west-2`.
- [x] `us-east-1`.
- [ ] `eu-west-1`.
- [ ] `us-central-1`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de las siguientes afirmaciones sobre SWF son verdaderas? (Elija TRES)

- [x] Las tareas de SWF se asignan una sola vez y nunca se duplican.
- [ ] SWF requiere un bucket de S3 para el almacenamiento del flujo de trabajo.
- [x] Las ejecuciones de flujo de trabajo de SWF pueden durar hasta un año.
- [ ] SWF activa notificaciones de SNS al asignar una tarea.
- [x] SWF usa deciders y workers para completar las tareas.
- [ ] SWF requiere al menos 1 instancia de EC2 por dominio.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de los siguientes son transportes de entrega válidos de SNS? (Elija DOS)

- [x] HTTP.
- [ ] UDP.
- [x] SMS.
- [ ] DynamoDB.
- [ ] Named Pipes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### La Empresa C ha lanzado recientemente un sitio de comercio en línea de bicicletas en AWS. Tienen una tabla de DynamoDB `Product` que almacena los detalles de cada bicicleta, como fabricante, color, precio, cantidad y talla, para mostrarlos en la tienda en línea. Debido a la demanda de los clientes, quieren incluir una imagen de cada bicicleta junto con los detalles existentes. ¿Cuál de los siguientes enfoques provoca el menor impacto en el throughput aprovisionado de la tabla `Product`?

- [ ] Serializar la imagen y almacenarla en varias tablas de DynamoDB.
- [ ] Crear una tabla de DynamoDB `Images` para almacenar la imagen con una restricción de clave externa hacia la tabla `Product`.
- [ ] Agregar un tipo de dato de imagen a la tabla `Product` para almacenar las imágenes en formato binario.
- [x] Almacenar las imágenes en Amazon S3 y agregar un puntero con la URL de S3 al elemento de la tabla `Product` para cada imagen.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué límites de DynamoDB pueden aumentarse contactando al soporte de AWS? (Elija DOS)

- [ ] El número de hash keys por cuenta.
- [ ] El almacenamiento máximo utilizado por cuenta.
- [x] El número de tablas por cuenta.
- [ ] El número de local secondary indexes por cuenta.
- [x] El número de unidades de throughput aprovisionado por cuenta.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Cuando un mensaje de Simple Queue Service desencadena una tarea que tarda 5 minutos en completarse, ¿cuál de los siguientes procesos dará como resultado el procesamiento exitoso del mensaje y su eliminación de la cola, minimizando al mismo tiempo las posibilidades de procesamiento duplicado?

- [x] Recuperar el mensaje con un visibility timeout aumentado, procesar el mensaje y eliminar el mensaje de la cola.
- [ ] Recuperar el mensaje con un visibility timeout aumentado, eliminar el mensaje de la cola y procesar el mensaje.
- [ ] Recuperar el mensaje con un `DelaySeconds` aumentado, procesar el mensaje y eliminar el mensaje de la cola.
- [ ] Recuperar el mensaje con un `DelaySeconds` aumentado, eliminar el mensaje de la cola y procesar el mensaje.

**[⬆ Back to Top](#tabla-de-contenidos)**

### La Empresa A tiene un bucket de S3 con contenido premium que pretende poner a disposición únicamente de los suscriptores de pago de su sitio web. Actualmente el bucket de S3 tiene permisos predeterminados en los que todos los objetos son privados, para evitar la exposición inadvertida del contenido premium a visitantes que no pagan. ¿Cómo puede la Empresa A permitir que solo los suscriptores de pago descarguen un archivo de contenido premium del bucket de S3?

- [ ] Aplicar una bucket policy que permita a los usuarios anónimos descargar el contenido del bucket de S3.
- [x] Generar una pre-signed object URL para el archivo de contenido premium cuando un suscriptor de pago solicite una descarga.
- [ ] Agregar una bucket policy que requiera Multi-Factor Authentication para las solicitudes de acceso a los objetos del bucket de S3.
- [ ] Habilitar el cifrado del lado del servidor en el bucket de S3 para proteger los datos frente a los visitantes que no pagan.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuál de los siguientes es un ejemplo de un buen esquema de hash key de DynamoDB para lograr eficiencia en el throughput aprovisionado?

- [x] User ID, cuando la aplicación tiene muchos usuarios diferentes.
- [ ] Status Code, cuando la mayoría de los códigos de estado son iguales.
- [ ] Device ID, cuando uno es por mucho más popular que todos los demás.
- [ ] Game Type, cuando hay tres tipos de juego posibles.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación almacena cada noche la información de nómina en DynamoDB para una gran cantidad de empleados de cientos de oficinas. Los atributos de cada elemento consisten en el nombre de la persona, el identificador de la oficina y las horas diarias acumuladas. Los gerentes ejecutan informes para rangos de nombres que trabajan en su oficina. Una consulta es: `Return all Items in this office for names starting with A through E`. ¿Qué configuración de tabla producirá el menor impacto en el throughput aprovisionado para esta consulta?

- [ ] Configurar la tabla con un hash index en el atributo de nombre y un range index en el identificador de la oficina.
- [x] Configurar la tabla con un range index en el atributo de nombre y un hash index en el identificador de la oficina.
- [ ] Configurar un hash index en el atributo de nombre y ningún range index.
- [ ] Configurar un hash index en el atributo de identificador de la oficina y ningún range index.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuál es una diferencia clave entre una instancia respaldada por Amazon EBS y una respaldada por instance store?

- [ ] Virtual Private Cloud requiere instancias respaldadas por EBS.
- [x] Las instancias respaldadas por Amazon EBS pueden detenerse y reiniciarse.
- [ ] Auto scaling requiere el uso de instancias respaldadas por Amazon EBS.
- [ ] Las instancias respaldadas por instance store pueden detenerse y reiniciarse.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Su aplicación intenta cargar un archivo de 6 GB a Simple Storage Service y recibe el mensaje de error `Your proposed upload exceeds the maximum allowed object size.`. ¿Cuál es una posible solución?

- [ ] Ninguna, los objetos de Simple Storage Service están limitados a 5 GB.
- [x] Usar la multi-part upload API para este objeto.
- [ ] Usar la large object upload API para este objeto.
- [ ] Contactar al soporte para aumentar su límite de tamaño de objeto.
- [ ] Cargar a una región diferente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de los siguientes lenguajes de programación tienen un SDK de AWS con soporte oficial? (Elija DOS)

- [ ] Perl.
- [x] PHP.
- [ ] Pascal.
- [x] Java.
- [ ] SQL.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un sistema meteorológico monitorea 600 sensores de temperatura, obtiene muestras de temperatura cada minuto y guarda cada muestra en una tabla de DynamoDB. Cada muestra implica escribir 1K de datos y las escrituras se distribuyen uniformemente en el tiempo. ¿Cuánto throughput de escritura se requiere para la tabla de destino?

- [ ] 1 unidad de capacidad de escritura.
- [x] 10 unidades de capacidad de escritura.
- [ ] 60 unidades de capacidad de escritura.
- [ ] 600 unidades de capacidad de escritura.
- [ ] 3600 unidades de capacidad de escritura.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un bucket de Amazon S3, `myawsbucket`, está configurado con hosting de sitio web en la región de Tokio. ¿Cuál es el endpoint del sitio web específico de la región?

- [ ] `www.myawsbucket.ap-northeast-1.amazonaws.com`.
- [x] `myawsbucket.s3-website-ap-northeast-1.amazonaws.com`.
- [ ] `myawsbucket.amazonaws.com`.
- [ ] `myawsbucket.tokyo.amazonaws.com`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Usted ha escrito una aplicación que usa el servicio Elastic Load Balancing para distribuir el tráfico entre varios servidores web. Sus usuarios se quejan de que a veces se ven obligados a iniciar sesión de nuevo en medio del uso de su aplicación, después de haber iniciado sesión. Este no es un comportamiento que usted haya diseñado. ¿Cuál es una posible solución para evitar que esto ocurra?

- [ ] Usar la memoria de la instancia para guardar el estado de la sesión.
- [ ] Usar el almacenamiento de la instancia para guardar el estado de la sesión.
- [ ] Usar EBS para guardar el estado de la sesión.
- [x] Usar ElastiCache para guardar el estado de la sesión.
- [ ] Usar Glacier para guardar el estado de la sesión.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué afirmaciones sobre DynamoDB son verdaderas? (Elija DOS)

- [ ] DynamoDB usa un modelo de bloqueo pesimista.
- [x] DynamoDB usa control de concurrencia optimista.
- [x] DynamoDB usa escrituras condicionales para la consistencia.
- [ ] DynamoDB restringe el acceso a los elementos durante las lecturas.
- [ ] DynamoDB restringe el acceso a los elementos durante las escrituras.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Usted brinda servicios de consultoría de AWS a una empresa que desarrolla una nueva aplicación móvil que aprovechará Amazon SNS Mobile Push para las notificaciones push. Para enviar mensajes de notificación directos a dispositivos individuales, el identificador de registro o token de cada dispositivo debe registrarse en SNS; sin embargo, los desarrolladores no están seguros de la mejor manera de hacerlo. Usted les aconseja:

- [ ] Cargar en bloque los tokens de dispositivo contenidos en un archivo CSV mediante la AWS Management Console.
- [ ] Dejar que el servicio de notificaciones push (p. ej., Amazon Device Messaging) se encargue del registro.
- [ ] Implementar un token vending service para manejar el registro.
- [x] Llamar a la función de API `CreatePlatformEndPoint` para registrar múltiples tokens de dispositivo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuál de las siguientes afirmaciones sobre SQS es verdadera?

- [ ] Los mensajes se entregarán exactamente una vez y en orden First in, First out.
- [ ] Los mensajes se entregarán exactamente una vez y el orden de entrega es indeterminado.
- [ ] Los mensajes se entregarán una o más veces y en orden First in, First out.
- [x] Los mensajes se entregarán una o más veces y el orden de entrega es indeterminado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### La Empresa C actualmente aloja su sitio corporativo en un bucket de Amazon S3 con Static Website Hosting habilitado. Actualmente, cuando los visitantes van a `http://www.companyc.com` se devuelve la página `index.html`. Ahora la Empresa C desea que se devuelva una nueva página welcome.html cuando un visitante ingrese `http://www.companyc.com` en el navegador. ¿Cuáles de los siguientes pasos permitirán a la Empresa C cumplir este requisito? (Elija DOS)

- [x] Cargar una página html llamada welcome.html a su bucket de S3.
- [ ] Crear una subcarpeta welcome en su bucket de S3.
- [x] Establecer la propiedad Index Document en welcome.html.
- [ ] Mover la página `index.html` a una subcarpeta welcome.
- [ ] Establecer la propiedad Error Document en welcome.html.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador creó una nueva cuenta de AWS y debe crear una función de AWS Lambda escalable que cumpla los siguientes requisitos de ejecución concurrente: tiempo de ejecución promedio de 100 segundos y 50 solicitudes por segundo. ¿Qué paso debe realizarse antes del despliegue para evitar errores?

- [ ] Implementar Dead Letter Queues (DLQ) para capturar los errores de invocación.
- [ ] Agregar un origen de eventos desde Amazon API Gateway a la función de Lambda.
- [ ] Implementar manejo de errores dentro del código de la aplicación.
- [x] Contactar a AWS Support para aumentar los límites de ejecución concurrente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está construyendo una aplicación web de tres capas que debe poder manejar un mínimo de 5000 solicitudes por minuto. Los requisitos indican que la capa web debe ser completamente stateless, mientras que la aplicación mantiene el estado de sesión de los usuarios. ¿Cómo se pueden externalizar los datos de sesión manteniendo la latencia en el valor MÁS bajo posible?

- [ ] Crear una instancia de Amazon RDS y luego implementar el manejo de sesiones a nivel de aplicación para aprovechar una base de datos dentro de la instancia de base de datos de RDS para almacenar los datos de sesión.
- [ ] Implementar una solución de sistema de archivos compartido entre las instancias de Amazon EC2 subyacentes y luego implementar el manejo de sesiones a nivel de aplicación para aprovechar el sistema de archivos compartido para almacenar los datos de sesión.
- [x] Crear un clúster de Amazon ElastiCache Memcached y luego implementar el manejo de sesiones a nivel de aplicación para aprovechar el clúster para almacenar los datos de sesión.
- [ ] Crear una tabla de Amazon DynamoDB y luego implementar el manejo de sesiones a nivel de aplicación para aprovechar la tabla para almacenar los datos de sesión.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ejecuta un sitio web de comercio electrónico que utiliza Amazon DynamoDB, donde los precios de los artículos se actualizan dinámicamente en tiempo real. En cualquier momento, pueden ocurrir múltiples actualizaciones simultáneas de la información de precios de un producto en particular. Esto provoca que los cambios del editor original se sobrescriban sin un proceso de revisión adecuado. ¿Qué opción de escritura de DynamoDB se debe seleccionar para evitar esta sobrescritura?

- [ ] Escrituras concurrentes.
- [x] Escrituras condicionales.
- [ ] Escrituras atómicas.
- [ ] Escrituras por lotes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Se le ha pedido a un desarrollador crear una función de AWS Lambda que se active cada vez que se realicen actualizaciones en los elementos de una tabla de Amazon DynamoDB. La función ha sido creada y se han agregado los permisos apropiados al rol de ejecución de Lambda. Los streams de Amazon DynamoDB se han habilitado para la tabla, pero la función aún no se activa. ¿Qué opción permitiría que las actualizaciones de la tabla de DynamoDB activen la función de Lambda?

- [ ] Cambiar el valor del parámetro `StreamViewType` a `NEW_AND_OLD_IMAGES` para la tabla de DynamoDB.
- [x] Configurar el event source mapping para la función de Lambda.
- [ ] Asignar un tema de Amazon SNS a los streams de DynamoDB.
- [ ] Aumentar la configuración de tiempo máximo de ejecución (timeout) de la función de Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa necesita ingerir terabytes de datos cada hora desde miles de fuentes que se entregan de forma casi continua durante todo el día. El volumen de mensajes generados varía a lo largo del día. Los mensajes deben entregarse en tiempo real para la detección de fraudes y para paneles operativos en vivo. ¿Qué enfoque cumplirá estos requisitos?

- [ ] Enviar los mensajes a una cola de Amazon SQS y luego procesar los mensajes mediante una flota de instancias de Amazon EC2.
- [ ] Usar la API de Amazon S3 para escribir mensajes en un bucket de S3 y luego procesar los mensajes mediante Amazon Redshift.
- [ ] Usar AWS Data Pipeline para automatizar el movimiento y la transformación de los datos.
- [x] Usar Amazon Kinesis Data Streams con Kinesis Client Library para ingerir y entregar los mensajes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación escribe elementos en una tabla de Amazon DynamoDB. A medida que la aplicación escala a miles de instancias, las llamadas a la API de DynamoDB generan errores `ThrottlingException` ocasionales. La aplicación está codificada en un lenguaje incompatible con el AWS SDK. ¿Cómo se debe manejar el error?

- [x] Agregar exponential backoff a la lógica de la aplicación.
- [ ] Usar Amazon SQS como bus de mensajes de API.
- [ ] Pasar las llamadas a la API a través de Amazon API Gateway.
- [ ] Enviar los elementos a DynamoDB mediante Amazon Kinesis Data Firehose.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación web de comercio electrónico que comparte el estado de sesión de forma local (on-premises) se está migrando a AWS. La aplicación debe ser tolerante a fallos, altamente escalable de forma nativa, y cualquier interrupción del servicio no debe afectar la experiencia del usuario. ¿Cuál es la mejor opción para almacenar el estado de sesión?

- [x] Almacenar el estado de sesión en Amazon ElastiCache.
- [ ] Almacenar el estado de sesión en Amazon CloudFront.
- [ ] Almacenar el estado de sesión en Amazon S3.
- [ ] Habilitar la persistencia de sesión (session stickiness) mediante elastic load balancers.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador tiene un servidor web con estado (stateful) on-premises que se está migrando a AWS. El desarrollador debe tener mayor elasticidad en el nuevo diseño. ¿Cómo debe el desarrollador refactorizar la aplicación para hacerla más elástica? (Elija DOS)

- [ ] Usar concurrencia pesimista en Amazon DynamoDB.
- [ ] Usar Amazon CloudFront con un Auto Scaling group.
- [ ] Usar Amazon CloudFront con un AWS Web Application Firewall.
- [x] Almacenar los datos de estado de sesión en una tabla de Amazon DynamoDB.
- [x] Usar un ELB con un Auto Scaling group.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está migrando una aplicación web on-premises de un solo servidor a AWS. La empresa pretende usar múltiples servidores detrás de un Elastic Load Balancer (ELB) para balancear la carga, y también almacenará los datos de sesión en memoria en el servidor web. La empresa no quiere perder esos datos de sesión si un servidor falla o queda fuera de línea, y quiere minimizar el tiempo de inactividad de los usuarios. ¿Dónde debe la empresa mover los datos de sesión para reducir de la forma MÁS efectiva el tiempo de inactividad y hacer que los datos de sesión de los usuarios sean más tolerantes a fallos?

- [x] Un clúster de Amazon ElastiCache for Redis.
- [ ] Un segundo volumen de Amazon EBS.
- [ ] El disco primario del servidor web.
- [ ] Una instancia de Amazon EC2 dedicada a los datos de sesión.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está construyendo una aplicación móvil y necesita que cualquier actualización de los datos del perfil de usuario se envíe a todos los dispositivos que accedan a la identidad específica. El desarrollador no quiere administrar un back end para mantener los datos del perfil de usuario. ¿Cuál es la forma MÁS eficiente para que el desarrollador logre estos requisitos usando Amazon Cognito?

- [ ] Usar Cognito federated identities.
- [ ] Usar un Cognito user pool.
- [x] Usar Cognito Sync.
- [ ] Usar Cognito events.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa mantiene un servicio REST que usa Amazon API Gateway y la validación de claves de API nativa de API Gateway. Recientemente la empresa lanzó una nueva página de registro que permite a los usuarios inscribirse en el servicio. La página de registro crea una nueva clave de API mediante `CreateApiKey` y envía la nueva clave al usuario. Cuando el usuario intenta llamar a la API con esta clave, recibe un error `403 Forbidden`. Los usuarios existentes no se ven afectados y aún pueden llamar a la API. ¿Qué actualizaciones de código otorgarán acceso a la API a estos nuevos usuarios?

- [ ] Se debe llamar al método `createDeployment` para que la API se vuelva a implementar e incluya la clave de API recién creada.
- [ ] Se debe llamar al método `updateAuthorizer` para actualizar el authorizer de la API e incluir la clave de API recién creada.
- [ ] Se debe llamar al método `importApiKeys` para importar todas las claves de API recién creadas en el stage actual de la API.
- [x] Se debe llamar al método `createUsagePlanKey` para asociar la clave de API recién creada con el usage plan correcto.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un trabajo por lotes nocturno carga 1 millón de registros nuevos en una tabla de DynamoDB. Los registros solo se necesitan durante una hora y la tabla debe estar vacía para el trabajo por lotes de la noche siguiente. ¿Cuál es el método MÁS eficiente y rentable para disponer de una tabla vacía?

- [ ] Usar `DeleteItem` con una `ConditionExpression`.
- [ ] Usar `BatchWriteItem` para vaciar todas las filas.
- [ ] Escribir una función recursiva que haga un scan y llame a `DeleteItem`.
- [x] Crear y luego eliminar la tabla una vez completada la tarea.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa presta servicios a muchos consumidores downstream. Cada consumidor puede conectarse a uno o más servicios. Esto ha dado lugar a una arquitectura compleja que es difícil de administrar y no escala bien. La empresa necesita una única interfaz para administrar estos servicios para los consumidores. ¿Qué servicio de AWS se debe usar para refactorizar esta arquitectura?

- [ ] AWS Lambda.
- [ ] AWS X-Ray.
- [ ] Amazon SQS.
- [x] Amazon API Gateway.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando un sitio web sin servidor con contenido que incluye archivos HTML, imágenes, videos y JavaScript (scripts del lado del cliente). ¿Qué combinación de servicios debe usar el desarrollador para crear el sitio web?

- [x] Amazon S3 y Amazon CloudFront.
- [ ] Amazon EC2 y Amazon ElastiCache.
- [ ] Amazon ECS y Redis.
- [ ] AWS Lambda y Amazon API Gateway.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo mantiene actualmente una aplicación que usa un almacén en memoria para guardar los resultados acumulados de juegos. Los resultados individuales se almacenan en una base de datos. Como parte de la migración a AWS, el equipo necesita usar escalado automático. El equipo sabe que esto producirá resultados inconsistentes. ¿Dónde debe almacenar el equipo estos resultados acumulados de juegos para permitir MEJOR resultados consistentes sin afectar el rendimiento?

- [ ] Amazon S3.
- [ ] Amazon RDS.
- [x] Amazon ElastiCache.
- [ ] Amazon Kinesis.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe crear una aplicación que usa Amazon DynamoDB. Los requisitos indican que los elementos almacenados en la tabla de DynamoDB tendrán un tamaño de 7 KB y que las lecturas deben ser fuertemente consistentes. La tasa máxima de lectura es de 3 elementos por segundo y la tasa máxima de escritura es de 10 elementos por segundo. ¿Cómo debe dimensionar el desarrollador la tabla de DynamoDB para cumplir estos requisitos?

- [ ] Read: 3 read capacity. `unitsWrite`: 70 write capacity units.
- [x] Read: 6 read capacity. `unitsWrite`: 70 write capacity units.
- [ ] Read: 6 read capacity. `unitsWrite`: 10 write capacity units.
- [ ] Read: 3 read capacity. `unitsWrite`: 10 write capacity units.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una función de AWS Lambda debe leer datos de una base de datos Amazon RDS MySQL en una VPC y también alcanzar un endpoint público a través de internet para obtener datos adicionales. ¿Qué pasos se deben seguir para permitir que la función acceda tanto al recurso de RDS como al endpoint público? (Seleccione DOS)

- [x] Modificar la configuración predeterminada de la función Lambda para asociarla con una subred privada de Amazon VPC.
- [ ] Modificar la network access control list predeterminada para permitir el tráfico de salida.
- [x] Agregar un NAT Gateway a la VPC.
- [ ] Modificar la configuración predeterminada de la función Lambda para asociarla con una subred pública de VPC.
- [ ] Agregar una variable de entorno a la función Lambda para permitir el acceso de salida a internet.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador quiere obtener una lista de elementos de un índice secundario global de una tabla de Amazon DynamoDB. ¿Qué llamada a la API de DynamoDB puede usar el desarrollador para consumir la MENOR cantidad de unidades de capacidad de lectura?

- [ ] Operación Scan con lecturas `eventually-consistent`.
- [ ] Operación Query con lecturas `strongly-consistent`.
- [x] Operación Query con lecturas `eventually-consistent`.
- [ ] Operación Scan con lecturas `strongly-consistent`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está diseñando un entorno tolerante a fallos donde se guardarán las sesiones de los clientes. ¿Cómo puede el desarrollador asegurarse de que no se pierda ninguna sesión si falla una instancia de Amazon EC2?

- [ ] Usar sesiones persistentes (sticky sessions) con un target group de Elastic Load Balancer.
- [ ] Usar Amazon SQS para guardar los datos de sesión.
- [x] Usar Amazon DynamoDB para realizar un manejo de sesiones escalable.
- [ ] Usar el connection draining de Elastic Load Balancer para dejar de enviar solicitudes a las instancias que fallan.

**[⬆ Back to Top](#tabla-de-contenidos)**

### En un movimiento hacia el uso de microservicios, el equipo de Administración de una empresa ha pedido a todos los equipos de desarrollo que construyan sus servicios de modo que las solicitudes de API dependan únicamente del almacén de datos de ese servicio. Un equipo está construyendo un servicio de Pagos que tiene su propia base de datos; el servicio necesita datos que se originan en la base de datos de Cuentas. Ambas usan Amazon DynamoDB. ¿Qué enfoque dará como resultado el método más simple, desacoplado y confiable para obtener actualizaciones casi en tiempo real desde la base de datos de Cuentas?

- [ ] Usar Amazon Glue para realizar actualizaciones ETL frecuentes desde la base de datos de Cuentas a la base de datos de Pagos.
- [ ] Usar Amazon ElastiCache en Pagos, con la caché actualizada mediante triggers en la base de datos de Cuentas.
- [ ] Usar Amazon Kinesis Data Firehose para entregar todos los cambios de la base de datos de Cuentas a la base de datos de Pagos.
- [x] Usar Amazon DynamoDB Streams para entregar todos los cambios de la base de datos de Cuentas a la base de datos de Pagos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una aplicación sin servidor que requiere que una función de AWS Lambda se invoque cada 10 minutos. ¿Cuál es una forma automatizada y sin servidor de activar la función?

- [ ] Implementar una instancia de Amazon EC2 basada en Linux y editar su archivo `/etc/crontab` agregando un comando para invocar periódicamente la función Lambda.
- [ ] Configurar una variable de entorno llamada PERIOD para la función Lambda. Establecer el valor en `600`.
- [x] Crear una regla de Amazon CloudWatch Events que se active según un programa regular para invocar la función Lambda.
- [ ] Crear un tema de Amazon SNS que tenga una suscripción a la función Lambda con un temporizador de 600 segundos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está construyendo una aplicación para dar seguimiento al rendimiento de atletas usando una tabla de Amazon DynamoDB. Cada elemento de la tabla se identifica mediante una clave de partición (`user_id`) y una clave de ordenación (`sport_name`). El diseño de la tabla se muestra a continuación. (Nota: no se muestran todos los atributos de la tabla) Se le pide a un desarrollador que escriba una aplicación de tabla de posiciones para mostrar a los mejores competidores (`user_id`) según la puntuación para cada `sport_name`. ¿Qué proceso permitirá al desarrollador extraer los resultados de la tabla de DynamoDB de la manera MÁS eficiente?

![Question 337](images/question337.jpg)

- [ ] Usar una operación query de DynamoDB con los atributos de clave `user_id` y `sport_name` y ordenar los resultados según el atributo de puntuación.
- [x] Crear un índice secundario global con una clave de partición `sport_name` y una clave de ordenación de puntuación, y obtener los resultados.
- [ ] Usar una operación scan de DynamoDB para recuperar las puntuaciones y `user_id` según `sport_name`, y ordenar los resultados según el atributo de puntuación.
- [ ] Crear un índice secundario local con una clave primaria `sport_name` y una clave de ordenación de puntuación, y obtener los resultados según el atributo de puntuación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué logra una cola de retraso (delay queue) de Amazon SQS?

- [x] Los mensajes se ocultan durante un período de tiempo configurable cuando se agregan por primera vez a la cola.
- [ ] Los mensajes se ocultan durante un período de tiempo configurable después de ser consumidos de la cola.
- [ ] El consumidor puede sondear la cola durante un período de tiempo configurable antes de recuperar un mensaje.
- [ ] Los mensajes no se pueden eliminar durante un período de tiempo configurable después de ser consumidos de la cola.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está usando la AWS CLI, pero al ejecutar comandos de listado sobre una gran cantidad de recursos, se agota el tiempo de espera. ¿Qué se puede hacer para evitar este tiempo de espera agotado?

- [x] Usar paginación.
- [ ] Usar sintaxis abreviada (shorthand).
- [ ] Usar valores de parámetros.
- [ ] Usar cadenas entre comillas.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Dónde se puede definir PortMapping al lanzar contenedores en Amazon ECS?

- [ ] Security groups.
- [ ] Amazon Elastic Container Registry (Amzon ECR).
- [ ] Container agent.
- [x] Task definition.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una organización almacena archivos grandes en Amazon S3 y está escribiendo una aplicación web para mostrar metadatos sobre los archivos a los usuarios finales. Según los metadatos, un usuario selecciona un objeto para descargar. La organización necesita un mecanismo para indexar los archivos y proporcionar una recuperación de los metadatos con latencia de un solo dígito en milisegundos. ¿Qué servicio de AWS se debe usar para lograrlo?

- [x] Amazon DynamoDB.
- [ ] Amazon EC2.
- [ ] AWS Lambda.
- [ ] Amazon RDS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación local (on-premises) realiza llamadas repetidas para almacenar archivos en Amazon S3. A medida que ha aumentado el uso de la aplicación, se están registrando errores `LimitExceeded`. ¿Qué se debe cambiar para corregir este error?

- [x] Implementar retroceso exponencial (exponential backoff) en la aplicación.
- [ ] Balancear la carga de la aplicación entre varios servidores.
- [ ] Mover la aplicación a Amazon EC2.
- [ ] Agregar un retraso de un segundo a cada llamada de API.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa almacena en caché la información de sesión de una aplicación web en una tabla de Amazon DynamoDB. La empresa quiere una forma automatizada de eliminar los elementos antiguos de la tabla. ¿Cuál es la forma más simple de hacerlo?

- [ ] Escribir un script que elimine los registros antiguos; programar el script como un cron job en una instancia de Amazon EC2.
- [x] Agregar un atributo con la hora de expiración; habilitar la característica `Time To Live` basada en ese atributo.
- [ ] Cada día, crear una tabla nueva para guardar los datos de sesión; eliminar la tabla del día anterior.
- [ ] Agregar un atributo con la hora de expiración; nombrar el atributo `ItemExpiration`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Se espera que una aplicación procese muchos archivos. Cada archivo tarda cuatro minutos en procesarse en cada invocación de AWS Lambda. La función Lambda no devuelve ningún dato importante. ¿Cuál es la forma más rápida de procesar todos los archivos?

- [ ] Primero dividir los archivos para hacerlos más pequeños y luego procesarlos con invocaciones síncronas RequestResponse de Lambda.
- [ ] Realizar invocaciones síncronas RequestResponse de Lambda y procesar los archivos uno por uno.
- [x] Realizar invocaciones asíncronas Event de Lambda y procesar los archivos en paralelo.
- [ ] Primero unir todos los archivos y luego procesarlo todo de una vez con una invocación asíncrona Event de Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Falla la carga de un objeto de 15 GB a Amazon S3. El mensaje de error dice: `Your proposed upload exceeds the maximum allowed object size.`. ¿Qué técnica permitirá al desarrollador cargar este objeto?

- [x] Cargar el objeto usando la API de carga multiparte (multi-part upload).
- [ ] Cargar el objeto a través de una conexión de AWS Direct Connect.
- [ ] Contactar a AWS Support para aumentar el límite de tamaño de objeto.
- [ ] Cargar el objeto a otra región de AWS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación usa Amazon DynamoDB como almacén de datos y debe poder leer 100 elementos por segundo como lecturas de consistencia fuerte. Cada elemento tiene un tamaño de 5 KB. ¿A qué valor se debe establecer el rendimiento de lectura aprovisionado de la tabla?

- [ ] 50 unidades de capacidad de lectura.
- [ ] 100 unidades de capacidad de lectura.
- [x] 200 unidades de capacidad de lectura.
- [ ] 500 unidades de capacidad de lectura.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una función de Lambda que generará y exportará un archivo. La función requiere 100 MB de almacenamiento temporal para archivos temporales durante su ejecución. Estos archivos no serán necesarios después de que la función termine. ¿Cómo puede el desarrollador manejar de la manera MÁS eficiente los archivos temporales?

- [ ] Almacenar los archivos en EBS y eliminarlos al final de la función Lambda.
- [ ] Copiar los archivos a EFS y eliminarlos al final de la función Lambda.
- [x] Almacenar los archivos en el directorio `/tmp` y eliminarlos al final de la función Lambda.
- [ ] Copiar los archivos a un bucket de S3 con una política de lifecycle para eliminarlos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación se ejecuta en múltiples instancias EC2 detrás de un ELB. ¿Dónde es mejor escribir los datos de sesión para que puedan servirse de manera confiable a través de múltiples solicitudes?

- [x] Escribir los datos en Amazon ElastiCache.
- [ ] Escribir los datos en Amazon Elastic Block Store.
- [ ] Escribir los datos en Amazon EC2 Instance Store.
- [ ] Escribir los datos en el sistema de archivos `root`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está migrando de una arquitectura monolítica a una arquitectura basada en microservicios. Los desarrolladores necesitan refactorizar la aplicación para que los numerosos microservicios puedan comunicarse de forma asíncrona entre sí sin afectar el rendimiento. ¿El uso de cuáles servicios administrados de AWS permitirá el paso de mensajes asíncrono? (Elija DOS)

- [x] Amazon SQS.
- [ ] Amazon Cognito.
- [ ] Amazon Kinesis.
- [x] Amazon SNS.
- [ ] Amazon ElastiCache.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación necesita usar la dirección IP del cliente en su procesamiento. La aplicación se ha movido a AWS y se ha colocado detrás de un Application Load Balancer (ALB). Sin embargo, ahora todas las direcciones IP de los clientes parecen ser la misma. La aplicación debe mantener la capacidad de escalar horizontalmente. Según este escenario, ¿cuál es la solución MÁS rentable a este problema?

- [ ] Quitar la aplicación del ALB. Eliminar el ALB y cambiar Amazon Route 53 para dirigir el tráfico a la instancia que ejecuta la aplicación.
- [ ] Quitar la aplicación del ALB. Crear un Classic Load Balancer en su lugar. Dirigir el tráfico a la aplicación usando el protocolo HTTP.
- [x] Modificar el código de la aplicación para inspeccionar el encabezado `X-Forwarded-For`. Asegurar que el código pueda funcionar correctamente si se pasa una lista de direcciones IP en el encabezado.
- [ ] Modificar el código de la aplicación para inspeccionar un encabezado personalizado. Modificar el código del cliente para pasar la dirección IP en el encabezado personalizado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación local (on-premises) está implementada usando una pila Linux, Apache, MySQL y PHP (LAMP). El desarrollador quiere ejecutar esta aplicación en AWS. ¿Cuál de los siguientes conjuntos de servicios de AWS puede usarse para ejecutar esta pila?

- [ ] Amazon API Gateway, Amazon S3.
- [ ] AWS Lambda, Amazon DynamoDB.
- [x] Amazon EC2, Amazon Aurora.
- [ ] Amazon Cognito, Amazon RDS.
- [ ] Amazon ECS, Amazon EBS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación muestra un panel de estado. El estado se actualiza mediante mensajes de 1 KB provenientes de una cola de SQS. Aunque el estado cambia con poca frecuencia, el desarrollador debe minimizar el tiempo entre la llegada del mensaje a la cola y la actualización del panel. ¿Qué técnica proporciona el menor retraso en la actualización del panel?

- [x] Recuperar los mensajes de la cola usando long polling cada 20 segundos.
- [ ] Reducir el tamaño de los mensajes comprimiéndolos antes de enviarlos.
- [ ] Recuperar los mensajes de la cola usando short polling cada 10 segundos.
- [ ] Reducir el tamaño del payload de cada mensaje enviándolo en dos partes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación heredada local (on-premises) almacena en caché archivos de datos localmente y escribe imágenes compartidas en discos locales. ¿Qué es necesario para permitir el escalado horizontal al migrar la aplicación a AWS?

- [ ] Modificar la aplicación para que tanto las imágenes compartidas como los datos de caché se escriban en Amazon EBS.
- [x] Modificar la aplicación para leer y escribir los datos de caché en Amazon S3, y también almacenar las imágenes compartidas en S3.
- [ ] Modificar la aplicación para usar Amazon S3 para servir las imágenes compartidas; los datos de caché pueden entonces escribirse en discos locales.
- [ ] Modificar la aplicación para leer y escribir los datos de caché en Amazon S3, mientras se continúa escribiendo las imágenes compartidas en discos locales.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe activar una función de AWS Lambda basándose en la actividad del ciclo de vida de los elementos en una tabla de Amazon DynamoDB. ¿Cómo puede el desarrollador crear la solución?

- [ ] Habilitar un stream de DynamoDB que publique un mensaje de Amazon SNS. Activar la función Lambda de forma síncrona desde el mensaje de SNS.
- [ ] Habilitar un stream de DynamoDB que publique un mensaje de SNS. Activar la función Lambda de forma asíncrona desde el mensaje de SNS.
- [ ] Habilitar un stream de DynamoDB y activar la función Lambda de forma síncrona desde el stream.
- [x] Habilitar un stream de DynamoDB y activar la función Lambda de forma asíncrona desde el stream.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Después de instalar el AWS CLI, un desarrollador intenta ejecutar el comando `aws configure` pero recibe el siguiente error: `Error: aws: command not found`. ¿Cuál es la causa más probable de este error?

- [x] El ejecutable `aws` no está en la variable de entorno `PATH`.
- [ ] Se ha denegado el acceso al ejecutable `aws` al instalador.
- [ ] Se proporcionaron credenciales de AWS incorrectas.
- [ ] El script `aws` no tiene un modo de archivo ejecutable.

**[⬆ Back to Top](#tabla-de-contenidos)**

### El desarrollador de una empresa minorista debe integrar una solución de detección de fraude en la solución de procesamiento de pedidos. La solución de detección de fraude tarda entre diez y treinta minutos en verificar un pedido. En horas pico, el sitio web puede recibir cien pedidos por minuto. ¿Cuál es el método más escalable para agregar la solución de detección de fraude a la canalización de procesamiento de pedidos?

- [ ] Agregar todos los pedidos nuevos a una cola de Amazon SQS. Configurar una flota de 10 instancias EC2 distribuidas en múltiples AZ con la solución de detección de fraude instalada para extraer pedidos de esta cola. Actualizar el pedido con un estado de aprobado o rechazado.
- [x] Agregar todos los pedidos nuevos a una cola de SQS. Configurar un Auto Scaling group que use la métrica de profundidad de la cola como su unidad de escalado para lanzar una flota de instancias EC2 de tamaño dinámico distribuidas en múltiples AZ con la solución de detección de fraude instalada para extraer pedidos de esta cola. Actualizar el pedido con un estado de aprobado o rechazado.
- [ ] Agregar todos los pedidos nuevos a un Amazon Kinesis Stream. Suscribir una función Lambda para leer automáticamente lotes de registros del Kinesis Stream. La función Lambda incluye el software de detección de fraude y actualizará el pedido con un estado de aprobado o rechazado.
- [ ] Escribir todos los pedidos nuevos en Amazon DynamoDB. Configurar DynamoDB Streams para incluir todos los pedidos nuevos. Suscribir una función Lambda para leer automáticamente lotes de registros del Kinesis Stream. La función Lambda incluye el software de detección de fraude y actualizará el pedido con un estado de aprobado o rechazado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un conjunto de APIs se expone a los clientes mediante Amazon API Gateway. Estas APIs tienen el almacenamiento en caché habilitado en API Gateway. Los clientes han solicitado una opción para invalidar esta caché para cada una de las APIs. ¿Qué acción se puede tomar para permitir que los clientes de la API invaliden la caché de la API?

- [ ] Pedir a los clientes que usen credenciales de AWS para llamar a la API `InvalidateCache`.
- [ ] Pedir a los clientes que invoquen un endpoint de la API de AWS que invalide la caché.
- [x] Pedir a los clientes que pasen un encabezado HTTP llamado `Cache-Control:max-age=0`.
- [ ] Pedir a los clientes que agreguen un parámetro de cadena de consulta llamado `INVALIDATE_CACHE` al realizar una llamada a la API.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Se ha pedido a un desarrollador que construya una aplicación web de panel en tiempo real para visualizar los prefijos de clave y el tamaño de almacenamiento de los objetos en buckets de Amazon S3. Se usará Amazon DynamoDB para almacenar los metadatos de Amazon S3. ¿Cuál es el diseño óptimo y MÁS rentable para asegurar que el panel en tiempo real se mantenga actualizado con el estado de los objetos en los buckets de Amazon S3?

- [ ] Usar un evento de Amazon CloudWatch respaldado por una función de AWS Lambda. Emitir una llamada a la API de Amazon S3 para obtener una lista de todos los objetos de Amazon S3 y persistir los metadatos en DynamoDB. Hacer que la aplicación web consulte periódicamente (poll) la tabla de DynamoDB para reflejar este cambio.
- [x] Usar Amazon S3 Event Notification respaldado por una función Lambda para persistir los metadatos en DynamoDB. Hacer que la aplicación web consulte periódicamente (poll) la tabla de DynamoDB para reflejar este cambio.
- [ ] Ejecutar un cron job dentro de una instancia de Amazon EC2 para listar todos los objetos en Amazon S3 y persistir los metadatos en DynamoDB. Hacer que la aplicación web consulte periódicamente (poll) la tabla de DynamoDB para reflejar este cambio.
- [ ] Crear un nuevo clúster de Amazon EMR para obtener todos los metadatos sobre los objetos de Amazon S3; persistir los metadatos en DynamoDB. Hacer que la aplicación web consulte periódicamente (poll) la tabla de DynamoDB para reflejar este cambio.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación sin servidor existente procesa archivos de imagen cargados. El proceso actualmente usa una única función Lambda que toma un archivo de imagen, realiza el procesamiento y almacena el archivo en Amazon S3. Los usuarios de la aplicación ahora requieren la generación de miniaturas de las imágenes. Los usuarios quieren evitar cualquier impacto en el tiempo que toma realizar las cargas de imágenes. ¿Cómo se puede agregar la generación de miniaturas a la aplicación, cumpliendo los requisitos de los usuarios y minimizando los cambios al código existente?

- [ ] Cambiar la función Lambda existente que maneja las cargas para que cree miniaturas al momento de la carga. Hacer que la función almacene tanto la imagen como la miniatura en Amazon S3.
- [ ] Crear una segunda función Lambda que maneje la generación y el almacenamiento de miniaturas. Cambiar la función Lambda existente para que la invoque de forma asíncrona.
- [x] Crear una notificación de eventos de S3 con una función Lambda como destino. Crear una nueva función Lambda para generar y almacenar las miniaturas.
- [ ] Crear una notificación de eventos de S3 hacia una cola de SQS. Crear una función Lambda programada que procese la cola y genere y almacene las miniaturas.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un sitio web estático está alojado en un bucket de Amazon S3. Varias páginas HTML del sitio usan JavaScript para descargar imágenes desde otro bucket de Amazon S3. Estas imágenes no se muestran cuando los usuarios navegan por el sitio. ¿Cuál es la posible causa del problema?

- [ ] El bucket de Amazon S3 referenciado está en otra región.
- [ ] Las imágenes deben almacenarse en el mismo bucket de Amazon S3.
- [ ] El puerto 80 debe estar abierto en el security group en el que se encuentra el bucket de Amazon S3.
- [x] Cross Origin Resource Sharing debe estar habilitado en el bucket de Amazon S3.

**[⬆ Back to Top](#tabla-de-contenidos)**
