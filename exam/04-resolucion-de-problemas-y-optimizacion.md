# Dominio 4: Resolución de problemas y optimización (18 %)

Preguntas de práctica AWS Certified Developer Associate (DVA-C02) — 92 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [¿Cuáles de los siguientes son buenos casos de uso de cómo Amazon ElastiCache puede ayudar a una aplicación? (Seleccione DOS)](#cuáles-de-los-siguientes-son-buenos-casos-de-uso-de-cómo-amazon-elasticache-puede-ayudar-a-una-aplicación-seleccione-dos) |
| 2 | [Una empresa global tiene una aplicación que se ejecuta en instancias de Amazon EC2 y que sirve archivos de imagen desde Amazon S3. Las solicitudes de los usuarios desde el navegador están generando un alto tráfico, lo que provoca un rendimiento degradado. ¿Qué solución de optimización debe implementar un desarrollador para aumentar el rendimiento de la aplicación?](#una-empresa-global-tiene-una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-y-que-sirve-archivos-de-imagen-desde-amazon-s3-las-solicitudes-de-los-usuarios-desde-el-navegador-están-generando-un-alto-tráfico-lo-que-provoca-un-rendimiento-degradado-qué-solución-de-optimización-debe-implementar-un-desarrollador-para-aumentar-el-rendimiento-de-la-aplicación) |
| 3 | [El equipo de desarrollo está trabajando en una API que se servirá desde Amazon API Gateway. La API se servirá desde tres entornos: desarrollo, pruebas y producción. API Gateway está configurado para usar 237 GB de caché en las tres stages. ¿Cuál es la estrategia de implementación MÁS rentable?](#el-equipo-de-desarrollo-está-trabajando-en-una-api-que-se-servirá-desde-amazon-api-gateway-la-api-se-servirá-desde-tres-entornos-desarrollo-pruebas-y-producción-api-gateway-está-configurado-para-usar-237-gb-de-caché-en-las-tres-stages-cuál-es-la-estrategia-de-implementación-más-rentable) |
| 4 | [Una empresa está migrando su base de datos local (on-premises) a Amazon RDS for MySQL. La empresa tiene cargas de trabajo con muchas lecturas y quiere asegurarse de refactorizar su código para lograr un rendimiento de lectura óptimo en sus consultas. ¿Cómo se puede lograr este objetivo?](#una-empresa-está-migrando-su-base-de-datos-local-on-premises-a-amazon-rds-for-mysql-la-empresa-tiene-cargas-de-trabajo-con-muchas-lecturas-y-quiere-asegurarse-de-refactorizar-su-código-para-lograr-un-rendimiento-de-lectura-óptimo-en-sus-consultas-cómo-se-puede-lograr-este-objetivo) |
| 5 | [Un desarrollador ha creado una aplicación que inserta datos en una tabla de Amazon DynamoDB. La tabla está configurada para usar capacidad aprovisionada. La aplicación está implementada en una instancia de Amazon EC2 nano con capacidad de ráfaga (burstable). Los registros de la aplicación muestran que la aplicación ha estado fallando debido a un error `ProvisionedThroughputExceedException`. ¿Qué acciones debe tomar el desarrollador para resolver este problema? (Elija dos.)](#un-desarrollador-ha-creado-una-aplicación-que-inserta-datos-en-una-tabla-de-amazon-dynamodb-la-tabla-está-configurada-para-usar-capacidad-aprovisionada-la-aplicación-está-implementada-en-una-instancia-de-amazon-ec2-nano-con-capacidad-de-ráfaga-burstable-los-registros-de-la-aplicación-muestran-que-la-aplicación-ha-estado-fallando-debido-a-un-error-provisionedthroughputexceedexception-qué-acciones-debe-tomar-el-desarrollador-para-resolver-este-problema-elija-dos) |
| 6 | [Una empresa ejecuta una aplicación construida con funciones de AWS Lambda. Una función Lambda tiene problemas de rendimiento cuando debe descargar un archivo de 50 MB desde Internet en cada ejecución. Esta función se invoca varias veces por segundo. ¿Qué solución daría el MEJOR aumento de rendimiento?](#una-empresa-ejecuta-una-aplicación-construida-con-funciones-de-aws-lambda-una-función-lambda-tiene-problemas-de-rendimiento-cuando-debe-descargar-un-archivo-de-50-mb-desde-internet-en-cada-ejecución-esta-función-se-invoca-varias-veces-por-segundo-qué-solución-daría-el-mejor-aumento-de-rendimiento) |
| 7 | [Las consultas a una tabla de Amazon DynamoDB están consumiendo una gran cantidad de capacidad de lectura. La tabla tiene una cantidad significativa de atributos grandes. La aplicación no necesita todos los datos de los atributos. ¿Cómo se pueden minimizar los costos de DynamoDB mientras se maximiza el rendimiento de la aplicación?](#las-consultas-a-una-tabla-de-amazon-dynamodb-están-consumiendo-una-gran-cantidad-de-capacidad-de-lectura-la-tabla-tiene-una-cantidad-significativa-de-atributos-grandes-la-aplicación-no-necesita-todos-los-datos-de-los-atributos-cómo-se-pueden-minimizar-los-costos-de-dynamodb-mientras-se-maximiza-el-rendimiento-de-la-aplicación) |
| 8 | [Los tiempos de carga de las páginas de un sitio web aumentan gradualmente a medida que más usuarios acceden al sistema al mismo tiempo. El análisis indica que el perfil de usuario se carga desde una base de datos en todas las páginas web que visita cada usuario, lo que aumenta la carga de la base de datos y la latencia de carga de las páginas. Para abordar este problema, el desarrollador decide almacenar en caché los datos del perfil de usuario. ¿Qué estrategia de caché abordará esta situación de la manera MÁS eficiente?](#los-tiempos-de-carga-de-las-páginas-de-un-sitio-web-aumentan-gradualmente-a-medida-que-más-usuarios-acceden-al-sistema-al-mismo-tiempo-el-análisis-indica-que-el-perfil-de-usuario-se-carga-desde-una-base-de-datos-en-todas-las-páginas-web-que-visita-cada-usuario-lo-que-aumenta-la-carga-de-la-base-de-datos-y-la-latencia-de-carga-de-las-páginas-para-abordar-este-problema-el-desarrollador-decide-almacenar-en-caché-los-datos-del-perfil-de-usuario-qué-estrategia-de-caché-abordará-esta-situación-de-la-manera-más-eficiente) |
| 9 | [Un desarrollador está escribiendo una función de AWS Lambda. El desarrollador desea registrar los eventos clave que ocurren durante la ejecución de la función de Lambda e incluir un identificador único para asociar los eventos con una invocación específica de la función. ¿Cuál de las siguientes opciones ayudará al desarrollador a lograr este objetivo?](#un-desarrollador-está-escribiendo-una-función-de-aws-lambda-el-desarrollador-desea-registrar-los-eventos-clave-que-ocurren-durante-la-ejecución-de-la-función-de-lambda-e-incluir-un-identificador-único-para-asociar-los-eventos-con-una-invocación-específica-de-la-función-cuál-de-las-siguientes-opciones-ayudará-al-desarrollador-a-lograr-este-objetivo) |
| 10 | [Una función de AWS Lambda accede a dos tablas de Amazon DynamoDB. Un desarrollador desea mejorar el rendimiento de la función de Lambda identificando cuellos de botella en la función. ¿Cómo puede el desarrollador inspeccionar los tiempos de las llamadas a la API de DynamoDB?](#una-función-de-aws-lambda-accede-a-dos-tablas-de-amazon-dynamodb-un-desarrollador-desea-mejorar-el-rendimiento-de-la-función-de-lambda-identificando-cuellos-de-botella-en-la-función-cómo-puede-el-desarrollador-inspeccionar-los-tiempos-de-las-llamadas-a-la-api-de-dynamodb) |
| 11 | [Una instancia de base de datos de Amazon RDS es utilizada por muchas aplicaciones para consultar datos históricos. La tasa de consultas es relativamente constante. Cuando los datos históricos se actualizan cada día, el tráfico de escritura resultante ralentiza el rendimiento de las consultas de lectura y afecta a todos los usuarios de las aplicaciones. ¿Qué se puede hacer para eliminar el impacto en el rendimiento para los usuarios de las aplicaciones?](#una-instancia-de-base-de-datos-de-amazon-rds-es-utilizada-por-muchas-aplicaciones-para-consultar-datos-históricos-la-tasa-de-consultas-es-relativamente-constante-cuando-los-datos-históricos-se-actualizan-cada-día-el-tráfico-de-escritura-resultante-ralentiza-el-rendimiento-de-las-consultas-de-lectura-y-afecta-a-todos-los-usuarios-de-las-aplicaciones-qué-se-puede-hacer-para-eliminar-el-impacto-en-el-rendimiento-para-los-usuarios-de-las-aplicaciones) |
| 12 | [Una aplicación se ejecuta en una instancia de EC2. El desarrollador desea almacenar una métrica de la aplicación en Amazon CloudWatch. ¿Cuál es la mejor práctica para implementar este requisito?](#una-aplicación-se-ejecuta-en-una-instancia-de-ec2-el-desarrollador-desea-almacenar-una-métrica-de-la-aplicación-en-amazon-cloudwatch-cuál-es-la-mejor-práctica-para-implementar-este-requisito) |
| 13 | [Un desarrollador ha escrito una aplicación multihilo que se ejecuta en una flota de instancias de Amazon EC2. El equipo de operaciones ha solicitado un método gráfico para monitorear el número de hilos en ejecución a lo largo del tiempo. ¿Cuál es la forma MÁS eficiente de cumplir con esta solicitud?](#un-desarrollador-ha-escrito-una-aplicación-multihilo-que-se-ejecuta-en-una-flota-de-instancias-de-amazon-ec2-el-equipo-de-operaciones-ha-solicitado-un-método-gráfico-para-monitorear-el-número-de-hilos-en-ejecución-a-lo-largo-del-tiempo-cuál-es-la-forma-más-eficiente-de-cumplir-con-esta-solicitud) |
| 14 | [La función de Lambda que se muestra a continuación se invoca a través de una API mediante Amazon API Gateway. El tiempo promedio de ejecución de la función de Lambda es de aproximadamente 1 segundo. El pseudocódigo de la función de Lambda se muestra en la imagen. ¿Qué dos acciones se pueden tomar para mejorar el rendimiento de esta función de Lambda sin aumentar el costo de la solución? (Seleccione DOS)](#la-función-de-lambda-que-se-muestra-a-continuación-se-invoca-a-través-de-una-api-mediante-amazon-api-gateway-el-tiempo-promedio-de-ejecución-de-la-función-de-lambda-es-de-aproximadamente-1-segundo-el-pseudocódigo-de-la-función-de-lambda-se-muestra-en-la-imagen-qué-dos-acciones-se-pueden-tomar-para-mejorar-el-rendimiento-de-esta-función-de-lambda-sin-aumentar-el-costo-de-la-solución-seleccione-dos) |
| 15 | [Una aplicación en AWS utiliza APIs de terceros. El desarrollador necesita monitorear los errores de las APIs en el código y desea recibir notificaciones si las fallas superan un valor de umbral establecido. ¿Cómo puede el desarrollador cumplir con estos requisitos?](#una-aplicación-en-aws-utiliza-apis-de-terceros-el-desarrollador-necesita-monitorear-los-errores-de-las-apis-en-el-código-y-desea-recibir-notificaciones-si-las-fallas-superan-un-valor-de-umbral-establecido-cómo-puede-el-desarrollador-cumplir-con-estos-requisitos) |
| 16 | [Una empresa ha escrito una función de AWS Lambda en Java que se activa cada vez que un usuario carga una imagen en un bucket de Amazon S3. La función convierte la imagen original a varios formatos diferentes y luego copia las imágenes resultantes a otro bucket de Amazon S3. Los desarrolladores descubren que no se está copiando ninguna imagen al segundo bucket de Amazon S3. Probaron el código en una instancia de Amazon EC2 con 1 GB de RAM y tarda en promedio 500 segundos en completarse. ¿Cuál es la causa MÁS probable del problema?](#una-empresa-ha-escrito-una-función-de-aws-lambda-en-java-que-se-activa-cada-vez-que-un-usuario-carga-una-imagen-en-un-bucket-de-amazon-s3-la-función-convierte-la-imagen-original-a-varios-formatos-diferentes-y-luego-copia-las-imágenes-resultantes-a-otro-bucket-de-amazon-s3-los-desarrolladores-descubren-que-no-se-está-copiando-ninguna-imagen-al-segundo-bucket-de-amazon-s3-probaron-el-código-en-una-instancia-de-amazon-ec2-con-1-gb-de-ram-y-tarda-en-promedio-500-segundos-en-completarse-cuál-es-la-causa-más-probable-del-problema) |
| 17 | [Una empresa desea migrar su aplicación web a AWS y aprovechar Auto Scaling para manejar las cargas de trabajo pico. El arquitecto de soluciones determinó que la mejor métrica para un evento de Auto Scaling es el número de usuarios concurrentes. Con base en esta información, ¿qué debe usar el desarrollador para escalar automáticamente según los usuarios concurrentes?](#una-empresa-desea-migrar-su-aplicación-web-a-aws-y-aprovechar-auto-scaling-para-manejar-las-cargas-de-trabajo-pico-el-arquitecto-de-soluciones-determinó-que-la-mejor-métrica-para-un-evento-de-auto-scaling-es-el-número-de-usuarios-concurrentes-con-base-en-esta-información-qué-debe-usar-el-desarrollador-para-escalar-automáticamente-según-los-usuarios-concurrentes) |
| 18 | [Una aplicación lee datos de una tabla de Amazon DynamoDB. Varias veces al día, durante un período de 15 segundos, la aplicación recibe múltiples errores `ProvisionedThroughputExceeded`. ¿Cómo debería manejarse esta excepción?](#una-aplicación-lee-datos-de-una-tabla-de-amazon-dynamodb-varias-veces-al-día-durante-un-período-de-15-segundos-la-aplicación-recibe-múltiples-errores-provisionedthroughputexceeded-cómo-debería-manejarse-esta-excepción) |
| 19 | [Al escribir una función Lambda, ¿cuál es el beneficio de instanciar los clientes de AWS fuera del ámbito del handler?](#al-escribir-una-función-lambda-cuál-es-el-beneficio-de-instanciar-los-clientes-de-aws-fuera-del-ámbito-del-handler) |
| 20 | [Un desarrollador recibe errores HTTP `400`: `ThrottlingException` de forma intermitente al llamar a la API de Amazon CloudWatch. Cuando una llamada falla, no se recupera ningún dato. ¿Qué mejor práctica debería aplicarse primero para resolver este problema?](#un-desarrollador-recibe-errores-http-400-throttlingexception-de-forma-intermitente-al-llamar-a-la-api-de-amazon-cloudwatch-cuando-una-llamada-falla-no-se-recupera-ningún-dato-qué-mejor-práctica-debería-aplicarse-primero-para-resolver-este-problema) |
| 21 | [Durante las horas de menor actividad, un desarrollador quiere minimizar el tiempo de ejecución de un escaneo completo de una tabla de Amazon DynamoDB sin afectar las cargas de trabajo normales. Las cargas de trabajo consumen en promedio la mitad de las unidades de capacidad de lectura consistente fuerte durante las horas de menor actividad. ¿Cómo podría el desarrollador optimizar este escaneo?](#durante-las-horas-de-menor-actividad-un-desarrollador-quiere-minimizar-el-tiempo-de-ejecución-de-un-escaneo-completo-de-una-tabla-de-amazon-dynamodb-sin-afectar-las-cargas-de-trabajo-normales-las-cargas-de-trabajo-consumen-en-promedio-la-mitad-de-las-unidades-de-capacidad-de-lectura-consistente-fuerte-durante-las-horas-de-menor-actividad-cómo-podría-el-desarrollador-optimizar-este-escaneo) |
| 22 | [Se está diseñando un sitio grande de comercio electrónico para entregar objetos estáticos desde Amazon S3. El bucket de Amazon S3 atenderá más de 300 solicitudes GET por segundo. ¿Qué debería hacerse para optimizar el rendimiento? (Elija DOS)](#se-está-diseñando-un-sitio-grande-de-comercio-electrónico-para-entregar-objetos-estáticos-desde-amazon-s3-el-bucket-de-amazon-s3-atenderá-más-de-300-solicitudes-get-por-segundo-qué-debería-hacerse-para-optimizar-el-rendimiento-elija-dos) |
| 23 | [Un desarrollador tiene una aplicación que puede cargar decenas de miles de objetos por segundo a Amazon S3 en paralelo dentro de una única cuenta de AWS. Como parte de nuevos requisitos, los datos almacenados en S3 deben usar cifrado del lado del servidor con AWS KMS (SSE-KMS). Después de realizar este cambio, el rendimiento de la aplicación es más lento. ¿Cuál es la causa MÁS probable de la latencia de la aplicación?](#un-desarrollador-tiene-una-aplicación-que-puede-cargar-decenas-de-miles-de-objetos-por-segundo-a-amazon-s3-en-paralelo-dentro-de-una-única-cuenta-de-aws-como-parte-de-nuevos-requisitos-los-datos-almacenados-en-s3-deben-usar-cifrado-del-lado-del-servidor-con-aws-kms-sse-kms-después-de-realizar-este-cambio-el-rendimiento-de-la-aplicación-es-más-lento-cuál-es-la-causa-más-probable-de-la-latencia-de-la-aplicación) |
| 24 | [Un desarrollador necesita usar AWS X-Ray para monitorear una aplicación que está desplegada en instancias de EC2. ¿Qué pasos deben ejecutarse para realizar el monitoreo?](#un-desarrollador-necesita-usar-aws-x-ray-para-monitorear-una-aplicación-que-está-desplegada-en-instancias-de-ec2-qué-pasos-deben-ejecutarse-para-realizar-el-monitoreo) |
| 25 | [Un desarrollador ha creado un bucket de S3` s3://mycoolapp` y ha habilitado el registro de acceso al servidor que apunta a la carpeta `s3://mycoolapp/logs`. El desarrollador movió 100 KB de documentos de hojas de estilo en cascada (CSS) a la carpeta `s3://mycoolapp/css` y luego dejó de trabajar. Cuando el desarrollador regresó unos días después, el bucket pesaba 50 GB. ¿Cuál es la causa MÁS probable de esta situación?](#un-desarrollador-ha-creado-un-bucket-de-s3-s3mycoolapp-y-ha-habilitado-el-registro-de-acceso-al-servidor-que-apunta-a-la-carpeta-s3mycoolapplogs-el-desarrollador-movió-100-kb-de-documentos-de-hojas-de-estilo-en-cascada-css-a-la-carpeta-s3mycoolappcss-y-luego-dejó-de-trabajar-cuando-el-desarrollador-regresó-unos-días-después-el-bucket-pesaba-50-gb-cuál-es-la-causa-más-probable-de-esta-situación) |
| 26 | [Una empresa está usando AWS CodeBuild para compilar un sitio web a partir de código fuente almacenado en AWS CodeCommit. Un cambio reciente en el código fuente ha provocado que el proyecto de CodeBuild no pueda compilar el sitio web correctamente. ¿Cómo debería el desarrollador identificar la causa de las fallas?](#una-empresa-está-usando-aws-codebuild-para-compilar-un-sitio-web-a-partir-de-código-fuente-almacenado-en-aws-codecommit-un-cambio-reciente-en-el-código-fuente-ha-provocado-que-el-proyecto-de-codebuild-no-pueda-compilar-el-sitio-web-correctamente-cómo-debería-el-desarrollador-identificar-la-causa-de-las-fallas) |
| 27 | [Un desarrollador ejecutó un comando de la AWS CLI y recibió el error que se muestra a continuación. ¿Qué acción debería realizar el desarrollador para que este error sea legible para las personas?](#un-desarrollador-ejecutó-un-comando-de-la-aws-cli-y-recibió-el-error-que-se-muestra-a-continuación-qué-acción-debería-realizar-el-desarrollador-para-que-este-error-sea-legible-para-las-personas) |
| 28 | [Una aplicación deja de funcionar con el siguiente error: `The specified bucket does not exist`. ¿Cuál es el MEJOR lugar para comenzar el análisis de la causa raíz?](#una-aplicación-deja-de-funcionar-con-el-siguiente-error-the-specified-bucket-does-not-exist-cuál-es-el-mejor-lugar-para-comenzar-el-análisis-de-la-causa-raíz) |
| 29 | [Una empresa está construyendo una aplicación de negociación de acciones que requiere una latencia de submilisegundos al procesar las solicitudes de negociación. Amazon DynamoDB se usa para almacenar todos los datos de negociación que se utilizan para procesar cada solicitud. Tras las pruebas de carga de la aplicación, el equipo de desarrollo encontró que, debido a los tiempos de recuperación de datos, no se cumple el requisito de latencia. Debido a los picos repentinos en el número de solicitudes, la capacidad de lectura de DynamoDB tiene que estar significativamente sobreaprovisionada para evitar el throttling. ¿Qué pasos se deben seguir para cumplir con los requisitos de latencia y reducir el costo de ejecución de la aplicación?](#una-empresa-está-construyendo-una-aplicación-de-negociación-de-acciones-que-requiere-una-latencia-de-submilisegundos-al-procesar-las-solicitudes-de-negociación-amazon-dynamodb-se-usa-para-almacenar-todos-los-datos-de-negociación-que-se-utilizan-para-procesar-cada-solicitud-tras-las-pruebas-de-carga-de-la-aplicación-el-equipo-de-desarrollo-encontró-que-debido-a-los-tiempos-de-recuperación-de-datos-no-se-cumple-el-requisito-de-latencia-debido-a-los-picos-repentinos-en-el-número-de-solicitudes-la-capacidad-de-lectura-de-dynamodb-tiene-que-estar-significativamente-sobreaprovisionada-para-evitar-el-throttling-qué-pasos-se-deben-seguir-para-cumplir-con-los-requisitos-de-latencia-y-reducir-el-costo-de-ejecución-de-la-aplicación) |
| 30 | [Un desarrollador creó una función Lambda para el backend de una aplicación web. Al probar la función Lambda desde la consola de AWS Lambda, el desarrollador puede ver que la función se está ejecutando, pero no se genera ningún dato de log en Amazon CloudWatch Logs, incluso después de varios minutos. ¿Qué podría causar esta situación?](#un-desarrollador-creó-una-función-lambda-para-el-backend-de-una-aplicación-web-al-probar-la-función-lambda-desde-la-consola-de-aws-lambda-el-desarrollador-puede-ver-que-la-función-se-está-ejecutando-pero-no-se-genera-ningún-dato-de-log-en-amazon-cloudwatch-logs-incluso-después-de-varios-minutos-qué-podría-causar-esta-situación) |
| 31 | [Un desarrollador quiere usar AWS X-Ray para rastrear una solicitud de usuario de extremo a extremo a lo largo de la pila de software. El desarrollador realizó los cambios necesarios en la aplicación, la probó y encontró que la aplicación puede enviar las trazas a AWS X-Ray. Sin embargo, cuando la aplicación se despliega en una instancia EC2, las trazas no están disponibles. ¿Cuáles de los siguientes podrían crear esta situación? (Elija DOS)](#un-desarrollador-quiere-usar-aws-x-ray-para-rastrear-una-solicitud-de-usuario-de-extremo-a-extremo-a-lo-largo-de-la-pila-de-software-el-desarrollador-realizó-los-cambios-necesarios-en-la-aplicación-la-probó-y-encontró-que-la-aplicación-puede-enviar-las-trazas-a-aws-x-ray-sin-embargo-cuando-la-aplicación-se-despliega-en-una-instancia-ec2-las-trazas-no-están-disponibles-cuáles-de-los-siguientes-podrían-crear-esta-situación-elija-dos) |
| 32 | [Un desarrollador está probando una aplicación que invoca una función de AWS Lambda de forma asíncrona. Durante la fase de pruebas, la función Lambda no logra procesar tras dos reintentos. ¿Cómo puede el desarrollador solucionar el problema de la falla?](#un-desarrollador-está-probando-una-aplicación-que-invoca-una-función-de-aws-lambda-de-forma-asíncrona-durante-la-fase-de-pruebas-la-función-lambda-no-logra-procesar-tras-dos-reintentos-cómo-puede-el-desarrollador-solucionar-el-problema-de-la-falla) |
| 33 | [Una startup de comercio electrónico se está preparando para un evento anual de ventas. A medida que aumenta el tráfico hacia la aplicación de la empresa, el equipo de desarrollo quiere recibir una notificación cuando la utilización de CPU de la instancia de Amazon EC2 supere el 80 %. ¿Qué solución cumplirá con este requisito?](#una-startup-de-comercio-electrónico-se-está-preparando-para-un-evento-anual-de-ventas-a-medida-que-aumenta-el-tráfico-hacia-la-aplicación-de-la-empresa-el-equipo-de-desarrollo-quiere-recibir-una-notificación-cuando-la-utilización-de-cpu-de-la-instancia-de-amazon-ec2-supere-el-80--qué-solución-cumplirá-con-este-requisito) |
| 34 | [Un desarrollador recibe el siguiente mensaje de error al intentar lanzar o terminar una instancia de Amazon EC2 usando un script de boto3. ¿Qué debe hacer el desarrollador para corregir este mensaje de error?](#un-desarrollador-recibe-el-siguiente-mensaje-de-error-al-intentar-lanzar-o-terminar-una-instancia-de-amazon-ec2-usando-un-script-de-boto3-qué-debe-hacer-el-desarrollador-para-corregir-este-mensaje-de-error) |
| 35 | [Un desarrollador está usando Amazon DynamoDB para almacenar datos de la aplicación. El desarrollador quiere mejorar aún más el rendimiento de la aplicación reduciendo los tiempos de respuesta de las operaciones de lectura y escritura. ¿Qué característica de DynamoDB se debe usar para cumplir con estos requisitos?](#un-desarrollador-está-usando-amazon-dynamodb-para-almacenar-datos-de-la-aplicación-el-desarrollador-quiere-mejorar-aún-más-el-rendimiento-de-la-aplicación-reduciendo-los-tiempos-de-respuesta-de-las-operaciones-de-lectura-y-escritura-qué-característica-de-dynamodb-se-debe-usar-para-cumplir-con-estos-requisitos) |
| 36 | [Un desarrollador ha escrito una función de AWS Lambda usando Java como entorno de ejecución. El desarrollador quiere aislar un cuello de botella de rendimiento en el código. ¿Qué pasos se deben seguir para revelar el cuello de botella?](#un-desarrollador-ha-escrito-una-función-de-aws-lambda-usando-java-como-entorno-de-ejecución-el-desarrollador-quiere-aislar-un-cuello-de-botella-de-rendimiento-en-el-código-qué-pasos-se-deben-seguir-para-revelar-el-cuello-de-botella) |
| 37 | [Un desarrollador agregó una nueva funcionalidad a una aplicación que se ejecuta en una instancia de Amazon EC2 y que usa Amazon SQS. Después del despliegue, el desarrollador notó un aumento significativo en los costos de Amazon SQS. Al monitorear las métricas de Amazon SQS en Amazon CloudWatch, el desarrollador encontró que, en promedio, se publica un mensaje por minuto en esta cola. ¿Qué se puede hacer para reducir los costos de Amazon SQS de esta aplicación?](#un-desarrollador-agregó-una-nueva-funcionalidad-a-una-aplicación-que-se-ejecuta-en-una-instancia-de-amazon-ec2-y-que-usa-amazon-sqs-después-del-despliegue-el-desarrollador-notó-un-aumento-significativo-en-los-costos-de-amazon-sqs-al-monitorear-las-métricas-de-amazon-sqs-en-amazon-cloudwatch-el-desarrollador-encontró-que-en-promedio-se-publica-un-mensaje-por-minuto-en-esta-cola-qué-se-puede-hacer-para-reducir-los-costos-de-amazon-sqs-de-esta-aplicación) |
| 38 | [Un desarrollador está creando una aplicación que usa un backend de API REST de Amazon API Gateway respaldado por una función de AWS Lambda que interactúa con una tabla de Amazon DynamoDB. Durante las pruebas, el desarrollador observa una latencia alta al hacer solicitudes a la API. ¿Cómo puede el desarrollador evaluar la latencia de extremo a extremo e identificar los cuellos de botella de rendimiento?](#un-desarrollador-está-creando-una-aplicación-que-usa-un-backend-de-api-rest-de-amazon-api-gateway-respaldado-por-una-función-de-aws-lambda-que-interactúa-con-una-tabla-de-amazon-dynamodb-durante-las-pruebas-el-desarrollador-observa-una-latencia-alta-al-hacer-solicitudes-a-la-api-cómo-puede-el-desarrollador-evaluar-la-latencia-de-extremo-a-extremo-e-identificar-los-cuellos-de-botella-de-rendimiento) |
| 39 | [¿Qué se requiere para rastrear aplicaciones basadas en Lambda con AWS X-Ray?](#qué-se-requiere-para-rastrear-aplicaciones-basadas-en-lambda-con-aws-x-ray) |
| 40 | [Una empresa requiere que las funciones de AWS Lambda escritas por los desarrolladores registren errores para que los administradores de sistemas puedan solucionar problemas de forma más eficaz. ¿Qué deberían implementar los desarrolladores para cumplir esta necesidad?](#una-empresa-requiere-que-las-funciones-de-aws-lambda-escritas-por-los-desarrolladores-registren-errores-para-que-los-administradores-de-sistemas-puedan-solucionar-problemas-de-forma-más-eficaz-qué-deberían-implementar-los-desarrolladores-para-cumplir-esta-necesidad) |
| 41 | [Una aplicación presenta problemas de rendimiento debido a una mayor demanda. Esta mayor demanda se da sobre registros históricos de solo lectura extraídos de una base de datos alojada en Amazon RDS con vistas y consultas personalizadas. Un desarrollador debe mejorar el rendimiento sin cambiar la estructura de la base de datos. ¿Qué enfoque mejorará el rendimiento y MINIMIZARÁ la sobrecarga de administración?](#una-aplicación-presenta-problemas-de-rendimiento-debido-a-una-mayor-demanda-esta-mayor-demanda-se-da-sobre-registros-históricos-de-solo-lectura-extraídos-de-una-base-de-datos-alojada-en-amazon-rds-con-vistas-y-consultas-personalizadas-un-desarrollador-debe-mejorar-el-rendimiento-sin-cambiar-la-estructura-de-la-base-de-datos-qué-enfoque-mejorará-el-rendimiento-y-minimizará-la-sobrecarga-de-administración) |
| 42 | [Una aplicación usa una instancia de Amazon ElastiCache for Redis de un solo nodo para mejorar el rendimiento de lectura. Con el tiempo, la demanda de la aplicación ha aumentado exponencialmente, lo que ha incrementado la carga sobre la instancia de ElastiCache. Es crítico que esta capa de caché soporte la carga y sea resiliente ante fallas de nodos. ¿Qué puede hacer el desarrollador para abordar los requisitos de carga y resiliencia?](#una-aplicación-usa-una-instancia-de-amazon-elasticache-for-redis-de-un-solo-nodo-para-mejorar-el-rendimiento-de-lectura-con-el-tiempo-la-demanda-de-la-aplicación-ha-aumentado-exponencialmente-lo-que-ha-incrementado-la-carga-sobre-la-instancia-de-elasticache-es-crítico-que-esta-capa-de-caché-soporte-la-carga-y-sea-resiliente-ante-fallas-de-nodos-qué-puede-hacer-el-desarrollador-para-abordar-los-requisitos-de-carga-y-resiliencia) |
| 43 | [Un desarrollador está investigando problemas de rendimiento de una aplicación. La aplicación consta de cientos de microservicios, y una sola llamada a la API puede tener potencialmente una pila de llamadas profunda. El desarrollador debe aislar el componente que causa el problema. ¿Qué servicio o característica de AWS debería usar el desarrollador para recopilar información sobre lo que sucede y aislar la falla?](#un-desarrollador-está-investigando-problemas-de-rendimiento-de-una-aplicación-la-aplicación-consta-de-cientos-de-microservicios-y-una-sola-llamada-a-la-api-puede-tener-potencialmente-una-pila-de-llamadas-profunda-el-desarrollador-debe-aislar-el-componente-que-causa-el-problema-qué-servicio-o-característica-de-aws-debería-usar-el-desarrollador-para-recopilar-información-sobre-lo-que-sucede-y-aislar-la-falla) |
| 44 | [Un desarrollador registró una función de AWS Lambda como destino (target) de un Application Load Balancer (ALB) mediante un comando de CLI. Sin embargo, la función Lambda no se invoca cuando el cliente envía solicitudes a través del ALB. ¿Por qué no se invoca la función Lambda?](#un-desarrollador-registró-una-función-de-aws-lambda-como-destino-target-de-un-application-load-balancer-alb-mediante-un-comando-de-cli-sin-embargo-la-función-lambda-no-se-invoca-cuando-el-cliente-envía-solicitudes-a-través-del-alb-por-qué-no-se-invoca-la-función-lambda) |
| 45 | [Un desarrollador intenta monitorear el estado de una aplicación ejecutando un cron job que devuelve 1 si el servicio está activo y 0 si está inactivo. El desarrollador creó código que usa un comando `put-metric-alarm` de la AWS CLI para publicar las métricas personalizadas en Amazon CloudWatch y crear una alarma. Sin embargo, el desarrollador no puede crear una alarma porque las métricas personalizadas no aparecen en la consola de CloudWatch. ¿Qué causa este problema?](#un-desarrollador-intenta-monitorear-el-estado-de-una-aplicación-ejecutando-un-cron-job-que-devuelve-1-si-el-servicio-está-activo-y-0-si-está-inactivo-el-desarrollador-creó-código-que-usa-un-comando-put-metric-alarm-de-la-aws-cli-para-publicar-las-métricas-personalizadas-en-amazon-cloudwatch-y-crear-una-alarma-sin-embargo-el-desarrollador-no-puede-crear-una-alarma-porque-las-métricas-personalizadas-no-aparecen-en-la-consola-de-cloudwatch-qué-causa-este-problema) |
| 46 | [Un desarrollador ha escrito una aplicación que se ejecuta en instancias de Amazon EC2 y genera un valor cada minuto. El desarrollador quiere monitorear y graficar los valores generados a lo largo del tiempo sin iniciar sesión en la instancia cada vez. ¿Qué enfoque debería usar el desarrollador para lograr este objetivo?](#un-desarrollador-ha-escrito-una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-y-genera-un-valor-cada-minuto-el-desarrollador-quiere-monitorear-y-graficar-los-valores-generados-a-lo-largo-del-tiempo-sin-iniciar-sesión-en-la-instancia-cada-vez-qué-enfoque-debería-usar-el-desarrollador-para-lograr-este-objetivo) |
| 47 | [Una empresa está lanzando un sitio web de comercio electrónico y alojará los datos estáticos en Amazon S3. La empresa espera aproximadamente 1,000 transacciones por segundo (TPS) para solicitudes GET y PUT en total. Se debe habilitar el registro (logging) para rastrear todas las solicitudes y debe conservarse con fines de auditoría. ¿Cuál es la solución MÁS rentable?](#una-empresa-está-lanzando-un-sitio-web-de-comercio-electrónico-y-alojará-los-datos-estáticos-en-amazon-s3-la-empresa-espera-aproximadamente-1000-transacciones-por-segundo-tps-para-solicitudes-get-y-put-en-total-se-debe-habilitar-el-registro-logging-para-rastrear-todas-las-solicitudes-y-debe-conservarse-con-fines-de-auditoría-cuál-es-la-solución-más-rentable) |
| 48 | [Un Developer ha escrito una aplicación de Amazon Kinesis Data Streams. A medida que el uso crece y el tráfico aumenta con el tiempo, la aplicación recibe regularmente mensajes de error `ProvisionedThroughputExceededException`. ¿Qué pasos debe seguir el Developer para resolver el error? (Elija DOS)](#un-developer-ha-escrito-una-aplicación-de-amazon-kinesis-data-streams-a-medida-que-el-uso-crece-y-el-tráfico-aumenta-con-el-tiempo-la-aplicación-recibe-regularmente-mensajes-de-error-provisionedthroughputexceededexception-qué-pasos-debe-seguir-el-developer-para-resolver-el-error-elija-dos) |
| 49 | [Un Software Engineer desarrolló una función de AWS Lambda en Node.js para realizar un procesamiento de datos que requiere mucha CPU. Con la configuración predeterminada, la función de Lambda tarda unos 5 minutos en completarse. ¿Qué enfoque debe adoptar un Developer para aumentar la velocidad de finalización?](#un-software-engineer-desarrolló-una-función-de-aws-lambda-en-nodejs-para-realizar-un-procesamiento-de-datos-que-requiere-mucha-cpu-con-la-configuración-predeterminada-la-función-de-lambda-tarda-unos-5-minutos-en-completarse-qué-enfoque-debe-adoptar-un-developer-para-aumentar-la-velocidad-de-finalización) |
| 50 | [Un Developer tiene una aplicación heredada alojada on-premises. Otras aplicaciones alojadas en AWS dependen de la aplicación on-premises para su correcto funcionamiento. En caso de errores en las aplicaciones, el Developer quiere poder usar Amazon CloudWatch para monitorear y solucionar problemas de todas las aplicaciones desde un solo lugar. ¿Cómo puede lograrlo el Developer?](#un-developer-tiene-una-aplicación-heredada-alojada-on-premises-otras-aplicaciones-alojadas-en-aws-dependen-de-la-aplicación-on-premises-para-su-correcto-funcionamiento-en-caso-de-errores-en-las-aplicaciones-el-developer-quiere-poder-usar-amazon-cloudwatch-para-monitorear-y-solucionar-problemas-de-todas-las-aplicaciones-desde-un-solo-lugar-cómo-puede-lograrlo-el-developer) |
| 51 | [Un Developer está trabajando en un proyecto sin servidor basado en Java. Las pruebas iniciales muestran que un cold start tarda en promedio unos 8 segundos en las funciones de AWS Lambda. ¿Qué debe hacer el Developer para reducir el tiempo de cold start? (Elija DOS)](#un-developer-está-trabajando-en-un-proyecto-sin-servidor-basado-en-java-las-pruebas-iniciales-muestran-que-un-cold-start-tarda-en-promedio-unos-8-segundos-en-las-funciones-de-aws-lambda-qué-debe-hacer-el-developer-para-reducir-el-tiempo-de-cold-start-elija-dos) |
| 52 | [Un Developer está aprovechando una conexión AWS VPN basada en Border Gateway Protocol (BGP) para conectarse desde on-premises a instancias de Amazon EC2 en la cuenta del Developer. El Developer puede acceder a una instancia de EC2 en la subred A, pero no puede acceder a una instancia de EC2 en la subred B de la misma VPC. ¿Qué registros puede usar el Developer para verificar si el tráfico está llegando a la subred B?](#un-developer-está-aprovechando-una-conexión-aws-vpn-basada-en-border-gateway-protocol-bgp-para-conectarse-desde-on-premises-a-instancias-de-amazon-ec2-en-la-cuenta-del-developer-el-developer-puede-acceder-a-una-instancia-de-ec2-en-la-subred-a-pero-no-puede-acceder-a-una-instancia-de-ec2-en-la-subred-b-de-la-misma-vpc-qué-registros-puede-usar-el-developer-para-verificar-si-el-tráfico-está-llegando-a-la-subred-b) |
| 53 | [El sitio web de una empresa se ejecuta en una instancia de Amazon EC2 y usa Auto Scaling para escalar el entorno en horas pico. Los usuarios del sitio web en todo el mundo experimentan alta latencia debido al contenido estático en la instancia de EC2, incluso en horas no pico. ¿Qué combinación de pasos resolverá el problema de latencia? (Elija DOS)](#el-sitio-web-de-una-empresa-se-ejecuta-en-una-instancia-de-amazon-ec2-y-usa-auto-scaling-para-escalar-el-entorno-en-horas-pico-los-usuarios-del-sitio-web-en-todo-el-mundo-experimentan-alta-latencia-debido-al-contenido-estático-en-la-instancia-de-ec2-incluso-en-horas-no-pico-qué-combinación-de-pasos-resolverá-el-problema-de-latencia-elija-dos) |
| 54 | [Un Developer va a desplegar una función de AWS Lambda que requiere un uso significativo de CPU. ¿Qué enfoque MINIMIZARÁ el tiempo de ejecución promedio de la función?](#un-developer-va-a-desplegar-una-función-de-aws-lambda-que-requiere-un-uso-significativo-de-cpu-qué-enfoque-minimizará-el-tiempo-de-ejecución-promedio-de-la-función) |
| 55 | [Un Developer tiene una API de comercio electrónico alojada en Amazon ECS. La demanda variable y con picos en la aplicación está causando que el procesamiento de pedidos tarde demasiado. La aplicación procesa colas de Amazon SQS. La métrica `ApproximateNumberOfMessagesVisible` presenta picos de valores muy altos a lo largo del día, lo que provoca activaciones de alarmas de Amazon CloudWatch. Otras métricas de ECS para los contenedores de la API están muy por debajo de los límites. ¿Qué puede implementar el Developer para mejorar el rendimiento manteniendo bajos los costos?](#un-developer-tiene-una-api-de-comercio-electrónico-alojada-en-amazon-ecs-la-demanda-variable-y-con-picos-en-la-aplicación-está-causando-que-el-procesamiento-de-pedidos-tarde-demasiado-la-aplicación-procesa-colas-de-amazon-sqs-la-métrica-approximatenumberofmessagesvisible-presenta-picos-de-valores-muy-altos-a-lo-largo-del-día-lo-que-provoca-activaciones-de-alarmas-de-amazon-cloudwatch-otras-métricas-de-ecs-para-los-contenedores-de-la-api-están-muy-por-debajo-de-los-límites-qué-puede-implementar-el-developer-para-mejorar-el-rendimiento-manteniendo-bajos-los-costos) |
| 56 | [Una aplicación se ejecuta en un clúster de instancias de Amazon EC2. Al intentar leer objetos almacenados en un único bucket de Amazon S3 que están cifrados con cifrado del lado del servidor con claves administradas por AWS KMS (SSE-KMS), la aplicación recibe el siguiente error. ¿Qué combinación de pasos se debe seguir para evitar este fallo? (Elija DOS)](#una-aplicación-se-ejecuta-en-un-clúster-de-instancias-de-amazon-ec2-al-intentar-leer-objetos-almacenados-en-un-único-bucket-de-amazon-s3-que-están-cifrados-con-cifrado-del-lado-del-servidor-con-claves-administradas-por-aws-kms-sse-kms-la-aplicación-recibe-el-siguiente-error-qué-combinación-de-pasos-se-debe-seguir-para-evitar-este-fallo-elija-dos) |
| 57 | [Después de lanzar una instancia que pretende servir como dispositivo NAT (Network Address Translation) en una subred pública, usted modifica sus tablas de enrutamiento para que el dispositivo NAT sea el destino del tráfico con destino a Internet de su subred privada. Cuando intenta realizar una conexión saliente a Internet desde una instancia en la subred privada, no tiene éxito. El dispositivo NAT debe ser el destino del tráfico con destino a Internet de su subred privada. ¿Cuál de los siguientes pasos podría resolver el problema?](#después-de-lanzar-una-instancia-que-pretende-servir-como-dispositivo-nat-network-address-translation-en-una-subred-pública-usted-modifica-sus-tablas-de-enrutamiento-para-que-el-dispositivo-nat-sea-el-destino-del-tráfico-con-destino-a-internet-de-su-subred-privada-cuando-intenta-realizar-una-conexión-saliente-a-internet-desde-una-instancia-en-la-subred-privada-no-tiene-éxito-el-dispositivo-nat-debe-ser-el-destino-del-tráfico-con-destino-a-internet-de-su-subred-privada-cuál-de-los-siguientes-pasos-podría-resolver-el-problema) |
| 58 | [Usted tiene un entorno que consta de una subred pública con Amazon VPC y 3 instancias que se ejecutan en esta subred. Estas tres instancias pueden comunicarse correctamente con otros hosts en Internet. Usted lanza una cuarta instancia en la misma subred, usando la misma AMI y la misma configuración de security group que usó para las otras, pero descubre que no se puede acceder a esta instancia desde Internet. ¿Qué debe hacer para habilitar el acceso a Internet?](#usted-tiene-un-entorno-que-consta-de-una-subred-pública-con-amazon-vpc-y-3-instancias-que-se-ejecutan-en-esta-subred-estas-tres-instancias-pueden-comunicarse-correctamente-con-otros-hosts-en-internet-usted-lanza-una-cuarta-instancia-en-la-misma-subred-usando-la-misma-ami-y-la-misma-configuración-de-security-group-que-usó-para-las-otras-pero-descubre-que-no-se-puede-acceder-a-esta-instancia-desde-internet-qué-debe-hacer-para-habilitar-el-acceso-a-internet) |
| 59 | [Al usar una operación Scan grande en DynamoDB, ¿qué técnica se puede utilizar para minimizar el impacto de un scan en el throughput aprovisionado de una tabla?](#al-usar-una-operación-scan-grande-en-dynamodb-qué-técnica-se-puede-utilizar-para-minimizar-el-impacto-de-un-scan-en-el-throughput-aprovisionado-de-una-tabla) |
| 60 | [El sitio de intercambio de fotos de una startup está desplegado en una VPC. Un ELB distribuye el tráfico web entre dos subnets. La session stickiness del ELB está configurada para usar la cookie de sesión generada por AWS, con un TTL de sesión de 5 minutos. El Auto Scaling Group de servidores web está configurado como: `min-size=4`, `max-size=4`. La startup se prepara para un lanzamiento público ejecutando software de pruebas de carga instalado en una única instancia EC2 que se ejecuta en `us-west-2`. Después de 60 minutos de pruebas de carga, los logs de los servidores web muestran lo siguiente. ¿Qué recomendaciones pueden ayudar a asegurar que las solicitudes HTTP de las pruebas de carga se distribuyan uniformemente entre los cuatro servidores web? (Elija DOS)](#el-sitio-de-intercambio-de-fotos-de-una-startup-está-desplegado-en-una-vpc-un-elb-distribuye-el-tráfico-web-entre-dos-subnets-la-session-stickiness-del-elb-está-configurada-para-usar-la-cookie-de-sesión-generada-por-aws-con-un-ttl-de-sesión-de-5-minutos-el-auto-scaling-group-de-servidores-web-está-configurado-como-min-size4-max-size4-la-startup-se-prepara-para-un-lanzamiento-público-ejecutando-software-de-pruebas-de-carga-instalado-en-una-única-instancia-ec2-que-se-ejecuta-en-us-west-2-después-de-60-minutos-de-pruebas-de-carga-los-logs-de-los-servidores-web-muestran-lo-siguiente-qué-recomendaciones-pueden-ayudar-a-asegurar-que-las-solicitudes-http-de-las-pruebas-de-carga-se-distribuyan-uniformemente-entre-los-cuatro-servidores-web-elija-dos) |
| 61 | [¿Cuáles de los siguientes servicios se incluyen sin costo adicional con el uso de la plataforma AWS?](#cuáles-de-los-siguientes-servicios-se-incluyen-sin-costo-adicional-con-el-uso-de-la-plataforma-aws) |
| 62 | [En DynamoDB, ¿qué tipo de códigos de respuesta HTTP indica que se encontró un problema con la solicitud del cliente enviada al servicio?](#en-dynamodb-qué-tipo-de-códigos-de-respuesta-http-indica-que-se-encontró-un-problema-con-la-solicitud-del-cliente-enviada-al-servicio) |
| 63 | [La Empresa B ofrece un servicio de reconocimiento de imágenes en línea y utiliza SQS para desacoplar los componentes del sistema y lograr escalabilidad. Los consumidores de SQS consultan (poll) la cola de imágenes con la mayor frecuencia posible para mantener lo más alto posible el throughput de extremo a extremo. Sin embargo, la Empresa B se da cuenta de que consultar en bucles cerrados consume ciclos de CPU y aumenta los costos con respuestas vacías. ¿Cómo puede la Empresa B reducir el número de respuestas vacías?](#la-empresa-b-ofrece-un-servicio-de-reconocimiento-de-imágenes-en-línea-y-utiliza-sqs-para-desacoplar-los-componentes-del-sistema-y-lograr-escalabilidad-los-consumidores-de-sqs-consultan-poll-la-cola-de-imágenes-con-la-mayor-frecuencia-posible-para-mantener-lo-más-alto-posible-el-throughput-de-extremo-a-extremo-sin-embargo-la-empresa-b-se-da-cuenta-de-que-consultar-en-bucles-cerrados-consume-ciclos-de-cpu-y-aumenta-los-costos-con-respuestas-vacías-cómo-puede-la-empresa-b-reducir-el-número-de-respuestas-vacías) |
| 64 | [Usted inserta 1000 elementos nuevos cada segundo en una tabla de DynamoDB. Una vez por hora estos elementos se analizan y luego ya no se necesitan. Necesita minimizar el throughput aprovisionado, el almacenamiento y las llamadas a la API. Dados estos requisitos, ¿cuál es la forma más eficiente de gestionar estos elementos después del análisis?](#usted-inserta-1000-elementos-nuevos-cada-segundo-en-una-tabla-de-dynamodb-una-vez-por-hora-estos-elementos-se-analizan-y-luego-ya-no-se-necesitan-necesita-minimizar-el-throughput-aprovisionado-el-almacenamiento-y-las-llamadas-a-la-api-dados-estos-requisitos-cuál-es-la-forma-más-eficiente-de-gestionar-estos-elementos-después-del-análisis) |
| 65 | [Está escribiendo en una tabla de DynamoDB y recibe la siguiente excepción: `ProvisionedThroughputExceededException`, aunque según las métricas de CloudWatch de la tabla no está excediendo su throughput aprovisionado. ¿Cuál podría ser una explicación?](#está-escribiendo-en-una-tabla-de-dynamodb-y-recibe-la-siguiente-excepción-provisionedthroughputexceededexception-aunque-según-las-métricas-de-cloudwatch-de-la-tabla-no-está-excediendo-su-throughput-aprovisionado-cuál-podría-ser-una-explicación) |
| 66 | [Si una aplicación almacena archivos de log por hora de miles de instancias de un sitio web de alto tráfico, ¿qué esquema de nombres daría el rendimiento óptimo en S3?](#si-una-aplicación-almacena-archivos-de-log-por-hora-de-miles-de-instancias-de-un-sitio-web-de-alto-tráfico-qué-esquema-de-nombres-daría-el-rendimiento-óptimo-en-s3) |
| 67 | [Un equipo de desarrollo quiere instrumentar su código para proporcionar a AWS X-Ray información más detallada que las simples solicitudes salientes y entrantes. Esto generará grandes cantidades de datos, por lo que el equipo de desarrollo quiere implementar indexación para poder filtrar los datos. ¿Qué debe hacer el equipo de desarrollo para lograrlo?](#un-equipo-de-desarrollo-quiere-instrumentar-su-código-para-proporcionar-a-aws-x-ray-información-más-detallada-que-las-simples-solicitudes-salientes-y-entrantes-esto-generará-grandes-cantidades-de-datos-por-lo-que-el-equipo-de-desarrollo-quiere-implementar-indexación-para-poder-filtrar-los-datos-qué-debe-hacer-el-equipo-de-desarrollo-para-lograrlo) |
| 68 | [Una tabla de Amazon DynamoDB utiliza un Global Secondary Index (GSI) para soportar consultas de lectura. La tabla principal tiene mucha carga de escritura, mientras que el GSI se usa para operaciones de lectura. Al revisar las métricas de Amazon CloudWatch, el desarrollador nota que las operaciones de escritura a la tabla principal sufren limitación (throttling) con frecuencia durante una alta actividad de escritura. Sin embargo, las unidades de capacidad de escritura de la tabla principal están disponibles y no se consumen por completo. ¿Por qué se está limitando la tabla?](#una-tabla-de-amazon-dynamodb-utiliza-un-global-secondary-index-gsi-para-soportar-consultas-de-lectura-la-tabla-principal-tiene-mucha-carga-de-escritura-mientras-que-el-gsi-se-usa-para-operaciones-de-lectura-al-revisar-las-métricas-de-amazon-cloudwatch-el-desarrollador-nota-que-las-operaciones-de-escritura-a-la-tabla-principal-sufren-limitación-throttling-con-frecuencia-durante-una-alta-actividad-de-escritura-sin-embargo-las-unidades-de-capacidad-de-escritura-de-la-tabla-principal-están-disponibles-y-no-se-consumen-por-completo-por-qué-se-está-limitando-la-tabla) |
| 69 | [Una empresa ejecuta una aplicación Docker en Amazon ECS. La aplicación debe escalar según la carga de usuarios de los últimos 15 segundos. ¿Cómo debe instrumentar el código un desarrollador para cumplir el requisito?](#una-empresa-ejecuta-una-aplicación-docker-en-amazon-ecs-la-aplicación-debe-escalar-según-la-carga-de-usuarios-de-los-últimos-15-segundos-cómo-debe-instrumentar-el-código-un-desarrollador-para-cumplir-el-requisito) |
| 70 | [Un desarrollador está construyendo una aplicación web que utiliza Amazon API Gateway para exponer una función de AWS Lambda que procesa solicitudes de clientes. Durante las pruebas, el desarrollador nota que API Gateway sufre timeout aunque la función de Lambda termina dentro del límite de tiempo establecido. ¿Cuáles de las siguientes métricas de API Gateway en Amazon CloudWatch pueden ayudar al desarrollador a solucionar el problema? (Elija DOS)](#un-desarrollador-está-construyendo-una-aplicación-web-que-utiliza-amazon-api-gateway-para-exponer-una-función-de-aws-lambda-que-procesa-solicitudes-de-clientes-durante-las-pruebas-el-desarrollador-nota-que-api-gateway-sufre-timeout-aunque-la-función-de-lambda-termina-dentro-del-límite-de-tiempo-establecido-cuáles-de-las-siguientes-métricas-de-api-gateway-en-amazon-cloudwatch-pueden-ayudar-al-desarrollador-a-solucionar-el-problema-elija-dos) |
| 71 | [Un desarrollador debe analizar problemas de rendimiento en aplicaciones distribuidas de producción escritas como funciones de AWS Lambda. Estas aplicaciones Lambda distribuidas invocan otros componentes que conforman las aplicaciones. ¿Cómo debe el desarrollador identificar y solucionar la causa raíz de los problemas de rendimiento en producción?](#un-desarrollador-debe-analizar-problemas-de-rendimiento-en-aplicaciones-distribuidas-de-producción-escritas-como-funciones-de-aws-lambda-estas-aplicaciones-lambda-distribuidas-invocan-otros-componentes-que-conforman-las-aplicaciones-cómo-debe-el-desarrollador-identificar-y-solucionar-la-causa-raíz-de-los-problemas-de-rendimiento-en-producción) |
| 72 | [Un desarrollador quiere depurar una aplicación buscando y filtrando datos de log. Los logs de la aplicación se almacenan en Amazon CloudWatch Logs. El desarrollador crea un nuevo metric filter para contar las excepciones en los logs de la aplicación. Sin embargo, no se devuelven resultados de los logs. ¿Cuál es la razón por la que no se devuelven resultados filtrados?](#un-desarrollador-quiere-depurar-una-aplicación-buscando-y-filtrando-datos-de-log-los-logs-de-la-aplicación-se-almacenan-en-amazon-cloudwatch-logs-el-desarrollador-crea-un-nuevo-metric-filter-para-contar-las-excepciones-en-los-logs-de-la-aplicación-sin-embargo-no-se-devuelven-resultados-de-los-logs-cuál-es-la-razón-por-la-que-no-se-devuelven-resultados-filtrados) |
| 73 | [Una empresa utiliza instancias de Amazon RDS MySQL para la capa de base de datos de su aplicación y servidores Apache Tomcat para su capa web. La mayoría de las consultas a la base de datos desde las aplicaciones web son solicitudes de lectura repetidas. ¿El uso de qué servicio de AWS aumentaría el rendimiento al agregar un almacén en memoria para las consultas de lectura repetidas?](#una-empresa-utiliza-instancias-de-amazon-rds-mysql-para-la-capa-de-base-de-datos-de-su-aplicación-y-servidores-apache-tomcat-para-su-capa-web-la-mayoría-de-las-consultas-a-la-base-de-datos-desde-las-aplicaciones-web-son-solicitudes-de-lectura-repetidas-el-uso-de-qué-servicio-de-aws-aumentaría-el-rendimiento-al-agregar-un-almacén-en-memoria-para-las-consultas-de-lectura-repetidas) |
| 74 | [Un desarrollador está investigando un problema por el cual ciertas solicitudes pasan por un endpoint de Amazon API Gateway /MyAPI, pero las solicitudes no llegan a la función de AWS Lambda que respalda /MyAPI. El desarrollador descubrió que una segunda función de Lambda a veces se ejecuta en la concurrencia máxima permitida para la cuenta de AWS dada. ¿Cómo puede el desarrollador resolver este problema?](#un-desarrollador-está-investigando-un-problema-por-el-cual-ciertas-solicitudes-pasan-por-un-endpoint-de-amazon-api-gateway-myapi-pero-las-solicitudes-no-llegan-a-la-función-de-aws-lambda-que-respalda-myapi-el-desarrollador-descubrió-que-una-segunda-función-de-lambda-a-veces-se-ejecuta-en-la-concurrencia-máxima-permitida-para-la-cuenta-de-aws-dada-cómo-puede-el-desarrollador-resolver-este-problema) |
| 75 | [Un desarrollador ha creado una función de Lambda y encuentra que la función tarda más de lo esperado en completarse. Después de depurar, el desarrollador ha descubierto que aumentar la capacidad de cómputo mejoraría el rendimiento. ¿Cómo puede el desarrollador aumentar los recursos de cómputo de Lambda?](#un-desarrollador-ha-creado-una-función-de-lambda-y-encuentra-que-la-función-tarda-más-de-lo-esperado-en-completarse-después-de-depurar-el-desarrollador-ha-descubierto-que-aumentar-la-capacidad-de-cómputo-mejoraría-el-rendimiento-cómo-puede-el-desarrollador-aumentar-los-recursos-de-cómputo-de-lambda) |
| 76 | [Un sitio de comercio electrónico permite que los usuarios recurrentes inicien sesión para mostrar páginas web personalizadas. El flujo de trabajo se muestra en la imagen a continuación. Una aplicación se ejecuta en instancias de EC2. Amazon RDS se utiliza para la base de datos que almacena las cuentas y preferencias de los usuarios. El sitio web se congela o carga lentamente mientras espera que se complete el paso de inicio de sesión. Los demás componentes del sitio están bien optimizados. ¿Cuáles de las siguientes técnicas resolverán este problema? (Seleccione DOS)](#un-sitio-de-comercio-electrónico-permite-que-los-usuarios-recurrentes-inicien-sesión-para-mostrar-páginas-web-personalizadas-el-flujo-de-trabajo-se-muestra-en-la-imagen-a-continuación-una-aplicación-se-ejecuta-en-instancias-de-ec2-amazon-rds-se-utiliza-para-la-base-de-datos-que-almacena-las-cuentas-y-preferencias-de-los-usuarios-el-sitio-web-se-congela-o-carga-lentamente-mientras-espera-que-se-complete-el-paso-de-inicio-de-sesión-los-demás-componentes-del-sitio-están-bien-optimizados-cuáles-de-las-siguientes-técnicas-resolverán-este-problema-seleccione-dos) |
| 77 | [Un desarrollador quiere que los datos de registro de una aplicación que se ejecuta en una instancia de EC2 estén disponibles para los administradores de sistemas. ¿Cuál de las siguientes opciones permite monitorear esta métrica en Amazon CloudWatch?](#un-desarrollador-quiere-que-los-datos-de-registro-de-una-aplicación-que-se-ejecuta-en-una-instancia-de-ec2-estén-disponibles-para-los-administradores-de-sistemas-cuál-de-las-siguientes-opciones-permite-monitorear-esta-métrica-en-amazon-cloudwatch) |
| 78 | [Una empresa tiene una aplicación que registra toda la información en Amazon S3. Cada vez que hay un nuevo archivo de registro, se invoca una función de AWS Lambda para procesar los archivos de registro. El código funciona y reúne toda la información necesaria. Sin embargo, al revisar los registros de la función Lambda, se encuentran entradas duplicadas con el mismo ID de solicitud. ¿Qué está causando las entradas duplicadas?](#una-empresa-tiene-una-aplicación-que-registra-toda-la-información-en-amazon-s3-cada-vez-que-hay-un-nuevo-archivo-de-registro-se-invoca-una-función-de-aws-lambda-para-procesar-los-archivos-de-registro-el-código-funciona-y-reúne-toda-la-información-necesaria-sin-embargo-al-revisar-los-registros-de-la-función-lambda-se-encuentran-entradas-duplicadas-con-el-mismo-id-de-solicitud-qué-está-causando-las-entradas-duplicadas) |
| 79 | [Un equipo de desarrollo ha puesto en producción 10 aplicaciones que se ejecutan en varias instancias de Amazon EC2. El equipo de operaciones solicita una representación gráfica de una métrica clave de rendimiento para cada aplicación. Estas métricas deben estar disponibles en una sola pantalla para facilitar el monitoreo. ¿Qué pasos debe seguir el desarrollador para lograr esto con Amazon CloudWatch?](#un-equipo-de-desarrollo-ha-puesto-en-producción-10-aplicaciones-que-se-ejecutan-en-varias-instancias-de-amazon-ec2-el-equipo-de-operaciones-solicita-una-representación-gráfica-de-una-métrica-clave-de-rendimiento-para-cada-aplicación-estas-métricas-deben-estar-disponibles-en-una-sola-pantalla-para-facilitar-el-monitoreo-qué-pasos-debe-seguir-el-desarrollador-para-lograr-esto-con-amazon-cloudwatch) |
| 80 | [Una empresa usa Amazon DynamoDB para administrar y rastrear pedidos. La tabla de DynamoDB está particionada según la fecha del pedido. La empresa recibe un aumento enorme de pedidos durante un evento de ventas, lo que causa limitación (throttling) en las escrituras de DynamoDB, y el rendimiento consumido está muy por debajo del rendimiento aprovisionado. De acuerdo con las mejores prácticas de AWS, ¿cómo se puede resolver este problema con costos MÍNIMOS?](#una-empresa-usa-amazon-dynamodb-para-administrar-y-rastrear-pedidos-la-tabla-de-dynamodb-está-particionada-según-la-fecha-del-pedido-la-empresa-recibe-un-aumento-enorme-de-pedidos-durante-un-evento-de-ventas-lo-que-causa-limitación-throttling-en-las-escrituras-de-dynamodb-y-el-rendimiento-consumido-está-muy-por-debajo-del-rendimiento-aprovisionado-de-acuerdo-con-las-mejores-prácticas-de-aws-cómo-se-puede-resolver-este-problema-con-costos-mínimos) |
| 81 | [Una empresa mantiene una aplicación responsable de procesar varios miles de callbacks externos cada día. Los administradores de sistemas de la empresa quieren saber cuántos callbacks se reciben de forma continua y quieren que estos datos estén disponibles durante 10 días. La empresa también quiere poder emitir alertas automáticas si el número de callbacks supera los umbrales definidos. ¿Cuál es la forma MÁS rentable de atender la necesidad de rastrear y alertar sobre estas estadísticas?](#una-empresa-mantiene-una-aplicación-responsable-de-procesar-varios-miles-de-callbacks-externos-cada-día-los-administradores-de-sistemas-de-la-empresa-quieren-saber-cuántos-callbacks-se-reciben-de-forma-continua-y-quieren-que-estos-datos-estén-disponibles-durante-10-días-la-empresa-también-quiere-poder-emitir-alertas-automáticas-si-el-número-de-callbacks-supera-los-umbrales-definidos-cuál-es-la-forma-más-rentable-de-atender-la-necesidad-de-rastrear-y-alertar-sobre-estas-estadísticas) |
| 82 | [Una empresa tiene una aplicación web de varios niveles en AWS. Durante un reciente pico de tráfico, una de las bases de datos relacionales principales en Amazon RDS no pudo atender todo el tráfico. Algunas consultas de lectura de elementos a los que se accede repetidamente fallaron, por lo que los usuarios recibieron mensajes de error. ¿Qué se puede hacer para minimizar el impacto en las consultas de lectura de la base de datos de la forma MÁS eficiente durante futuros picos de tráfico?](#una-empresa-tiene-una-aplicación-web-de-varios-niveles-en-aws-durante-un-reciente-pico-de-tráfico-una-de-las-bases-de-datos-relacionales-principales-en-amazon-rds-no-pudo-atender-todo-el-tráfico-algunas-consultas-de-lectura-de-elementos-a-los-que-se-accede-repetidamente-fallaron-por-lo-que-los-usuarios-recibieron-mensajes-de-error-qué-se-puede-hacer-para-minimizar-el-impacto-en-las-consultas-de-lectura-de-la-base-de-datos-de-la-forma-más-eficiente-durante-futuros-picos-de-tráfico) |
| 83 | [Un desarrollador está creando una función de AWS Lambda para procesar un flujo de datos de un Amazon Kinesis Data Stream. Cuando la función Lambda analiza los datos y encuentra un campo faltante, termina la función con un error. La función está generando registros duplicados a partir del flujo de Kinesis. Cuando el desarrollador examina la salida del flujo sin la función Lambda, no hay registros duplicados. ¿Cuál es el motivo de los duplicados?](#un-desarrollador-está-creando-una-función-de-aws-lambda-para-procesar-un-flujo-de-datos-de-un-amazon-kinesis-data-stream-cuando-la-función-lambda-analiza-los-datos-y-encuentra-un-campo-faltante-termina-la-función-con-un-error-la-función-está-generando-registros-duplicados-a-partir-del-flujo-de-kinesis-cuando-el-desarrollador-examina-la-salida-del-flujo-sin-la-función-lambda-no-hay-registros-duplicados-cuál-es-el-motivo-de-los-duplicados) |
| 84 | [Un desarrollador quiere habilitar AWS X-Ray para una aplicación segura que se ejecuta en un entorno de Amazon ECS. ¿Qué combinación de pasos habilitará X-Ray? (Seleccione TRES)](#un-desarrollador-quiere-habilitar-aws-x-ray-para-una-aplicación-segura-que-se-ejecuta-en-un-entorno-de-amazon-ecs-qué-combinación-de-pasos-habilitará-x-ray-seleccione-tres) |
| 85 | [Un desarrollador ha publicado una actualización de una aplicación que se sirve a una base de usuarios global mediante Amazon CloudFront. Después de implementar la aplicación, los usuarios no pueden ver los cambios actualizados. ¿Cómo puede el desarrollador resolver este problema?](#un-desarrollador-ha-publicado-una-actualización-de-una-aplicación-que-se-sirve-a-una-base-de-usuarios-global-mediante-amazon-cloudfront-después-de-implementar-la-aplicación-los-usuarios-no-pueden-ver-los-cambios-actualizados-cómo-puede-el-desarrollador-resolver-este-problema) |
| 86 | [Una empresa migró recientemente sus capas web, de aplicación y de base de datos NoSQL a AWS. La empresa usa Auto Scaling para escalar las capas web y de aplicación. Más del 95 por ciento de las solicitudes a Amazon DynamoDB son solicitudes de lectura repetidas. ¿Cómo se puede escalar la capa NoSQL de DynamoDB para almacenar en caché estas solicitudes repetidas?](#una-empresa-migró-recientemente-sus-capas-web-de-aplicación-y-de-base-de-datos-nosql-a-aws-la-empresa-usa-auto-scaling-para-escalar-las-capas-web-y-de-aplicación-más-del-95-por-ciento-de-las-solicitudes-a-amazon-dynamodb-son-solicitudes-de-lectura-repetidas-cómo-se-puede-escalar-la-capa-nosql-de-dynamodb-para-almacenar-en-caché-estas-solicitudes-repetidas) |
| 87 | [Mientras desarrolla una aplicación que se ejecuta en Amazon EC2 dentro de una Amazon VPC, un desarrollador identifica la necesidad de almacenamiento centralizado de los registros (logs) a nivel de aplicación. ¿Qué servicio de AWS se puede usar para almacenar estos registros de forma segura?](#mientras-desarrolla-una-aplicación-que-se-ejecuta-en-amazon-ec2-dentro-de-una-amazon-vpc-un-desarrollador-identifica-la-necesidad-de-almacenamiento-centralizado-de-los-registros-logs-a-nivel-de-aplicación-qué-servicio-de-aws-se-puede-usar-para-almacenar-estos-registros-de-forma-segura) |
| 88 | [Una aplicación de monitoreo del mercado bursátil usa Amazon Kinesis para la ingesta de datos. Durante pruebas simuladas de tasas de datos pico, el stream de Kinesis no puede seguir el ritmo de los datos entrantes. ¿Qué paso permitirá a Kinesis acomodar el tráfico durante las horas pico?](#una-aplicación-de-monitoreo-del-mercado-bursátil-usa-amazon-kinesis-para-la-ingesta-de-datos-durante-pruebas-simuladas-de-tasas-de-datos-pico-el-stream-de-kinesis-no-puede-seguir-el-ritmo-de-los-datos-entrantes-qué-paso-permitirá-a-kinesis-acomodar-el-tráfico-durante-las-horas-pico) |
| 89 | [Una aplicación usa funciones Lambda para extraer metadatos de archivos cargados a un bucket de S3; los metadatos se almacenan en Amazon DynamoDB. La aplicación comienza a comportarse de forma inesperada y el desarrollador quiere examinar los registros (logs) del código de la función Lambda en busca de errores. Según esta configuración del sistema, ¿dónde encontraría el desarrollador los registros?](#una-aplicación-usa-funciones-lambda-para-extraer-metadatos-de-archivos-cargados-a-un-bucket-de-s3-los-metadatos-se-almacenan-en-amazon-dynamodb-la-aplicación-comienza-a-comportarse-de-forma-inesperada-y-el-desarrollador-quiere-examinar-los-registros-logs-del-código-de-la-función-lambda-en-busca-de-errores-según-esta-configuración-del-sistema-dónde-encontraría-el-desarrollador-los-registros) |
| 90 | [Una empresa está usando AWS CodePipeline para entregar una de sus aplicaciones. La canalización de entrega se activa con los cambios en la rama master de un repositorio de AWS CodeCommit y usa AWS CodeBuild para implementar las etapas de prueba y compilación del proceso, y AWS CodeDeploy para desplegar la aplicación. La canalización ha estado funcionando correctamente durante varios meses y no ha habido modificaciones. Tras un cambio reciente en el código fuente de la aplicación, AWS CodeDeploy no ha desplegado la aplicación actualizada como se esperaba. ¿Cuáles son las posibles causas? (Elija DOS)](#una-empresa-está-usando-aws-codepipeline-para-entregar-una-de-sus-aplicaciones-la-canalización-de-entrega-se-activa-con-los-cambios-en-la-rama-master-de-un-repositorio-de-aws-codecommit-y-usa-aws-codebuild-para-implementar-las-etapas-de-prueba-y-compilación-del-proceso-y-aws-codedeploy-para-desplegar-la-aplicación-la-canalización-ha-estado-funcionando-correctamente-durante-varios-meses-y-no-ha-habido-modificaciones-tras-un-cambio-reciente-en-el-código-fuente-de-la-aplicación-aws-codedeploy-no-ha-desplegado-la-aplicación-actualizada-como-se-esperaba-cuáles-son-las-posibles-causas-elija-dos) |
| 91 | [Un desarrollador ha implementado una función Lambda que necesita agregar nuevos clientes a una base de datos RDS y que se espera que se ejecute cientos de veces por hora. La función Lambda está configurada para usar 512MB de RAM y se basa en el siguiente pseudocódigo. Después de probar la función Lambda, el desarrollador nota que el tiempo de ejecución de Lambda es mucho mayor de lo esperado. ¿Qué debe hacer el desarrollador para mejorar el rendimiento?](#un-desarrollador-ha-implementado-una-función-lambda-que-necesita-agregar-nuevos-clientes-a-una-base-de-datos-rds-y-que-se-espera-que-se-ejecute-cientos-de-veces-por-hora-la-función-lambda-está-configurada-para-usar-512mb-de-ram-y-se-basa-en-el-siguiente-pseudocódigo-después-de-probar-la-función-lambda-el-desarrollador-nota-que-el-tiempo-de-ejecución-de-lambda-es-mucho-mayor-de-lo-esperado-qué-debe-hacer-el-desarrollador-para-mejorar-el-rendimiento) |
| 92 | [Amazon S3 tiene la siguiente estructura: `S3://BUCKET/FOLDERNAME/FILENAME.zip`. ¿Qué mejor práctica de S3 optimizaría el rendimiento con miles de solicitudes PUT por segundo a un único bucket?](#amazon-s3-tiene-la-siguiente-estructura-s3bucketfoldernamefilenamezip-qué-mejor-práctica-de-s3-optimizaría-el-rendimiento-con-miles-de-solicitudes-put-por-segundo-a-un-único-bucket) |

### ¿Cuáles de los siguientes son buenos casos de uso de cómo Amazon ElastiCache puede ayudar a una aplicación? (Seleccione DOS)

- [ ] Mejorar el rendimiento de las operaciones PUT de S3.
- [ ] Mejorar la latencia de las implementaciones realizadas por AWS CodeDeploy.
- [x] Mejorar la latencia y el rendimiento (throughput) de las cargas de trabajo de aplicaciones con muchas lecturas.
- [ ] Reducir el tiempo necesario para fusionar ramas de AWS CodeCommit.
- [x] Mejorar el rendimiento de las aplicaciones de uso intensivo de cómputo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa global tiene una aplicación que se ejecuta en instancias de Amazon EC2 y que sirve archivos de imagen desde Amazon S3. Las solicitudes de los usuarios desde el navegador están generando un alto tráfico, lo que provoca un rendimiento degradado. ¿Qué solución de optimización debe implementar un desarrollador para aumentar el rendimiento de la aplicación?

- [ ] Crear varios prefijos en el bucket de S3 para aumentar la tasa de solicitudes.
- [ ] Crear un clúster de Amazon ElastiCache para almacenar en caché y servir los elementos a los que se accede con frecuencia.
- [x] Usar Amazon CloudFront para servir el contenido de las imágenes almacenadas en Amazon S3.
- [ ] Enviar un ticket a AWS Support para solicitar un aumento del límite de tasa para el bucket de S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### El equipo de desarrollo está trabajando en una API que se servirá desde Amazon API Gateway. La API se servirá desde tres entornos: desarrollo, pruebas y producción. API Gateway está configurado para usar 237 GB de caché en las tres stages. ¿Cuál es la estrategia de implementación MÁS rentable?

- [ ] Crear un único API Gateway con las tres stages.
- [ ] Crear tres API Gateways, uno para cada stage, en una sola cuenta de AWS.
- [ ] Crear un API Gateway en tres cuentas de AWS separadas.
- [x] Habilitar la caché para los entornos de desarrollo y pruebas solo cuando sea necesario.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está migrando su base de datos local (on-premises) a Amazon RDS for MySQL. La empresa tiene cargas de trabajo con muchas lecturas y quiere asegurarse de refactorizar su código para lograr un rendimiento de lectura óptimo en sus consultas. ¿Cómo se puede lograr este objetivo?

- [ ] Agregar reintentos de base de datos para usar eficazmente RDS con escalamiento vertical.
- [ ] Usar RDS con implementación Multi-AZ.
- [x] Agregar una cadena de conexión para usar una réplica de lectura de RDS para las consultas de lectura.
- [ ] Agregar una cadena de conexión para usar una réplica de lectura en una instancia EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha creado una aplicación que inserta datos en una tabla de Amazon DynamoDB. La tabla está configurada para usar capacidad aprovisionada. La aplicación está implementada en una instancia de Amazon EC2 nano con capacidad de ráfaga (burstable). Los registros de la aplicación muestran que la aplicación ha estado fallando debido a un error `ProvisionedThroughputExceedException`. ¿Qué acciones debe tomar el desarrollador para resolver este problema? (Elija dos.)

- [ ] Mover la aplicación a una instancia EC2 más grande.
- [ ] Aumentar el número de unidades de capacidad de lectura (RCUs) aprovisionadas para la tabla de DynamoDB.
- [x] Reducir la frecuencia de las solicitudes a DynamoDB implementando retroceso exponencial (exponential backoff).
- [ ] Aumentar la frecuencia de las solicitudes a DynamoDB disminuyendo el retraso de reintento.
- [x] Cambiar el modo de capacidad de la tabla de DynamoDB de aprovisionado a bajo demanda (on-demand).

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación construida con funciones de AWS Lambda. Una función Lambda tiene problemas de rendimiento cuando debe descargar un archivo de 50 MB desde Internet en cada ejecución. Esta función se invoca varias veces por segundo. ¿Qué solución daría el MEJOR aumento de rendimiento?

- [x] Almacenar el archivo en caché en el directorio `/tmp`.
- [ ] Aumentar el tiempo máximo de ejecución de Lambda.
- [ ] Colocar un Elastic Load Balancer frente a la función Lambda.
- [ ] Almacenar el archivo en caché en Amazon S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Las consultas a una tabla de Amazon DynamoDB están consumiendo una gran cantidad de capacidad de lectura. La tabla tiene una cantidad significativa de atributos grandes. La aplicación no necesita todos los datos de los atributos. ¿Cómo se pueden minimizar los costos de DynamoDB mientras se maximiza el rendimiento de la aplicación?

- [ ] Agrupar todas las escrituras en lotes y realizar las operaciones de escritura cuando no haya lecturas o haya pocas.
- [x] Crear un índice secundario global (global secondary index) con un conjunto mínimo de atributos proyectados.
- [ ] Implementar retroceso exponencial (exponential backoff) en la aplicación.
- [ ] Balancear la carga de las lecturas a la tabla mediante un Application Load Balancer.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Los tiempos de carga de las páginas de un sitio web aumentan gradualmente a medida que más usuarios acceden al sistema al mismo tiempo. El análisis indica que el perfil de usuario se carga desde una base de datos en todas las páginas web que visita cada usuario, lo que aumenta la carga de la base de datos y la latencia de carga de las páginas. Para abordar este problema, el desarrollador decide almacenar en caché los datos del perfil de usuario. ¿Qué estrategia de caché abordará esta situación de la manera MÁS eficiente?

- [ ] Crear una nueva instancia de Amazon EC2 y ejecutar en ella una base de datos NoSQL. Almacenar en caché los datos del perfil dentro de esta base de datos usando la estrategia de caché write-through.
- [x] Crear un clúster de Amazon ElastiCache para almacenar en caché los datos del perfil de usuario. Usar una estrategia de caché cache-aside.
- [ ] Usar una instancia dedicada de Amazon RDS para almacenar en caché los datos del perfil. Usar una estrategia de caché write-through.
- [ ] Crear un clúster de ElastiCache para almacenar en caché los datos del perfil de usuario. Usar una estrategia de caché write-through.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una función de AWS Lambda. El desarrollador desea registrar los eventos clave que ocurren durante la ejecución de la función de Lambda e incluir un identificador único para asociar los eventos con una invocación específica de la función. ¿Cuál de las siguientes opciones ayudará al desarrollador a lograr este objetivo?

- [x] Obtener el identificador de solicitud del objeto context de Lambda. Diseñar la aplicación para que escriba los logs en la consola.
- [ ] Obtener el identificador de solicitud del objeto event de Lambda. Diseñar la aplicación para que escriba los logs en un archivo.
- [ ] Obtener el identificador de solicitud del objeto event de Lambda. Diseñar la aplicación para que escriba los logs en la consola.
- [ ] Obtener el identificador de solicitud del objeto context de Lambda. Diseñar la aplicación para que escriba los logs en un archivo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una función de AWS Lambda accede a dos tablas de Amazon DynamoDB. Un desarrollador desea mejorar el rendimiento de la función de Lambda identificando cuellos de botella en la función. ¿Cómo puede el desarrollador inspeccionar los tiempos de las llamadas a la API de DynamoDB?

- [ ] Agregar DynamoDB como origen de eventos de la función de Lambda. Ver el rendimiento con las métricas de Amazon CloudWatch.
- [ ] Colocar un Application Load Balancer (ALB) delante de las dos tablas de DynamoDB. Inspeccionar los logs del ALB.
- [ ] Limitar Lambda a no más de cinco invocaciones concurrentes. Monitorear desde la consola de Lambda.
- [x] Habilitar el rastreo de AWS X-Ray para la función. Ver las trazas desde el servicio X-Ray.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una instancia de base de datos de Amazon RDS es utilizada por muchas aplicaciones para consultar datos históricos. La tasa de consultas es relativamente constante. Cuando los datos históricos se actualizan cada día, el tráfico de escritura resultante ralentiza el rendimiento de las consultas de lectura y afecta a todos los usuarios de las aplicaciones. ¿Qué se puede hacer para eliminar el impacto en el rendimiento para los usuarios de las aplicaciones?

- [ ] Asegurarse de que Amazon RDS sea Multi-AZ para que pueda absorber mejor el aumento de tráfico.
- [x] Crear una Read Replica de RDS y dirigir todo el tráfico de lectura a la réplica.
- [ ] Implementar Amazon ElastiCache delante de Amazon RDS para amortiguar el tráfico de escritura.
- [ ] Usar Amazon DynamoDB en lugar de Amazon RDS para amortiguar el tráfico de lectura.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación se ejecuta en una instancia de EC2. El desarrollador desea almacenar una métrica de la aplicación en Amazon CloudWatch. ¿Cuál es la mejor práctica para implementar este requisito?

- [ ] Usar la llamada a la API PUT Object para enviar datos a un bucket de S3. Usar una notificación de eventos para invocar una función de Lambda que publique los datos en CloudWatch.
- [ ] Publicar los datos de la métrica en un Amazon Kinesis Stream mediante una llamada a la API `PutRecord`. Suscribir una función de Lambda que publique los datos en CloudWatch.
- [ ] Usar la llamada a la API `PutMetricData` de CloudWatch para enviar una métrica personalizada a CloudWatch. Proporcionar las credenciales necesarias para habilitar la llamada a la API.
- [x] Usar la llamada a la API `PutMetricData` de CloudWatch para enviar una métrica personalizada a CloudWatch. Lanzar la instancia de EC2 con el rol de IAM necesario para habilitar la llamada a la API.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha escrito una aplicación multihilo que se ejecuta en una flota de instancias de Amazon EC2. El equipo de operaciones ha solicitado un método gráfico para monitorear el número de hilos en ejecución a lo largo del tiempo. ¿Cuál es la forma MÁS eficiente de cumplir con esta solicitud?

- [ ] Enviar periódicamente el conteo de hilos a los segmentos de AWS X-Ray y luego generar un service graph bajo demanda.
- [x] Crear una métrica personalizada de Amazon CloudWatch y realizar periódicamente una llamada `PutMetricData` con el conteo actual de hilos.
- [ ] Registrar periódicamente los datos del conteo de hilos en Amazon S3. Usar Amazon Kinesis para procesar los datos y convertirlos en un gráfico.
- [ ] Escribir periódicamente el conteo actual de hilos en una tabla mediante Amazon DynarnoDB y usar Amazon CloudFront para crear un gráfico.

**[⬆ Back to Top](#tabla-de-contenidos)**

### La función de Lambda que se muestra a continuación se invoca a través de una API mediante Amazon API Gateway. El tiempo promedio de ejecución de la función de Lambda es de aproximadamente 1 segundo. El pseudocódigo de la función de Lambda se muestra en la imagen. ¿Qué dos acciones se pueden tomar para mejorar el rendimiento de esta función de Lambda sin aumentar el costo de la solución? (Seleccione DOS)

![Question 48](images/question48.jpg)

- [x] Empaquetar solo los módulos que la función de Lambda requiere.
- [ ] Usar Amazon DynamoDB en lugar de Amazon RDS.
- [x] Mover la inicialización de la variable de conexión de Amazon RDS fuera de la función handler.
- [ ] Implementar un connection pooling de base de datos personalizado con la función de Lambda.
- [ ] Implementar una caché local de los datos de Amazon RDS para que Lambda pueda reutilizarla.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación en AWS utiliza APIs de terceros. El desarrollador necesita monitorear los errores de las APIs en el código y desea recibir notificaciones si las fallas superan un valor de umbral establecido. ¿Cómo puede el desarrollador cumplir con estos requisitos?

- [ ] Publicar una métrica personalizada en Amazon CloudWatch y usar Amazon Simple Email Service (SES) para las notificaciones.
- [ ] Usar una métrica de errores de API de Amazon CloudWatch y usar Amazon Simple Notification Service (SNS) para las notificaciones.
- [ ] Usar una métrica de errores de API de Amazon CloudWatch y usar Amazon SES para las notificaciones.
- [x] Publicar una métrica personalizada en Amazon CloudWatch y usar Amazon SNS para las notificaciones.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ha escrito una función de AWS Lambda en Java que se activa cada vez que un usuario carga una imagen en un bucket de Amazon S3. La función convierte la imagen original a varios formatos diferentes y luego copia las imágenes resultantes a otro bucket de Amazon S3. Los desarrolladores descubren que no se está copiando ninguna imagen al segundo bucket de Amazon S3. Probaron el código en una instancia de Amazon EC2 con 1 GB de RAM y tarda en promedio 500 segundos en completarse. ¿Cuál es la causa MÁS probable del problema?

- [x] La función de Lambda tiene memoria insuficiente y es necesario aumentarla a 1 GB para igualar la instancia de Amazon EC2.
- [ ] Los archivos deben copiarse al mismo bucket de Amazon S3 para su procesamiento, por lo que el segundo bucket debe eliminarse.
- [ ] Las funciones de Lambda tienen un límite máximo de ejecución de 15 minutos, por lo tanto la función no se completa.
- [ ] Hay un problema con el runtime de Java para Lambda, y la función debe convertirse a node.js.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa desea migrar su aplicación web a AWS y aprovechar Auto Scaling para manejar las cargas de trabajo pico. El arquitecto de soluciones determinó que la mejor métrica para un evento de Auto Scaling es el número de usuarios concurrentes. Con base en esta información, ¿qué debe usar el desarrollador para escalar automáticamente según los usuarios concurrentes?

- [ ] Un tema de Amazon SNS que se active cuando se alcance un umbral de usuarios concurrentes.
- [ ] Una métrica NetworkIn de Amazon Cloudwatch.
- [ ] Amazon CloudFront para aprovechar las Edge Locations de AWS.
- [x] Una métrica personalizada de Amazon CloudWatch para usuarios concurrentes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación lee datos de una tabla de Amazon DynamoDB. Varias veces al día, durante un período de 15 segundos, la aplicación recibe múltiples errores `ProvisionedThroughputExceeded`. ¿Cómo debería manejarse esta excepción?

- [ ] Crear un nuevo índice secundario global para la tabla para ayudar con las solicitudes adicionales.
- [x] Reintentar las solicitudes de lectura fallidas con backoff exponencial.
- [ ] Reintentar inmediatamente las solicitudes de lectura fallidas.
- [ ] Usar la API `UpdateItem` de DynamoDB para aumentar la capacidad de rendimiento aprovisionado de la tabla.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Al escribir una función Lambda, ¿cuál es el beneficio de instanciar los clientes de AWS fuera del ámbito del handler?

- [ ] Legibilidad y convención de estilo.
- [x] Aprovechar la reutilización de conexiones.
- [ ] Mejor manejo de errores.
- [ ] Crear una nueva instancia por cada invocación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador recibe errores HTTP `400`: `ThrottlingException` de forma intermitente al llamar a la API de Amazon CloudWatch. Cuando una llamada falla, no se recupera ningún dato. ¿Qué mejor práctica debería aplicarse primero para resolver este problema?

- [ ] Contactar a AWS Support para solicitar un aumento de límite.
- [ ] Usar la AWS CLI para obtener las métricas.
- [ ] Analizar las aplicaciones y eliminar la llamada a la API.
- [x] Reintentar la llamada con backoff exponencial.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Durante las horas de menor actividad, un desarrollador quiere minimizar el tiempo de ejecución de un escaneo completo de una tabla de Amazon DynamoDB sin afectar las cargas de trabajo normales. Las cargas de trabajo consumen en promedio la mitad de las unidades de capacidad de lectura consistente fuerte durante las horas de menor actividad. ¿Cómo podría el desarrollador optimizar este escaneo?

- [x] Usar escaneos paralelos limitando la tasa.
- [ ] Usar escaneos secuenciales.
- [ ] Aumentar las unidades de capacidad de lectura durante la operación de escaneo.
- [ ] Cambiar la consistencia a eventualmente consistente durante la operación de escaneo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Se está diseñando un sitio grande de comercio electrónico para entregar objetos estáticos desde Amazon S3. El bucket de Amazon S3 atenderá más de 300 solicitudes GET por segundo. ¿Qué debería hacerse para optimizar el rendimiento? (Elija DOS)

- [x] Integrar Amazon CloudFront con Amazon S3.
- [ ] Habilitar la replicación entre regiones de Amazon S3.
- [ ] Eliminar los archivos de registro de servidor de Amazon S3 expirados.
- [ ] Configurar reglas de ciclo de vida de Amazon S3.
- [x] Aleatorizar los prefijos de nombres de clave de Amazon S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador tiene una aplicación que puede cargar decenas de miles de objetos por segundo a Amazon S3 en paralelo dentro de una única cuenta de AWS. Como parte de nuevos requisitos, los datos almacenados en S3 deben usar cifrado del lado del servidor con AWS KMS (SSE-KMS). Después de realizar este cambio, el rendimiento de la aplicación es más lento. ¿Cuál es la causa MÁS probable de la latencia de la aplicación?

- [ ] Amazon S3 limita la tasa a la que pueden cifrarse los objetos cargados usando Customer Master Keys.
- [x] El límite de llamadas a la API de AWS KMS es menor que el necesario para lograr el rendimiento deseado.
- [ ] El cifrado del lado del cliente de los objetos usa un algoritmo deficiente.
- [ ] KMS requiere que se use un alias para crear un nombre para mostrar independiente que pueda asignarse a una CM.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita usar AWS X-Ray para monitorear una aplicación que está desplegada en instancias de EC2. ¿Qué pasos deben ejecutarse para realizar el monitoreo?

- [ ] Desplegar el X-Ray SDK con la aplicación y usar anotaciones de X-Ray.
- [x] Instalar el X-Ray daemon e instrumentar el código de la aplicación.
- [ ] Instalar el X-Ray daemon y configurarlo para reenviar los datos a Amazon CloudWatch Events.
- [ ] Desplegar el X-Ray SDK con la aplicación e instrumentar el código de la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha creado un bucket de S3` s3://mycoolapp` y ha habilitado el registro de acceso al servidor que apunta a la carpeta `s3://mycoolapp/logs`. El desarrollador movió 100 KB de documentos de hojas de estilo en cascada (CSS) a la carpeta `s3://mycoolapp/css` y luego dejó de trabajar. Cuando el desarrollador regresó unos días después, el bucket pesaba 50 GB. ¿Cuál es la causa MÁS probable de esta situación?

- [ ] Los archivos CSS no estaban comprimidos y el versionado de S3 estaba habilitado.
- [ ] La replicación de S3 estaba habilitada en el bucket.
- [x] El registro de logs en el mismo bucket causó un crecimiento exponencial de los logs.
- [ ] Una política de lifecycle de S3 movió el archivo CSS completo a S3 Infrequent Access.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está usando AWS CodeBuild para compilar un sitio web a partir de código fuente almacenado en AWS CodeCommit. Un cambio reciente en el código fuente ha provocado que el proyecto de CodeBuild no pueda compilar el sitio web correctamente. ¿Cómo debería el desarrollador identificar la causa de las fallas?

- [ ] Modificar el archivo `buildspec.yml` para incluir pasos que envíen la salida de los comandos de compilación a Amazon CloudWatch.
- [ ] Usar una imagen de Docker personalizada que incluya el agente de AWS X-Ray en la configuración del proyecto de AWS CodeBuild.
- [x] Revisar los logs de compilación de la fase fallida en el último intento de compilación en el historial de compilaciones del proyecto de AWS CodeBuild.
- [ ] Volver a ejecutar manualmente el proceso de compilación en una máquina local para poder visualizar la salida.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ejecutó un comando de la AWS CLI y recibió el error que se muestra a continuación. ¿Qué acción debería realizar el desarrollador para que este error sea legible para las personas?

![Question 99](images/question99.jpg)

- [ ] Hacer una llamada a AWS KMS para decodificar el mensaje.
- [x] Usar la API `decode-authorization-message` de AWS STS para decodificar el mensaje.
- [ ] Usar una biblioteca de decodificación de código abierto para decodificar el mensaje.
- [ ] Usar la API `decode-authorization-message` de AWS IAM para decodificar este mensaje.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación deja de funcionar con el siguiente error: `The specified bucket does not exist`. ¿Cuál es el MEJOR lugar para comenzar el análisis de la causa raíz?

- [ ] Revisar los logs del Elastic Load Balancer en busca de solicitudes `DeleteBucket`.
- [ ] Revisar los logs de la aplicación en Amazon CloudWatch Logs en busca de errores `DeleteBucket` de Amazon S3.
- [ ] Revisar AWS X-Ray en busca de alarmas `DeleteBucket` de Amazon S3.
- [x] Revisar AWS CloudTrail en busca de un evento `DeleteBucket`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está construyendo una aplicación de negociación de acciones que requiere una latencia de submilisegundos al procesar las solicitudes de negociación. Amazon DynamoDB se usa para almacenar todos los datos de negociación que se utilizan para procesar cada solicitud. Tras las pruebas de carga de la aplicación, el equipo de desarrollo encontró que, debido a los tiempos de recuperación de datos, no se cumple el requisito de latencia. Debido a los picos repentinos en el número de solicitudes, la capacidad de lectura de DynamoDB tiene que estar significativamente sobreaprovisionada para evitar el throttling. ¿Qué pasos se deben seguir para cumplir con los requisitos de latencia y reducir el costo de ejecución de la aplicación?

- [ ] Agregar Global Secondary Indexes para los datos de negociación.
- [ ] Almacenar los datos de negociación en Amazon S3 y usar Transfer Acceleration.
- [ ] Agregar reintentos con retroceso exponencial (exponential back-off) para las consultas de DynamoDB.
- [x] Usar DynamoDB Accelerator para almacenar en caché los datos de negociación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador creó una función Lambda para el backend de una aplicación web. Al probar la función Lambda desde la consola de AWS Lambda, el desarrollador puede ver que la función se está ejecutando, pero no se genera ningún dato de log en Amazon CloudWatch Logs, incluso después de varios minutos. ¿Qué podría causar esta situación?

- [ ] La función Lambda no tiene ninguna instrucción de log explícita para que los datos de log se envíen a CloudWatch Logs.
- [ ] A la función Lambda le falta CloudWatch Logs como desencadenador de origen para enviar datos de log.
- [x] Al rol de ejecución de la función Lambda le faltan permisos para escribir datos de log en CloudWatch Logs.
- [ ] A la función Lambda le falta un grupo de logs de CloudWatch de destino.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador quiere usar AWS X-Ray para rastrear una solicitud de usuario de extremo a extremo a lo largo de la pila de software. El desarrollador realizó los cambios necesarios en la aplicación, la probó y encontró que la aplicación puede enviar las trazas a AWS X-Ray. Sin embargo, cuando la aplicación se despliega en una instancia EC2, las trazas no están disponibles. ¿Cuáles de los siguientes podrían crear esta situación? (Elija DOS)

- [ ] Las trazas llegan a X-Ray, pero el desarrollador no tiene acceso para ver los registros.
- [x] El daemon de X-Ray no está instalado en la instancia EC2.
- [ ] El endpoint de X-Ray especificado en la configuración de la aplicación es incorrecto.
- [ ] El rol de la instancia no tiene los permisos `xray:BatchGetTraces` y `xray:GetTraceGraph`. El rol de la instancia no tiene los permisos `xray:PutTraceSegments` y `xray:PutTelemetryRecords`.
- [x] El rol de la instancia no tiene los permisos `xray:PutTraceSegments` y `xray:PutTelemetryRecords`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está probando una aplicación que invoca una función de AWS Lambda de forma asíncrona. Durante la fase de pruebas, la función Lambda no logra procesar tras dos reintentos. ¿Cómo puede el desarrollador solucionar el problema de la falla?

- [ ] Configurar el registro de AWS CloudTrail para investigar las fallas de invocación.
- [x] Configurar Dead Letter Queues (DLQ) enviando los eventos a Amazon SQS para su investigación.
- [ ] Configurar Amazon Simple Workflow Service para procesar cualquier evento directo no procesado.
- [ ] Configurar AWS Config para procesar cualquier evento directo no procesado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una startup de comercio electrónico se está preparando para un evento anual de ventas. A medida que aumenta el tráfico hacia la aplicación de la empresa, el equipo de desarrollo quiere recibir una notificación cuando la utilización de CPU de la instancia de Amazon EC2 supere el 80 %. ¿Qué solución cumplirá con este requisito?

- [x] Crear una alarma personalizada de Amazon CloudWatch que envíe una notificación a un tema de Amazon SNS cuando la utilización de CPU supere el 80 %.
- [ ] Crear una alarma personalizada de AWS Cloud Trail que envíe una notificación a un tema de Amazon SNS cuando la utilización de CPU supere el 80 %.
- [ ] Crear un cron job en la instancia de EC2 que ejecute el comando `–describe-instance-information` en la instancia host cada 15 minutos y envíe los resultados a un tema de Amazon SNS.
- [ ] Crear una función de AWS Lambda que consulte los logs de AWS CloudTrail para la métrica CPUUtilization cada 15 minutos y envíe una notificación a un tema de Amazon SNS cuando la utilización de CPU supere el 80 %.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador recibe el siguiente mensaje de error al intentar lanzar o terminar una instancia de Amazon EC2 usando un script de boto3. ¿Qué debe hacer el desarrollador para corregir este mensaje de error?

![Question 129](images/question129.jpg)

- [ ] Asignar un rol de IAM a la instancia de EC2 para permitir las llamadas a la API necesarias en nombre del cliente.
- [x] Implementar un algoritmo de exponential backoff para optimizar el número de solicitudes de API realizadas a Amazon EC2.
- [ ] Aumentar el ancho de banda de red general para manejar tasas más altas de solicitudes de API.
- [ ] Actualizar a la última versión de AWS CLI para que boto3 pueda manejar tasas más altas de solicitudes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está usando Amazon DynamoDB para almacenar datos de la aplicación. El desarrollador quiere mejorar aún más el rendimiento de la aplicación reduciendo los tiempos de respuesta de las operaciones de lectura y escritura. ¿Qué característica de DynamoDB se debe usar para cumplir con estos requisitos?

- [ ] Amazon DynamoDB Streams.
- [x] Amazon DynamoDB Accelerator.
- [ ] Tablas globales de Amazon DynamoDB.
- [ ] Transacciones de Amazon DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha escrito una función de AWS Lambda usando Java como entorno de ejecución. El desarrollador quiere aislar un cuello de botella de rendimiento en el código. ¿Qué pasos se deben seguir para revelar el cuello de botella?

- [ ] Usar la API de Amazon CloudWatch para escribir marcas de tiempo en una métrica personalizada de CloudWatch. Usar la consola de CloudWatch para analizar los datos resultantes.
- [ ] Usar la API de AWS X-Ray para escribir datos de traza en X-Ray desde puntos estratégicos dentro del código. Usar la consola de Amazon CloudWatch para analizar los datos resultantes.
- [x] Usar la API de AWS X-Ray para escribir datos de traza en X-Ray desde puntos estratégicos dentro del código. Usar la consola de X-Ray para analizar los datos resultantes.
- [ ] Usar la API de Amazon CloudWatch para escribir marcas de tiempo en una métrica personalizada de CloudWatch. Usar la consola de AWS X-Ray para analizar los datos resultantes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador agregó una nueva funcionalidad a una aplicación que se ejecuta en una instancia de Amazon EC2 y que usa Amazon SQS. Después del despliegue, el desarrollador notó un aumento significativo en los costos de Amazon SQS. Al monitorear las métricas de Amazon SQS en Amazon CloudWatch, el desarrollador encontró que, en promedio, se publica un mensaje por minuto en esta cola. ¿Qué se puede hacer para reducir los costos de Amazon SQS de esta aplicación?

- [x] Aumentar el tiempo de espera de sondeo (polling timeout) de la cola de Amazon SQS.
- [ ] Reducir la cola de Amazon SQS al tamaño adecuado para la baja demanda de tráfico.
- [ ] Configurar la entrega push mediante Amazon SNS en lugar de sondear la cola de Amazon SQS.
- [ ] Usar una cola first-in, first-out (FIFO) de Amazon SQS en lugar de una cola estándar.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación que usa un backend de API REST de Amazon API Gateway respaldado por una función de AWS Lambda que interactúa con una tabla de Amazon DynamoDB. Durante las pruebas, el desarrollador observa una latencia alta al hacer solicitudes a la API. ¿Cómo puede el desarrollador evaluar la latencia de extremo a extremo e identificar los cuellos de botella de rendimiento?

- [ ] Habilitar el registro de AWS CloudTrail y usar los logs para mapear cada latencia y cuello de botella.
- [x] Habilitar y configurar el rastreo de AWS X-Ray en API Gateway y en la función de Lambda. Usar X-Ray para rastrear y analizar las solicitudes de los usuarios.
- [ ] Habilitar Amazon CloudWatch Logs para la función de Lambda. Habilitar los logs de ejecución de API Gateway para ver y analizar los logs de las solicitudes de los usuarios.
- [ ] Habilitar VPC Flow Logs para capturar y analizar el tráfico de red dentro de la VPC.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué se requiere para rastrear aplicaciones basadas en Lambda con AWS X-Ray?

- [ ] Enviar los logs de la aplicación Lambda a un bucket de S3; activar una función de Lambda desde el bucket para enviar datos a AWS X-Ray.
- [ ] Activar una función de Lambda desde los logs de la aplicación en Amazon CloudWatch para enviar datos de rastreo a AWS X-Ray.
- [x] Usar un rol de ejecución de IAM para otorgar permisos a la función de Lambda y habilitar el rastreo.
- [ ] Actualizar y agregar código del daemon de AWS X-Ray en las partes relevantes de la función de Lambda para configurar el rastreo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa requiere que las funciones de AWS Lambda escritas por los desarrolladores registren errores para que los administradores de sistemas puedan solucionar problemas de forma más eficaz. ¿Qué deberían implementar los desarrolladores para cumplir esta necesidad?

- [ ] Publicar los errores en una cola dedicada de Amazon SQS.
- [ ] Crear un disparador de evento de Amazon CloudWatch Events basado en ciertos eventos de Lambda.
- [x] Reportar los errores mediante sentencias de registro (logging) en el código de la función Lambda.
- [ ] Configurar un tema de Amazon SNS que envíe sentencias de registro (logging) cuando ocurra una falla.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación presenta problemas de rendimiento debido a una mayor demanda. Esta mayor demanda se da sobre registros históricos de solo lectura extraídos de una base de datos alojada en Amazon RDS con vistas y consultas personalizadas. Un desarrollador debe mejorar el rendimiento sin cambiar la estructura de la base de datos. ¿Qué enfoque mejorará el rendimiento y MINIMIZARÁ la sobrecarga de administración?

- [ ] Desplegar Amazon DynamoDB, mover todos los datos y apuntar a DynamoDB.
- [x] Desplegar Amazon ElastiCache for Redis y almacenar los datos en caché para la aplicación.
- [ ] Desplegar Memcached en Amazon EC2 y almacenar los datos en caché para la aplicación.
- [ ] Desplegar Amazon DynamoDB Accelerator (DAX) sobre Amazon RDS para mejorar el rendimiento de la caché.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación usa una instancia de Amazon ElastiCache for Redis de un solo nodo para mejorar el rendimiento de lectura. Con el tiempo, la demanda de la aplicación ha aumentado exponencialmente, lo que ha incrementado la carga sobre la instancia de ElastiCache. Es crítico que esta capa de caché soporte la carga y sea resiliente ante fallas de nodos. ¿Qué puede hacer el desarrollador para abordar los requisitos de carga y resiliencia?

- [x] Agregar una instancia de réplica de lectura.
- [ ] Migrar a un clúster de Memcached.
- [ ] Migrar a un clúster de Amazon Elasticsearch Service.
- [ ] Escalar verticalmente la instancia de ElastiCache.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está investigando problemas de rendimiento de una aplicación. La aplicación consta de cientos de microservicios, y una sola llamada a la API puede tener potencialmente una pila de llamadas profunda. El desarrollador debe aislar el componente que causa el problema. ¿Qué servicio o característica de AWS debería usar el desarrollador para recopilar información sobre lo que sucede y aislar la falla?

- [x] AWS X-Ray.
- [ ] VPC Flow Logs.
- [ ] Amazon GuardDuty.
- [ ] Amazon Macie.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador registró una función de AWS Lambda como destino (target) de un Application Load Balancer (ALB) mediante un comando de CLI. Sin embargo, la función Lambda no se invoca cuando el cliente envía solicitudes a través del ALB. ¿Por qué no se invoca la función Lambda?

- [ ] Una función Lambda no puede registrarse como destino de un ALB.
- [ ] Una función Lambda solo puede registrarse en un ALB usando la AWS Management Console.
- [x] Faltan los permisos para invocar la función Lambda.
- [ ] Cross-zone no está habilitado en el ALB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador intenta monitorear el estado de una aplicación ejecutando un cron job que devuelve 1 si el servicio está activo y 0 si está inactivo. El desarrollador creó código que usa un comando `put-metric-alarm` de la AWS CLI para publicar las métricas personalizadas en Amazon CloudWatch y crear una alarma. Sin embargo, el desarrollador no puede crear una alarma porque las métricas personalizadas no aparecen en la consola de CloudWatch. ¿Qué causa este problema?

- [ ] No se admite el envío de métricas personalizadas mediante la CLI.
- [x] El desarrollador necesita usar el comando `put-metric-data`.
- [ ] El desarrollador debe usar un agente unificado de CloudWatch para publicar métricas personalizadas.
- [ ] El código no se está ejecutando en una instancia de Amazon EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha escrito una aplicación que se ejecuta en instancias de Amazon EC2 y genera un valor cada minuto. El desarrollador quiere monitorear y graficar los valores generados a lo largo del tiempo sin iniciar sesión en la instancia cada vez. ¿Qué enfoque debería usar el desarrollador para lograr este objetivo?

- [ ] Usar las métricas de Amazon CloudWatch informadas de forma predeterminada para todas las instancias EC2. Ver cada valor desde la consola de CloudWatch.
- [ ] Desarrollar la aplicación para almacenar cada valor en un archivo en Amazon S3 cada minuto, con la marca de tiempo como nombre.
- [x] Publicar cada valor generado como una métrica personalizada en Amazon CloudWatch usando los SDK de AWS disponibles.
- [ ] Almacenar cada valor como una variable y agregar la variable a la lista de métricas de EC2 que deben informarse a la consola de Amazon CloudWatch.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está lanzando un sitio web de comercio electrónico y alojará los datos estáticos en Amazon S3. La empresa espera aproximadamente 1,000 transacciones por segundo (TPS) para solicitudes GET y PUT en total. Se debe habilitar el registro (logging) para rastrear todas las solicitudes y debe conservarse con fines de auditoría. ¿Cuál es la solución MÁS rentable?

- [ ] Habilitar el registro de AWS CloudTrail para la acción a nivel de bucket de S3 y crear una política de ciclo de vida (lifecycle) para mover los datos del bucket de registros a Amazon S3 Glacier en 90 días.
- [ ] Habilitar el registro de acceso del servidor de S3 y crear una política de ciclo de vida (lifecycle) para expirar los datos en 90 días.
- [ ] Habilitar el registro de AWS CloudTrail para la acción a nivel de bucket de S3 y crear una política de ciclo de vida (lifecycle) para expirar los datos en 90 días.
- [x] Habilitar el registro de acceso del servidor de S3 y crear una política de ciclo de vida (lifecycle) para mover los datos a Amazon S3 Glacier en 90 días.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer ha escrito una aplicación de Amazon Kinesis Data Streams. A medida que el uso crece y el tráfico aumenta con el tiempo, la aplicación recibe regularmente mensajes de error `ProvisionedThroughputExceededException`. ¿Qué pasos debe seguir el Developer para resolver el error? (Elija DOS)

- [ ] Usar Auto Scaling para escalar el stream y obtener un mejor rendimiento.
- [ ] Aumentar el retraso entre la llamada a `GetRecords` y la llamada a `PutRecords`.
- [x] Aumentar el número de shards en el data stream.
- [ ] Especificar un shard iterator usando el parámetro `ShardIterator`.
- [x] Implementar exponential backoff en la llamada a `GetRecords` y en la llamada a `PutRecords`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Software Engineer desarrolló una función de AWS Lambda en Node.js para realizar un procesamiento de datos que requiere mucha CPU. Con la configuración predeterminada, la función de Lambda tarda unos 5 minutos en completarse. ¿Qué enfoque debe adoptar un Developer para aumentar la velocidad de finalización?

- [ ] En lugar de usar Node.js, reescribir la función de Lambda usando Python.
- [ ] En lugar de empaquetar las bibliotecas en el archivo `ZIP` con la función, moverlas a un Lambda layer y usar el layer con la función.
- [ ] Asignar el máximo de unidades de CPU disponibles a la función.
- [x] Aumentar la memoria disponible para la función.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer tiene una aplicación heredada alojada on-premises. Otras aplicaciones alojadas en AWS dependen de la aplicación on-premises para su correcto funcionamiento. En caso de errores en las aplicaciones, el Developer quiere poder usar Amazon CloudWatch para monitorear y solucionar problemas de todas las aplicaciones desde un solo lugar. ¿Cómo puede lograrlo el Developer?

- [ ] Instalar un AWS SDK en el servidor on-premises para enviar automáticamente los registros a CloudWatch.
- [x] Descargar el agente de CloudWatch en el servidor on-premises. Configurar el agente para que use credenciales de usuario de IAM con permisos para CloudWatch.
- [ ] Cargar los archivos de registro del servidor on-premises en Amazon S3 y hacer que CloudWatch lea los archivos.
- [ ] Cargar los archivos de registro del servidor on-premises en una instancia de Amazon EC2 y hacer que la instancia reenvíe los registros a CloudWatch.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer está trabajando en un proyecto sin servidor basado en Java. Las pruebas iniciales muestran que un cold start tarda en promedio unos 8 segundos en las funciones de AWS Lambda. ¿Qué debe hacer el Developer para reducir el tiempo de cold start? (Elija DOS)

- [ ] Agregar el Spring Framework al proyecto y habilitar la inyección de dependencias.
- [x] Reducir el paquete de despliegue incluyendo solo los módulos necesarios del AWS SDK for Java.
- [x] Aumentar la configuración de asignación de memoria de la función de Lambda.
- [ ] Aumentar la configuración de tiempo de espera (timeout) de la función de Lambda.
- [ ] Cambiar el modo de invocación de Lambda de síncrono a asíncrono.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer está aprovechando una conexión AWS VPN basada en Border Gateway Protocol (BGP) para conectarse desde on-premises a instancias de Amazon EC2 en la cuenta del Developer. El Developer puede acceder a una instancia de EC2 en la subred A, pero no puede acceder a una instancia de EC2 en la subred B de la misma VPC. ¿Qué registros puede usar el Developer para verificar si el tráfico está llegando a la subred B?

- [ ] Registros de VPN.
- [ ] Registros de BGP
- [x] VPC Flow Logs.
- [ ] Registros de AWS CloudTrail.

**[⬆ Back to Top](#tabla-de-contenidos)**

### El sitio web de una empresa se ejecuta en una instancia de Amazon EC2 y usa Auto Scaling para escalar el entorno en horas pico. Los usuarios del sitio web en todo el mundo experimentan alta latencia debido al contenido estático en la instancia de EC2, incluso en horas no pico. ¿Qué combinación de pasos resolverá el problema de latencia? (Elija DOS)

- [ ] Duplicar el número máximo de servidores del Auto Scaling group.
- [ ] Alojar el código de la aplicación en AWS Lambda.
- [ ] Escalar verticalmente cambiando el tamaño de las instancias de EC2.
- [x] Crear una distribución de Amazon CloudFront para almacenar en caché el contenido estático.
- [x] Almacenar el contenido estático de la aplicación en Amazon S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer va a desplegar una función de AWS Lambda que requiere un uso significativo de CPU. ¿Qué enfoque MINIMIZARÁ el tiempo de ejecución promedio de la función?

- [ ] Desplegar la función en múltiples Regiones de AWS.
- [ ] Desplegar la función en múltiples Zonas de Disponibilidad.
- [ ] Desplegar la función usando Lambda layers.
- [x] Desplegar la función con su asignación de memoria configurada al máximo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer tiene una API de comercio electrónico alojada en Amazon ECS. La demanda variable y con picos en la aplicación está causando que el procesamiento de pedidos tarde demasiado. La aplicación procesa colas de Amazon SQS. La métrica `ApproximateNumberOfMessagesVisible` presenta picos de valores muy altos a lo largo del día, lo que provoca activaciones de alarmas de Amazon CloudWatch. Otras métricas de ECS para los contenedores de la API están muy por debajo de los límites. ¿Qué puede implementar el Developer para mejorar el rendimiento manteniendo bajos los costos?

- [x] Política de escalado de seguimiento de destino (target tracking scaling policy).
- [ ] Docker Swarm.
- [ ] Service scheduler.
- [ ] Política de escalado por pasos (step scaling policy).

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación se ejecuta en un clúster de instancias de Amazon EC2. Al intentar leer objetos almacenados en un único bucket de Amazon S3 que están cifrados con cifrado del lado del servidor con claves administradas por AWS KMS (SSE-KMS), la aplicación recibe el siguiente error. ¿Qué combinación de pasos se debe seguir para evitar este fallo? (Elija DOS)

![Question 212](images/question212.jpg)

- [x] Contactar a AWS Support para solicitar un aumento del límite de tasa de AWS KMS.
- [x] Realizar reintentos de error con exponential backoff en el código de la aplicación.
- [ ] Contactar a AWS Support para solicitar un aumento del límite de tasa de S3.
- [ ] Importar una customer master key (CMK) con un tamaño de clave mayor.
- [ ] Usar más de una customer master key (CMK) para cifrar los datos de S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Después de lanzar una instancia que pretende servir como dispositivo NAT (Network Address Translation) en una subred pública, usted modifica sus tablas de enrutamiento para que el dispositivo NAT sea el destino del tráfico con destino a Internet de su subred privada. Cuando intenta realizar una conexión saliente a Internet desde una instancia en la subred privada, no tiene éxito. El dispositivo NAT debe ser el destino del tráfico con destino a Internet de su subred privada. ¿Cuál de los siguientes pasos podría resolver el problema?

- [ ] Adjuntar una segunda Elastic Network Interface (ENI) a la instancia NAT y colocarla en la subred privada.
- [ ] Adjuntar una segunda Elastic Network Interface (ENI) a la instancia en la subred privada y colocarla en la subred pública.
- [x] Deshabilitar el atributo `Source/Destination Check` en la instancia NAT.
- [ ] Adjuntar una dirección Elastic IP a la instancia en la subred privada.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Usted tiene un entorno que consta de una subred pública con Amazon VPC y 3 instancias que se ejecutan en esta subred. Estas tres instancias pueden comunicarse correctamente con otros hosts en Internet. Usted lanza una cuarta instancia en la misma subred, usando la misma AMI y la misma configuración de security group que usó para las otras, pero descubre que no se puede acceder a esta instancia desde Internet. ¿Qué debe hacer para habilitar el acceso a Internet?

- [ ] Desplegar una instancia NAT en la subred pública.
- [ ] Modificar la tabla de enrutamiento de la subred pública.
- [ ] Configurar una dirección IP con enrutamiento público en el sistema operativo del host de la cuarta instancia.
- [x] Asignar una dirección Elastic IP a la cuarta instancia.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Al usar una operación Scan grande en DynamoDB, ¿qué técnica se puede utilizar para minimizar el impacto de un scan en el throughput aprovisionado de una tabla?

- [x] Establecer un tamaño de página más pequeño para el scan.
- [ ] Usar scans paralelos.
- [ ] Definir un range index en la tabla.
- [ ] Precalentar la tabla actualizando todos los elementos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### El sitio de intercambio de fotos de una startup está desplegado en una VPC. Un ELB distribuye el tráfico web entre dos subnets. La session stickiness del ELB está configurada para usar la cookie de sesión generada por AWS, con un TTL de sesión de 5 minutos. El Auto Scaling Group de servidores web está configurado como: `min-size=4`, `max-size=4`. La startup se prepara para un lanzamiento público ejecutando software de pruebas de carga instalado en una única instancia EC2 que se ejecuta en `us-west-2`. Después de 60 minutos de pruebas de carga, los logs de los servidores web muestran lo siguiente. ¿Qué recomendaciones pueden ayudar a asegurar que las solicitudes HTTP de las pruebas de carga se distribuyan uniformemente entre los cuatro servidores web? (Elija DOS)

![Question 241](images/question241.jpg)

- [ ] Lanzar y ejecutar la instancia EC2 del probador de carga desde `us-east-1` en su lugar.
- [x] Reconfigurar el software de pruebas de carga para volver a resolver el DNS en cada solicitud web.
- [x] Usar un servicio de pruebas de carga de terceros que ofrezca clientes de prueba distribuidos globalmente.
- [ ] Configurar ELB y Auto Scaling para distribuir entre `us-west-2a` y `us-west-2c`.
- [ ] Configurar la session stickiness del ELB para usar la cookie de sesión específica de la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de los siguientes servicios se incluyen sin costo adicional con el uso de la plataforma AWS?

- [ ] Simple Storage Service.
- [ ] Elastic Compute Cloud.
- [x] Auto Scaling.
- [ ] Elastic Load Balancing.
- [x] CloudFormation.
- [ ] Simple Workflow Service.

**[⬆ Back to Top](#tabla-de-contenidos)**

### En DynamoDB, ¿qué tipo de códigos de respuesta HTTP indica que se encontró un problema con la solicitud del cliente enviada al servicio?

- [ ] Código de respuesta HTTP 5xx.
- [ ] Código de respuesta HTTP 200.
- [ ] Código de respuesta HTTP 306.
- [x] Código de respuesta HTTP 4xx.

**[⬆ Back to Top](#tabla-de-contenidos)**

### La Empresa B ofrece un servicio de reconocimiento de imágenes en línea y utiliza SQS para desacoplar los componentes del sistema y lograr escalabilidad. Los consumidores de SQS consultan (poll) la cola de imágenes con la mayor frecuencia posible para mantener lo más alto posible el throughput de extremo a extremo. Sin embargo, la Empresa B se da cuenta de que consultar en bucles cerrados consume ciclos de CPU y aumenta los costos con respuestas vacías. ¿Cómo puede la Empresa B reducir el número de respuestas vacías?

- [ ] Establecer el atributo `Timeout` de visibilidad de la cola de imágenes en 20 segundos.
- [x] Establecer el atributo `ReceiveMessageWaitTimeSeconds` de la cola de imágenes en 20 segundos.
- [ ] Establecer el atributo `MessageRetentionPeriod` de la cola de imágenes en 20 segundos.
- [ ] Establecer el parámetro `DelaySeconds` de un mensaje en 20 segundos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Usted inserta 1000 elementos nuevos cada segundo en una tabla de DynamoDB. Una vez por hora estos elementos se analizan y luego ya no se necesitan. Necesita minimizar el throughput aprovisionado, el almacenamiento y las llamadas a la API. Dados estos requisitos, ¿cuál es la forma más eficiente de gestionar estos elementos después del análisis?

- [ ] Conservar los elementos en una sola tabla.
- [ ] Eliminar los elementos individualmente a lo largo de un periodo de 24 horas.
- [x] Eliminar la tabla y crear una nueva tabla por hora.
- [ ] Crear una nueva tabla por hora.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Está escribiendo en una tabla de DynamoDB y recibe la siguiente excepción: `ProvisionedThroughputExceededException`, aunque según las métricas de CloudWatch de la tabla no está excediendo su throughput aprovisionado. ¿Cuál podría ser una explicación?

- [ ] No ha aprovisionado suficientes instancias de almacenamiento de DynamoDB.
- [ ] Está excediendo su capacidad en una `Range Key` particular.
- [x] Está excediendo su capacidad en una `Hash Key` particular.
- [ ] Está excediendo su capacidad en una `Sort Key` particular.
- [ ] No ha configurado los triggers de DynamoDB Auto Scaling.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Si una aplicación almacena archivos de log por hora de miles de instancias de un sitio web de alto tráfico, ¿qué esquema de nombres daría el rendimiento óptimo en S3?

- [ ] Secuencial.
- [x] `instanceID_log-HH-DD-MM-YYYY`.
- [ ] `instanceIDLog-YYYY-MM-DD-HH`.
- [ ] `HH-DD-MM-YYYY-log_instanceID`.
- [ ] `YYYY-MM-DD-HH-logInstanceID`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo quiere instrumentar su código para proporcionar a AWS X-Ray información más detallada que las simples solicitudes salientes y entrantes. Esto generará grandes cantidades de datos, por lo que el equipo de desarrollo quiere implementar indexación para poder filtrar los datos. ¿Qué debe hacer el equipo de desarrollo para lograrlo?

- [x] Agregar annotations al documento de segmento y al código.
- [ ] Agregar metadata al documento de segmento y al código.
- [ ] Configurar las variables de entorno necesarias de X-Ray.
- [ ] Instalar los plugins requeridos para el AWS SDK correspondiente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una tabla de Amazon DynamoDB utiliza un Global Secondary Index (GSI) para soportar consultas de lectura. La tabla principal tiene mucha carga de escritura, mientras que el GSI se usa para operaciones de lectura. Al revisar las métricas de Amazon CloudWatch, el desarrollador nota que las operaciones de escritura a la tabla principal sufren limitación (throttling) con frecuencia durante una alta actividad de escritura. Sin embargo, las unidades de capacidad de escritura de la tabla principal están disponibles y no se consumen por completo. ¿Por qué se está limitando la tabla?

- [x] Las unidades de capacidad de escritura del GSI están subaprovisionadas.
- [ ] No hay suficientes unidades de capacidad de lectura en la tabla principal.
- [ ] Amazon DynamoDB Streams no está habilitado en la tabla.
- [ ] Se está realizando una operación de escritura grande contra otra tabla.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación Docker en Amazon ECS. La aplicación debe escalar según la carga de usuarios de los últimos 15 segundos. ¿Cómo debe instrumentar el código un desarrollador para cumplir el requisito?

- [ ] Crear una métrica personalizada de Amazon CloudWatch de alta resolución para los datos de actividad de usuarios y luego publicar los datos cada 30 segundos.
- [x] Crear una métrica personalizada de Amazon CloudWatch de alta resolución para los datos de actividad de usuarios y luego publicar los datos cada 5 segundos.
- [ ] Crear una métrica personalizada de Amazon CloudWatch de resolución estándar para los datos de actividad de usuarios y luego publicar los datos cada 30 segundos.
- [ ] Crear una métrica personalizada de Amazon CloudWatch de resolución estándar para los datos de actividad de usuarios y luego publicar los datos cada 5 segundos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está construyendo una aplicación web que utiliza Amazon API Gateway para exponer una función de AWS Lambda que procesa solicitudes de clientes. Durante las pruebas, el desarrollador nota que API Gateway sufre timeout aunque la función de Lambda termina dentro del límite de tiempo establecido. ¿Cuáles de las siguientes métricas de API Gateway en Amazon CloudWatch pueden ayudar al desarrollador a solucionar el problema? (Elija DOS)

- [ ] CacheHitCount.
- [x] IntegrationLatency.
- [ ] CacheMissCount.
- [x] Latency.
- [ ] Count.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe analizar problemas de rendimiento en aplicaciones distribuidas de producción escritas como funciones de AWS Lambda. Estas aplicaciones Lambda distribuidas invocan otros componentes que conforman las aplicaciones. ¿Cómo debe el desarrollador identificar y solucionar la causa raíz de los problemas de rendimiento en producción?

- [ ] Agregar instrucciones de logging a las funciones de Lambda y luego usar Amazon CloudWatch para ver los logs.
- [ ] Usar AWS Cloud Trail y luego examinar los logs.
- [x] Usar AWS X-Ray y luego examinar los segmentos y errores.
- [ ] Ejecutar agentes de Amazon Inspector y luego analizar el rendimiento.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador quiere depurar una aplicación buscando y filtrando datos de log. Los logs de la aplicación se almacenan en Amazon CloudWatch Logs. El desarrollador crea un nuevo metric filter para contar las excepciones en los logs de la aplicación. Sin embargo, no se devuelven resultados de los logs. ¿Cuál es la razón por la que no se devuelven resultados filtrados?

- [ ] Se requiere configurar un VPC endpoint de interfaz de Amazon CloudWatch para filtrar los CloudWatch Logs en la VPC.
- [x] CloudWatch Logs solo publica datos de métricas para los eventos que ocurren después de que se crea el filtro.
- [ ] El log group de CloudWatch Logs debe enviarse primero mediante streaming a Amazon Elasticsearch Service antes de que el filtrado de métricas devuelva los resultados.
- [ ] Los puntos de datos de métricas de los log groups solo se pueden filtrar después de exportarlos a un bucket de Amazon S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa utiliza instancias de Amazon RDS MySQL para la capa de base de datos de su aplicación y servidores Apache Tomcat para su capa web. La mayoría de las consultas a la base de datos desde las aplicaciones web son solicitudes de lectura repetidas. ¿El uso de qué servicio de AWS aumentaría el rendimiento al agregar un almacén en memoria para las consultas de lectura repetidas?

- [ ] Amazon RDS Multi-AZ.
- [ ] Amazon SQS.
- [x] Amazon ElastiCache.
- [ ] Amazon RDS read replica.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está investigando un problema por el cual ciertas solicitudes pasan por un endpoint de Amazon API Gateway /MyAPI, pero las solicitudes no llegan a la función de AWS Lambda que respalda /MyAPI. El desarrollador descubrió que una segunda función de Lambda a veces se ejecuta en la concurrencia máxima permitida para la cuenta de AWS dada. ¿Cómo puede el desarrollador resolver este problema?

- [ ] Reducir manualmente el límite de ejecución concurrente a nivel de cuenta.
- [ ] Agregar otro stage de API Gateway para /MyAPI y distribuir las solicitudes (sharding).
- [x] Configurar el límite de ejecución concurrente de la segunda función de Lambda.
- [ ] Reducir los límites de throttling en el endpoint /MyAPI de API Gateway

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha creado una función de Lambda y encuentra que la función tarda más de lo esperado en completarse. Después de depurar, el desarrollador ha descubierto que aumentar la capacidad de cómputo mejoraría el rendimiento. ¿Cómo puede el desarrollador aumentar los recursos de cómputo de Lambda?

- [ ] Ejecutar en una instancia de mayor tamaño con más capacidad de cómputo.
- [ ] Aumentar el tiempo máximo de ejecución.
- [ ] Especificar una mayor capacidad de cómputo al invocar la función de Lambda.
- [x] Aumentar la memoria asignada a la función de Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un sitio de comercio electrónico permite que los usuarios recurrentes inicien sesión para mostrar páginas web personalizadas. El flujo de trabajo se muestra en la imagen a continuación. Una aplicación se ejecuta en instancias de EC2. Amazon RDS se utiliza para la base de datos que almacena las cuentas y preferencias de los usuarios. El sitio web se congela o carga lentamente mientras espera que se complete el paso de inicio de sesión. Los demás componentes del sitio están bien optimizados. ¿Cuáles de las siguientes técnicas resolverán este problema? (Seleccione DOS)

![Question 299](images/question299.jpeg)

- [ ] Implementar la página de inicio de sesión de usuario como una función de Lambda asíncrona.
- [x] Usar Amazon ElastiCache for MemCached para almacenar en caché los datos de usuario.
- [ ] Usar Amazon Application Load Balancer para balancear el tráfico hacia el sitio web.
- [x] Llamar a la base de datos de forma asíncrona para que el código pueda continuar ejecutándose.
- [ ] Agrupar en lote las solicitudes de inicio de sesión de cientos de usuarios en una sola solicitud de lectura a la base de datos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador quiere que los datos de registro de una aplicación que se ejecuta en una instancia de EC2 estén disponibles para los administradores de sistemas. ¿Cuál de las siguientes opciones permite monitorear esta métrica en Amazon CloudWatch?

- [ ] Recuperar los datos de registro desde CloudWatch mediante la llamada a la API `GetMetricData`.
- [ ] Recuperar los datos de registro desde AWS CloudTrail mediante la llamada a la API `LookupEvents`.
- [ ] Lanzar una nueva instancia de EC2, configurar Amazon CloudWatch Events y luego instalar la aplicación.
- [x] Instalar el agente de Amazon CloudWatch Logs en la instancia de EC2 donde se ejecuta la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene una aplicación que registra toda la información en Amazon S3. Cada vez que hay un nuevo archivo de registro, se invoca una función de AWS Lambda para procesar los archivos de registro. El código funciona y reúne toda la información necesaria. Sin embargo, al revisar los registros de la función Lambda, se encuentran entradas duplicadas con el mismo ID de solicitud. ¿Qué está causando las entradas duplicadas?

- [ ] El nombre del bucket de S3 se especificó incorrectamente.
- [x] La función Lambda falló y el servicio Lambda reintentó la invocación con un retraso.
- [ ] Hubo una interrupción de S3, lo que causó entradas duplicadas del archivo de registro de ventas.
- [ ] La aplicación se detuvo de forma intermitente y luego se reanudó.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo ha puesto en producción 10 aplicaciones que se ejecutan en varias instancias de Amazon EC2. El equipo de operaciones solicita una representación gráfica de una métrica clave de rendimiento para cada aplicación. Estas métricas deben estar disponibles en una sola pantalla para facilitar el monitoreo. ¿Qué pasos debe seguir el desarrollador para lograr esto con Amazon CloudWatch?

- [x] Crear un namespace personalizado con un nombre de métrica único para cada aplicación.
- [ ] Crear una dimension personalizada con un nombre de métrica único para cada aplicación.
- [ ] Crear un evento personalizado con un nombre de métrica único para cada aplicación.
- [ ] Crear una alarma personalizada con un nombre de métrica único para cada aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa usa Amazon DynamoDB para administrar y rastrear pedidos. La tabla de DynamoDB está particionada según la fecha del pedido. La empresa recibe un aumento enorme de pedidos durante un evento de ventas, lo que causa limitación (throttling) en las escrituras de DynamoDB, y el rendimiento consumido está muy por debajo del rendimiento aprovisionado. De acuerdo con las mejores prácticas de AWS, ¿cómo se puede resolver este problema con costos MÍNIMOS?

- [ ] Crear una nueva tabla de DynamoDB para cada fecha de pedido.
- [ ] Aumentar las unidades de capacidad de lectura y escritura de la tabla de DynamoDB.
- [x] Agregar un sufijo numérico aleatorio a los valores de la clave de partición.
- [ ] Agregar un índice secundario global a la tabla de DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa mantiene una aplicación responsable de procesar varios miles de callbacks externos cada día. Los administradores de sistemas de la empresa quieren saber cuántos callbacks se reciben de forma continua y quieren que estos datos estén disponibles durante 10 días. La empresa también quiere poder emitir alertas automáticas si el número de callbacks supera los umbrales definidos. ¿Cuál es la forma MÁS rentable de atender la necesidad de rastrear y alertar sobre estas estadísticas?

- [ ] Enviar los datos de callbacks a una base de datos de Amazon RDS que se pueda consultar para mostrar datos históricos y alertar cuando se superen los umbrales.
- [ ] Enviar los datos de callbacks a AWS X-Ray y usar AWS Lambda para consultar, mostrar y alertar cuando se superen los umbrales.
- [ ] Enviar los datos de callbacks a Amazon Kinesis Data Streams e invocar una función de AWS Lambda que almacene los datos en Amazon DynamoDB y envíe las alertas necesarias.
- [x] Enviar los datos de callbacks a Amazon CloudWatch como una métrica personalizada y usar los mecanismos de alerta de CloudWatch para alertar a los administradores de sistemas.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene una aplicación web de varios niveles en AWS. Durante un reciente pico de tráfico, una de las bases de datos relacionales principales en Amazon RDS no pudo atender todo el tráfico. Algunas consultas de lectura de elementos a los que se accede repetidamente fallaron, por lo que los usuarios recibieron mensajes de error. ¿Qué se puede hacer para minimizar el impacto en las consultas de lectura de la base de datos de la forma MÁS eficiente durante futuros picos de tráfico?

- [ ] Usar Amazon S3 para almacenar en caché los resultados de las consultas a la base de datos.
- [ ] Usar Amazon RDS como origen personalizado de Amazon CloudFront.
- [ ] Usar el almacenamiento local y la memoria de las instancias de Amazon EC2 para almacenar datos en caché.
- [x] Usar Amazon ElastiCache frente a la base de datos principal para almacenar datos en caché.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una función de AWS Lambda para procesar un flujo de datos de un Amazon Kinesis Data Stream. Cuando la función Lambda analiza los datos y encuentra un campo faltante, termina la función con un error. La función está generando registros duplicados a partir del flujo de Kinesis. Cuando el desarrollador examina la salida del flujo sin la función Lambda, no hay registros duplicados. ¿Cuál es el motivo de los duplicados?

- [ ] La función Lambda no avanzó el puntero del flujo de Kinesis al siguiente registro después del error.
- [ ] El origen de eventos de Lambda usó invocación asíncrona, lo que produjo registros duplicados.
- [x] La función Lambda no manejó el error y el servicio Lambda intentó reprocesar los datos.
- [ ] La función Lambda no puede seguir el ritmo de la cantidad de datos que llegan del flujo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador quiere habilitar AWS X-Ray para una aplicación segura que se ejecuta en un entorno de Amazon ECS. ¿Qué combinación de pasos habilitará X-Ray? (Seleccione TRES)

- [x] Crear una imagen de Docker que ejecute el daemon de X-Ray.
- [x] Agregar instrumentación al código de la aplicación para X-Ray.
- [ ] Instalar el daemon de X-Ray en la instancia de EC2 subyacente.
- [ ] Configurar y usar un rol de instancia de EC2 de IAM.
- [ ] Registrar la aplicación en X-Ray.
- [x] Configurar y usar un rol de IAM para tareas.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha publicado una actualización de una aplicación que se sirve a una base de usuarios global mediante Amazon CloudFront. Después de implementar la aplicación, los usuarios no pueden ver los cambios actualizados. ¿Cómo puede el desarrollador resolver este problema?

- [ ] Quitar el origen de la configuración de CloudFront y agregarlo de nuevo.
- [ ] Deshabilitar el reenvío de cadenas de consulta y encabezados de solicitud desde la configuración de la distribución de CloudFront.
- [x] Invalidar todos los objetos de la aplicación de las edge caches.
- [ ] Deshabilitar la distribución de CloudFront y habilitarla de nuevo para actualizar todas las ubicaciones perimetrales.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa migró recientemente sus capas web, de aplicación y de base de datos NoSQL a AWS. La empresa usa Auto Scaling para escalar las capas web y de aplicación. Más del 95 por ciento de las solicitudes a Amazon DynamoDB son solicitudes de lectura repetidas. ¿Cómo se puede escalar la capa NoSQL de DynamoDB para almacenar en caché estas solicitudes repetidas?

- [ ] Amazon EMR.
- [x] Amazon DynamoDB Accelerator.
- [ ] Amazon SQS.
- [ ] Amazon CloudFront.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Mientras desarrolla una aplicación que se ejecuta en Amazon EC2 dentro de una Amazon VPC, un desarrollador identifica la necesidad de almacenamiento centralizado de los registros (logs) a nivel de aplicación. ¿Qué servicio de AWS se puede usar para almacenar estos registros de forma segura?

- [ ] Amazon EC2 VPC Flow Logs.
- [x] Amazon CloudWatch Logs.
- [ ] Amazon CloudSearch.
- [ ] AWS CloudTrail

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación de monitoreo del mercado bursátil usa Amazon Kinesis para la ingesta de datos. Durante pruebas simuladas de tasas de datos pico, el stream de Kinesis no puede seguir el ritmo de los datos entrantes. ¿Qué paso permitirá a Kinesis acomodar el tráfico durante las horas pico?

- [ ] Instalar la Kinesis Producer Library (KPL) para ingerir datos en el stream.
- [ ] Reducir el período de retención de datos para permitir mayor ingesta de datos usando `DecreaseStreamRetentionPeriod`.
- [x] Aumentar la cantidad de shards del stream usando `UpdateShardCount`.
- [ ] Ingerir múltiples registros en el stream en una sola llamada usando `PutRecords`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación usa funciones Lambda para extraer metadatos de archivos cargados a un bucket de S3; los metadatos se almacenan en Amazon DynamoDB. La aplicación comienza a comportarse de forma inesperada y el desarrollador quiere examinar los registros (logs) del código de la función Lambda en busca de errores. Según esta configuración del sistema, ¿dónde encontraría el desarrollador los registros?

- [ ] Amazon S3.
- [ ] AWS CloudTrail.
- [x] Amazon CloudWatch.
- [ ] Amazon DynamoDB

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está usando AWS CodePipeline para entregar una de sus aplicaciones. La canalización de entrega se activa con los cambios en la rama master de un repositorio de AWS CodeCommit y usa AWS CodeBuild para implementar las etapas de prueba y compilación del proceso, y AWS CodeDeploy para desplegar la aplicación. La canalización ha estado funcionando correctamente durante varios meses y no ha habido modificaciones. Tras un cambio reciente en el código fuente de la aplicación, AWS CodeDeploy no ha desplegado la aplicación actualizada como se esperaba. ¿Cuáles son las posibles causas? (Elija DOS)

- [x] El cambio no se realizó en la rama master del repositorio de AWS CodeCommit.
- [x] Una de las etapas anteriores de la canalización falló y la canalización terminó.
- [ ] Una de las instancias de Amazon EC2 en el clúster de AWS CodePipeline de la empresa está inactiva.
- [ ] AWS CodePipeline está configurado incorrectamente y no está ejecutando AWS CodeDeploy.
- [ ] AWS CodePipeline no tiene permisos para acceder a AWS CodeCommit.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha implementado una función Lambda que necesita agregar nuevos clientes a una base de datos RDS y que se espera que se ejecute cientos de veces por hora. La función Lambda está configurada para usar 512MB de RAM y se basa en el siguiente pseudocódigo. Después de probar la función Lambda, el desarrollador nota que el tiempo de ejecución de Lambda es mucho mayor de lo esperado. ¿Qué debe hacer el desarrollador para mejorar el rendimiento?

![Question 385](images/question385.jpg)

- [ ] Aumentar la cantidad de RAM asignada a la función Lambda, lo que aumentará el número de hilos que Lambda puede usar.
- [ ] Aumentar el tamaño de la base de datos RDS para permitir un mayor número de conexiones a la base de datos por hora.
- [x] Mover la conexión a la base de datos y la sentencia de cierre fuera del handler. Colocar la conexión en el espacio global.
- [ ] Reemplazar RDS con Amazon DynamoDB para implementar control sobre el número de escrituras por segundo.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Amazon S3 tiene la siguiente estructura: `S3://BUCKET/FOLDERNAME/FILENAME.zip`. ¿Qué mejor práctica de S3 optimizaría el rendimiento con miles de solicitudes PUT por segundo a un único bucket?

- [ ] Anteponer el id de usuario a los nombres de carpeta; por ejemplo, `s3://BUCKET/2013-FOLDERNAME/FILENAME.zip`.
- [ ] Anteponer marcas de tiempo a los nombres de archivo; por ejemplo, `s3://BUCKET/FOLDERNAME/2013-26-05-15-00-00-FILENAME.zip`.
- [ ] Anteponer hashes hexadecimales aleatorios a los nombres de archivo; por ejemplo, `s3://BUCKET/FOLDERNAME/23a6-FILENAME.zip`.
- [x] Anteponer hashes hexadecimales aleatorios a los nombres de carpeta; por ejemplo, `s3://BUCKET/23a6-FOLDERNAME/FILENAME.zip`.

**[⬆ Back to Top](#tabla-de-contenidos)**
