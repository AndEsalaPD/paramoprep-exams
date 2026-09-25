# Dominio 2: Seguridad (26 %)

Preguntas de práctica AWS Certified Developer Associate (DVA-C02) — 89 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [Un desarrollador desea cargar datos en Amazon S3 y debe cifrar los datos en tránsito. ¿Cuáles de las siguientes soluciones lograrán esta tarea? (Elija DOS)](#un-desarrollador-desea-cargar-datos-en-amazon-s3-y-debe-cifrar-los-datos-en-tránsito-cuáles-de-las-siguientes-soluciones-lograrán-esta-tarea-elija-dos) |
| 2 | [Un desarrollador desea cifrar los nuevos objetos que una aplicación carga en un bucket de Amazon S3. Debe existir un registro de auditoría de quién ha utilizado la clave durante este proceso. No debe haber ningún cambio en el rendimiento de la aplicación. ¿Qué tipo de cifrado cumple con estos requisitos?](#un-desarrollador-desea-cifrar-los-nuevos-objetos-que-una-aplicación-carga-en-un-bucket-de-amazon-s3-debe-existir-un-registro-de-auditoría-de-quién-ha-utilizado-la-clave-durante-este-proceso-no-debe-haber-ningún-cambio-en-el-rendimiento-de-la-aplicación-qué-tipo-de-cifrado-cumple-con-estos-requisitos) |
| 3 | [Se está desarrollando una aplicación para auditar varias cuentas de AWS. La aplicación se ejecutará en la Cuenta A y debe acceder a servicios de AWS en las Cuentas B y C. ¿Cuál es la forma MÁS segura de permitir que la aplicación llame a los servicios de AWS en cada cuenta auditada?](#se-está-desarrollando-una-aplicación-para-auditar-varias-cuentas-de-aws-la-aplicación-se-ejecutará-en-la-cuenta-a-y-debe-acceder-a-servicios-de-aws-en-las-cuentas-b-y-c-cuál-es-la-forma-más-segura-de-permitir-que-la-aplicación-llame-a-los-servicios-de-aws-en-cada-cuenta-auditada) |
| 4 | [Una empresa está construyendo una aplicación de uso intensivo de cómputo que se ejecutará en una flota de instancias de Amazon EC2. La aplicación utiliza discos de Amazon EBS conectados para almacenar datos. La aplicación procesará información confidencial y todos los datos deben estar cifrados. ¿Qué debe hacer un desarrollador para asegurar que los datos estén cifrados en disco sin afectar el rendimiento?](#una-empresa-está-construyendo-una-aplicación-de-uso-intensivo-de-cómputo-que-se-ejecutará-en-una-flota-de-instancias-de-amazon-ec2-la-aplicación-utiliza-discos-de-amazon-ebs-conectados-para-almacenar-datos-la-aplicación-procesará-información-confidencial-y-todos-los-datos-deben-estar-cifrados-qué-debe-hacer-un-desarrollador-para-asegurar-que-los-datos-estén-cifrados-en-disco-sin-afectar-el-rendimiento) |
| 5 | [Una función de AWS Lambda genera un archivo JSON de 3 MB y luego lo carga diariamente en un bucket de Amazon S3. El archivo contiene información confidencial, por lo que el desarrollador debe asegurarse de que esté cifrado antes de cargarlo en el bucket. ¿Cuál de las siguientes modificaciones debe realizar el desarrollador para asegurar que los datos estén cifrados antes de cargarlos en el bucket?](#una-función-de-aws-lambda-genera-un-archivo-json-de-3-mb-y-luego-lo-carga-diariamente-en-un-bucket-de-amazon-s3-el-archivo-contiene-información-confidencial-por-lo-que-el-desarrollador-debe-asegurarse-de-que-esté-cifrado-antes-de-cargarlo-en-el-bucket-cuál-de-las-siguientes-modificaciones-debe-realizar-el-desarrollador-para-asegurar-que-los-datos-estén-cifrados-antes-de-cargarlos-en-el-bucket) |
| 6 | [Una empresa de software necesita asegurarse de que los documentos cargados por los usuarios se almacenen de forma segura en Amazon S3. Los documentos deben estar cifrados en reposo en Amazon S3. La empresa no desea administrar la infraestructura de seguridad internamente, pero aun así necesita protección adicional para asegurar que tiene control sobre sus claves de cifrado debido a regulaciones de la industria. ¿Qué estrategia de cifrado debe usar un desarrollador para cumplir con estos requisitos?](#una-empresa-de-software-necesita-asegurarse-de-que-los-documentos-cargados-por-los-usuarios-se-almacenen-de-forma-segura-en-amazon-s3-los-documentos-deben-estar-cifrados-en-reposo-en-amazon-s3-la-empresa-no-desea-administrar-la-infraestructura-de-seguridad-internamente-pero-aun-así-necesita-protección-adicional-para-asegurar-que-tiene-control-sobre-sus-claves-de-cifrado-debido-a-regulaciones-de-la-industria-qué-estrategia-de-cifrado-debe-usar-un-desarrollador-para-cumplir-con-estos-requisitos) |
| 7 | [Un equipo de desarrollo está creando una nueva aplicación diseñada para ejecutarse en AWS. Mientras que los entornos de prueba y producción se ejecutarán en instancias de Amazon EC2, cada desarrollador ejecutará su propio entorno en su laptop. ¿Cuál de las siguientes es la forma más simple y MÁS segura de acceder a los servicios de AWS desde las máquinas de desarrollo locales?](#un-equipo-de-desarrollo-está-creando-una-nueva-aplicación-diseñada-para-ejecutarse-en-aws-mientras-que-los-entornos-de-prueba-y-producción-se-ejecutarán-en-instancias-de-amazon-ec2-cada-desarrollador-ejecutará-su-propio-entorno-en-su-laptop-cuál-de-las-siguientes-es-la-forma-más-simple-y-más-segura-de-acceder-a-los-servicios-de-aws-desde-las-máquinas-de-desarrollo-locales) |
| 8 | [Una aplicación de juegos almacena las puntuaciones de los jugadores en una tabla de Amazon DynamoDB que tiene cuatro atributos: `user_id`, `user_name`, `user_score` y `user_rank`. Los usuarios pueden actualizar sus nombres únicamente si están autenticados mediante federación de identidad web (web identity federation). ¿Qué conjunto de condiciones debe agregarse en la política asociada al rol para la llamada a la API `dynamodb:PutItem`?](#una-aplicación-de-juegos-almacena-las-puntuaciones-de-los-jugadores-en-una-tabla-de-amazon-dynamodb-que-tiene-cuatro-atributos-user_id-user_name-user_score-y-user_rank-los-usuarios-pueden-actualizar-sus-nombres-únicamente-si-están-autenticados-mediante-federación-de-identidad-web-web-identity-federation-qué-conjunto-de-condiciones-debe-agregarse-en-la-política-asociada-al-rol-para-la-llamada-a-la-api-dynamodbputitem) |
| 9 | [Una aplicación que se ejecuta en instancias de EC2 almacena datos en un bucket de S3. La política de seguridad exige que todos los datos estén cifrados en tránsito. ¿Cómo puede el desarrollador asegurarse de que todo el tráfico hacia el bucket de S3 esté cifrado?](#una-aplicación-que-se-ejecuta-en-instancias-de-ec2-almacena-datos-en-un-bucket-de-s3-la-política-de-seguridad-exige-que-todos-los-datos-estén-cifrados-en-tránsito-cómo-puede-el-desarrollador-asegurarse-de-que-todo-el-tráfico-hacia-el-bucket-de-s3-esté-cifrado) |
| 10 | [Una empresa almacena toda la información de identificación personal (PII) en una tabla de Amazon DynamoDB llamada PII en la Cuenta A. Una aplicación que se ejecuta en instancias de Amazon EC2 en la Cuenta B requiere acceso a la tabla PII. Un administrador de la Cuenta A creó un rol de IAM llamado AccessPII con privilegios para acceder a la tabla PII y designó a la cuenta B como entidad de confianza. ¿Qué combinación de pasos de acción deben realizar los desarrolladores para acceder a la tabla? (Seleccione DOS)](#una-empresa-almacena-toda-la-información-de-identificación-personal-pii-en-una-tabla-de-amazon-dynamodb-llamada-pii-en-la-cuenta-a-una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-en-la-cuenta-b-requiere-acceso-a-la-tabla-pii-un-administrador-de-la-cuenta-a-creó-un-rol-de-iam-llamado-accesspii-con-privilegios-para-acceder-a-la-tabla-pii-y-designó-a-la-cuenta-b-como-entidad-de-confianza-qué-combinación-de-pasos-de-acción-deben-realizar-los-desarrolladores-para-acceder-a-la-tabla-seleccione-dos) |
| 11 | [Una aplicación web utiliza Amazon Kinesis Streams para datos de clickstream que podrían no consumirse hasta por 12 horas. ¿Cómo puede el desarrollador implementar el cifrado en reposo para los datos dentro de Kinesis Streams?](#una-aplicación-web-utiliza-amazon-kinesis-streams-para-datos-de-clickstream-que-podrían-no-consumirse-hasta-por-12-horas-cómo-puede-el-desarrollador-implementar-el-cifrado-en-reposo-para-los-datos-dentro-de-kinesis-streams) |
| 12 | [Un desarrollador está creando una aplicación móvil con un presupuesto limitado. La solución requiere un servicio escalable que permita a los clientes registrarse y autenticarse en la aplicación móvil utilizando el proveedor de identidad SAML 2.0 actual de la organización. ¿Qué servicio de AWS se debe utilizar para cumplir con estos requisitos?](#un-desarrollador-está-creando-una-aplicación-móvil-con-un-presupuesto-limitado-la-solución-requiere-un-servicio-escalable-que-permita-a-los-clientes-registrarse-y-autenticarse-en-la-aplicación-móvil-utilizando-el-proveedor-de-identidad-saml-20-actual-de-la-organización-qué-servicio-de-aws-se-debe-utilizar-para-cumplir-con-estos-requisitos) |
| 13 | [Un juego almacena los datos de juego de los usuarios en una tabla de Amazon DynamoDB. Los usuarios individuales no deben tener acceso a los datos de juego de otros usuarios. ¿Cómo se puede lograr esto?](#un-juego-almacena-los-datos-de-juego-de-los-usuarios-en-una-tabla-de-amazon-dynamodb-los-usuarios-individuales-no-deben-tener-acceso-a-los-datos-de-juego-de-otros-usuarios-cómo-se-puede-lograr-esto) |
| 14 | [Un desarrollador está creando una aplicación web que requiere autenticación, pero que también necesita admitir el acceso de invitados para brindar a los usuarios un acceso limitado sin tener que autenticarse. ¿Qué servicio puede permitir que la aplicación admita el acceso de invitados?](#un-desarrollador-está-creando-una-aplicación-web-que-requiere-autenticación-pero-que-también-necesita-admitir-el-acceso-de-invitados-para-brindar-a-los-usuarios-un-acceso-limitado-sin-tener-que-autenticarse-qué-servicio-puede-permitir-que-la-aplicación-admita-el-acceso-de-invitados) |
| 15 | [Una empresa está desarrollando un nuevo juego en línea que se ejecutará sobre Amazon ECS. Cuatro servicios distintos de Amazon ECS formarán parte de la arquitectura, y cada uno requiere permisos específicos para diversos servicios de AWS. La empresa quiere optimizar el uso de las instancias de Amazon EC2 subyacentes mediante bin packing de los contenedores según la reserva de memoria. ¿Qué configuración permitiría al equipo de desarrollo cumplir con estos requisitos de la forma MÁS segura?](#una-empresa-está-desarrollando-un-nuevo-juego-en-línea-que-se-ejecutará-sobre-amazon-ecs-cuatro-servicios-distintos-de-amazon-ecs-formarán-parte-de-la-arquitectura-y-cada-uno-requiere-permisos-específicos-para-diversos-servicios-de-aws-la-empresa-quiere-optimizar-el-uso-de-las-instancias-de-amazon-ec2-subyacentes-mediante-bin-packing-de-los-contenedores-según-la-reserva-de-memoria-qué-configuración-permitiría-al-equipo-de-desarrollo-cumplir-con-estos-requisitos-de-la-forma-más-segura) |
| 16 | [Una organización debe almacenar miles de archivos de audio y video sensibles en un bucket de Amazon S3. Las políticas de seguridad de la organización exigen que todos los datos escritos en este bucket estén cifrados. ¿Cómo se puede garantizar el cumplimiento de esta política?](#una-organización-debe-almacenar-miles-de-archivos-de-audio-y-video-sensibles-en-un-bucket-de-amazon-s3-las-políticas-de-seguridad-de-la-organización-exigen-que-todos-los-datos-escritos-en-este-bucket-estén-cifrados-cómo-se-puede-garantizar-el-cumplimiento-de-esta-política) |
| 17 | [Un desarrollador creó un dashboard para una aplicación que usa Amazon API Gateway, Amazon S3, AWS Lambda y Amazon RDS. El desarrollador necesita un mecanismo de autenticación que permita a un usuario iniciar sesión y ver el dashboard. Debe ser accesible desde aplicaciones móviles, equipos de escritorio y tablets, y debe recordar las preferencias del usuario entre plataformas. ¿Qué servicio de AWS debería usar el desarrollador para dar soporte a este escenario de autenticación?](#un-desarrollador-creó-un-dashboard-para-una-aplicación-que-usa-amazon-api-gateway-amazon-s3-aws-lambda-y-amazon-rds-el-desarrollador-necesita-un-mecanismo-de-autenticación-que-permita-a-un-usuario-iniciar-sesión-y-ver-el-dashboard-debe-ser-accesible-desde-aplicaciones-móviles-equipos-de-escritorio-y-tablets-y-debe-recordar-las-preferencias-del-usuario-entre-plataformas-qué-servicio-de-aws-debería-usar-el-desarrollador-para-dar-soporte-a-este-escenario-de-autenticación) |
| 18 | [Un desarrollador necesita acceso temporal a recursos en una segunda cuenta. ¿Cuál es la forma MÁS segura de lograrlo?](#un-desarrollador-necesita-acceso-temporal-a-recursos-en-una-segunda-cuenta-cuál-es-la-forma-más-segura-de-lograrlo) |
| 19 | [Un desarrollador está creando un Auto Scaling group cuyas instancias necesitan publicar una métrica personalizada en Amazon CloudWatch. ¿Qué método sería la forma MÁS segura de autenticar una solicitud PUT a CloudWatch?](#un-desarrollador-está-creando-un-auto-scaling-group-cuyas-instancias-necesitan-publicar-una-métrica-personalizada-en-amazon-cloudwatch-qué-método-sería-la-forma-más-segura-de-autenticar-una-solicitud-put-a-cloudwatch) |
| 20 | [Un equipo de desarrollo consta de 10 miembros. De forma similar a un directorio personal para cada miembro del equipo, el gerente quiere otorgar acceso a carpetas específicas de cada usuario en un bucket de Amazon S3. Para el miembro del equipo con el nombre de usuario `TeamMemberX`, el fragmento de la política de IAM se ve así. En lugar de crear políticas distintas para cada miembro del equipo, ¿qué enfoque puede usarse para hacer que este fragmento de política sea genérico para todos los miembros del equipo?](#un-equipo-de-desarrollo-consta-de-10-miembros-de-forma-similar-a-un-directorio-personal-para-cada-miembro-del-equipo-el-gerente-quiere-otorgar-acceso-a-carpetas-específicas-de-cada-usuario-en-un-bucket-de-amazon-s3-para-el-miembro-del-equipo-con-el-nombre-de-usuario-teammemberx-el-fragmento-de-la-política-de-iam-se-ve-así-en-lugar-de-crear-políticas-distintas-para-cada-miembro-del-equipo-qué-enfoque-puede-usarse-para-hacer-que-este-fragmento-de-política-sea-genérico-para-todos-los-miembros-del-equipo) |
| 21 | [Una empresa necesita cifrar datos en reposo, pero quiere aprovechar un servicio administrado de AWS usando su propia clave maestra. ¿Cuál de los siguientes servicios de AWS puede usarse para cumplir con estos requisitos?](#una-empresa-necesita-cifrar-datos-en-reposo-pero-quiere-aprovechar-un-servicio-administrado-de-aws-usando-su-propia-clave-maestra-cuál-de-los-siguientes-servicios-de-aws-puede-usarse-para-cumplir-con-estos-requisitos) |
| 22 | [Un desarrollador ha creado un paquete de software para desplegarlo en varias instancias de EC2 usando roles de IAM. ¿Qué acciones podrían realizarse para verificar el acceso de IAM para obtener registros de Amazon Kinesis Streams? (Seleccione DOS)](#un-desarrollador-ha-creado-un-paquete-de-software-para-desplegarlo-en-varias-instancias-de-ec2-usando-roles-de-iam-qué-acciones-podrían-realizarse-para-verificar-el-acceso-de-iam-para-obtener-registros-de-amazon-kinesis-streams-seleccione-dos) |
| 23 | [Un desarrollador está creando una aplicación que administra transacciones financieras. Para mejorar la seguridad, se requerirá la autenticación multifactor (MFA) como parte del protocolo de inicio de sesión. ¿Qué servicios puede usar el desarrollador para cumplir con estos requisitos?](#un-desarrollador-está-creando-una-aplicación-que-administra-transacciones-financieras-para-mejorar-la-seguridad-se-requerirá-la-autenticación-multifactor-mfa-como-parte-del-protocolo-de-inicio-de-sesión-qué-servicios-puede-usar-el-desarrollador-para-cumplir-con-estos-requisitos) |
| 24 | [Un desarrollador está probando una aplicación basada en Docker que usa el AWS SDK para interactuar con Amazon DynamoDB. En el entorno de desarrollo local, la aplicación ha usado claves de acceso de IAM. La aplicación ahora está lista para desplegarse en un clúster de ECS. ¿Cómo debería autenticarse la aplicación con los servicios de AWS en producción?](#un-desarrollador-está-probando-una-aplicación-basada-en-docker-que-usa-el-aws-sdk-para-interactuar-con-amazon-dynamodb-en-el-entorno-de-desarrollo-local-la-aplicación-ha-usado-claves-de-acceso-de-iam-la-aplicación-ahora-está-lista-para-desplegarse-en-un-clúster-de-ecs-cómo-debería-autenticarse-la-aplicación-con-los-servicios-de-aws-en-producción) |
| 25 | [Un desarrollador usa AWS CodeDeploy para automatizar el despliegue de una aplicación que se conecta a una base de datos MySQL externa. El desarrollador quiere acceder de forma segura a los secretos cifrados, como claves de API y contraseñas de bases de datos. ¿Cuál de las siguientes soluciones implicaría el MENOR esfuerzo administrativo?](#un-desarrollador-usa-aws-codedeploy-para-automatizar-el-despliegue-de-una-aplicación-que-se-conecta-a-una-base-de-datos-mysql-externa-el-desarrollador-quiere-acceder-de-forma-segura-a-los-secretos-cifrados-como-claves-de-api-y-contraseñas-de-bases-de-datos-cuál-de-las-siguientes-soluciones-implicaría-el-menor-esfuerzo-administrativo) |
| 26 | [Un desarrollador usará la AWS CLI en un servidor de desarrollo local para administrar servicios de AWS. ¿Qué se puede hacer para asegurar que la CLI use los permisos de IAM del desarrollador al ejecutar comandos?](#un-desarrollador-usará-la-aws-cli-en-un-servidor-de-desarrollo-local-para-administrar-servicios-de-aws-qué-se-puede-hacer-para-asegurar-que-la-cli-use-los-permisos-de-iam-del-desarrollador-al-ejecutar-comandos) |
| 27 | [Una aplicación tiene cientos de usuarios. Cada usuario puede usar múltiples dispositivos para acceder a la aplicación. El desarrollador quiere asignar identificadores únicos a estos usuarios sin importar el dispositivo que utilicen. ¿Cuál de los siguientes métodos debería usarse para obtener identificadores únicos?](#una-aplicación-tiene-cientos-de-usuarios-cada-usuario-puede-usar-múltiples-dispositivos-para-acceder-a-la-aplicación-el-desarrollador-quiere-asignar-identificadores-únicos-a-estos-usuarios-sin-importar-el-dispositivo-que-utilicen-cuál-de-los-siguientes-métodos-debería-usarse-para-obtener-identificadores-únicos) |
| 28 | [Un paquete de despliegue usa la AWS CLI para copiar archivos a cualquier bucket de S3 de la cuenta, usando claves de acceso almacenadas en variables de entorno. El paquete se ejecuta en instancias EC2, y las instancias se han modificado para ejecutarse con un rol de IAM asumido y una política más restrictiva que permite el acceso a un solo bucket. Después del cambio, el desarrollador inicia sesión en el host y aún tiene la capacidad de escribir en todos los buckets de S3 de esa cuenta. ¿Cuál es la causa MÁS probable de esta situación?](#un-paquete-de-despliegue-usa-la-aws-cli-para-copiar-archivos-a-cualquier-bucket-de-s3-de-la-cuenta-usando-claves-de-acceso-almacenadas-en-variables-de-entorno-el-paquete-se-ejecuta-en-instancias-ec2-y-las-instancias-se-han-modificado-para-ejecutarse-con-un-rol-de-iam-asumido-y-una-política-más-restrictiva-que-permite-el-acceso-a-un-solo-bucket-después-del-cambio-el-desarrollador-inicia-sesión-en-el-host-y-aún-tiene-la-capacidad-de-escribir-en-todos-los-buckets-de-s3-de-esa-cuenta-cuál-es-la-causa-más-probable-de-esta-situación) |
| 29 | [Una aplicación en desarrollo debe almacenar cientos de archivos de video. Los datos deben cifrarse dentro de la aplicación antes de almacenarse, con una clave única para cada archivo de video. ¿Cómo debería programar el desarrollador la aplicación?](#una-aplicación-en-desarrollo-debe-almacenar-cientos-de-archivos-de-video-los-datos-deben-cifrarse-dentro-de-la-aplicación-antes-de-almacenarse-con-una-clave-única-para-cada-archivo-de-video-cómo-debería-programar-el-desarrollador-la-aplicación) |
| 30 | [Un desarrollador debe asegurar que las credenciales de IAM usadas por una aplicación en Amazon EC2 no se usen indebidamente ni se vean comprometidas. ¿Qué debería usar el desarrollador para mantener seguras las credenciales de usuario?](#un-desarrollador-debe-asegurar-que-las-credenciales-de-iam-usadas-por-una-aplicación-en-amazon-ec2-no-se-usen-indebidamente-ni-se-vean-comprometidas-qué-debería-usar-el-desarrollador-para-mantener-seguras-las-credenciales-de-usuario) |
| 31 | [Una empresa tiene una aplicación donde la lectura de objetos desde Amazon S3 se basa en el tipo de usuario. Los tipos de usuario son usuario registrado y usuario invitado. La empresa tiene 25,000 usuarios y sigue creciendo. La información se obtiene de un bucket de S3 según el tipo de usuario. ¿Qué enfoques se recomiendan para proporcionar acceso a ambos tipos de usuarios? (Elija DOS)](#una-empresa-tiene-una-aplicación-donde-la-lectura-de-objetos-desde-amazon-s3-se-basa-en-el-tipo-de-usuario-los-tipos-de-usuario-son-usuario-registrado-y-usuario-invitado-la-empresa-tiene-25000-usuarios-y-sigue-creciendo-la-información-se-obtiene-de-un-bucket-de-s3-según-el-tipo-de-usuario-qué-enfoques-se-recomiendan-para-proporcionar-acceso-a-ambos-tipos-de-usuarios-elija-dos) |
| 32 | [Una empresa tiene 25,000 empleados y sigue creciendo. La empresa está creando una aplicación que será accesible solo para sus empleados. Un desarrollador está usando Amazon S3 para almacenar imágenes y Amazon RDS para almacenar los datos de la aplicación. La empresa requiere que toda la información de los empleados permanezca únicamente en el directorio de empleados heredado basado en Security Assertion Markup Language (SAML) y no está interesada en replicar ninguna información de los empleados en AWS. ¿Cómo puede el desarrollador proporcionar acceso autorizado a los empleados que usarán esta aplicación para que cada empleado pueda acceder solo a sus propios datos de la aplicación?](#una-empresa-tiene-25000-empleados-y-sigue-creciendo-la-empresa-está-creando-una-aplicación-que-será-accesible-solo-para-sus-empleados-un-desarrollador-está-usando-amazon-s3-para-almacenar-imágenes-y-amazon-rds-para-almacenar-los-datos-de-la-aplicación-la-empresa-requiere-que-toda-la-información-de-los-empleados-permanezca-únicamente-en-el-directorio-de-empleados-heredado-basado-en-security-assertion-markup-language-saml-y-no-está-interesada-en-replicar-ninguna-información-de-los-empleados-en-aws-cómo-puede-el-desarrollador-proporcionar-acceso-autorizado-a-los-empleados-que-usarán-esta-aplicación-para-que-cada-empleado-pueda-acceder-solo-a-sus-propios-datos-de-la-aplicación) |
| 33 | [Una aplicación necesita cifrar los datos que se escriben en Amazon S3, donde las claves se administran en un centro de datos on-premises y el cifrado lo gestiona S3. ¿Qué tipo de cifrado se debe utilizar?](#una-aplicación-necesita-cifrar-los-datos-que-se-escriben-en-amazon-s3-donde-las-claves-se-administran-en-un-centro-de-datos-on-premises-y-el-cifrado-lo-gestiona-s3-qué-tipo-de-cifrado-se-debe-utilizar) |
| 34 | [Una aplicación que se ejecuta en Amazon EC2 abre conexiones a una base de datos Amazon RDS SQL Server. El desarrollador no quiere almacenar el nombre de usuario y la contraseña de la base de datos en el código. El desarrollador también desea rotar las credenciales automáticamente. ¿Cuál es la forma MÁS segura de almacenar y acceder a las credenciales de la base de datos?](#una-aplicación-que-se-ejecuta-en-amazon-ec2-abre-conexiones-a-una-base-de-datos-amazon-rds-sql-server-el-desarrollador-no-quiere-almacenar-el-nombre-de-usuario-y-la-contraseña-de-la-base-de-datos-en-el-código-el-desarrollador-también-desea-rotar-las-credenciales-automáticamente-cuál-es-la-forma-más-segura-de-almacenar-y-acceder-a-las-credenciales-de-la-base-de-datos) |
| 35 | [Un equipo de desarrollo está diseñando una aplicación móvil que requiere autenticación multifactor. ¿Qué pasos se deben seguir para lograrlo? (Elija DOS)](#un-equipo-de-desarrollo-está-diseñando-una-aplicación-móvil-que-requiere-autenticación-multifactor-qué-pasos-se-deben-seguir-para-lograrlo-elija-dos) |
| 36 | [Dos microservicios en contenedores están alojados en Amazon EC2 ECS. El primer microservicio lee de una instancia de base de datos Amazon RDS Aurora y el segundo microservicio lee de una tabla de Amazon DynamoDB. ¿Cómo se pueden otorgar a cada microservicio los privilegios mínimos?](#dos-microservicios-en-contenedores-están-alojados-en-amazon-ec2-ecs-el-primer-microservicio-lee-de-una-instancia-de-base-de-datos-amazon-rds-aurora-y-el-segundo-microservicio-lee-de-una-tabla-de-amazon-dynamodb-cómo-se-pueden-otorgar-a-cada-microservicio-los-privilegios-mínimos) |
| 37 | [Un rol de IAM asociado a una instancia de Amazon EC2 deniega explícitamente el acceso a todas las acciones de la API de Amazon S3. El archivo de credenciales de la instancia de EC2 especifica la clave de acceso y la clave de acceso secreta de IAM, que permiten acceso administrativo completo. Dado que existen múltiples modos de acceso de IAM para esta instancia de EC2, ¿cuál de las siguientes afirmaciones es correcta?](#un-rol-de-iam-asociado-a-una-instancia-de-amazon-ec2-deniega-explícitamente-el-acceso-a-todas-las-acciones-de-la-api-de-amazon-s3-el-archivo-de-credenciales-de-la-instancia-de-ec2-especifica-la-clave-de-acceso-y-la-clave-de-acceso-secreta-de-iam-que-permiten-acceso-administrativo-completo-dado-que-existen-múltiples-modos-de-acceso-de-iam-para-esta-instancia-de-ec2-cuál-de-las-siguientes-afirmaciones-es-correcta) |
| 38 | [Un equipo de desarrollo está construyendo una nueva aplicación que se ejecutará en Amazon EC2 y usará Amazon DynamoDB como capa de almacenamiento. Todos los desarrolladores tienen cuentas de usuario de IAM asignadas en el mismo grupo de IAM. Actualmente los desarrolladores pueden lanzar instancias de EC2 y necesitan poder lanzar instancias de EC2 con un rol de instancia que permita el acceso a Amazon DynamoDB. ¿Qué cambios de AWS IAM son necesarios al crear un rol de instancia para proporcionar esta funcionalidad?](#un-equipo-de-desarrollo-está-construyendo-una-nueva-aplicación-que-se-ejecutará-en-amazon-ec2-y-usará-amazon-dynamodb-como-capa-de-almacenamiento-todos-los-desarrolladores-tienen-cuentas-de-usuario-de-iam-asignadas-en-el-mismo-grupo-de-iam-actualmente-los-desarrolladores-pueden-lanzar-instancias-de-ec2-y-necesitan-poder-lanzar-instancias-de-ec2-con-un-rol-de-instancia-que-permita-el-acceso-a-amazon-dynamodb-qué-cambios-de-aws-iam-son-necesarios-al-crear-un-rol-de-instancia-para-proporcionar-esta-funcionalidad) |
| 39 | [Una aplicación web de front-end usa los user pools de Amazon Cognito para gestionar el flujo de autenticación de usuarios. Un desarrollador está integrando Amazon DynamoDB en la aplicación usando el AWS SDK para JavaScript. ¿Cómo podría el desarrollador llamar a la API de forma segura sin exponer las claves de acceso ni secreta?](#una-aplicación-web-de-front-end-usa-los-user-pools-de-amazon-cognito-para-gestionar-el-flujo-de-autenticación-de-usuarios-un-desarrollador-está-integrando-amazon-dynamodb-en-la-aplicación-usando-el-aws-sdk-para-javascript-cómo-podría-el-desarrollador-llamar-a-la-api-de-forma-segura-sin-exponer-las-claves-de-acceso-ni-secreta) |
| 40 | [Una empresa usa Amazon API Gateway para administrar su API de cara al público. El CISO requiere que las APIs sean usadas únicamente por usuarios de la cuenta de prueba. ¿Cuál es la forma MÁS segura de restringir el acceso a la API a los usuarios de esta cuenta de AWS en particular?](#una-empresa-usa-amazon-api-gateway-para-administrar-su-api-de-cara-al-público-el-ciso-requiere-que-las-apis-sean-usadas-únicamente-por-usuarios-de-la-cuenta-de-prueba-cuál-es-la-forma-más-segura-de-restringir-el-acceso-a-la-api-a-los-usuarios-de-esta-cuenta-de-aws-en-particular) |
| 41 | [Un desarrollador debe permitir que usuarios invitados sin inicio de sesión accedan a un sitio habilitado con Amazon Cognito para ver archivos almacenados en un bucket de Amazon S3. ¿Cómo debería cumplir el desarrollador estos requisitos?](#un-desarrollador-debe-permitir-que-usuarios-invitados-sin-inicio-de-sesión-accedan-a-un-sitio-habilitado-con-amazon-cognito-para-ver-archivos-almacenados-en-un-bucket-de-amazon-s3-cómo-debería-cumplir-el-desarrollador-estos-requisitos) |
| 42 | [Un desarrollador necesita crear una aplicación que admita Security Assertion Markup Language (SAML) y autenticación con Facebook. También debe permitir el acceso a servicios de AWS, como Amazon DynamoDB. ¿Qué servicio o característica de AWS cumplirá estos requisitos con la MENOR cantidad de codificación adicional?](#un-desarrollador-necesita-crear-una-aplicación-que-admita-security-assertion-markup-language-saml-y-autenticación-con-facebook-también-debe-permitir-el-acceso-a-servicios-de-aws-como-amazon-dynamodb-qué-servicio-o-característica-de-aws-cumplirá-estos-requisitos-con-la-menor-cantidad-de-codificación-adicional) |
| 43 | [Un desarrollador está escribiendo una aplicación en AWS Lambda. Para simplificar las pruebas y los despliegues, el desarrollador necesita que la cadena de conexión a la base de datos pueda cambiarse fácilmente sin modificar el código de Lambda. ¿Cómo se puede cumplir este requisito?](#un-desarrollador-está-escribiendo-una-aplicación-en-aws-lambda-para-simplificar-las-pruebas-y-los-despliegues-el-desarrollador-necesita-que-la-cadena-de-conexión-a-la-base-de-datos-pueda-cambiarse-fácilmente-sin-modificar-el-código-de-lambda-cómo-se-puede-cumplir-este-requisito) |
| 44 | [Un desarrollador decide almacenar datos altamente seguros en Amazon S3 y quiere implementar cifrado del lado del servidor (SSE) con control granular sobre quién puede acceder a la clave maestra. La política de la empresa requiere que la clave maestra pueda crearse, rotarse y deshabilitarse fácilmente cuando sea necesario, todo por razones de seguridad. ¿Qué solución debería usarse para cumplir estos requisitos?](#un-desarrollador-decide-almacenar-datos-altamente-seguros-en-amazon-s3-y-quiere-implementar-cifrado-del-lado-del-servidor-sse-con-control-granular-sobre-quién-puede-acceder-a-la-clave-maestra-la-política-de-la-empresa-requiere-que-la-clave-maestra-pueda-crearse-rotarse-y-deshabilitarse-fácilmente-cuando-sea-necesario-todo-por-razones-de-seguridad-qué-solución-debería-usarse-para-cumplir-estos-requisitos) |
| 45 | [Un desarrollador está creando una aplicación que necesita almacenar datos en Amazon S3. La gerencia requiere que los datos se cifren antes de enviarse a Amazon S3 para su almacenamiento. Las claves de cifrado deben ser administradas por el equipo de Seguridad. ¿Qué enfoque debería adoptar el desarrollador para cumplir estos requisitos?](#un-desarrollador-está-creando-una-aplicación-que-necesita-almacenar-datos-en-amazon-s3-la-gerencia-requiere-que-los-datos-se-cifren-antes-de-enviarse-a-amazon-s3-para-su-almacenamiento-las-claves-de-cifrado-deben-ser-administradas-por-el-equipo-de-seguridad-qué-enfoque-debería-adoptar-el-desarrollador-para-cumplir-estos-requisitos) |
| 46 | [Un Developer está publicando datos de registro críticos en un log group de Amazon CloudWatch Logs, que fue creado hace 2 meses. El Developer debe cifrar los datos de registro usando una customer master key (CMK) de AWS KMS para que los datos futuros puedan cifrarse y así cumplir con la política de seguridad de la empresa. ¿Cómo puede el Developer cumplir este requisito?](#un-developer-está-publicando-datos-de-registro-críticos-en-un-log-group-de-amazon-cloudwatch-logs-que-fue-creado-hace-2-meses-el-developer-debe-cifrar-los-datos-de-registro-usando-una-customer-master-key-cmk-de-aws-kms-para-que-los-datos-futuros-puedan-cifrarse-y-así-cumplir-con-la-política-de-seguridad-de-la-empresa-cómo-puede-el-developer-cumplir-este-requisito) |
| 47 | [Un Developer tiene código que se ejecuta en instancias de Amazon EC2 y que necesita acceso de solo lectura a una tabla de Amazon DynamoDB. ¿Cuál es el enfoque MÁS seguro que debe adoptar el Developer para lograr esta tarea?](#un-developer-tiene-código-que-se-ejecuta-en-instancias-de-amazon-ec2-y-que-necesita-acceso-de-solo-lectura-a-una-tabla-de-amazon-dynamodb-cuál-es-el-enfoque-más-seguro-que-debe-adoptar-el-developer-para-lograr-esta-tarea) |
| 48 | [Un Developer usa buckets de Amazon S3 para el alojamiento de sitios web estáticos. El Developer crea un bucket de S3 para el código y otro bucket de S3 para los recursos (assets), como archivos de imagen y video. Se deniega el acceso cuando un usuario intenta acceder al bucket de recursos desde el bucket de código, y la aplicación del sitio web muestra un error `403`. ¿Cómo debe resolver el Developer este problema?](#un-developer-usa-buckets-de-amazon-s3-para-el-alojamiento-de-sitios-web-estáticos-el-developer-crea-un-bucket-de-s3-para-el-código-y-otro-bucket-de-s3-para-los-recursos-assets-como-archivos-de-imagen-y-video-se-deniega-el-acceso-cuando-un-usuario-intenta-acceder-al-bucket-de-recursos-desde-el-bucket-de-código-y-la-aplicación-del-sitio-web-muestra-un-error-403-cómo-debe-resolver-el-developer-este-problema) |
| 49 | [Una empresa quiere migrar un servicio de imágenes a Amazon EC2 siguiendo las mejores prácticas de seguridad. Las imágenes se obtienen y se leen desde un bucket de Amazon S3 no público. ¿Qué debe hacer un Developer para cumplir estos requisitos?](#una-empresa-quiere-migrar-un-servicio-de-imágenes-a-amazon-ec2-siguiendo-las-mejores-prácticas-de-seguridad-las-imágenes-se-obtienen-y-se-leen-desde-un-bucket-de-amazon-s3-no-público-qué-debe-hacer-un-developer-para-cumplir-estos-requisitos) |
| 50 | [Una empresa está desarrollando una aplicación a la que se accederá a través de la API REST de Amazon API Gateway. Solo los usuarios registrados deben poder acceder a ciertos recursos de esta API. El token utilizado debe expirar automáticamente y necesita actualizarse periódicamente. ¿Cómo puede un Developer cumplir estos requisitos?](#una-empresa-está-desarrollando-una-aplicación-a-la-que-se-accederá-a-través-de-la-api-rest-de-amazon-api-gateway-solo-los-usuarios-registrados-deben-poder-acceder-a-ciertos-recursos-de-esta-api-el-token-utilizado-debe-expirar-automáticamente-y-necesita-actualizarse-periódicamente-cómo-puede-un-developer-cumplir-estos-requisitos) |
| 51 | [Un Developer ha creado un nuevo usuario de AWS IAM que tiene el permiso `s3:putObject` para escribir en un bucket específico de Amazon S3. Este bucket de S3 usa cifrado del lado del servidor con claves administradas por AWS KMS (SSE-KMS) como cifrado predeterminado. Usando la clave de acceso y la clave secreta del usuario de IAM, la aplicación recibió un error de acceso denegado al llamar a la API `PutObject`. ¿Cómo se puede resolver este problema?](#un-developer-ha-creado-un-nuevo-usuario-de-aws-iam-que-tiene-el-permiso-s3putobject-para-escribir-en-un-bucket-específico-de-amazon-s3-este-bucket-de-s3-usa-cifrado-del-lado-del-servidor-con-claves-administradas-por-aws-kms-sse-kms-como-cifrado-predeterminado-usando-la-clave-de-acceso-y-la-clave-secreta-del-usuario-de-iam-la-aplicación-recibió-un-error-de-acceso-denegado-al-llamar-a-la-api-putobject-cómo-se-puede-resolver-este-problema) |
| 52 | [Una empresa tiene una aplicación web que usa un user pool de Amazon Cognito para la autenticación. La empresa quiere crear una página de inicio de sesión con el logotipo de la empresa. ¿Qué debe hacer un Developer para cumplir estos requisitos?](#una-empresa-tiene-una-aplicación-web-que-usa-un-user-pool-de-amazon-cognito-para-la-autenticación-la-empresa-quiere-crear-una-página-de-inicio-de-sesión-con-el-logotipo-de-la-empresa-qué-debe-hacer-un-developer-para-cumplir-estos-requisitos) |
| 53 | [Un Developer está trabajando en una función de AWS Lambda que accede a Amazon DynamoDB. La función de Lambda debe recuperar un elemento y actualizar algunos de sus atributos, o crear el elemento si no existe. La función de Lambda tiene acceso a la clave primaria. ¿Qué permisos de IAM debe solicitar el Developer para que la función de Lambda logre esta funcionalidad?](#un-developer-está-trabajando-en-una-función-de-aws-lambda-que-accede-a-amazon-dynamodb-la-función-de-lambda-debe-recuperar-un-elemento-y-actualizar-algunos-de-sus-atributos-o-crear-el-elemento-si-no-existe-la-función-de-lambda-tiene-acceso-a-la-clave-primaria-qué-permisos-de-iam-debe-solicitar-el-developer-para-que-la-función-de-lambda-logre-esta-funcionalidad) |
| 54 | [Un Developer está almacenando en Amazon S3 datos sensibles generados por una aplicación. El Developer quiere cifrar los datos en reposo. Una política de la empresa requiere un registro de auditoría de cuándo se usó la clave maestra y por quién. ¿Qué opción de cifrado cumplirá estos requisitos?](#un-developer-está-almacenando-en-amazon-s3-datos-sensibles-generados-por-una-aplicación-el-developer-quiere-cifrar-los-datos-en-reposo-una-política-de-la-empresa-requiere-un-registro-de-auditoría-de-cuándo-se-usó-la-clave-maestra-y-por-quién-qué-opción-de-cifrado-cumplirá-estos-requisitos) |
| 55 | [Un Developer quiere crear una aplicación que permita a nuevos usuarios registrarse y crear nuevas cuentas de usuario. La aplicación también debe permitir que los usuarios con cuentas de redes sociales inicien sesión usando sus credenciales de redes sociales. ¿Qué servicio o característica de AWS se puede usar para cumplir estos requisitos?](#un-developer-quiere-crear-una-aplicación-que-permita-a-nuevos-usuarios-registrarse-y-crear-nuevas-cuentas-de-usuario-la-aplicación-también-debe-permitir-que-los-usuarios-con-cuentas-de-redes-sociales-inicien-sesión-usando-sus-credenciales-de-redes-sociales-qué-servicio-o-característica-de-aws-se-puede-usar-para-cumplir-estos-requisitos) |
| 56 | [Un Desarrollador está intentando realizar llamadas a la API usando el SDK. Las credenciales del usuario de IAM utilizadas por la aplicación requieren autenticación multifactor para todas las llamadas a la API. ¿Qué método debe usar el Desarrollador para acceder a la API protegida con autenticación multifactor?](#un-desarrollador-está-intentando-realizar-llamadas-a-la-api-usando-el-sdk-las-credenciales-del-usuario-de-iam-utilizadas-por-la-aplicación-requieren-autenticación-multifactor-para-todas-las-llamadas-a-la-api-qué-método-debe-usar-el-desarrollador-para-acceder-a-la-api-protegida-con-autenticación-multifactor) |
| 57 | [Un Desarrollador está almacenando documentos sensibles en Amazon S3 que requerirán cifrado en reposo. Las claves de cifrado deben rotarse anualmente, como mínimo. ¿Cuál es la forma más sencilla de lograr esto?](#un-desarrollador-está-almacenando-documentos-sensibles-en-amazon-s3-que-requerirán-cifrado-en-reposo-las-claves-de-cifrado-deben-rotarse-anualmente-como-mínimo-cuál-es-la-forma-más-sencilla-de-lograr-esto) |
| 58 | [Un Desarrollador debe cifrar un objeto de 100 GB usando AWS KMS. ¿Cuál es el MEJOR enfoque?](#un-desarrollador-debe-cifrar-un-objeto-de-100-gb-usando-aws-kms-cuál-es-el-mejor-enfoque) |
| 59 | [¿Cuáles de los siguientes elementos se requieren para permitir que una aplicación desplegada en una instancia de EC2 escriba datos en una tabla de DynamoDB? Suponga que no se permite almacenar claves de seguridad en la instancia de EC2. (Elija DOS)](#cuáles-de-los-siguientes-elementos-se-requieren-para-permitir-que-una-aplicación-desplegada-en-una-instancia-de-ec2-escriba-datos-en-una-tabla-de-dynamodb-suponga-que-no-se-permite-almacenar-claves-de-seguridad-en-la-instancia-de-ec2-elija-dos) |
| 60 | [¿Cuáles de las siguientes son afirmaciones correctas sobre la lógica de evaluación de políticas en AWS Identity and Access Management? (Elija DOS)](#cuáles-de-las-siguientes-son-afirmaciones-correctas-sobre-la-lógica-de-evaluación-de-políticas-en-aws-identity-and-access-management-elija-dos) |
| 61 | [Al cargar un objeto, ¿qué encabezado de solicitud se puede especificar explícitamente en una solicitud a Amazon S3 para cifrar los datos del objeto cuando se guardan en el lado del servidor?](#al-cargar-un-objeto-qué-encabezado-de-solicitud-se-puede-especificar-explícitamente-en-una-solicitud-a-amazon-s3-para-cifrar-los-datos-del-objeto-cuando-se-guardan-en-el-lado-del-servidor) |
| 62 | [¿Qué características se pueden usar para restringir el acceso a los datos en S3? (Elija DOS)](#qué-características-se-pueden-usar-para-restringir-el-acceso-a-los-datos-en-s3-elija-dos) |
| 63 | [En AWS, ¿qué aspectos de seguridad son responsabilidad del cliente? (Elija CUATRO)](#en-aws-qué-aspectos-de-seguridad-son-responsabilidad-del-cliente-elija-cuatro) |
| 64 | [¿Cómo se pueden proteger los datos en reposo en un volumen de EBS?](#cómo-se-pueden-proteger-los-datos-en-reposo-en-un-volumen-de-ebs) |
| 65 | [Games-R-Us va a lanzar una nueva aplicación de juegos para dispositivos móviles. Los usuarios iniciarán sesión en el juego con su cuenta de Facebook existente y el juego registrará los datos del jugador y la información de puntuación directamente en una tabla de DynamoDB. ¿Cuál es el enfoque más seguro para firmar las solicitudes a la API de DynamoDB?](#games-r-us-va-a-lanzar-una-nueva-aplicación-de-juegos-para-dispositivos-móviles-los-usuarios-iniciarán-sesión-en-el-juego-con-su-cuenta-de-facebook-existente-y-el-juego-registrará-los-datos-del-jugador-y-la-información-de-puntuación-directamente-en-una-tabla-de-dynamodb-cuál-es-el-enfoque-más-seguro-para-firmar-las-solicitudes-a-la-api-de-dynamodb) |
| 66 | [Usted opera un sitio web de fotos con publicidad que usa S3 para servir fotos a los visitantes de su sitio. En algún momento descubre que otros sitios han estado enlazando a las fotos de su sitio, lo que causa pérdidas a su negocio. ¿Cuál es un método eficaz para mitigar esto?](#usted-opera-un-sitio-web-de-fotos-con-publicidad-que-usa-s3-para-servir-fotos-a-los-visitantes-de-su-sitio-en-algún-momento-descubre-que-otros-sitios-han-estado-enlazando-a-las-fotos-de-su-sitio-lo-que-causa-pérdidas-a-su-negocio-cuál-es-un-método-eficaz-para-mitigar-esto) |
| 67 | [Una aplicación web corporativa está desplegada dentro de una Amazon VPC y está conectada al centro de datos corporativo mediante una VPN IPSec. La aplicación debe autenticarse contra el servidor LDAP local (on-premise). Una vez autenticados, los usuarios que iniciaron sesión solo pueden acceder a un keyspace de S3 específico del usuario. ¿Qué dos enfoques pueden satisfacer los objetivos? (Elija DOS)](#una-aplicación-web-corporativa-está-desplegada-dentro-de-una-amazon-vpc-y-está-conectada-al-centro-de-datos-corporativo-mediante-una-vpn-ipsec-la-aplicación-debe-autenticarse-contra-el-servidor-ldap-local-on-premise-una-vez-autenticados-los-usuarios-que-iniciaron-sesión-solo-pueden-acceder-a-un-keyspace-de-s3-específico-del-usuario-qué-dos-enfoques-pueden-satisfacer-los-objetivos-elija-dos) |
| 68 | [¿Qué tipo de cifrado por bloques ofrece Amazon S3 para el cifrado del lado del servidor?](#qué-tipo-de-cifrado-por-bloques-ofrece-amazon-s3-para-el-cifrado-del-lado-del-servidor) |
| 69 | [Un desarrollador accede a AWS CodeCommit mediante SSH. Las claves SSH configuradas para acceder a AWS CodeCommit están asociadas a un usuario con los siguientes permisos. El desarrollador necesita crear/eliminar ramas. ¿Qué permisos específicos de IAM deben agregarse, según el principio de mínimo privilegio?](#un-desarrollador-accede-a-aws-codecommit-mediante-ssh-las-claves-ssh-configuradas-para-acceder-a-aws-codecommit-están-asociadas-a-un-usuario-con-los-siguientes-permisos-el-desarrollador-necesita-creareliminar-ramas-qué-permisos-específicos-de-iam-deben-agregarse-según-el-principio-de-mínimo-privilegio) |
| 70 | [Una función de AWS Lambda debe acceder a un sitio externo utilizando un nombre de usuario y una contraseña que se rotan regularmente. Estos elementos deben mantenerse de forma segura y no pueden almacenarse en el código de la función. ¿Qué combinación de servicios de AWS se puede usar para lograrlo? (Elija DOS)](#una-función-de-aws-lambda-debe-acceder-a-un-sitio-externo-utilizando-un-nombre-de-usuario-y-una-contraseña-que-se-rotan-regularmente-estos-elementos-deben-mantenerse-de-forma-segura-y-no-pueden-almacenarse-en-el-código-de-la-función-qué-combinación-de-servicios-de-aws-se-puede-usar-para-lograrlo-elija-dos) |
| 71 | [Un desarrollador está trabajando en una aplicación que maneja documentos de 10MB que contienen datos altamente sensibles. La aplicación usará AWS KMS para realizar cifrado del lado del cliente. ¿Qué pasos se deben seguir?](#un-desarrollador-está-trabajando-en-una-aplicación-que-maneja-documentos-de-10mb-que-contienen-datos-altamente-sensibles-la-aplicación-usará-aws-kms-para-realizar-cifrado-del-lado-del-cliente-qué-pasos-se-deben-seguir) |
| 72 | [Una empresa necesita distribuir actualizaciones de firmware a sus clientes en todo el mundo. ¿Qué servicio permitirá un control fácil y seguro del acceso a las descargas al menor costo?](#una-empresa-necesita-distribuir-actualizaciones-de-firmware-a-sus-clientes-en-todo-el-mundo-qué-servicio-permitirá-un-control-fácil-y-seguro-del-acceso-a-las-descargas-al-menor-costo) |
| 73 | [Un desarrollador está escribiendo una aplicación móvil que permite a los usuarios ver imágenes de un bucket de S3. Los usuarios deben poder iniciar sesión con su cuenta de Amazon, así como con cuentas de Facebook y/o Google. ¿Cómo puede el desarrollador proporcionar esta funcionalidad de autenticación?](#un-desarrollador-está-escribiendo-una-aplicación-móvil-que-permite-a-los-usuarios-ver-imágenes-de-un-bucket-de-s3-los-usuarios-deben-poder-iniciar-sesión-con-su-cuenta-de-amazon-así-como-con-cuentas-de-facebook-yo-google-cómo-puede-el-desarrollador-proporcionar-esta-funcionalidad-de-autenticación) |
| 74 | [Una empresa está creando una aplicación que requerirá que los usuarios accedan a servicios de AWS y les permitirá restablecer sus propias contraseñas. ¿Cuál de las siguientes opciones permitiría a la empresa administrar usuarios y autorización, y a la vez permitir que los usuarios restablezcan sus propias contraseñas?](#una-empresa-está-creando-una-aplicación-que-requerirá-que-los-usuarios-accedan-a-servicios-de-aws-y-les-permitirá-restablecer-sus-propias-contraseñas-cuál-de-las-siguientes-opciones-permitiría-a-la-empresa-administrar-usuarios-y-autorización-y-a-la-vez-permitir-que-los-usuarios-restablezcan-sus-propias-contraseñas) |
| 75 | [Una aplicación que se ejecuta en una instancia de Amazon EC2 necesita acceder y realizar llamadas a la API de varios servicios de AWS. ¿Cuál es la forma MÁS segura de proporcionar acceso a los servicios de AWS con una sobrecarga de administración MÍNIMA?](#una-aplicación-que-se-ejecuta-en-una-instancia-de-amazon-ec2-necesita-acceder-y-realizar-llamadas-a-la-api-de-varios-servicios-de-aws-cuál-es-la-forma-más-segura-de-proporcionar-acceso-a-los-servicios-de-aws-con-una-sobrecarga-de-administración-mínima) |
| 76 | [Una empresa está desarrollando una aplicación que se ejecutará en varias instancias de Amazon EC2 en un Auto Scaling group y que puede acceder a una base de datos que se ejecuta en Amazon EC2. La aplicación necesita almacenar los secretos necesarios para conectarse a la base de datos. La aplicación debe permitir la rotación periódica de secretos y no debe requerir cambios cuando un secreto cambie. ¿Cuál es la forma MÁS segura de cumplir estos requisitos?](#una-empresa-está-desarrollando-una-aplicación-que-se-ejecutará-en-varias-instancias-de-amazon-ec2-en-un-auto-scaling-group-y-que-puede-acceder-a-una-base-de-datos-que-se-ejecuta-en-amazon-ec2-la-aplicación-necesita-almacenar-los-secretos-necesarios-para-conectarse-a-la-base-de-datos-la-aplicación-debe-permitir-la-rotación-periódica-de-secretos-y-no-debe-requerir-cambios-cuando-un-secreto-cambie-cuál-es-la-forma-más-segura-de-cumplir-estos-requisitos) |
| 77 | [Un desarrollador está diseñando una nueva aplicación que usa Amazon S3. Para cumplir con los requisitos de conformidad, el desarrollador debe cifrar los datos en reposo. ¿Cómo puede lograrlo el desarrollador?](#un-desarrollador-está-diseñando-una-nueva-aplicación-que-usa-amazon-s3-para-cumplir-con-los-requisitos-de-conformidad-el-desarrollador-debe-cifrar-los-datos-en-reposo-cómo-puede-lograrlo-el-desarrollador) |
| 78 | [Una empresa necesita proteger su sitio web existente que se ejecuta detrás de un Elastic Load Balancer. Las instancias de Amazon EC2 del sitio web tienen limitaciones de CPU. ¿Qué se debe hacer para proteger el sitio web sin aumentar la carga de CPU de los servidores web EC2? (Seleccione DOS)](#una-empresa-necesita-proteger-su-sitio-web-existente-que-se-ejecuta-detrás-de-un-elastic-load-balancer-las-instancias-de-amazon-ec2-del-sitio-web-tienen-limitaciones-de-cpu-qué-se-debe-hacer-para-proteger-el-sitio-web-sin-aumentar-la-carga-de-cpu-de-los-servidores-web-ec2-seleccione-dos) |
| 79 | [Un desarrollador está creando una aplicación móvil que no requerirá que los usuarios inicien sesión. ¿Cuál es el método MÁS eficiente para otorgar a los usuarios acceso a los recursos de AWS?](#un-desarrollador-está-creando-una-aplicación-móvil-que-no-requerirá-que-los-usuarios-inicien-sesión-cuál-es-el-método-más-eficiente-para-otorgar-a-los-usuarios-acceso-a-los-recursos-de-aws) |
| 80 | [Una aplicación que se ejecuta en instancias de Amazon EC2 debe acceder a objetos dentro de un bucket de Amazon S3 que están cifrados mediante cifrado del lado del servidor con claves de cifrado de AWS KMS (SSE-KMS). La aplicación debe tener acceso a la customer master key (CMK) para descifrar los objetos. ¿Qué combinación de pasos otorgará acceso a la aplicación? (Seleccione DOS)](#una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-debe-acceder-a-objetos-dentro-de-un-bucket-de-amazon-s3-que-están-cifrados-mediante-cifrado-del-lado-del-servidor-con-claves-de-cifrado-de-aws-kms-sse-kms-la-aplicación-debe-tener-acceso-a-la-customer-master-key-cmk-para-descifrar-los-objetos-qué-combinación-de-pasos-otorgará-acceso-a-la-aplicación-seleccione-dos) |
| 81 | [Un equipo de desarrollo está trabajando en una solución de gestión de casos que permite procesar y revisar reclamaciones médicas. Los usuarios inician sesión para proporcionar información relacionada con su situación médica y financiera. Como parte de la aplicación, se cargan a Amazon S3 documentos sensibles como historiales médicos, imágenes médicas, estados de cuenta bancarios y recibos. Todos los documentos deben transmitirse y almacenarse de forma segura. Todo acceso a los documentos debe registrarse para auditoría. ¿Cuál es el enfoque MÁS seguro?](#un-equipo-de-desarrollo-está-trabajando-en-una-solución-de-gestión-de-casos-que-permite-procesar-y-revisar-reclamaciones-médicas-los-usuarios-inician-sesión-para-proporcionar-información-relacionada-con-su-situación-médica-y-financiera-como-parte-de-la-aplicación-se-cargan-a-amazon-s3-documentos-sensibles-como-historiales-médicos-imágenes-médicas-estados-de-cuenta-bancarios-y-recibos-todos-los-documentos-deben-transmitirse-y-almacenarse-de-forma-segura-todo-acceso-a-los-documentos-debe-registrarse-para-auditoría-cuál-es-el-enfoque-más-seguro) |
| 82 | [Una empresa tiene una aplicación expuesta a internet que usa Web Identity Federation para obtener una credencial temporal de AWS Security Token Service (AWS STS). Luego la aplicación usa el token para acceder a servicios de AWS. Revise la siguiente respuesta: Según la respuesta mostrada, ¿qué permisos están asociados con la llamada de la aplicación?](#una-empresa-tiene-una-aplicación-expuesta-a-internet-que-usa-web-identity-federation-para-obtener-una-credencial-temporal-de-aws-security-token-service-aws-sts-luego-la-aplicación-usa-el-token-para-acceder-a-servicios-de-aws-revise-la-siguiente-respuesta-según-la-respuesta-mostrada-qué-permisos-están-asociados-con-la-llamada-de-la-aplicación) |
| 83 | [Una aplicación web está diseñada para permitir que nuevos usuarios creen cuentas usando sus direcciones de correo electrónico. La aplicación almacenará atributos de cada usuario y se espera que se registren millones de usuarios. ¿Qué debe implementar el desarrollador para lograr los objetivos de diseño?](#una-aplicación-web-está-diseñada-para-permitir-que-nuevos-usuarios-creen-cuentas-usando-sus-direcciones-de-correo-electrónico-la-aplicación-almacenará-atributos-de-cada-usuario-y-se-espera-que-se-registren-millones-de-usuarios-qué-debe-implementar-el-desarrollador-para-lograr-los-objetivos-de-diseño) |
| 84 | [Una empresa necesita una nueva API REST que pueda devolver información sobre el contenido de un bucket de Amazon S3, como el conteo de objetos almacenados en él. La empresa ha decidido que la nueva API se escriba como un microservicio usando AWS Lambda y Amazon API Gateway. ¿Cómo debe asegurarse el desarrollador de que el microservicio tenga el acceso necesario al bucket de Amazon S3, respetando las mejores prácticas de seguridad?](#una-empresa-necesita-una-nueva-api-rest-que-pueda-devolver-información-sobre-el-contenido-de-un-bucket-de-amazon-s3-como-el-conteo-de-objetos-almacenados-en-él-la-empresa-ha-decidido-que-la-nueva-api-se-escriba-como-un-microservicio-usando-aws-lambda-y-amazon-api-gateway-cómo-debe-asegurarse-el-desarrollador-de-que-el-microservicio-tenga-el-acceso-necesario-al-bucket-de-amazon-s3-respetando-las-mejores-prácticas-de-seguridad) |
| 85 | [Una organización usa Amazon CloudFront para asegurar que sus usuarios tengan acceso de baja latencia a su aplicación web. La organización ha identificado la necesidad de cifrar todo el tráfico entre los usuarios y CloudFront, y todo el tráfico entre CloudFront y la aplicación web. ¿Cómo se pueden cumplir estos requisitos? (Elija DOS)](#una-organización-usa-amazon-cloudfront-para-asegurar-que-sus-usuarios-tengan-acceso-de-baja-latencia-a-su-aplicación-web-la-organización-ha-identificado-la-necesidad-de-cifrar-todo-el-tráfico-entre-los-usuarios-y-cloudfront-y-todo-el-tráfico-entre-cloudfront-y-la-aplicación-web-cómo-se-pueden-cumplir-estos-requisitos-elija-dos) |
| 86 | [Según las mejores prácticas, ¿cómo deben administrarse las claves de acceso en AWS? (Elija DOS)](#según-las-mejores-prácticas-cómo-deben-administrarse-las-claves-de-acceso-en-aws-elija-dos) |
| 87 | [Una aplicación que se ejecuta en una instancia EC2 de Amazon Linux necesita administrar la infraestructura de AWS. ¿Cómo se puede configurar la instancia EC2 para realizar llamadas a la API de AWS de forma segura?](#una-aplicación-que-se-ejecuta-en-una-instancia-ec2-de-amazon-linux-necesita-administrar-la-infraestructura-de-aws-cómo-se-puede-configurar-la-instancia-ec2-para-realizar-llamadas-a-la-api-de-aws-de-forma-segura) |
| 88 | [Una empresa de redes sociales usa Amazon Cognito para sincronizar perfiles entre diferentes dispositivos móviles, con el fin de que los usuarios finales tengan una experiencia fluida. ¿Cuál de las siguientes configuraciones puede usarse para notificar de forma silenciosa a los usuarios cada vez que haya una actualización disponible en todos los demás dispositivos?](#una-empresa-de-redes-sociales-usa-amazon-cognito-para-sincronizar-perfiles-entre-diferentes-dispositivos-móviles-con-el-fin-de-que-los-usuarios-finales-tengan-una-experiencia-fluida-cuál-de-las-siguientes-configuraciones-puede-usarse-para-notificar-de-forma-silenciosa-a-los-usuarios-cada-vez-que-haya-una-actualización-disponible-en-todos-los-demás-dispositivos) |
| 89 | [Una empresa desarrolló un conjunto de APIs que se sirven a través de Amazon API Gateway. Las llamadas a la API deben autenticarse basándose en proveedores de identidad OpenID como Amazon o Facebook. Las APIs deben permitir el acceso basándose en un modelo de autorización personalizado. ¿Cuál es el diseño más simple y MÁS seguro para construir un modelo de autenticación y autorización para las APIs?](#una-empresa-desarrolló-un-conjunto-de-apis-que-se-sirven-a-través-de-amazon-api-gateway-las-llamadas-a-la-api-deben-autenticarse-basándose-en-proveedores-de-identidad-openid-como-amazon-o-facebook-las-apis-deben-permitir-el-acceso-basándose-en-un-modelo-de-autorización-personalizado-cuál-es-el-diseño-más-simple-y-más-seguro-para-construir-un-modelo-de-autenticación-y-autorización-para-las-apis) |

### Un desarrollador desea cargar datos en Amazon S3 y debe cifrar los datos en tránsito. ¿Cuáles de las siguientes soluciones lograrán esta tarea? (Elija DOS)

- [ ] Configurar túneles VPN de hardware hacia una VPC y acceder a S3 a través de un VPC endpoint.
- [x] Configurar el cifrado del lado del cliente con una Customer Master Key administrada por AWS KMS.
- [ ] Configurar el cifrado del lado del servidor con claves administradas por AWS KMS.
- [x] Transferir los datos a través de una conexión SSL.
- [ ] Configurar el cifrado del lado del servidor con claves administradas por S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador desea cifrar los nuevos objetos que una aplicación carga en un bucket de Amazon S3. Debe existir un registro de auditoría de quién ha utilizado la clave durante este proceso. No debe haber ningún cambio en el rendimiento de la aplicación. ¿Qué tipo de cifrado cumple con estos requisitos?

- [ ] Cifrado del lado del servidor con claves administradas por S3.
- [x] Cifrado del lado del servidor con claves administradas por AWS KMS.
- [ ] Cifrado del lado del cliente con una clave maestra simétrica del lado del cliente.
- [ ] Cifrado del lado del cliente con claves administradas por AWS KMS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Se está desarrollando una aplicación para auditar varias cuentas de AWS. La aplicación se ejecutará en la Cuenta A y debe acceder a servicios de AWS en las Cuentas B y C. ¿Cuál es la forma MÁS segura de permitir que la aplicación llame a los servicios de AWS en cada cuenta auditada?

- [x] Configurar roles entre cuentas (cross-account) en cada cuenta auditada. Escribir código en la Cuenta A que asuma esos roles.
- [ ] Usar la replicación entre regiones de S3 para comunicarse entre las cuentas, con notificaciones de eventos de Amazon S3 para activar funciones Lambda.
- [ ] Implementar una aplicación en cada cuenta auditada con su propio rol. Hacer que la Cuenta A se autentique con la aplicación.
- [ ] Crear un usuario de IAM con una clave de acceso en cada cuenta auditada. Escribir código en la Cuenta A que use esas claves de acceso.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está construyendo una aplicación de uso intensivo de cómputo que se ejecutará en una flota de instancias de Amazon EC2. La aplicación utiliza discos de Amazon EBS conectados para almacenar datos. La aplicación procesará información confidencial y todos los datos deben estar cifrados. ¿Qué debe hacer un desarrollador para asegurar que los datos estén cifrados en disco sin afectar el rendimiento?

- [x] Configurar la flota de instancias de Amazon EC2 para que use volúmenes de EBS cifrados para almacenar datos.
- [ ] Agregar lógica para escribir todos los datos en un bucket de Amazon S3 cifrado.
- [ ] Agregar un algoritmo de cifrado personalizado a la aplicación que cifre y descifre todos los datos.
- [ ] Crear una nueva Amazon Machine Image (AMI) con un volumen raíz cifrado y almacenar los datos en discos efímeros.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una función de AWS Lambda genera un archivo JSON de 3 MB y luego lo carga diariamente en un bucket de Amazon S3. El archivo contiene información confidencial, por lo que el desarrollador debe asegurarse de que esté cifrado antes de cargarlo en el bucket. ¿Cuál de las siguientes modificaciones debe realizar el desarrollador para asegurar que los datos estén cifrados antes de cargarlos en el bucket?

- [ ] Usar la customer master key de AWS KMS predeterminada para S3 en el código de la función Lambda.
- [ ] Usar la clave administrada por S3 y llamar a la API `GenerateDataKey` para cifrar el archivo.
- [x] Usar la API `GenerateDataKey` y luego usar esa clave de datos para cifrar el archivo en el código de la función Lambda.
- [ ] Usar una customer master key de KMS personalizada creada para S3 en el código de la función Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa de software necesita asegurarse de que los documentos cargados por los usuarios se almacenen de forma segura en Amazon S3. Los documentos deben estar cifrados en reposo en Amazon S3. La empresa no desea administrar la infraestructura de seguridad internamente, pero aun así necesita protección adicional para asegurar que tiene control sobre sus claves de cifrado debido a regulaciones de la industria. ¿Qué estrategia de cifrado debe usar un desarrollador para cumplir con estos requisitos?

- [ ] Cifrado del lado del servidor con claves administradas por Amazon S3 (SSE-S3).
- [ ] Cifrado del lado del servidor con claves de cifrado proporcionadas por el cliente (SSE-C).
- [x] Cifrado del lado del servidor con claves administradas por AWS KMS (SSE-KMS).
- [ ] Cifrado del lado del cliente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo está creando una nueva aplicación diseñada para ejecutarse en AWS. Mientras que los entornos de prueba y producción se ejecutarán en instancias de Amazon EC2, cada desarrollador ejecutará su propio entorno en su laptop. ¿Cuál de las siguientes es la forma más simple y MÁS segura de acceder a los servicios de AWS desde las máquinas de desarrollo locales?

- [ ] Usar un rol de IAM para asumir un rol y ejecutar llamadas a la API utilizando ese rol.
- [ ] Crear un usuario de IAM compartido con todo el equipo de desarrollo y proporcionarle al equipo la clave de acceso.
- [x] Crear un usuario de IAM para cada desarrollador del equipo: proporcionar a cada desarrollador una clave de acceso única.
- [ ] Configurar una federación a través de un Amazon Cognito user pool.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación de juegos almacena las puntuaciones de los jugadores en una tabla de Amazon DynamoDB que tiene cuatro atributos: `user_id`, `user_name`, `user_score` y `user_rank`. Los usuarios pueden actualizar sus nombres únicamente si están autenticados mediante federación de identidad web (web identity federation). ¿Qué conjunto de condiciones debe agregarse en la política asociada al rol para la llamada a la API `dynamodb:PutItem`?

- [x] Opción A.
![Question 30 option A](images/question30_A.jpg)
- [ ] Opción B.
![Question 30 option B](images/question30_B.jpg)
- [ ] Opción C.
![Question 30 option C](images/question30_C.jpg)
- [ ] Opción D.
![Question 30 option D](images/question30_D.jpg)

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación que se ejecuta en instancias de EC2 almacena datos en un bucket de S3. La política de seguridad exige que todos los datos estén cifrados en tránsito. ¿Cómo puede el desarrollador asegurarse de que todo el tráfico hacia el bucket de S3 esté cifrado?

- [ ] Instalar certificados en las instancias de EC2.
- [ ] Crear una política de bucket que permita el tráfico donde `SecureTransport` sea `true`.
- [ ] Crear una redirección HTTPS en las instancias de EC2.
- [x] Crear una política de bucket que deniegue el tráfico donde `SecureTransport` sea `false`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa almacena toda la información de identificación personal (PII) en una tabla de Amazon DynamoDB llamada PII en la Cuenta A. Una aplicación que se ejecuta en instancias de Amazon EC2 en la Cuenta B requiere acceso a la tabla PII. Un administrador de la Cuenta A creó un rol de IAM llamado AccessPII con privilegios para acceder a la tabla PII y designó a la cuenta B como entidad de confianza. ¿Qué combinación de pasos de acción deben realizar los desarrolladores para acceder a la tabla? (Seleccione DOS)

- [x] Permitir que el rol de IAM de EC2 tenga el permiso para asumir el rol AccessPII.
- [ ] Permitir que el rol de IAM de EC2 tenga el permiso para acceder a la tabla PII.
- [ ] Incluir la AWS API en la lógica del código de la aplicación para obtener credenciales temporales del rol de IAM de EC2 y acceder a la tabla PII.
- [x] Incluir la operación de API `AssumeRole` en la lógica del código de la aplicación para obtener credenciales temporales y acceder a la tabla PII.
- [ ] Incluir la operación de API GetSessionToken en la lógica del código de la aplicación para obtener credenciales temporales y acceder a la tabla PII.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación web utiliza Amazon Kinesis Streams para datos de clickstream que podrían no consumirse hasta por 12 horas. ¿Cómo puede el desarrollador implementar el cifrado en reposo para los datos dentro de Kinesis Streams?

- [ ] Habilitar conexiones SSL a Kinesis.
- [ ] Usar la Amazon Kinesis Consumer Library.
- [ ] Cifrar los datos una vez en reposo con una función de Lambda.
- [x] Habilitar el cifrado del lado del servidor en Kinesis Streams.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación móvil con un presupuesto limitado. La solución requiere un servicio escalable que permita a los clientes registrarse y autenticarse en la aplicación móvil utilizando el proveedor de identidad SAML 2.0 actual de la organización. ¿Qué servicio de AWS se debe utilizar para cumplir con estos requisitos?

- [ ] AWS Lambda.
- [x] Amazon Cognito.
- [ ] AWS IAM.
- [ ] Amazon EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un juego almacena los datos de juego de los usuarios en una tabla de Amazon DynamoDB. Los usuarios individuales no deben tener acceso a los datos de juego de otros usuarios. ¿Cómo se puede lograr esto?

- [ ] Cifrar los datos del juego con claves individuales por usuario.
- [x] Restringir el acceso a elementos específicos según ciertos valores de la clave primaria.
- [ ] Almacenar temporalmente los datos en colas de SQS para inyectar metadatos antes de acceder a DynamoDB.
- [ ] Leer los registros de DynamoDB y descartar los datos irrelevantes del lado del cliente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación web que requiere autenticación, pero que también necesita admitir el acceso de invitados para brindar a los usuarios un acceso limitado sin tener que autenticarse. ¿Qué servicio puede permitir que la aplicación admita el acceso de invitados?

- [ ] Credenciales temporales de IAM mediante AWS STS.
- [ ] Amazon Directory Service.
- [x] Amazon Cognito con acceso no autenticado habilitado.
- [ ] IAM con integración SAML

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está desarrollando un nuevo juego en línea que se ejecutará sobre Amazon ECS. Cuatro servicios distintos de Amazon ECS formarán parte de la arquitectura, y cada uno requiere permisos específicos para diversos servicios de AWS. La empresa quiere optimizar el uso de las instancias de Amazon EC2 subyacentes mediante bin packing de los contenedores según la reserva de memoria. ¿Qué configuración permitiría al equipo de desarrollo cumplir con estos requisitos de la forma MÁS segura?

- [ ] Crear un nuevo perfil de instancia de Identity and Access Management (IAM) que contenga los permisos requeridos para los diversos servicios de ECS y luego asociar ese rol de instancia con las instancias de EC2 subyacentes.
- [ ] Crear cuatro roles de IAM distintos, cada uno con los permisos requeridos para el servicio de ECS asociado, y luego configurar cada servicio de ECS para que haga referencia al rol de IAM asociado.
- [ ] Crear cuatro roles de IAM distintos, cada uno con los permisos requeridos para el servicio de ECS asociado, y luego crear un grupo de IAM y configurar el clúster de ECS para que haga referencia a ese grupo.
- [x] Crear cuatro roles de IAM distintos, cada uno con los permisos requeridos para el servicio de ECS asociado, y luego configurar cada task definition de ECS para que haga referencia al rol de IAM asociado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una organización debe almacenar miles de archivos de audio y video sensibles en un bucket de Amazon S3. Las políticas de seguridad de la organización exigen que todos los datos escritos en este bucket estén cifrados. ¿Cómo se puede garantizar el cumplimiento de esta política?

- [ ] Usar AWS Lambda para enviar notificaciones al equipo de seguridad si se colocan objetos sin cifrar en el bucket.
- [x] Configurar una política de bucket de Amazon S3 para impedir la carga de objetos que no contengan el encabezado `x-amz­-server-side-encryption`.
- [ ] Crear una regla de evento de Amazon CloudWatch para verificar que todos los objetos almacenados en el bucket de Amazon S3 estén cifrados.
- [ ] Configurar una política de bucket de Amazon S3 para impedir la carga de objetos que contengan el encabezado `x-amz-server­side-encryption`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador creó un dashboard para una aplicación que usa Amazon API Gateway, Amazon S3, AWS Lambda y Amazon RDS. El desarrollador necesita un mecanismo de autenticación que permita a un usuario iniciar sesión y ver el dashboard. Debe ser accesible desde aplicaciones móviles, equipos de escritorio y tablets, y debe recordar las preferencias del usuario entre plataformas. ¿Qué servicio de AWS debería usar el desarrollador para dar soporte a este escenario de autenticación?

- [ ] AWS KMS.
- [x] Amazon Cognito.
- [ ] AWS Directory Service.
- [ ] Amazon IAM.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita acceso temporal a recursos en una segunda cuenta. ¿Cuál es la forma MÁS segura de lograrlo?

- [ ] Usar los user pools de Amazon Cognito para obtener credenciales de corta duración para la segunda cuenta.
- [ ] Crear una clave de acceso de IAM dedicada para la segunda cuenta y enviarla por correo.
- [x] Crear un rol de acceso entre cuentas y usar la API `sts:AssumeRole` para obtener credenciales de corta duración.
- [ ] Establecer una relación de confianza y agregar una clave SSH de la segunda cuenta al usuario de IAM.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando un Auto Scaling group cuyas instancias necesitan publicar una métrica personalizada en Amazon CloudWatch. ¿Qué método sería la forma MÁS segura de autenticar una solicitud PUT a CloudWatch?

- [ ] Crear un usuario de IAM con el permiso `PutMetricData` y colocar las credenciales del usuario en un repositorio privado; hacer que las aplicaciones obtengan las credenciales según sea necesario.
- [ ] Crear un usuario de IAM con el permiso `PutMetricData` y modificar la launch configuration del Auto Scaling para inyectar las credenciales del usuario en el user data de la instancia.
- [ ] Modificar las políticas de métricas de CloudWatch para permitir el permiso `PutMetricData` a las instancias del Auto Scaling group.
- [x] Crear un rol de IAM con el permiso `PutMetricData` y modificar la launch configuration del Auto Scaling para lanzar instancias usando ese rol.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo consta de 10 miembros. De forma similar a un directorio personal para cada miembro del equipo, el gerente quiere otorgar acceso a carpetas específicas de cada usuario en un bucket de Amazon S3. Para el miembro del equipo con el nombre de usuario `TeamMemberX`, el fragmento de la política de IAM se ve así. En lugar de crear políticas distintas para cada miembro del equipo, ¿qué enfoque puede usarse para hacer que este fragmento de política sea genérico para todos los miembros del equipo?

![Question 88](images/question88.jpg)

- [x] Usar una condición de política de IAM.
- [ ] Usar un principal de política de IAM.
- [ ] Usar variables de política de IAM.
- [ ] Usar un recurso de política de IAM.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa necesita cifrar datos en reposo, pero quiere aprovechar un servicio administrado de AWS usando su propia clave maestra. ¿Cuál de los siguientes servicios de AWS puede usarse para cumplir con estos requisitos?

- [ ] SSE con Amazon S3.
- [x] SSE con AWS KMS.
- [ ] Cifrado del lado del cliente.
- [ ] Roles y políticas de AWS IAM.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha creado un paquete de software para desplegarlo en varias instancias de EC2 usando roles de IAM. ¿Qué acciones podrían realizarse para verificar el acceso de IAM para obtener registros de Amazon Kinesis Streams? (Seleccione DOS)

- [ ] Usar la AWS CLI para recuperar el grupo de IAM.
- [ ] Consultar los metadatos de Amazon EC2 para obtener las políticas de IAM en línea.
- [ ] Solicitar un token a AWS STS y realizar una acción describe.
- [x] Realizar una acción get usando el argumento `--dry-run`.
- [x] Validar la política del rol de IAM con el IAM policy simulator.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación que administra transacciones financieras. Para mejorar la seguridad, se requerirá la autenticación multifactor (MFA) como parte del protocolo de inicio de sesión. ¿Qué servicios puede usar el desarrollador para cumplir con estos requisitos?

- [ ] Amazon DynamoDB para almacenar los datos de sesión de MFA y Amazon SNS para enviar los códigos de MFA.
- [x] Amazon Cognito con MFA.
- [ ] AWS Directory Service.
- [ ] AWS IAM con MFA habilitado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está probando una aplicación basada en Docker que usa el AWS SDK para interactuar con Amazon DynamoDB. En el entorno de desarrollo local, la aplicación ha usado claves de acceso de IAM. La aplicación ahora está lista para desplegarse en un clúster de ECS. ¿Cómo debería autenticarse la aplicación con los servicios de AWS en producción?

- [x] Configurar un rol de IAM de tarea de ECS para que la aplicación lo use.
- [ ] Refactorizar la aplicación para llamar a AWS STS `AssumeRole` basado en un rol de instancia.
- [ ] Configurar variables de entorno de clave de acceso/secreto de AWS con nuevas credenciales.
- [ ] Configurar el archivo de credenciales con un nuevo par de clave de acceso/secreto.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador usa AWS CodeDeploy para automatizar el despliegue de una aplicación que se conecta a una base de datos MySQL externa. El desarrollador quiere acceder de forma segura a los secretos cifrados, como claves de API y contraseñas de bases de datos. ¿Cuál de las siguientes soluciones implicaría el MENOR esfuerzo administrativo?

- [ ] Guardar los secretos en Amazon S3 con cifrado del lado del servidor de AWS KMS y usar una URL firmada para acceder a ellos mediante el rol de IAM de las instancias de Amazon EC2.
- [ ] Usar los metadatos de la instancia para almacenar los secretos y acceder a ellos programáticamente desde las instancias EC2.
- [ ] Usar la biblioteca de cifrado del lado del cliente de Amazon DynamoDB para guardar los secretos en DynamoDB y acceder a ellos programáticamente desde las instancias EC2.
- [x] Usar AWS SSM Parameter Store para almacenar los secretos y acceder a ellos programáticamente mediante el rol de IAM de las instancias EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador usará la AWS CLI en un servidor de desarrollo local para administrar servicios de AWS. ¿Qué se puede hacer para asegurar que la CLI use los permisos de IAM del desarrollador al ejecutar comandos?

- [ ] Especificar el ID de clave de acceso y la clave de acceso secreta de IAM del desarrollador como parámetros en cada comando de la CLI.
- [x] Ejecutar el comando `aws configure` de la CLI y proporcionar el ID de clave de acceso y la clave de acceso secreta de IAM del desarrollador.
- [ ] Especificar el nombre de usuario y la contraseña de IAM del desarrollador como parámetros en cada comando de la CLI.
- [ ] Usar el rol de IAM del desarrollador al ejecutar el comando de la CLI.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación tiene cientos de usuarios. Cada usuario puede usar múltiples dispositivos para acceder a la aplicación. El desarrollador quiere asignar identificadores únicos a estos usuarios sin importar el dispositivo que utilicen. ¿Cuál de los siguientes métodos debería usarse para obtener identificadores únicos?

- [ ] Crear una tabla de usuarios en Amazon DynamoDB como pares clave-valor de usuarios y sus dispositivos. Usar estas claves como identificadores únicos.
- [ ] Usar los ID de clave de acceso generados por IAM para los usuarios como identificador único, pero no almacenar las claves secretas.
- [x] Implementar identidades autenticadas por el desarrollador (developer-authenticated identities) mediante Amazon Cognito y obtener credenciales para estas identidades.
- [ ] Asignar usuarios y roles de IAM a los usuarios. Usar el ID de recurso único de IAM como identificador único.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un paquete de despliegue usa la AWS CLI para copiar archivos a cualquier bucket de S3 de la cuenta, usando claves de acceso almacenadas en variables de entorno. El paquete se ejecuta en instancias EC2, y las instancias se han modificado para ejecutarse con un rol de IAM asumido y una política más restrictiva que permite el acceso a un solo bucket. Después del cambio, el desarrollador inicia sesión en el host y aún tiene la capacidad de escribir en todos los buckets de S3 de esa cuenta. ¿Cuál es la causa MÁS probable de esta situación?

- [ ] Se está usando una política en línea (inline) de IAM en el rol de IAM.
- [x] Se está usando una política administrada de IAM en el rol de IAM.
- [ ] La AWS CLI está dañada y necesita reinstalarse.
- [ ] El proveedor de credenciales de AWS busca las credenciales del perfil de instancia al final.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación en desarrollo debe almacenar cientos de archivos de video. Los datos deben cifrarse dentro de la aplicación antes de almacenarse, con una clave única para cada archivo de video. ¿Cómo debería programar el desarrollador la aplicación?

- [ ] Usar la API `KMS Encrypt` para cifrar los datos. Almacenar la clave de datos cifrada y los datos.
- [ ] Usar una biblioteca de criptografía para generar una clave de cifrado para la aplicación. Usar la clave de cifrado para cifrar los datos. Almacenar los datos cifrados.
- [x] Usar la API `KMS GenerateDataKey` para obtener una clave de datos. Cifrar los datos con la clave de datos. Almacenar la clave de datos cifrada y los datos.
- [ ] Cargar los datos en un bucket de S3 usando cifrado del lado del servidor con una clave de AWS KMS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe asegurar que las credenciales de IAM usadas por una aplicación en Amazon EC2 no se usen indebidamente ni se vean comprometidas. ¿Qué debería usar el desarrollador para mantener seguras las credenciales de usuario?

- [ ] Variables de entorno.
- [ ] Archivo de credenciales de AWS.
- [x] Credenciales del perfil de instancia.
- [ ] Opciones de la línea de comandos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene una aplicación donde la lectura de objetos desde Amazon S3 se basa en el tipo de usuario. Los tipos de usuario son usuario registrado y usuario invitado. La empresa tiene 25,000 usuarios y sigue creciendo. La información se obtiene de un bucket de S3 según el tipo de usuario. ¿Qué enfoques se recomiendan para proporcionar acceso a ambos tipos de usuarios? (Elija DOS)

- [ ] Proporcionar una clave de acceso y una clave de acceso secreta diferentes en el código de la aplicación para los usuarios registrados y los usuarios invitados para dar acceso de lectura a los objetos.
- [ ] Usar políticas de bucket de S3 para restringir el acceso de lectura a usuarios de IAM específicos.
- [x] Usar Amazon Cognito para proporcionar acceso mediante roles autenticados y no autenticados.
- [ ] Crear un nuevo usuario de IAM para cada usuario y otorgarle acceso de lectura.
- [x] Usar el servicio AWS IAM y permitir que la aplicación asuma los diferentes roles mediante la acción `AssumeRole` de AWS Security Token Service (AWS STS) según el tipo de usuario, y proporcionar acceso de lectura a Amazon S3 mediante el rol asumido.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene 25,000 empleados y sigue creciendo. La empresa está creando una aplicación que será accesible solo para sus empleados. Un desarrollador está usando Amazon S3 para almacenar imágenes y Amazon RDS para almacenar los datos de la aplicación. La empresa requiere que toda la información de los empleados permanezca únicamente en el directorio de empleados heredado basado en Security Assertion Markup Language (SAML) y no está interesada en replicar ninguna información de los empleados en AWS. ¿Cómo puede el desarrollador proporcionar acceso autorizado a los empleados que usarán esta aplicación para que cada empleado pueda acceder solo a sus propios datos de la aplicación?

- [ ] Usar Amazon VPC y mantener todos los recursos dentro de la VPC, y usar un VPC link para el bucket de S3 con la política de bucket.
- [ ] Usar los user pools de Amazon Cognito, federar con el proveedor SAML y usar grupos del user pool con una política de IAM.
- [x] Usar un identity pool de Amazon Cognito, federar con el proveedor SAML y usar una clave de condición de IAM con un valor para la variable `cognito-identity.amazonaws.com:sub` para otorgar acceso a los empleados.
- [ ] Crear un rol de IAM único para cada empleado y hacer que cada empleado asuma el rol para acceder a la aplicación de modo que solo pueda acceder a sus datos personales.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación necesita cifrar los datos que se escriben en Amazon S3, donde las claves se administran en un centro de datos on-premises y el cifrado lo gestiona S3. ¿Qué tipo de cifrado se debe utilizar?

- [ ] Usar cifrado del lado del servidor con claves administradas por Amazon S3.
- [ ] Usar cifrado del lado del servidor con claves administradas por AWS KMS.
- [ ] Usar cifrado del lado del cliente con customer master keys.
- [x] Usar cifrado del lado del servidor con claves proporcionadas por el cliente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación que se ejecuta en Amazon EC2 abre conexiones a una base de datos Amazon RDS SQL Server. El desarrollador no quiere almacenar el nombre de usuario y la contraseña de la base de datos en el código. El desarrollador también desea rotar las credenciales automáticamente. ¿Cuál es la forma MÁS segura de almacenar y acceder a las credenciales de la base de datos?

- [ ] Crear un rol de IAM que tenga permisos para acceder a la base de datos. Asociar el rol a la instancia de EC2.
- [x] Usar AWS Secrets Manager para almacenar las credenciales. Recuperar las credenciales desde Secrets Manager según sea necesario.
- [ ] Almacenar las credenciales en un archivo de texto cifrado en un bucket de Amazon S3. Configurar los datos de usuario (user data) de la instancia de EC2 para descargar las credenciales desde Amazon S3 cuando la instancia arranque.
- [ ] Almacenar el nombre de usuario y la contraseña directamente en el código fuente. No se requiere ninguna otra acción porque el código fuente se almacena en un repositorio privado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo está diseñando una aplicación móvil que requiere autenticación multifactor. ¿Qué pasos se deben seguir para lograrlo? (Elija DOS)

- [x] Usar Amazon Cognito para crear un user pool y crear usuarios en el user pool.
- [ ] Enviar códigos de autenticación multifactor por mensaje de texto a los usuarios con la llamada a la API Amazon SNS Publish en el código de la aplicación.
- [x] Habilitar la autenticación multifactor para el user pool de Amazon Cognito.
- [ ] Usar AWS IAM para crear usuarios de IAM.
- [ ] Habilitar la autenticación multifactor para los usuarios creados en AWS IAM.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Dos microservicios en contenedores están alojados en Amazon EC2 ECS. El primer microservicio lee de una instancia de base de datos Amazon RDS Aurora y el segundo microservicio lee de una tabla de Amazon DynamoDB. ¿Cómo se pueden otorgar a cada microservicio los privilegios mínimos?

- [ ] Establecer `ECS_ENABLE_TASK_IAM_ROLE` en `false` durante el arranque de la instancia de EC2 en el archivo de configuración del agente de ECS. Ejecutar el primer microservicio con un rol de IAM para tareas de ECS con acceso de solo lectura a la base de datos Aurora. Ejecutar el segundo microservicio con un rol de IAM para tareas de ECS con acceso de solo lectura a DynamoDB.
- [ ] Establecer `ECS_ENABLE_TASK_IAM_ROLE` en `false` durante el arranque de la instancia de EC2 en el archivo de configuración del agente de ECS. Otorgar al rol del instance profile acceso de solo lectura a la base de datos Aurora y a DynamoDB.
- [x] Establecer `ECS_ENABLE_TASK_IAM_ROLE` en `true` durante el arranque de la instancia de EC2 en el archivo de configuración del agente de ECS. Ejecutar el primer microservicio con un rol de IAM para tareas de ECS con acceso de solo lectura a la base de datos Aurora. Ejecutar el segundo microservicio con un rol de IAM para tareas de ECS con acceso de solo lectura a DynamoDB.
- [ ] Establecer `ECS_ENABLE_TASK_IAM_ROLE` en `true` durante el arranque de la instancia de EC2 en el archivo de configuración del agente de ECS. Otorgar al rol del instance profile acceso de solo lectura a la base de datos Aurora y a DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un rol de IAM asociado a una instancia de Amazon EC2 deniega explícitamente el acceso a todas las acciones de la API de Amazon S3. El archivo de credenciales de la instancia de EC2 especifica la clave de acceso y la clave de acceso secreta de IAM, que permiten acceso administrativo completo. Dado que existen múltiples modos de acceso de IAM para esta instancia de EC2, ¿cuál de las siguientes afirmaciones es correcta?

- [ ] La instancia de EC2 solo podrá listar los buckets de S3.
- [ ] La instancia de EC2 solo podrá listar el contenido de un bucket de S3 a la vez.
- [ ] La instancia de EC2 podrá realizar todas las acciones en cualquier bucket de S3.
- [x] La instancia de EC2 no podrá realizar ninguna acción de S3 en ningún bucket de S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo está construyendo una nueva aplicación que se ejecutará en Amazon EC2 y usará Amazon DynamoDB como capa de almacenamiento. Todos los desarrolladores tienen cuentas de usuario de IAM asignadas en el mismo grupo de IAM. Actualmente los desarrolladores pueden lanzar instancias de EC2 y necesitan poder lanzar instancias de EC2 con un rol de instancia que permita el acceso a Amazon DynamoDB. ¿Qué cambios de AWS IAM son necesarios al crear un rol de instancia para proporcionar esta funcionalidad?

- [ ] Crear una política de permisos de IAM asociada al rol que permita el acceso a DynamoDB. Agregar una política de confianza al rol que permita a DynamoDB asumir el rol. Asociar una política de permisos al grupo de desarrollo en AWS IAM que permita a los desarrolladores usar los permisos iam:GetRole e iam:PassRole para el rol.
- [x] Crear una política de permisos de IAM asociada al rol que permita el acceso a DynamoDB. Agregar una política de confianza al rol que permita a Amazon EC2 asumir el rol. Asociar una política de permisos al grupo de desarrollo en AWS IAM que permita a los desarrolladores usar el permiso iam:PassRole para el rol.
- [ ] Crear una política de permisos de IAM asociada al rol que permita el acceso a Amazon EC2. Agregar una política de confianza al rol que permita a DynamoDB asumir el rol. Asociar una política de permisos al grupo de desarrollo en AWS IAM que permita a los desarrolladores usar el permiso iam:PassRole para el rol.
- [ ] Crear una política de permisos de IAM asociada al rol que permita el acceso a DynamoDB. Agregar una política de confianza al rol que permita a Amazon EC2 asumir el rol. Asociar una política de permisos al grupo de desarrollo en AWS IAM que permita a los desarrolladores usar el permiso iam:GetRole para el rol.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación web de front-end usa los user pools de Amazon Cognito para gestionar el flujo de autenticación de usuarios. Un desarrollador está integrando Amazon DynamoDB en la aplicación usando el AWS SDK para JavaScript. ¿Cómo podría el desarrollador llamar a la API de forma segura sin exponer las claves de acceso ni secreta?

- [x] Configurar los identity pools de Amazon Cognito e intercambiar el JSON Web Token (JWT) por credenciales temporales.
- [ ] Ejecutar la aplicación web en una instancia de Amazon EC2 con el instance profile configurado.
- [ ] Codificar las credenciales directamente en el código (hardcode), usar Amazon S3 para alojar la aplicación web y habilitar el cifrado del lado del servidor.
- [ ] Usar los JSON Web Tokens (JWITs) del user pool de Amazon Cognito para acceder a las API de DynamoDB.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa usa Amazon API Gateway para administrar su API de cara al público. El CISO requiere que las APIs sean usadas únicamente por usuarios de la cuenta de prueba. ¿Cuál es la forma MÁS segura de restringir el acceso a la API a los usuarios de esta cuenta de AWS en particular?

- [ ] Certificados SSL del lado del cliente para la autenticación.
- [x] Políticas de recursos de API Gateway.
- [ ] Uso compartido de recursos de origen cruzado (CORS).
- [ ] Usage plans.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe permitir que usuarios invitados sin inicio de sesión accedan a un sitio habilitado con Amazon Cognito para ver archivos almacenados en un bucket de Amazon S3. ¿Cómo debería cumplir el desarrollador estos requisitos?

- [ ] Crear un ID de usuario en blanco en un user pool, agregarlo al grupo de usuarios y otorgar acceso a los recursos de AWS.
- [x] Crear un nuevo identity pool, habilitar el acceso a identidades no autenticadas y otorgar acceso a los recursos de AWS.
- [ ] Crear un nuevo user pool, habilitar el acceso a identidades autenticadas y otorgar acceso a los recursos de AWS.
- [ ] Crear un nuevo user pool, deshabilitar el acceso de autenticación y otorgar acceso a los recursos de AWS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita crear una aplicación que admita Security Assertion Markup Language (SAML) y autenticación con Facebook. También debe permitir el acceso a servicios de AWS, como Amazon DynamoDB. ¿Qué servicio o característica de AWS cumplirá estos requisitos con la MENOR cantidad de codificación adicional?

- [ ] AWS AppSync.
- [x] Amazon Cognito identity pools.
- [ ] Amazon Cognito user pools.
- [ ] Amazon Lambda@Edge.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una aplicación en AWS Lambda. Para simplificar las pruebas y los despliegues, el desarrollador necesita que la cadena de conexión a la base de datos pueda cambiarse fácilmente sin modificar el código de Lambda. ¿Cómo se puede cumplir este requisito?

- [x] Almacenar la cadena de conexión como un secreto en AWS Secrets Manager.
- [ ] Almacenar la cadena de conexión en una cuenta de usuario de IAM.
- [ ] Almacenar la cadena de conexión en AWS KMS.
- [ ] Almacenar la cadena de conexión como una Lambda layer.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador decide almacenar datos altamente seguros en Amazon S3 y quiere implementar cifrado del lado del servidor (SSE) con control granular sobre quién puede acceder a la clave maestra. La política de la empresa requiere que la clave maestra pueda crearse, rotarse y deshabilitarse fácilmente cuando sea necesario, todo por razones de seguridad. ¿Qué solución debería usarse para cumplir estos requisitos?

- [ ] SSE con claves administradas por Amazon S3 (SSE-S3).
- [x] SSE con claves administradas por AWS KMS (SSE-KMS).
- [ ] SSE con AWS Secrets Manager.
- [ ] SSE con claves de cifrado proporcionadas por el cliente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación que necesita almacenar datos en Amazon S3. La gerencia requiere que los datos se cifren antes de enviarse a Amazon S3 para su almacenamiento. Las claves de cifrado deben ser administradas por el equipo de Seguridad. ¿Qué enfoque debería adoptar el desarrollador para cumplir estos requisitos?

- [ ] Implementar cifrado del lado del servidor usando claves de cifrado proporcionadas por el cliente (SSE-C).
- [ ] Implementar cifrado del lado del servidor usando una clave maestra del lado del cliente.
- [x] Implementar cifrado del lado del cliente usando una customer master key (CMK) administrada por AWS KMS.
- [ ] Implementar cifrado del lado del cliente usando claves administradas por Amazon S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer está publicando datos de registro críticos en un log group de Amazon CloudWatch Logs, que fue creado hace 2 meses. El Developer debe cifrar los datos de registro usando una customer master key (CMK) de AWS KMS para que los datos futuros puedan cifrarse y así cumplir con la política de seguridad de la empresa. ¿Cómo puede el Developer cumplir este requisito?

- [ ] Usar la consola de CloudWatch Logs y habilitar la función de cifrado en el log group.
- [ ] Usar el comando `create-log-group` de la AWS CLI y especificar el Amazon Resource Name (ARN) de la clave.
- [ ] Usar la consola de KMS y asociar la CMK con el log group.
- [x] Usar el comando `associate-kms-key` de la AWS CLI y especificar el Amazon Resource Name (ARN) de la clave

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer tiene código que se ejecuta en instancias de Amazon EC2 y que necesita acceso de solo lectura a una tabla de Amazon DynamoDB. ¿Cuál es el enfoque MÁS seguro que debe adoptar el Developer para lograr esta tarea?

- [ ] Crear una clave de acceso de usuario para cada instancia de EC2 con acceso de solo lectura a DynamoDB. Colocar las claves en el código. Volver a desplegar el código a medida que las claves rotan.
- [x] Usar un rol de IAM con una política AmazonDynamoDBReadOnlyAccess aplicada a las instancias de EC2.
- [ ] Ejecutar todo el código únicamente con las claves de acceso del usuario raíz de la cuenta de AWS para garantizar el máximo acceso a los servicios.
- [ ] Usar un rol de IAM con acceso de Administrator aplicado a la instancia de EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer usa buckets de Amazon S3 para el alojamiento de sitios web estáticos. El Developer crea un bucket de S3 para el código y otro bucket de S3 para los recursos (assets), como archivos de imagen y video. Se deniega el acceso cuando un usuario intenta acceder al bucket de recursos desde el bucket de código, y la aplicación del sitio web muestra un error `403`. ¿Cómo debe resolver el Developer este problema?

- [ ] Crear un rol de IAM y aplicarlo al bucket de recursos para que se le otorgue acceso al bucket de código.
- [x] Editar la bucket policy del bucket de recursos para permitir el acceso desde el bucket de código.
- [ ] Editar la bucket policy del bucket de recursos para abrir el acceso a todos los principals.
- [ ] Cambiar el bucket de código para que use funciones de AWS Lambda en lugar del alojamiento de sitios web estáticos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa quiere migrar un servicio de imágenes a Amazon EC2 siguiendo las mejores prácticas de seguridad. Las imágenes se obtienen y se leen desde un bucket de Amazon S3 no público. ¿Qué debe hacer un Developer para cumplir estos requisitos?

- [ ] Crear un usuario de IAM con permisos de solo lectura para el bucket de S3. Almacenar temporalmente las credenciales del usuario en el volumen de Amazon EBS de la instancia de EC2.
- [ ] Crear un usuario de IAM con permisos de solo lectura para el bucket de S3. Almacenar temporalmente las credenciales del usuario en los datos de usuario (user data) de la instancia de EC2.
- [x] Crear un rol de servicio de EC2 con permisos de solo lectura para el bucket de S3. Asociar el rol a la instancia de EC2.
- [ ] Crear un rol de servicio de S3 con permisos de solo lectura para el bucket de S3. Asociar el rol a la instancia de EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está desarrollando una aplicación a la que se accederá a través de la API REST de Amazon API Gateway. Solo los usuarios registrados deben poder acceder a ciertos recursos de esta API. El token utilizado debe expirar automáticamente y necesita actualizarse periódicamente. ¿Cómo puede un Developer cumplir estos requisitos?

- [ ] Crear un identity pool de Amazon Cognito, configurar el Amazon Cognito Authorizer en API Gateway y usar las credenciales temporales generadas por el identity pool.
- [ ] Crear y mantener un registro en una base de datos para cada usuario con un token correspondiente y usar un Lambda authorizer de AWS Lambda en API Gateway.
- [x] Crear un user pool de Amazon Cognito, configurar el Cognito Authorizer en API Gateway y usar el token de identidad o de acceso.
- [ ] Crear un usuario de IAM para cada usuario de la API, adjuntar una política de permisos de invocación a la API y usar un IAM authorizer en API Gateway.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer ha creado un nuevo usuario de AWS IAM que tiene el permiso `s3:putObject` para escribir en un bucket específico de Amazon S3. Este bucket de S3 usa cifrado del lado del servidor con claves administradas por AWS KMS (SSE-KMS) como cifrado predeterminado. Usando la clave de acceso y la clave secreta del usuario de IAM, la aplicación recibió un error de acceso denegado al llamar a la API `PutObject`. ¿Cómo se puede resolver este problema?

- [ ] Actualizar la política del usuario de IAM para permitir la acción `s3:EncryptionConfiguration`.
- [ ] Actualizar la bucket policy del bucket de S3 para permitir que el usuario de IAM cargue objetos.
- [x] Actualizar la política del usuario de IAM para permitir la acción `kms:GenerateDataKey`.
- [ ] Actualizar la ACL del bucket de S3 para permitir que el usuario de IAM cargue objetos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene una aplicación web que usa un user pool de Amazon Cognito para la autenticación. La empresa quiere crear una página de inicio de sesión con el logotipo de la empresa. ¿Qué debe hacer un Developer para cumplir estos requisitos?

- [x] Crear una interfaz de usuario alojada (hosted UI) en Amazon Cognito y personalizarla con el logotipo de la empresa.
- [ ] Crear una página de inicio de sesión con el logotipo de la empresa y cargarla en Amazon Cognito.
- [ ] Crear una página de inicio de sesión en Amazon API Gateway con el logotipo y guardar el enlace en Amazon Cognito.
- [ ] Cargar el logotipo en la configuración de la app de Amazon Cognito y apuntar al logotipo desde una página de inicio de sesión personalizada.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer está trabajando en una función de AWS Lambda que accede a Amazon DynamoDB. La función de Lambda debe recuperar un elemento y actualizar algunos de sus atributos, o crear el elemento si no existe. La función de Lambda tiene acceso a la clave primaria. ¿Qué permisos de IAM debe solicitar el Developer para que la función de Lambda logre esta funcionalidad?

- [ ] `dynamodb:DeleteItem dynamodb:GetItem dynamodb:PutItem`.
- [ ] `dynamodb:UpdateItem dynamodb:GetItem dynamodb:DescribeTable`.
- [ ] `dynamodb:GetRecords dynamodb:PutItem dynamodb:UpdateTable`.
- [x] `dynamodb:UpdateItem dynamodb:GetItem dynamodb:PutItem`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer está almacenando en Amazon S3 datos sensibles generados por una aplicación. El Developer quiere cifrar los datos en reposo. Una política de la empresa requiere un registro de auditoría de cuándo se usó la clave maestra y por quién. ¿Qué opción de cifrado cumplirá estos requisitos?

- [ ] Cifrado del lado del servidor con claves administradas por Amazon S3 (SSE-S3).
- [x] Cifrado del lado del servidor con claves administradas por AWS KMS (SSE-KMS).
- [ ] Cifrado del lado del servidor con claves proporcionadas por el cliente (SSE-C).
- [ ] Cifrado del lado del servidor con claves autoadministradas.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer quiere crear una aplicación que permita a nuevos usuarios registrarse y crear nuevas cuentas de usuario. La aplicación también debe permitir que los usuarios con cuentas de redes sociales inicien sesión usando sus credenciales de redes sociales. ¿Qué servicio o característica de AWS se puede usar para cumplir estos requisitos?

- [ ] AWS IAM.
- [ ] Amazon Cognito identity pools.
- [x] Amazon Cognito user pools.
- [ ] AWS Directory Service.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Desarrollador está intentando realizar llamadas a la API usando el SDK. Las credenciales del usuario de IAM utilizadas por la aplicación requieren autenticación multifactor para todas las llamadas a la API. ¿Qué método debe usar el Desarrollador para acceder a la API protegida con autenticación multifactor?

- [ ] GetFederationToken.
- [ ] GetCallerIdentity.
- [x] GetSessionToken.
- [ ] DecodeAutherizationMessage.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Desarrollador está almacenando documentos sensibles en Amazon S3 que requerirán cifrado en reposo. Las claves de cifrado deben rotarse anualmente, como mínimo. ¿Cuál es la forma más sencilla de lograr esto?

- [ ] Cifrar los datos antes de enviarlos a Amazon S3.
- [ ] Importar una clave personalizada en AWS KMS con rotación anual habilitada.
- [x] Usar AWS KMS con rotación automática de claves.
- [ ] Exportar una clave de AWS KMS para cifrar los datos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Desarrollador debe cifrar un objeto de 100 GB usando AWS KMS. ¿Cuál es el MEJOR enfoque?

- [ ] Realizar una llamada a la API `Encrypt` para cifrar los datos en texto plano como texto cifrado usando una customer master key (CMK).
- [ ] Realizar una llamada a la API `Encrypt` para cifrar los datos en texto plano como texto cifrado usando una customer master key (CMK) con material de clave importado.
- [x] Realizar una llamada a la API `GenerateDataKey` que devuelve una clave en texto plano y una copia cifrada de una clave de datos. Usar la clave en texto plano para cifrar los datos.
- [ ] Realizar una llamada a la API `GenerateDataKeyWithoutPlaintext` que devuelve una copia cifrada de una clave de datos. Usar la clave cifrada para cifrar los datos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de los siguientes elementos se requieren para permitir que una aplicación desplegada en una instancia de EC2 escriba datos en una tabla de DynamoDB? Suponga que no se permite almacenar claves de seguridad en la instancia de EC2. (Elija DOS)

- [ ] Crear un usuario de IAM que permita acceso de escritura a la tabla de DynamoDB.
- [ ] Agregar un rol de IAM a una instancia de EC2 en ejecución.
- [ ] Agregar un usuario de IAM a una instancia de EC2 en ejecución.
- [x] Lanzar una instancia de EC2 con el rol de IAM incluido en la configuración de lanzamiento.
- [x] Crear un rol de IAM que permita acceso de escritura a la tabla de DynamoDB.
- [ ] Lanzar una instancia de EC2 con el usuario de IAM incluido en la configuración de lanzamiento.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de las siguientes son afirmaciones correctas sobre la lógica de evaluación de políticas en AWS Identity and Access Management? (Elija DOS)

- [x] Por defecto, todas las solicitudes se deniegan.
- [ ] Un allow explícito anula un deny explícito.
- [x] Un allow explícito anula el deny por defecto.
- [ ] Un deny explícito no anula un allow explícito.
- [ ] Por defecto, todas las solicitudes se permiten.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Al cargar un objeto, ¿qué encabezado de solicitud se puede especificar explícitamente en una solicitud a Amazon S3 para cifrar los datos del objeto cuando se guardan en el lado del servidor?

- [ ] `x-amz-storage-class`.
- [ ] `Content-MD5`.
- [ ] `x-amz-security-token`.
- [x] `x-amz-server-side-encryption`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué características se pueden usar para restringir el acceso a los datos en S3? (Elija DOS)

- [ ] Usar S3 Virtual Hosting.
- [x] Establecer una política de bucket de S3.
- [ ] Habilitar IAM Identity Federation.
- [x] Establecer una ACL de S3 en el bucket o en el objeto.
- [ ] Crear una distribución de CloudFront para el bucket.

**[⬆ Back to Top](#tabla-de-contenidos)**

### En AWS, ¿qué aspectos de seguridad son responsabilidad del cliente? (Elija CUATRO)

- [x] Gestión del ciclo de vida de las credenciales de IAM.
- [ ] Baja de dispositivos de almacenamiento.
- [x] Configuración de Security Groups y ACL (Access Control List).
- [x] Cifrado de volúmenes EBS (Elastic Block Storage).
- [ ] Control del acceso físico a los recursos de cómputo.
- [x] Gestión de parches del sistema operativo de la instancia de EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cómo se pueden proteger los datos en reposo en un volumen de EBS?

- [ ] Adjuntar el volumen a una instancia usando la interfaz SSL de EC2.
- [ ] Escribir los datos de forma aleatoria en lugar de secuencial.
- [x] Usar un sistema de archivos cifrado sobre el volumen de EBS.
- [ ] Cifrar el volumen usando el servicio de cifrado del lado del servidor de S3.
- [ ] Crear una política de IAM que restrinja el acceso de lectura y escritura al volumen.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Games-R-Us va a lanzar una nueva aplicación de juegos para dispositivos móviles. Los usuarios iniciarán sesión en el juego con su cuenta de Facebook existente y el juego registrará los datos del jugador y la información de puntuación directamente en una tabla de DynamoDB. ¿Cuál es el enfoque más seguro para firmar las solicitudes a la API de DynamoDB?

- [ ] Crear un usuario de IAM con credenciales de acceso que se distribuyan con la aplicación móvil para firmar las solicitudes.
- [ ] Distribuir las credenciales de acceso de la cuenta root de AWS con la aplicación móvil para firmar las solicitudes.
- [x] Solicitar credenciales de seguridad temporales mediante web identity federation para firmar las solicitudes.
- [ ] Establecer acceso entre cuentas (cross account) entre la aplicación móvil y la tabla de DynamoDB para firmar las solicitudes

**[⬆ Back to Top](#tabla-de-contenidos)**

### Usted opera un sitio web de fotos con publicidad que usa S3 para servir fotos a los visitantes de su sitio. En algún momento descubre que otros sitios han estado enlazando a las fotos de su sitio, lo que causa pérdidas a su negocio. ¿Cuál es un método eficaz para mitigar esto?

- [ ] Almacenar las fotos en un volumen EBS del servidor web.
- [x] Eliminar el acceso de lectura público y usar signed URLs con fechas de expiración.
- [ ] Usar distribuciones de CloudFront para el contenido estático.
- [ ] Bloquear las IP de los sitios infractores en los Security Groups.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación web corporativa está desplegada dentro de una Amazon VPC y está conectada al centro de datos corporativo mediante una VPN IPSec. La aplicación debe autenticarse contra el servidor LDAP local (on-premise). Una vez autenticados, los usuarios que iniciaron sesión solo pueden acceder a un keyspace de S3 específico del usuario. ¿Qué dos enfoques pueden satisfacer los objetivos? (Elija DOS)

- [ ] La aplicación se autentica contra LDAP. Luego la aplicación llama al IAM Security Service para iniciar sesión en IAM usando las credenciales de LDAP. La aplicación puede usar las credenciales temporales de 1AM para acceder al bucket de S3 correspondiente.
- [x] La aplicación se autentica contra LDAP y recupera el nombre de un rol de IAM asociado con el usuario. Luego la aplicación llama al IAM Security Token Service para asumir ese rol de IAM. La aplicación puede usar las credenciales temporales para acceder al bucket de S3 correspondiente.
- [ ] La aplicación se autentica contra IAM Security Token Service usando las credenciales de LDAP. La aplicación usa esas credenciales de seguridad temporales de AWS para acceder al bucket de S3 correspondiente.
- [x] Desarrollar un identity broker que se autentique contra LDAP y luego llame a IAM Security Token Service para obtener credenciales de usuario federado de IAM. La aplicación llama al identity broker para obtener credenciales de usuario federado de IAM con acceso al bucket de S3 correspondiente.
- [ ] Desarrollar un identity broker que se autentique contra IAM Security Token Service para asumir un rol de IAM y obtener credenciales de seguridad temporales de AWS. La aplicación llama al identity broker para obtener credenciales de seguridad temporales de AWS con acceso al bucket de S3 correspondiente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué tipo de cifrado por bloques ofrece Amazon S3 para el cifrado del lado del servidor?

- [ ] Triple DES.
- [x] Advanced Encryption Standard.
- [ ] Blowfish.
- [ ] RC5.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador accede a AWS CodeCommit mediante SSH. Las claves SSH configuradas para acceder a AWS CodeCommit están asociadas a un usuario con los siguientes permisos. El desarrollador necesita crear/eliminar ramas. ¿Qué permisos específicos de IAM deben agregarse, según el principio de mínimo privilegio?

![Question 281](images/question281.jpg)

- [x] `"codecommit:CreateBranch" "codecommit:DeleteBranch"`.
- [ ] `"codecommit:Put*"`.
- [ ] `"codecommit:Update*"`.
- [ ] `"codecommit:*"`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una función de AWS Lambda debe acceder a un sitio externo utilizando un nombre de usuario y una contraseña que se rotan regularmente. Estos elementos deben mantenerse de forma segura y no pueden almacenarse en el código de la función. ¿Qué combinación de servicios de AWS se puede usar para lograrlo? (Elija DOS)

- [ ] AWS Certificate Manager (ACM).
- [x] AWS Systems Manager Parameter Store.
- [ ] AWS Trusted Advisor.
- [x] AWS KMS.
- [ ] Amazon GuardDuty.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está trabajando en una aplicación que maneja documentos de 10MB que contienen datos altamente sensibles. La aplicación usará AWS KMS para realizar cifrado del lado del cliente. ¿Qué pasos se deben seguir?

- [ ] Invocar la API Encrypt pasando los datos en texto plano que deben cifrarse y luego hacer referencia al ARN de la customer managed key en el parámetro `KeyId`.
- [ ] Invocar la API `GenerateRandom` para obtener una data encryption key y luego usar la data encryption key para cifrar los datos.
- [ ] Invocar la API `GenerateDataKey` para recuperar la versión cifrada de la data encryption key para cifrar los datos.
- [x] Invocar la API `GenerateDataKey` para recuperar la versión en texto plano de la data encryption key para cifrar los datos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa necesita distribuir actualizaciones de firmware a sus clientes en todo el mundo. ¿Qué servicio permitirá un control fácil y seguro del acceso a las descargas al menor costo?

- [x] Usar Amazon CloudFront con signed URLs para Amazon S3.
- [ ] Crear una distribución dedicada de Amazon CloudFront para cada cliente.
- [ ] Usar Amazon CloudFront con AWS Lambda@Edge.
- [ ] Usar Amazon API Gateway y AWS Lambda para controlar el acceso a un bucket de S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una aplicación móvil que permite a los usuarios ver imágenes de un bucket de S3. Los usuarios deben poder iniciar sesión con su cuenta de Amazon, así como con cuentas de Facebook y/o Google. ¿Cómo puede el desarrollador proporcionar esta funcionalidad de autenticación?

- [x] Usar Amazon Cognito con web identity federation.
- [ ] Usar Amazon Cognito con federación de identidades basada en SAML.
- [ ] Usar las claves de acceso/secretas de AWS IAM en el código de la aplicación para permitir `Get*` en el bucket de S3.
- [ ] Usar AWS STS `AssumeRole` en el código de la aplicación y asumir un rol con permisos `Get*` en el bucket de S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está creando una aplicación que requerirá que los usuarios accedan a servicios de AWS y les permitirá restablecer sus propias contraseñas. ¿Cuál de las siguientes opciones permitiría a la empresa administrar usuarios y autorización, y a la vez permitir que los usuarios restablezcan sus propias contraseñas?

- [ ] Amazon Cognito identify pools y AWS STS.
- [ ] Amazon Cognito identity pools y AWS IAM.
- [ ] Amazon Cognito user pools y AWS KMS.
- [x] Amazon Cognito user pools e identity pools.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación que se ejecuta en una instancia de Amazon EC2 necesita acceder y realizar llamadas a la API de varios servicios de AWS. ¿Cuál es la forma MÁS segura de proporcionar acceso a los servicios de AWS con una sobrecarga de administración MÍNIMA?

- [ ] Usar AWS KMS para almacenar y recuperar credenciales.
- [x] Usar instance profiles de EC2.
- [ ] Usar el usuario `root` de AWS para realizar solicitudes a la aplicación.
- [ ] Almacenar y recuperar credenciales desde AWS CodeCommit.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está desarrollando una aplicación que se ejecutará en varias instancias de Amazon EC2 en un Auto Scaling group y que puede acceder a una base de datos que se ejecuta en Amazon EC2. La aplicación necesita almacenar los secretos necesarios para conectarse a la base de datos. La aplicación debe permitir la rotación periódica de secretos y no debe requerir cambios cuando un secreto cambie. ¿Cuál es la forma MÁS segura de cumplir estos requisitos?

- [ ] Asociar un rol de IAM a la instancia EC2 donde se ejecuta la aplicación con permiso para acceder a la base de datos.
- [x] Usar AWS Systems Manager Parameter Store con el tipo de datos SecureString para almacenar los secretos.
- [ ] Configurar la aplicación para almacenar los secretos en los metadatos de objetos de Amazon S3.
- [ ] Codificar los secretos de la base de datos directamente en el código de la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está diseñando una nueva aplicación que usa Amazon S3. Para cumplir con los requisitos de conformidad, el desarrollador debe cifrar los datos en reposo. ¿Cómo puede lograrlo el desarrollador?

- [ ] Usar `s3:x-amz-acl` como condición en la política del bucket de S3.
- [ ] Usar Amazon RDS con cifrado predeterminado.
- [ ] Usar `aws:SecureTransport` como condición en la política del bucket de S3.
- [x] Activar el cifrado predeterminado de S3 para el bucket de S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa necesita proteger su sitio web existente que se ejecuta detrás de un Elastic Load Balancer. Las instancias de Amazon EC2 del sitio web tienen limitaciones de CPU. ¿Qué se debe hacer para proteger el sitio web sin aumentar la carga de CPU de los servidores web EC2? (Seleccione DOS)

- [ ] Configurar un Elastic Load Balancer con SSL pass-through.
- [x] Configurar certificados SSL en un Elastic Load Balancer.
- [ ] Configurar un Elastic Load Balancer con un Loadable Storage System.
- [ ] Instalar certificados SSL en las instancias EC2.
- [x] Configurar un Elastic Load Balancer con terminación SSL.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación móvil que no requerirá que los usuarios inicien sesión. ¿Cuál es el método MÁS eficiente para otorgar a los usuarios acceso a los recursos de AWS?

- [ ] Usar un proveedor de identidad para autenticarse de forma segura con la aplicación.
- [ ] Crear una función de AWS Lambda para crear un usuario de IAM cuando un usuario accede a la aplicación.
- [ ] Crear credenciales usando AWS KMS y aplicarlas a los usuarios al usar la aplicación.
- [x] Usar Amazon Cognito para asociar a los usuarios no autenticados con un rol de IAM que tenga acceso limitado a los recursos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación que se ejecuta en instancias de Amazon EC2 debe acceder a objetos dentro de un bucket de Amazon S3 que están cifrados mediante cifrado del lado del servidor con claves de cifrado de AWS KMS (SSE-KMS). La aplicación debe tener acceso a la customer master key (CMK) para descifrar los objetos. ¿Qué combinación de pasos otorgará acceso a la aplicación? (Seleccione DOS)

- [ ] Escribir una política de bucket de S3 que otorgue al bucket acceso a la clave.
- [x] Otorgar acceso a la clave en el rol de IAM de EC2 asociado a las instancias EC2 de la aplicación.
- [x] Escribir una key policy que permita que las políticas de IAM otorguen acceso a la clave.
- [ ] Otorgar acceso a la clave en la ACL del bucket de S3.
- [ ] Crear un parámetro de Systems Manager que exponga la clave de KMS a las instancias EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo está trabajando en una solución de gestión de casos que permite procesar y revisar reclamaciones médicas. Los usuarios inician sesión para proporcionar información relacionada con su situación médica y financiera. Como parte de la aplicación, se cargan a Amazon S3 documentos sensibles como historiales médicos, imágenes médicas, estados de cuenta bancarios y recibos. Todos los documentos deben transmitirse y almacenarse de forma segura. Todo acceso a los documentos debe registrarse para auditoría. ¿Cuál es el enfoque MÁS seguro?

- [ ] Usar el cifrado predeterminado de S3 con Advanced Encryption Standard-256 (AES-256) en el bucket de destino.
- [ ] Usar Amazon Cognito para la autorización y autenticación para garantizar la seguridad de la aplicación y de los documentos.
- [ ] Usar AWS Lambda para cifrar y descifrar los objetos a medida que se colocan en el bucket de S3.
- [x] Usar cifrado/descifrado del lado del cliente con Amazon S3 y AWS KMS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene una aplicación expuesta a internet que usa Web Identity Federation para obtener una credencial temporal de AWS Security Token Service (AWS STS). Luego la aplicación usa el token para acceder a servicios de AWS. Revise la siguiente respuesta: Según la respuesta mostrada, ¿qué permisos están asociados con la llamada de la aplicación?

![Question 344](images/question344.jpg)

- [ ] Permisos asociados con el rol `AROACLKWSDQRAOEXAMPLE:app1`.
- [ ] Permisos asociados con el rol predeterminado utilizado cuando se creó el servicio de AWS.
- [x] Permisos asociados con el IAM principal propietario del `AccessKeyID` `ASgeIAIOSFODNN7EXAMPLE`.
- [ ] Permisos asociados con la cuenta propietaria del servicio de AWS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación web está diseñada para permitir que nuevos usuarios creen cuentas usando sus direcciones de correo electrónico. La aplicación almacenará atributos de cada usuario y se espera que se registren millones de usuarios. ¿Qué debe implementar el desarrollador para lograr los objetivos de diseño?

- [x] Amazon Cognito user pools.
- [ ] AWS Mobile Hub user data storage.
- [ ] Amazon Cognito Sync.
- [ ] AWS Mobile Hub cloud logic.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa necesita una nueva API REST que pueda devolver información sobre el contenido de un bucket de Amazon S3, como el conteo de objetos almacenados en él. La empresa ha decidido que la nueva API se escriba como un microservicio usando AWS Lambda y Amazon API Gateway. ¿Cómo debe asegurarse el desarrollador de que el microservicio tenga el acceso necesario al bucket de Amazon S3, respetando las mejores prácticas de seguridad?

- [ ] Crear un usuario de IAM que tenga permisos para acceder al bucket de Amazon S3 y almacenar las credenciales del usuario de IAM en el código fuente de la función Lambda.
- [x] Crear un rol de IAM que tenga permisos para acceder al bucket de Amazon S3 y asignarlo a la función Lambda como su rol de ejecución.
- [ ] Crear una política de bucket de Amazon S3 que especifique el servicio Lambda como su principal y asignarla al bucket de Amazon S3.
- [ ] Crear un rol de IAM, asociarle la política administrada AmazonS3FullAccess y asignar el rol a la función Lambda como su rol de ejecución.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una organización usa Amazon CloudFront para asegurar que sus usuarios tengan acceso de baja latencia a su aplicación web. La organización ha identificado la necesidad de cifrar todo el tráfico entre los usuarios y CloudFront, y todo el tráfico entre CloudFront y la aplicación web. ¿Cómo se pueden cumplir estos requisitos? (Elija DOS)

- [ ] Usar AWS KMS para cifrar el tráfico entre CloudFront y la aplicación web.
- [x] Establecer la Origin Protocol Policy en `HTTPS Only`.
- [ ] Establecer el HTTP Port del origen en `443`.
- [x] Establecer la Viewer Protocol Policy en `HTTPS Only` o `Redirect HTTP to HTTPS`.
- [ ] Habilitar la opción de CloudFront `Restrict Viewer Access`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Según las mejores prácticas, ¿cómo deben administrarse las claves de acceso en AWS? (Elija DOS)

- [ ] Usar la misma clave de acceso en todas las aplicaciones por consistencia.
- [x] Eliminar todas las claves de acceso del usuario `root` de la cuenta.
- [ ] Dejar las claves de acceso sin usar en la cuenta con fines de seguimiento.
- [ ] Incrustar y cifrar las claves de acceso en el código para el despliegue continuo.
- [x] Usar roles de Amazon IAM en lugar de claves de acceso siempre que sea posible.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación que se ejecuta en una instancia EC2 de Amazon Linux necesita administrar la infraestructura de AWS. ¿Cómo se puede configurar la instancia EC2 para realizar llamadas a la API de AWS de forma segura?

- [ ] Firmar el comando de AWS CLI usando el proceso de firma versión 4.
- [ ] Ejecutar el comando `aws configure` de AWS CLI y especificar el access key id y la secret access key.
- [x] Especificar un rol para la instancia EC2 con los privilegios necesarios.
- [ ] Pasar el access key id y la secret access key como parámetros en cada comando de AWS CLI.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa de redes sociales usa Amazon Cognito para sincronizar perfiles entre diferentes dispositivos móviles, con el fin de que los usuarios finales tengan una experiencia fluida. ¿Cuál de las siguientes configuraciones puede usarse para notificar de forma silenciosa a los usuarios cada vez que haya una actualización disponible en todos los demás dispositivos?

- [ ] Modificar el user pool para incluir todos los dispositivos que los mantienen sincronizados.
- [ ] Usar la interfaz SyncCallback para recibir notificaciones en la aplicación.
- [ ] Usar un Amazon Cognito stream para analizar los datos y enviar las notificaciones.
- [x] Usar la característica de sincronización push con el rol de IAM apropiado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa desarrolló un conjunto de APIs que se sirven a través de Amazon API Gateway. Las llamadas a la API deben autenticarse basándose en proveedores de identidad OpenID como Amazon o Facebook. Las APIs deben permitir el acceso basándose en un modelo de autorización personalizado. ¿Cuál es el diseño más simple y MÁS seguro para construir un modelo de autenticación y autorización para las APIs?

- [x] Usar Amazon Cognito user pools y un custom authorizer para autenticar y autorizar a los usuarios basándose en JSON Web Tokens.
- [ ] Construir un token broker de OpenID con Amazon y Facebook. Los usuarios se autenticarán con estos proveedores de identidad y pasarán el JSON Web Token a la API para autenticar cada llamada a la API.
- [ ] Almacenar las credenciales de usuario en Amazon DynamoDB y hacer que la aplicación obtenga credenciales temporales de AWS STS. Realizar las llamadas a la API pasando las credenciales del usuario a las APIs para la autenticación y autorización.
- [ ] Usar Amazon RDS para almacenar las credenciales de usuario y pasarlas a las APIs para la autenticación y autorización.

**[⬆ Back to Top](#tabla-de-contenidos)**
