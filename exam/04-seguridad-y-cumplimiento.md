# Dominio 4: Seguridad y cumplimiento (16 %)

Preguntas de práctica AWS Certified CloudOps Engineer – Associate (SOA-C03) — 80 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [El sitio web público de una empresa está alojado en un bucket de Amazon S3 en la región `us-east-1`, detrás de una distribución de Amazon CloudFront. La empresa quiere asegurarse de que el sitio web esté protegido contra ataques DDoS. Un ingeniero de CloudOps necesita implementar una solución que le dé a la empresa la capacidad de mantener control sobre el límite de velocidad (rate limit) con el que se aplican las protecciones contra DDoS. ¿Qué solución cumple con estos requisitos?](#el-sitio-web-público-de-una-empresa-está-alojado-en-un-bucket-de-amazon-s3-en-la-región-us-east-1-detrás-de-una-distribución-de-amazon-cloudfront-la-empresa-quiere-asegurarse-de-que-el-sitio-web-esté-protegido-contra-ataques-ddos-un-ingeniero-de-cloudops-necesita-implementar-una-solución-que-le-dé-a-la-empresa-la-capacidad-de-mantener-control-sobre-el-límite-de-velocidad-rate-limit-con-el-que-se-aplican-las-protecciones-contra-ddos-qué-solución-cumple-con-estos-requisitos) |
| 2 | [Una empresa aloja un portal de compras en línea en la nube de AWS. El portal ofrece seguridad `HTTPS` mediante un certificado TLS en un Elastic Load Balancer (ELB). Recientemente, el portal sufrió una interrupción porque el certificado TLS expiró. Un ingeniero de CloudOps debe crear una solución para renovar automáticamente los certificados y evitar este problema en el futuro. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-aloja-un-portal-de-compras-en-línea-en-la-nube-de-aws-el-portal-ofrece-seguridad-https-mediante-un-certificado-tls-en-un-elastic-load-balancer-elb-recientemente-el-portal-sufrió-una-interrupción-porque-el-certificado-tls-expiró-un-ingeniero-de-cloudops-debe-crear-una-solución-para-renovar-automáticamente-los-certificados-y-evitar-este-problema-en-el-futuro-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 3 | [Ante la amenaza de virus de ransomware que cifran y retienen como rehenes los datos de la empresa, ¿qué acción se debe tomar para proteger un bucket de Amazon S3?](#ante-la-amenaza-de-virus-de-ransomware-que-cifran-y-retienen-como-rehenes-los-datos-de-la-empresa-qué-acción-se-debe-tomar-para-proteger-un-bucket-de-amazon-s3) |
| 4 | [Una empresa se está asociando con un proveedor externo para brindar servicios de procesamiento de datos. Para esta integración, el proveedor debe alojar los datos de la empresa en un bucket de Amazon S3 dentro de la cuenta de AWS del proveedor. El proveedor permite que la empresa proporcione una clave de AWS Key Management Service (AWS KMS) para cifrar los datos de la empresa. El proveedor le ha entregado a la empresa el Amazon Resource Name (ARN) de un rol de IAM para esta integración. ¿Qué debe hacer un ingeniero de CloudOps para configurar esta integración?](#una-empresa-se-está-asociando-con-un-proveedor-externo-para-brindar-servicios-de-procesamiento-de-datos-para-esta-integración-el-proveedor-debe-alojar-los-datos-de-la-empresa-en-un-bucket-de-amazon-s3-dentro-de-la-cuenta-de-aws-del-proveedor-el-proveedor-permite-que-la-empresa-proporcione-una-clave-de-aws-key-management-service-aws-kms-para-cifrar-los-datos-de-la-empresa-el-proveedor-le-ha-entregado-a-la-empresa-el-amazon-resource-name-arn-de-un-rol-de-iam-para-esta-integración-qué-debe-hacer-un-ingeniero-de-cloudops-para-configurar-esta-integración) |
| 5 | [Una base de datos se ejecuta en una instancia de Amazon RDS Multi-AZ. Una auditoría de seguridad reciente encontró que la base de datos no cumple con la normativa porque no está cifrada. ¿Qué enfoque resolverá el requisito de cifrado?](#una-base-de-datos-se-ejecuta-en-una-instancia-de-amazon-rds-multi-az-una-auditoría-de-seguridad-reciente-encontró-que-la-base-de-datos-no-cumple-con-la-normativa-porque-no-está-cifrada-qué-enfoque-resolverá-el-requisito-de-cifrado) |
| 6 | [Un ingeniero de CloudOps recibe una alerta de Amazon GuardDuty sobre actividad de red sospechosa en una instancia de Amazon EC2. El hallazgo de GuardDuty indica una nueva dirección IP externa como destino del tráfico. El ingeniero de CloudOps no reconoce esa dirección IP externa y debe bloquear el tráfico hacia la dirección IP externa identificada por GuardDuty. ¿Qué solución cumple con este requisito?](#un-ingeniero-de-cloudops-recibe-una-alerta-de-amazon-guardduty-sobre-actividad-de-red-sospechosa-en-una-instancia-de-amazon-ec2-el-hallazgo-de-guardduty-indica-una-nueva-dirección-ip-externa-como-destino-del-tráfico-el-ingeniero-de-cloudops-no-reconoce-esa-dirección-ip-externa-y-debe-bloquear-el-tráfico-hacia-la-dirección-ip-externa-identificada-por-guardduty-qué-solución-cumple-con-este-requisito) |
| 7 | [Un ingeniero de CloudOps necesita permitir que los usuarios carguen objetos a un bucket de Amazon S3. El ingeniero de CloudOps crea una URL prefirmada (presigned URL) y se la entrega a un usuario, pero el usuario no puede cargar un objeto al bucket de S3. La URL prefirmada no ha expirado y no hay ninguna política de bucket aplicada al bucket de S3. ¿Cuál de las siguientes podría ser la causa de este problema?](#un-ingeniero-de-cloudops-necesita-permitir-que-los-usuarios-carguen-objetos-a-un-bucket-de-amazon-s3-el-ingeniero-de-cloudops-crea-una-url-prefirmada-presigned-url-y-se-la-entrega-a-un-usuario-pero-el-usuario-no-puede-cargar-un-objeto-al-bucket-de-s3-la-url-prefirmada-no-ha-expirado-y-no-hay-ninguna-política-de-bucket-aplicada-al-bucket-de-s3-cuál-de-las-siguientes-podría-ser-la-causa-de-este-problema) |
| 8 | [Una empresa necesita restringir el acceso a un bucket de Amazon S3 únicamente a instancias de Amazon EC2 que estén dentro de una `VPC`. Todo el tráfico debe transitar por la red privada de AWS. ¿Qué acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?](#una-empresa-necesita-restringir-el-acceso-a-un-bucket-de-amazon-s3-únicamente-a-instancias-de-amazon-ec2-que-estén-dentro-de-una-vpc-todo-el-tráfico-debe-transitar-por-la-red-privada-de-aws-qué-acciones-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 9 | [Una empresa administra múltiples cuentas de AWS mediante una sola organización en AWS Organizations. La empresa está revisando la seguridad interna de su entorno de AWS. El ingeniero de seguridad de la empresa tiene su propia cuenta de AWS y quiere revisar la configuración de `VPC` de las cuentas de AWS de los desarrolladores. ¿Qué solución cumple con estos requisitos de la manera MÁS segura?](#una-empresa-administra-múltiples-cuentas-de-aws-mediante-una-sola-organización-en-aws-organizations-la-empresa-está-revisando-la-seguridad-interna-de-su-entorno-de-aws-el-ingeniero-de-seguridad-de-la-empresa-tiene-su-propia-cuenta-de-aws-y-quiere-revisar-la-configuración-de-vpc-de-las-cuentas-de-aws-de-los-desarrolladores-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-segura) |
| 10 | [Una empresa tiene múltiples conexiones AWS Site-to-Site `VPN` entre una `VPC` y sus oficinas remotas. La empresa administra un dominio de Amazon Elasticsearch Service (Amazon ES) configurado con acceso público. El dominio de Amazon ES tiene una política de acceso al dominio abierta. Un ingeniero de CloudOps necesita asegurarse de que Amazon ES solo pueda ser accedido desde las oficinas remotas, preservando los datos existentes. ¿Qué solución cumple con estos requisitos?](#una-empresa-tiene-múltiples-conexiones-aws-site-to-site-vpn-entre-una-vpc-y-sus-oficinas-remotas-la-empresa-administra-un-dominio-de-amazon-elasticsearch-service-amazon-es-configurado-con-acceso-público-el-dominio-de-amazon-es-tiene-una-política-de-acceso-al-dominio-abierta-un-ingeniero-de-cloudops-necesita-asegurarse-de-que-amazon-es-solo-pueda-ser-accedido-desde-las-oficinas-remotas-preservando-los-datos-existentes-qué-solución-cumple-con-estos-requisitos) |
| 11 | [Un equipo de desarrollo implementó recientemente una nueva versión de una aplicación web en producción. Después del lanzamiento, una prueba de penetración reveló una vulnerabilidad de cross-site scripting que podría exponer datos de usuarios. ¿Qué servicio de AWS mitigará este problema?](#un-equipo-de-desarrollo-implementó-recientemente-una-nueva-versión-de-una-aplicación-web-en-producción-después-del-lanzamiento-una-prueba-de-penetración-reveló-una-vulnerabilidad-de-cross-site-scripting-que-podría-exponer-datos-de-usuarios-qué-servicio-de-aws-mitigará-este-problema) |
| 12 | [Una instancia de Amazon EC2 ejecuta una aplicación que utiliza colas de Amazon Simple Queue Service (Amazon SQS). Un ingeniero de CloudOps debe asegurarse de que la aplicación pueda leer, escribir y eliminar mensajes de las colas de SQS. ¿Qué solución cumple con estos requisitos de la manera MÁS segura?](#una-instancia-de-amazon-ec2-ejecuta-una-aplicación-que-utiliza-colas-de-amazon-simple-queue-service-amazon-sqs-un-ingeniero-de-cloudops-debe-asegurarse-de-que-la-aplicación-pueda-leer-escribir-y-eliminar-mensajes-de-las-colas-de-sqs-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-segura) |
| 13 | [Una empresa le pide a un ingeniero de CloudOps que garantice que los archivos de AWS CloudTrail no sean alterados después de su creación. Actualmente, la empresa usa AWS Identity and Access Management (IAM) para restringir el acceso a rutas de seguimiento (trails) específicas. El equipo de seguridad de la empresa necesita poder rastrear la integridad de cada archivo. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-le-pide-a-un-ingeniero-de-cloudops-que-garantice-que-los-archivos-de-aws-cloudtrail-no-sean-alterados-después-de-su-creación-actualmente-la-empresa-usa-aws-identity-and-access-management-iam-para-restringir-el-acceso-a-rutas-de-seguimiento-trails-específicas-el-equipo-de-seguridad-de-la-empresa-necesita-poder-rastrear-la-integridad-de-cada-archivo-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 14 | [Una empresa usa Amazon Elasticsearch Service (Amazon ES) para analizar datos de ventas y de uso de clientes. Los miembros del equipo de ventas de la empresa, geográficamente dispersos, están de viaje. Necesitan iniciar sesión en Kibana usando sus credenciales corporativas existentes, almacenadas en Active Directory. La empresa ha implementado Active Directory Federation Services (AD FS) para habilitar la autenticación hacia servicios en la nube. ¿Qué solución cumple con estos requisitos?](#una-empresa-usa-amazon-elasticsearch-service-amazon-es-para-analizar-datos-de-ventas-y-de-uso-de-clientes-los-miembros-del-equipo-de-ventas-de-la-empresa-geográficamente-dispersos-están-de-viaje-necesitan-iniciar-sesión-en-kibana-usando-sus-credenciales-corporativas-existentes-almacenadas-en-active-directory-la-empresa-ha-implementado-active-directory-federation-services-ad-fs-para-habilitar-la-autenticación-hacia-servicios-en-la-nube-qué-solución-cumple-con-estos-requisitos) |
| 15 | [Una gran empresa utiliza AWS Organizations para administrar su entorno multi-cuenta de AWS. Según la política de la empresa, todos los usuarios deben tener acceso de solo lectura a un bucket de Amazon S3 en particular, ubicado en una cuenta central. Los datos del bucket de S3 no deben estar disponibles fuera de la organización. Un ingeniero de CloudOps debe configurar los permisos y agregar una política de bucket al bucket de S3. ¿Qué parámetros se deben especificar para lograr esto de la manera MÁS eficiente?](#una-gran-empresa-utiliza-aws-organizations-para-administrar-su-entorno-multi-cuenta-de-aws-según-la-política-de-la-empresa-todos-los-usuarios-deben-tener-acceso-de-solo-lectura-a-un-bucket-de-amazon-s3-en-particular-ubicado-en-una-cuenta-central-los-datos-del-bucket-de-s3-no-deben-estar-disponibles-fuera-de-la-organización-un-ingeniero-de-cloudops-debe-configurar-los-permisos-y-agregar-una-política-de-bucket-al-bucket-de-s3-qué-parámetros-se-deben-especificar-para-lograr-esto-de-la-manera-más-eficiente) |
| 16 | [Una empresa actualiza su política de seguridad para prohibir la exposición pública de cualquier dato en los buckets de Amazon S3 de la cuenta de la empresa. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-actualiza-su-política-de-seguridad-para-prohibir-la-exposición-pública-de-cualquier-dato-en-los-buckets-de-amazon-s3-de-la-cuenta-de-la-empresa-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 17 | [Un informe de Amazon S3 Inventory revela que más de 1 millón de objetos en un bucket de S3 no están cifrados. Estos objetos deben cifrarse, y todos los objetos futuros deben cifrarse en el momento en que se escriben. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Seleccione DOS)](#un-informe-de-amazon-s3-inventory-revela-que-más-de-1-millón-de-objetos-en-un-bucket-de-s3-no-están-cifrados-estos-objetos-deben-cifrarse-y-todos-los-objetos-futuros-deben-cifrarse-en-el-momento-en-que-se-escriben-qué-combinación-de-acciones-debe-tomar-un-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-seleccione-dos) |
| 18 | [Una empresa ha adjuntado la siguiente política a un usuario de IAM. ¿Cuál de las siguientes acciones está permitida para el usuario de IAM?](#una-empresa-ha-adjuntado-la-siguiente-política-a-un-usuario-de-iam-cuál-de-las-siguientes-acciones-está-permitida-para-el-usuario-de-iam) |
| 19 | [Un ingeniero de CloudOps no puede autenticar una llamada de la AWS CLI a un servicio de AWS. ¿Cuál de las siguientes es la causa de este problema?](#un-ingeniero-de-cloudops-no-puede-autenticar-una-llamada-de-la-aws-cli-a-un-servicio-de-aws-cuál-de-las-siguientes-es-la-causa-de-este-problema) |
| 20 | [Un ingeniero de CloudOps necesita proteger las credenciales de una base de datos de Amazon RDS que se crea mediante una plantilla de AWS CloudFormation. La solución debe cifrar las credenciales y debe admitir rotación automática. ¿Qué solución cumple con estos requisitos?](#un-ingeniero-de-cloudops-necesita-proteger-las-credenciales-de-una-base-de-datos-de-amazon-rds-que-se-crea-mediante-una-plantilla-de-aws-cloudformation-la-solución-debe-cifrar-las-credenciales-y-debe-admitir-rotación-automática-qué-solución-cumple-con-estos-requisitos) |
| 21 | [Una empresa debe garantizar que todos los objetos cargados a un bucket de S3 estén cifrados. ¿Cuáles de las siguientes acciones cumplen con este requisito? (Elija dos.)](#una-empresa-debe-garantizar-que-todos-los-objetos-cargados-a-un-bucket-de-s3-estén-cifrados-cuáles-de-las-siguientes-acciones-cumplen-con-este-requisito-elija-dos) |
| 22 | [Una empresa manufacturera usa una instancia de base de datos de Amazon RDS para almacenar el inventario de todos los artículos en stock. La empresa mantiene varias funciones de AWS Lambda que interactúan con la base de datos para agregar, actualizar y eliminar artículos. Las funciones Lambda usan credenciales embebidas (hardcoded) para conectarse a la base de datos. Un ingeniero de CloudOps debe asegurarse de que las credenciales de la base de datos nunca se almacenen en texto plano y de que la contraseña se rote cada 30 días. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?](#una-empresa-manufacturera-usa-una-instancia-de-base-de-datos-de-amazon-rds-para-almacenar-el-inventario-de-todos-los-artículos-en-stock-la-empresa-mantiene-varias-funciones-de-aws-lambda-que-interactúan-con-la-base-de-datos-para-agregar-actualizar-y-eliminar-artículos-las-funciones-lambda-usan-credenciales-embebidas-hardcoded-para-conectarse-a-la-base-de-datos-un-ingeniero-de-cloudops-debe-asegurarse-de-que-las-credenciales-de-la-base-de-datos-nunca-se-almacenen-en-texto-plano-y-de-que-la-contraseña-se-rote-cada-30-días-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-eficiente-operativamente) |
| 23 | [Un ingeniero de CloudOps necesita configurar la rotación automática de las credenciales de una base de datos de Amazon RDS. Las credenciales deben rotarse cada 30 días. La solución debe integrarse con Amazon RDS. ¿Qué solución cumple con estos requisitos con el MENOR esfuerzo operativo?](#un-ingeniero-de-cloudops-necesita-configurar-la-rotación-automática-de-las-credenciales-de-una-base-de-datos-de-amazon-rds-las-credenciales-deben-rotarse-cada-30-días-la-solución-debe-integrarse-con-amazon-rds-qué-solución-cumple-con-estos-requisitos-con-el-menor-esfuerzo-operativo) |
| 24 | [Una empresa almacena sus datos en un bucket de Amazon S3. La empresa necesita clasificar los datos y encontrar cualquier información personal sensible en sus archivos de S3. ¿Qué solución cumple con estos requisitos?](#una-empresa-almacena-sus-datos-en-un-bucket-de-amazon-s3-la-empresa-necesita-clasificar-los-datos-y-encontrar-cualquier-información-personal-sensible-en-sus-archivos-de-s3-qué-solución-cumple-con-estos-requisitos) |
| 25 | [Un ingeniero de CloudOps debe crear una política de IAM para un desarrollador que necesita acceso a servicios específicos de AWS. Con base en los requisitos, el ingeniero de CloudOps crea la siguiente política. ¿Qué acciones permite esta política? (Seleccione DOS.)](#un-ingeniero-de-cloudops-debe-crear-una-política-de-iam-para-un-desarrollador-que-necesita-acceso-a-servicios-específicos-de-aws-con-base-en-los-requisitos-el-ingeniero-de-cloudops-crea-la-siguiente-política-qué-acciones-permite-esta-política-seleccione-dos) |
| 26 | [Un ingeniero de CloudOps usa instancias de Amazon EC2 para alojar una aplicación. El ingeniero de CloudOps necesita otorgar permisos para que la aplicación acceda a una tabla de Amazon DynamoDB. ¿Qué solución cumple con este requisito?](#un-ingeniero-de-cloudops-usa-instancias-de-amazon-ec2-para-alojar-una-aplicación-el-ingeniero-de-cloudops-necesita-otorgar-permisos-para-que-la-aplicación-acceda-a-una-tabla-de-amazon-dynamodb-qué-solución-cumple-con-este-requisito) |
| 27 | [El propietario de una cuenta raíz (root) le ha dado acceso completo a su bucket de S3 a uno de los usuarios de IAM usando la `ACL` del bucket. Cuando el usuario de IAM inicia sesión en la consola de S3, ¿qué acciones puede realizar?](#el-propietario-de-una-cuenta-raíz-root-le-ha-dado-acceso-completo-a-su-bucket-de-s3-a-uno-de-los-usuarios-de-iam-usando-la-acl-del-bucket-cuando-el-usuario-de-iam-inicia-sesión-en-la-consola-de-s3-qué-acciones-puede-realizar) |
| 28 | [Un bucket de Amazon S3 en la cuenta de un ingeniero de CloudOps puede ser accedido por usuarios de otras cuentas de AWS. ¿Cómo puede el ingeniero asegurarse de que el bucket sea accesible únicamente para los miembros de su propia cuenta de AWS?](#un-bucket-de-amazon-s3-en-la-cuenta-de-un-ingeniero-de-cloudops-puede-ser-accedido-por-usuarios-de-otras-cuentas-de-aws-cómo-puede-el-ingeniero-asegurarse-de-que-el-bucket-sea-accesible-únicamente-para-los-miembros-de-su-propia-cuenta-de-aws) |
| 29 | [Un ingeniero de CloudOps está ayudando a un equipo de desarrollo a desplegar una aplicación en AWS. La plantilla de AWS CloudFormation incluye una instancia de EC2 con Amazon Linux, un clúster de base de datos de Amazon Aurora y una contraseña de base de datos embebida (hard-coded) que debe rotarse cada 90 días. ¿Cuál es la forma MÁS segura de administrar la contraseña de la base de datos?](#un-ingeniero-de-cloudops-está-ayudando-a-un-equipo-de-desarrollo-a-desplegar-una-aplicación-en-aws-la-plantilla-de-aws-cloudformation-incluye-una-instancia-de-ec2-con-amazon-linux-un-clúster-de-base-de-datos-de-amazon-aurora-y-una-contraseña-de-base-de-datos-embebida-hard-coded-que-debe-rotarse-cada-90-días-cuál-es-la-forma-más-segura-de-administrar-la-contraseña-de-la-base-de-datos) |
| 30 | [El ingeniero de CloudOps de una empresa ha creado una instancia de Amazon EC2 con software personalizado que se usará como plantilla para todas las nuevas instancias de EC2 en múltiples cuentas de AWS. Los volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos a la instancia de EC2 están cifrados con claves administradas por AWS. El ingeniero de CloudOps crea una Amazon Machine Image (AMI) de la instancia de EC2 personalizada y planea compartir la AMI con las demás cuentas de AWS de la empresa. La empresa exige que todas las AMIs estén cifradas con claves de AWS Key Management Service (AWS KMS) y que solo las cuentas de AWS autorizadas puedan acceder a las AMIs compartidas. ¿Qué solución compartirá la AMI de forma segura con las demás cuentas de AWS?](#el-ingeniero-de-cloudops-de-una-empresa-ha-creado-una-instancia-de-amazon-ec2-con-software-personalizado-que-se-usará-como-plantilla-para-todas-las-nuevas-instancias-de-ec2-en-múltiples-cuentas-de-aws-los-volúmenes-de-amazon-elastic-block-store-amazon-ebs-adjuntos-a-la-instancia-de-ec2-están-cifrados-con-claves-administradas-por-aws-el-ingeniero-de-cloudops-crea-una-amazon-machine-image-ami-de-la-instancia-de-ec2-personalizada-y-planea-compartir-la-ami-con-las-demás-cuentas-de-aws-de-la-empresa-la-empresa-exige-que-todas-las-amis-estén-cifradas-con-claves-de-aws-key-management-service-aws-kms-y-que-solo-las-cuentas-de-aws-autorizadas-puedan-acceder-a-las-amis-compartidas-qué-solución-compartirá-la-ami-de-forma-segura-con-las-demás-cuentas-de-aws) |
| 31 | [Una empresa monitorea la actividad de su cuenta usando AWS CloudTrail, y le preocupa que algunos archivos de registro estén siendo alterados después de que los registros se entregan al bucket de Amazon S3 de la cuenta. De ahora en adelante, ¿cómo puede el ingeniero de CloudOps confirmar que los archivos de registro no han sido modificados después de ser entregados al bucket de S3?](#una-empresa-monitorea-la-actividad-de-su-cuenta-usando-aws-cloudtrail-y-le-preocupa-que-algunos-archivos-de-registro-estén-siendo-alterados-después-de-que-los-registros-se-entregan-al-bucket-de-amazon-s3-de-la-cuenta-de-ahora-en-adelante-cómo-puede-el-ingeniero-de-cloudops-confirmar-que-los-archivos-de-registro-no-han-sido-modificados-después-de-ser-entregados-al-bucket-de-s3) |
| 32 | [Un equipo de ingenieros de guardia (on-call) necesita conectarse frecuentemente a instancias de Amazon EC2 en una subred privada para solucionar problemas y ejecutar comandos. Las instancias usan las últimas Amazon Machine Images (AMIs) de Windows o Amazon Linux proporcionadas por AWS. El equipo tiene un rol de IAM existente para autorización. Un ingeniero de CloudOps debe proporcionar al equipo acceso a las instancias otorgando permisos de IAM a este rol. ¿Qué solución cumple con este requisito?](#un-equipo-de-ingenieros-de-guardia-on-call-necesita-conectarse-frecuentemente-a-instancias-de-amazon-ec2-en-una-subred-privada-para-solucionar-problemas-y-ejecutar-comandos-las-instancias-usan-las-últimas-amazon-machine-images-amis-de-windows-o-amazon-linux-proporcionadas-por-aws-el-equipo-tiene-un-rol-de-iam-existente-para-autorización-un-ingeniero-de-cloudops-debe-proporcionar-al-equipo-acceso-a-las-instancias-otorgando-permisos-de-iam-a-este-rol-qué-solución-cumple-con-este-requisito) |
| 33 | [Una empresa tiene una plantilla de AWS CloudFormation que crea un bucket de Amazon S3. Un usuario se autentica en la cuenta corporativa de AWS con sus credenciales de Active Directory e intenta desplegar la plantilla de CloudFormation. Sin embargo, la creación del stack falla. ¿Qué factores podrían causar este fallo? (Seleccione DOS.)](#una-empresa-tiene-una-plantilla-de-aws-cloudformation-que-crea-un-bucket-de-amazon-s3-un-usuario-se-autentica-en-la-cuenta-corporativa-de-aws-con-sus-credenciales-de-active-directory-e-intenta-desplegar-la-plantilla-de-cloudformation-sin-embargo-la-creación-del-stack-falla-qué-factores-podrían-causar-este-fallo-seleccione-dos) |
| 34 | [Una empresa tiene un nuevo requisito que establece que todos los recursos en AWS deben etiquetarse según una política definida. ¿Qué servicio de AWS se debe usar para hacer cumplir e identificar continuamente todos los recursos que no cumplan con la política?](#una-empresa-tiene-un-nuevo-requisito-que-establece-que-todos-los-recursos-en-aws-deben-etiquetarse-según-una-política-definida-qué-servicio-de-aws-se-debe-usar-para-hacer-cumplir-e-identificar-continuamente-todos-los-recursos-que-no-cumplan-con-la-política) |
| 35 | [Una empresa ha desplegado AWS Security Hub y AWS Config en una organización recién implementada en AWS Organizations. Un ingeniero de CloudOps debe implementar una solución para restringir que todas las cuentas miembro de la organización desplieguen recursos de Amazon EC2 en la región `ap-southeast-2`. La solución debe implementarse desde un único punto y debe gobernar tanto las cuentas actuales como las futuras. El uso de credenciales raíz (root) también debe restringirse en las cuentas miembro. ¿Qué función de AWS debe usar el ingeniero de CloudOps para cumplir con estos requisitos?](#una-empresa-ha-desplegado-aws-security-hub-y-aws-config-en-una-organización-recién-implementada-en-aws-organizations-un-ingeniero-de-cloudops-debe-implementar-una-solución-para-restringir-que-todas-las-cuentas-miembro-de-la-organización-desplieguen-recursos-de-amazon-ec2-en-la-región-ap-southeast-2-la-solución-debe-implementarse-desde-un-único-punto-y-debe-gobernar-tanto-las-cuentas-actuales-como-las-futuras-el-uso-de-credenciales-raíz-root-también-debe-restringirse-en-las-cuentas-miembro-qué-función-de-aws-debe-usar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 36 | [Una solución existente y ya desplegada usa instancias de Amazon EC2 con volúmenes de Amazon EBS General Purpose SSD, una base de datos de Amazon RDS PostgreSQL, un sistema de archivos de Amazon EFS y objetos estáticos almacenados en un bucket de Amazon S3. El equipo de seguridad ahora exige que se active el cifrado en reposo (at-rest) de inmediato para todos los aspectos de la aplicación, sin crear nuevos recursos y sin tiempo de inactividad. Para cumplir con los requisitos, ¿en cuál de estos servicios puede el ingeniero de CloudOps habilitar el cifrado en reposo?](#una-solución-existente-y-ya-desplegada-usa-instancias-de-amazon-ec2-con-volúmenes-de-amazon-ebs-general-purpose-ssd-una-base-de-datos-de-amazon-rds-postgresql-un-sistema-de-archivos-de-amazon-efs-y-objetos-estáticos-almacenados-en-un-bucket-de-amazon-s3-el-equipo-de-seguridad-ahora-exige-que-se-active-el-cifrado-en-reposo-at-rest-de-inmediato-para-todos-los-aspectos-de-la-aplicación-sin-crear-nuevos-recursos-y-sin-tiempo-de-inactividad-para-cumplir-con-los-requisitos-en-cuál-de-estos-servicios-puede-el-ingeniero-de-cloudops-habilitar-el-cifrado-en-reposo) |
| 37 | [Una organización creó un volumen de Amazon Elastic File System (Amazon EFS) con un ID de sistema de archivos fs-85ba41fc, y es usado activamente por 10 hosts de Amazon EC2. A la organización le preocupa que el sistema de archivos no esté cifrado. ¿Cómo se puede resolver esto?](#una-organización-creó-un-volumen-de-amazon-elastic-file-system-amazon-efs-con-un-id-de-sistema-de-archivos-fs-85ba41fc-y-es-usado-activamente-por-10-hosts-de-amazon-ec2-a-la-organización-le-preocupa-que-el-sistema-de-archivos-no-esté-cifrado-cómo-se-puede-resolver-esto) |
| 38 | [Una organización con un departamento de TI grande ha decidido migrar a AWS. Con diferentes funciones de trabajo en el departamento de TI, no es deseable dar a todos los usuarios acceso a todos los recursos de AWS. Actualmente, la organización maneja el acceso mediante membresía a grupos de LDAP. ¿Cuál es el MEJOR método para permitir el acceso usando las credenciales de LDAP actuales?](#una-organización-con-un-departamento-de-ti-grande-ha-decidido-migrar-a-aws-con-diferentes-funciones-de-trabajo-en-el-departamento-de-ti-no-es-deseable-dar-a-todos-los-usuarios-acceso-a-todos-los-recursos-de-aws-actualmente-la-organización-maneja-el-acceso-mediante-membresía-a-grupos-de-ldap-cuál-es-el-mejor-método-para-permitir-el-acceso-usando-las-credenciales-de-ldap-actuales) |
| 39 | [Una empresa está usando una Clave Maestra del Cliente (CMK) de AWS KMS con material de clave importado. La empresa referencia la CMK por su alias en la aplicación Java para cifrar datos. La CMK debe rotarse cada 6 meses. ¿Cuál es el proceso para rotar la clave?](#una-empresa-está-usando-una-clave-maestra-del-cliente-cmk-de-aws-kms-con-material-de-clave-importado-la-empresa-referencia-la-cmk-por-su-alias-en-la-aplicación-java-para-cifrar-datos-la-cmk-debe-rotarse-cada-6-meses-cuál-es-el-proceso-para-rotar-la-clave) |
| 40 | [Un ingeniero de CloudOps está construyendo un proceso para compartir instantáneas de bases de datos de Amazon RDS entre diferentes cuentas asociadas con distintas unidades de negocio dentro de la misma empresa. Todos los datos deben estar cifrados en reposo. ¿Cómo debe implementar el ingeniero este proceso?](#un-ingeniero-de-cloudops-está-construyendo-un-proceso-para-compartir-instantáneas-de-bases-de-datos-de-amazon-rds-entre-diferentes-cuentas-asociadas-con-distintas-unidades-de-negocio-dentro-de-la-misma-empresa-todos-los-datos-deben-estar-cifrados-en-reposo-cómo-debe-implementar-el-ingeniero-este-proceso) |
| 41 | [Una empresa aloja una aplicación interna en instancias de Amazon EC2. Todos los datos y solicitudes de la aplicación se enrutan a través de una conexión AWS Site-to-Site `VPN` entre la red on-premises y AWS. La empresa debe monitorear la aplicación en busca de cambios que permitan acceso de red fuera de la red corporativa. Cualquier cambio que exponga la aplicación externamente debe restringirse automáticamente. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?](#una-empresa-aloja-una-aplicación-interna-en-instancias-de-amazon-ec2-todos-los-datos-y-solicitudes-de-la-aplicación-se-enrutan-a-través-de-una-conexión-aws-site-to-site-vpn-entre-la-red-on-premises-y-aws-la-empresa-debe-monitorear-la-aplicación-en-busca-de-cambios-que-permitan-acceso-de-red-fuera-de-la-red-corporativa-cualquier-cambio-que-exponga-la-aplicación-externamente-debe-restringirse-automáticamente-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-eficiente-operativamente) |
| 42 | [Una empresa ejecuta miles de instancias de Amazon EC2 basadas en la Amazon Machine Image (AMI) de Amazon Linux 2. Un ingeniero de CloudOps debe implementar una solución para registrar comandos y salida de cualquier usuario que necesite una sesión interactiva en una de las instancias de EC2. La solución debe registrar los datos en una ubicación de almacenamiento duradero. La solución también debe proporcionar notificaciones y alarmas automatizadas basadas en los datos de registro. ¿Qué solución cumple con estos requisitos con la MAYOR eficiencia operativa?](#una-empresa-ejecuta-miles-de-instancias-de-amazon-ec2-basadas-en-la-amazon-machine-image-ami-de-amazon-linux-2-un-ingeniero-de-cloudops-debe-implementar-una-solución-para-registrar-comandos-y-salida-de-cualquier-usuario-que-necesite-una-sesión-interactiva-en-una-de-las-instancias-de-ec2-la-solución-debe-registrar-los-datos-en-una-ubicación-de-almacenamiento-duradero-la-solución-también-debe-proporcionar-notificaciones-y-alarmas-automatizadas-basadas-en-los-datos-de-registro-qué-solución-cumple-con-estos-requisitos-con-la-mayor-eficiencia-operativa) |
| 43 | [Los usuarios de la cuenta de AWS de una empresa están lanzando instancias de Amazon EC2 sin las etiquetas de asignación de costos requeridas. Un ingeniero de CloudOps necesita evitar que los usuarios dentro de una organización en AWS Organizations lancen nuevas instancias de EC2 que no tengan las etiquetas requeridas. La solución debe requerir el menor esfuerzo operativo posible. ¿Qué solución cumple con estos requisitos?](#los-usuarios-de-la-cuenta-de-aws-de-una-empresa-están-lanzando-instancias-de-amazon-ec2-sin-las-etiquetas-de-asignación-de-costos-requeridas-un-ingeniero-de-cloudops-necesita-evitar-que-los-usuarios-dentro-de-una-organización-en-aws-organizations-lancen-nuevas-instancias-de-ec2-que-no-tengan-las-etiquetas-requeridas-la-solución-debe-requerir-el-menor-esfuerzo-operativo-posible-qué-solución-cumple-con-estos-requisitos) |
| 44 | [Una empresa está cargando archivos importantes como objetos a Amazon S3. La empresa necesita ser informada si un objeto se corrompe durante la carga. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-está-cargando-archivos-importantes-como-objetos-a-amazon-s3-la-empresa-necesita-ser-informada-si-un-objeto-se-corrompe-durante-la-carga-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 45 | [Un ingeniero de CloudOps debe configurar Amazon S3 para alojar una página web simple de no producción. El ingeniero de CloudOps ha creado un bucket de S3 vacío desde la consola de administración de AWS. El bucket de S3 tiene la configuración predeterminada. ¿Qué combinación de acciones debe tomar el ingeniero de CloudOps para completar este proceso? (Elija dos.)](#un-ingeniero-de-cloudops-debe-configurar-amazon-s3-para-alojar-una-página-web-simple-de-no-producción-el-ingeniero-de-cloudops-ha-creado-un-bucket-de-s3-vacío-desde-la-consola-de-administración-de-aws-el-bucket-de-s3-tiene-la-configuración-predeterminada-qué-combinación-de-acciones-debe-tomar-el-ingeniero-de-cloudops-para-completar-este-proceso-elija-dos) |
| 46 | [Una empresa usa AWS Organizations para administrar múltiples cuentas de AWS. La política corporativa exige que solo se puedan usar regiones específicas de AWS para almacenar y procesar datos de clientes. Un ingeniero de CloudOps debe evitar el aprovisionamiento de instancias de Amazon EC2 en regiones no autorizadas por parte de cualquier persona en la empresa. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-usa-aws-organizations-para-administrar-múltiples-cuentas-de-aws-la-política-corporativa-exige-que-solo-se-puedan-usar-regiones-específicas-de-aws-para-almacenar-y-procesar-datos-de-clientes-un-ingeniero-de-cloudops-debe-evitar-el-aprovisionamiento-de-instancias-de-amazon-ec2-en-regiones-no-autorizadas-por-parte-de-cualquier-persona-en-la-empresa-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 47 | [Una empresa tiene un bucket privado de Amazon S3 que contiene información confidencial. Un ingeniero de CloudOps necesita mantener registros de las direcciones IP de los fallos de autenticación resultantes de intentos de acceder a objetos en el bucket. Los registros deben almacenarse de manera que no puedan sobrescribirse ni eliminarse durante 90 días. ¿Qué solución cumple con estos requisitos?](#una-empresa-tiene-un-bucket-privado-de-amazon-s3-que-contiene-información-confidencial-un-ingeniero-de-cloudops-necesita-mantener-registros-de-las-direcciones-ip-de-los-fallos-de-autenticación-resultantes-de-intentos-de-acceder-a-objetos-en-el-bucket-los-registros-deben-almacenarse-de-manera-que-no-puedan-sobrescribirse-ni-eliminarse-durante-90-días-qué-solución-cumple-con-estos-requisitos) |
| 48 | [Un equipo de cumplimiento normativo requiere que todas las contraseñas de administrador de las instancias de base de datos de Amazon RDS se cambien al menos una vez al año. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?](#un-equipo-de-cumplimiento-normativo-requiere-que-todas-las-contraseñas-de-administrador-de-las-instancias-de-base-de-datos-de-amazon-rds-se-cambien-al-menos-una-vez-al-año-qué-solución-cumple-con-este-requisito-de-la-manera-más-eficiente-operativamente) |
| 49 | [Una empresa usa una distribución de Amazon CloudFront para entregar su sitio web. Los registros de tráfico del sitio web deben almacenarse de forma centralizada, y todos los datos deben estar cifrados en reposo. ¿Qué solución cumple con estos requisitos?](#una-empresa-usa-una-distribución-de-amazon-cloudfront-para-entregar-su-sitio-web-los-registros-de-tráfico-del-sitio-web-deben-almacenarse-de-forma-centralizada-y-todos-los-datos-deben-estar-cifrados-en-reposo-qué-solución-cumple-con-estos-requisitos) |
| 50 | [Una empresa ejecuta un sitio web minorista en múltiples instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa debe asegurar el tráfico hacia el sitio web mediante una conexión `HTTPS`. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)](#una-empresa-ejecuta-un-sitio-web-minorista-en-múltiples-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-alb-la-empresa-debe-asegurar-el-tráfico-hacia-el-sitio-web-mediante-una-conexión-https-qué-combinación-de-acciones-debe-tomar-un-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-elija-dos) |
| 51 | [Un ingeniero de CloudOps administra políticas para muchas cuentas miembro de AWS en una estructura de AWS Organizations. Ingenieros de otros equipos tienen acceso a las credenciales de usuario raíz de las cuentas miembro. El ingeniero de CloudOps debe impedir que todos los equipos, incluyendo sus administradores, usen Amazon DynamoDB. La solución no debe afectar la capacidad de los equipos para acceder a otros servicios de AWS. ¿Qué solución cumple con estos requisitos?](#un-ingeniero-de-cloudops-administra-políticas-para-muchas-cuentas-miembro-de-aws-en-una-estructura-de-aws-organizations-ingenieros-de-otros-equipos-tienen-acceso-a-las-credenciales-de-usuario-raíz-de-las-cuentas-miembro-el-ingeniero-de-cloudops-debe-impedir-que-todos-los-equipos-incluyendo-sus-administradores-usen-amazon-dynamodb-la-solución-no-debe-afectar-la-capacidad-de-los-equipos-para-acceder-a-otros-servicios-de-aws-qué-solución-cumple-con-estos-requisitos) |
| 52 | [Una empresa quiere crear una solución automatizada para todas las cuentas administradas por AWS Organizations que detecte cualquier grupo de seguridad que use `0.0.0.0/0` como dirección de origen para tráfico entrante. La empresa también quiere remediar automáticamente cualquier grupo de seguridad no conforme restringiendo el acceso a un bloque `CIDR` específico que corresponda con la intranet de la empresa. ¿Qué conjunto de acciones debe tomar el ingeniero de CloudOps para crear una solución?](#una-empresa-quiere-crear-una-solución-automatizada-para-todas-las-cuentas-administradas-por-aws-organizations-que-detecte-cualquier-grupo-de-seguridad-que-use-00000-como-dirección-de-origen-para-tráfico-entrante-la-empresa-también-quiere-remediar-automáticamente-cualquier-grupo-de-seguridad-no-conforme-restringiendo-el-acceso-a-un-bloque-cidr-específico-que-corresponda-con-la-intranet-de-la-empresa-qué-conjunto-de-acciones-debe-tomar-el-ingeniero-de-cloudops-para-crear-una-solución) |
| 53 | [Una empresa requiere que toda la actividad en su cuenta de AWS se registre usando AWS CloudTrail. Además, un ingeniero de CloudOps debe saber cuándo se modifican o eliminan los archivos de registro de CloudTrail. ¿Cómo debe el ingeniero de CloudOps cumplir con estos requisitos?](#una-empresa-requiere-que-toda-la-actividad-en-su-cuenta-de-aws-se-registre-usando-aws-cloudtrail-además-un-ingeniero-de-cloudops-debe-saber-cuándo-se-modifican-o-eliminan-los-archivos-de-registro-de-cloudtrail-cómo-debe-el-ingeniero-de-cloudops-cumplir-con-estos-requisitos) |
| 54 | [Una empresa ejecuta una aplicación que aloja datos críticos para varios clientes. La empresa usa AWS CloudTrail para rastrear las actividades de los usuarios en varios recursos de AWS. Para cumplir con nuevos requisitos de seguridad, la empresa necesita proteger los archivos de registro de CloudTrail contra modificación, eliminación o falsificación. ¿Qué solución cumple con este requisito?](#una-empresa-ejecuta-una-aplicación-que-aloja-datos-críticos-para-varios-clientes-la-empresa-usa-aws-cloudtrail-para-rastrear-las-actividades-de-los-usuarios-en-varios-recursos-de-aws-para-cumplir-con-nuevos-requisitos-de-seguridad-la-empresa-necesita-proteger-los-archivos-de-registro-de-cloudtrail-contra-modificación-eliminación-o-falsificación-qué-solución-cumple-con-este-requisito) |
| 55 | [Un ingeniero de CloudOps mantiene la seguridad y el cumplimiento normativo de la cuenta de AWS de una empresa. Para asegurar que las instancias de Amazon EC2 de la empresa sigan la política de la empresa, un ingeniero de CloudOps quiere terminar cualquier instancia de EC2 que no contenga una etiqueta de departamento. Los recursos no conformes deben terminarse casi en tiempo real. ¿Qué solución cumple con estos requisitos?](#un-ingeniero-de-cloudops-mantiene-la-seguridad-y-el-cumplimiento-normativo-de-la-cuenta-de-aws-de-una-empresa-para-asegurar-que-las-instancias-de-amazon-ec2-de-la-empresa-sigan-la-política-de-la-empresa-un-ingeniero-de-cloudops-quiere-terminar-cualquier-instancia-de-ec2-que-no-contenga-una-etiqueta-de-departamento-los-recursos-no-conformes-deben-terminarse-casi-en-tiempo-real-qué-solución-cumple-con-estos-requisitos) |
| 56 | [Una empresa quiere prohibir que sus desarrolladores usen una familia particular de instancias de Amazon EC2. La empresa usa AWS Organizations y quiere aplicar la restricción en múltiples cuentas. ¿Cuál es la forma MÁS eficiente operativamente para que la empresa aplique Políticas de Control de Servicio (SCP) y cumpla con estos requisitos?](#una-empresa-quiere-prohibir-que-sus-desarrolladores-usen-una-familia-particular-de-instancias-de-amazon-ec2-la-empresa-usa-aws-organizations-y-quiere-aplicar-la-restricción-en-múltiples-cuentas-cuál-es-la-forma-más-eficiente-operativamente-para-que-la-empresa-aplique-políticas-de-control-de-servicio-scp-y-cumpla-con-estos-requisitos) |
| 57 | [Un ingeniero de CloudOps quiere proporcionar acceso a servicios de AWS adjuntando una política de IAM a múltiples usuarios de IAM. El ingeniero de CloudOps también quiere poder cambiar la política y crear nuevas versiones. ¿Qué combinación de acciones cumple con estos requisitos? (Elija dos.)](#un-ingeniero-de-cloudops-quiere-proporcionar-acceso-a-servicios-de-aws-adjuntando-una-política-de-iam-a-múltiples-usuarios-de-iam-el-ingeniero-de-cloudops-también-quiere-poder-cambiar-la-política-y-crear-nuevas-versiones-qué-combinación-de-acciones-cumple-con-estos-requisitos-elija-dos) |
| 58 | [Una empresa almacena datos críticos en buckets de Amazon S3. Un ingeniero de CloudOps debe construir una solución para registrar toda la actividad de la API de S3. ¿Qué acción cumplirá con este requisito?](#una-empresa-almacena-datos-críticos-en-buckets-de-amazon-s3-un-ingeniero-de-cloudops-debe-construir-una-solución-para-registrar-toda-la-actividad-de-la-api-de-s3-qué-acción-cumplirá-con-este-requisito) |
| 59 | [Un ingeniero de CloudOps necesita controlar el acceso a grupos de instancias de Amazon EC2 usando AWS Systems Manager Session Manager. Ya se han agregado etiquetas específicas a las instancias de EC2. ¿Qué acciones adicionales debe tomar el ingeniero para controlar el acceso? (Elija dos.)](#un-ingeniero-de-cloudops-necesita-controlar-el-acceso-a-grupos-de-instancias-de-amazon-ec2-usando-aws-systems-manager-session-manager-ya-se-han-agregado-etiquetas-específicas-a-las-instancias-de-ec2-qué-acciones-adicionales-debe-tomar-el-ingeniero-para-controlar-el-acceso-elija-dos) |
| 60 | [Una empresa tiene una función de AWS Lambda en la Cuenta A. La función Lambda necesita leer los objetos en un bucket de Amazon S3 en la Cuenta B. Un ingeniero de CloudOps debe crear los roles de IAM correspondientes en ambas cuentas. ¿Qué solución cumple con estos requisitos?](#una-empresa-tiene-una-función-de-aws-lambda-en-la-cuenta-a-la-función-lambda-necesita-leer-los-objetos-en-un-bucket-de-amazon-s3-en-la-cuenta-b-un-ingeniero-de-cloudops-debe-crear-los-roles-de-iam-correspondientes-en-ambas-cuentas-qué-solución-cumple-con-estos-requisitos) |
| 61 | [Un ingeniero de CloudOps está diseñando una solución para una instancia de base de datos de Amazon RDS para PostgreSQL. Las credenciales de la base de datos deben almacenarse y rotarse mensualmente. Las aplicaciones que se conectan a la instancia de base de datos envían tráfico intensivo en escritura con conexiones de cliente variables que a veces aumentan significativamente en un corto período de tiempo. ¿Qué solución debe elegir un ingeniero de CloudOps para cumplir con estos requisitos?](#un-ingeniero-de-cloudops-está-diseñando-una-solución-para-una-instancia-de-base-de-datos-de-amazon-rds-para-postgresql-las-credenciales-de-la-base-de-datos-deben-almacenarse-y-rotarse-mensualmente-las-aplicaciones-que-se-conectan-a-la-instancia-de-base-de-datos-envían-tráfico-intensivo-en-escritura-con-conexiones-de-cliente-variables-que-a-veces-aumentan-significativamente-en-un-corto-período-de-tiempo-qué-solución-debe-elegir-un-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 62 | [Una empresa mantiene un gran conjunto de datos sensibles en un bucket de Amazon S3. El equipo de seguridad de la empresa le pide a un ingeniero de CloudOps que ayude a verificar que todos los objetos actuales en el bucket de S3 estén cifrados. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-mantiene-un-gran-conjunto-de-datos-sensibles-en-un-bucket-de-amazon-s3-el-equipo-de-seguridad-de-la-empresa-le-pide-a-un-ingeniero-de-cloudops-que-ayude-a-verificar-que-todos-los-objetos-actuales-en-el-bucket-de-s3-estén-cifrados-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 63 | [Una empresa realizó recientemente una auditoría de seguridad de todas sus aplicaciones internas desarrolladas internamente. Ciertas aplicaciones críticas para el negocio que manejan datos sensibles fueron marcadas porque usan clústeres de Amazon ES que están abiertos para lectura/escritura a un grupo de usuarios más amplio del previsto. ¿Quién es responsable de corregir el problema?](#una-empresa-realizó-recientemente-una-auditoría-de-seguridad-de-todas-sus-aplicaciones-internas-desarrolladas-internamente-ciertas-aplicaciones-críticas-para-el-negocio-que-manejan-datos-sensibles-fueron-marcadas-porque-usan-clústeres-de-amazon-es-que-están-abiertos-para-lecturaescritura-a-un-grupo-de-usuarios-más-amplio-del-previsto-quién-es-responsable-de-corregir-el-problema) |
| 64 | [Una empresa tiene una aplicación que usa un bucket de Amazon S3 para almacenamiento de objetos. Un desarrollador necesita configurar el cifrado en tránsito para el bucket de S3. Todos los objetos de S3 que contienen datos personales deben cifrarse en reposo con claves de AWS Key Management Service (AWS KMS), las cuales se pueden rotar bajo demanda. ¿Qué combinación de pasos cumple con estos requisitos? (Elija dos.)](#una-empresa-tiene-una-aplicación-que-usa-un-bucket-de-amazon-s3-para-almacenamiento-de-objetos-un-desarrollador-necesita-configurar-el-cifrado-en-tránsito-para-el-bucket-de-s3-todos-los-objetos-de-s3-que-contienen-datos-personales-deben-cifrarse-en-reposo-con-claves-de-aws-key-management-service-aws-kms-las-cuales-se-pueden-rotar-bajo-demanda-qué-combinación-de-pasos-cumple-con-estos-requisitos-elija-dos) |
| 65 | [Un ingeniero de CloudOps está usando credenciales de IAM para intentar subir un archivo al bucket de Amazon S3 de un cliente llamado `DOC-EXAMPLE-BUCKET`. El ingeniero de CloudOps está recibiendo un mensaje `AccessDenied`. ¿Qué combinación de cambios de configuración corregirá este problema? (Elija dos.)](#un-ingeniero-de-cloudops-está-usando-credenciales-de-iam-para-intentar-subir-un-archivo-al-bucket-de-amazon-s3-de-un-cliente-llamado-doc-example-bucket-el-ingeniero-de-cloudops-está-recibiendo-un-mensaje-accessdenied-qué-combinación-de-cambios-de-configuración-corregirá-este-problema-elija-dos) |
| 66 | [Una empresa ha exigido el uso de autenticación multifactor (MFA) para todos los usuarios de IAM, y requiere que los usuarios hagan todas las llamadas de API usando la CLI. Sin embargo, no se les pide a los usuarios que ingresen tokens de MFA, y pueden ejecutar comandos de la CLI sin MFA. En un intento por hacer cumplir MFA, la empresa adjuntó una política de IAM a todos los usuarios que deniega las llamadas de API que no se hayan autenticado con MFA. ¿Qué paso adicional se debe tomar para asegurar que las llamadas de API se autentiquen usando MFA?](#una-empresa-ha-exigido-el-uso-de-autenticación-multifactor-mfa-para-todos-los-usuarios-de-iam-y-requiere-que-los-usuarios-hagan-todas-las-llamadas-de-api-usando-la-cli-sin-embargo-no-se-les-pide-a-los-usuarios-que-ingresen-tokens-de-mfa-y-pueden-ejecutar-comandos-de-la-cli-sin-mfa-en-un-intento-por-hacer-cumplir-mfa-la-empresa-adjuntó-una-política-de-iam-a-todos-los-usuarios-que-deniega-las-llamadas-de-api-que-no-se-hayan-autenticado-con-mfa-qué-paso-adicional-se-debe-tomar-para-asegurar-que-las-llamadas-de-api-se-autentiquen-usando-mfa) |
| 67 | [Una empresa que usa AWS Organizations requiere que ningún bucket de Amazon S3 en sus cuentas de producción sea eliminado jamás. ¿Cuál es el enfoque MÁS SIMPLE que puede tomar el ingeniero de CloudOps para asegurar que los buckets de S3 en esas cuentas nunca puedan eliminarse?](#una-empresa-que-usa-aws-organizations-requiere-que-ningún-bucket-de-amazon-s3-en-sus-cuentas-de-producción-sea-eliminado-jamás-cuál-es-el-enfoque-más-simple-que-puede-tomar-el-ingeniero-de-cloudops-para-asegurar-que-los-buckets-de-s3-en-esas-cuentas-nunca-puedan-eliminarse) |
| 68 | [Una empresa usa AWS Organizations para alojar varias aplicaciones en múltiples cuentas de AWS. Varios equipos son responsables de construir y mantener la infraestructura de las aplicaciones en las cuentas de AWS. Un ingeniero de CloudOps debe implementar una solución para asegurar que las cuentas de usuario y los permisos se administren centralizadamente. La solución debe integrarse con el entorno de Active Directory local (on-premises) existente de la empresa. El ingeniero de CloudOps ya ha habilitado AWS IAM Identity Center (AWS Single Sign-On) y ha configurado una conexión de AWS Direct Connect. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-usa-aws-organizations-para-alojar-varias-aplicaciones-en-múltiples-cuentas-de-aws-varios-equipos-son-responsables-de-construir-y-mantener-la-infraestructura-de-las-aplicaciones-en-las-cuentas-de-aws-un-ingeniero-de-cloudops-debe-implementar-una-solución-para-asegurar-que-las-cuentas-de-usuario-y-los-permisos-se-administren-centralizadamente-la-solución-debe-integrarse-con-el-entorno-de-active-directory-local-on-premises-existente-de-la-empresa-el-ingeniero-de-cloudops-ya-ha-habilitado-aws-iam-identity-center-aws-single-sign-on-y-ha-configurado-una-conexión-de-aws-direct-connect-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 69 | [Recientemente, varios archivos críticos se eliminaron por error de un bucket compartido de Amazon S3. Un ingeniero de CloudOps necesita prevenir que ocurran eliminaciones accidentales en el futuro habilitando `MFA Delete`. Una vez habilitado, ¿qué actividades del bucket requerirán autenticación MFA? (Elija dos.)](#recientemente-varios-archivos-críticos-se-eliminaron-por-error-de-un-bucket-compartido-de-amazon-s3-un-ingeniero-de-cloudops-necesita-prevenir-que-ocurran-eliminaciones-accidentales-en-el-futuro-habilitando-mfa-delete-una-vez-habilitado-qué-actividades-del-bucket-requerirán-autenticación-mfa-elija-dos) |
| 70 | [Una empresa tiene varias cuentas miembro que forman parte de una organización en AWS Organizations. La empresa descubrió recientemente que los administradores han estado usando credenciales de usuario raíz de la cuenta. La empresa debe evitar que los ingenieros usen credenciales de usuario raíz para realizar cualquier acción en instancias de Amazon EC2. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-tiene-varias-cuentas-miembro-que-forman-parte-de-una-organización-en-aws-organizations-la-empresa-descubrió-recientemente-que-los-administradores-han-estado-usando-credenciales-de-usuario-raíz-de-la-cuenta-la-empresa-debe-evitar-que-los-ingenieros-usen-credenciales-de-usuario-raíz-para-realizar-cualquier-acción-en-instancias-de-amazon-ec2-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 71 | [Una empresa crea una nueva cuenta miembro usando AWS Organizations. Un ingeniero de CloudOps necesita agregar AWS Business Support a la nueva cuenta. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con este requisito? (Elija dos.)](#una-empresa-crea-una-nueva-cuenta-miembro-usando-aws-organizations-un-ingeniero-de-cloudops-necesita-agregar-aws-business-support-a-la-nueva-cuenta-qué-combinación-de-pasos-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito-elija-dos) |
| 72 | [Un ingeniero de CloudOps es responsable de la seguridad de la cuenta de AWS de una empresa. La empresa tiene una política según la cual un usuario solo puede detener o terminar instancias de Amazon EC2 cuando el usuario está autenticado usando un dispositivo de autenticación multifactor (MFA). ¿Qué política debe aplicar el ingeniero de CloudOps para cumplir con este requisito?](#un-ingeniero-de-cloudops-es-responsable-de-la-seguridad-de-la-cuenta-de-aws-de-una-empresa-la-empresa-tiene-una-política-según-la-cual-un-usuario-solo-puede-detener-o-terminar-instancias-de-amazon-ec2-cuando-el-usuario-está-autenticado-usando-un-dispositivo-de-autenticación-multifactor-mfa-qué-política-debe-aplicar-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 73 | [La aplicación de una empresa actualmente usa un rol de IAM que permite acceso total a todos los servicios de AWS. Un ingeniero de CloudOps debe asegurarse de que las políticas de IAM de la empresa permitan solo los permisos que la aplicación requiere. ¿Cómo puede el ingeniero de CloudOps crear una política que cumpla con este requisito?](#la-aplicación-de-una-empresa-actualmente-usa-un-rol-de-iam-que-permite-acceso-total-a-todos-los-servicios-de-aws-un-ingeniero-de-cloudops-debe-asegurarse-de-que-las-políticas-de-iam-de-la-empresa-permitan-solo-los-permisos-que-la-aplicación-requiere-cómo-puede-el-ingeniero-de-cloudops-crear-una-política-que-cumpla-con-este-requisito) |
| 74 | [Una empresa almacena datos sensibles en un bucket de Amazon S3. La empresa debe registrar todos los intentos de acceso al bucket de S3. El equipo de riesgos de la empresa debe recibir notificación inmediata sobre cualquier evento de eliminación. ¿Qué solución cumple con estos requisitos?](#una-empresa-almacena-datos-sensibles-en-un-bucket-de-amazon-s3-la-empresa-debe-registrar-todos-los-intentos-de-acceso-al-bucket-de-s3-el-equipo-de-riesgos-de-la-empresa-debe-recibir-notificación-inmediata-sobre-cualquier-evento-de-eliminación-qué-solución-cumple-con-estos-requisitos) |
| 75 | [Un ingeniero de CloudOps está escribiendo una función de AWS Lambda en la Cuenta A de AWS para colocar objetos en un bucket de Amazon S3 en la Cuenta B de AWS. La función Lambda puede escribir exitosamente nuevos objetos en el bucket de S3, pero los usuarios de IAM en la Cuenta B no pueden eliminar objetos escritos en el bucket por la Cuenta A. ¿Qué paso corregirá este problema?](#un-ingeniero-de-cloudops-está-escribiendo-una-función-de-aws-lambda-en-la-cuenta-a-de-aws-para-colocar-objetos-en-un-bucket-de-amazon-s3-en-la-cuenta-b-de-aws-la-función-lambda-puede-escribir-exitosamente-nuevos-objetos-en-el-bucket-de-s3-pero-los-usuarios-de-iam-en-la-cuenta-b-no-pueden-eliminar-objetos-escritos-en-el-bucket-por-la-cuenta-a-qué-paso-corregirá-este-problema) |
| 76 | [La política de seguridad de una empresa establece que no está permitido conectarse a instancias de Amazon EC2 mediante `SSH` y `RDP`. Si se requiere acceso, el personal autorizado puede conectarse a las instancias usando AWS Systems Manager Session Manager. Los usuarios reportan que no pueden conectarse a una instancia específica de Amazon EC2 que ejecuta Ubuntu y tiene preinstalado AWS Systems Manager Agent (SSM Agent). Estos usuarios pueden usar Session Manager para conectarse a otras instancias en la misma subred, y están en un grupo de IAM que tiene permiso de Session Manager para todas las instancias. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?](#la-política-de-seguridad-de-una-empresa-establece-que-no-está-permitido-conectarse-a-instancias-de-amazon-ec2-mediante-ssh-y-rdp-si-se-requiere-acceso-el-personal-autorizado-puede-conectarse-a-las-instancias-usando-aws-systems-manager-session-manager-los-usuarios-reportan-que-no-pueden-conectarse-a-una-instancia-específica-de-amazon-ec2-que-ejecuta-ubuntu-y-tiene-preinstalado-aws-systems-manager-agent-ssm-agent-estos-usuarios-pueden-usar-session-manager-para-conectarse-a-otras-instancias-en-la-misma-subred-y-están-en-un-grupo-de-iam-que-tiene-permiso-de-session-manager-para-todas-las-instancias-qué-debe-hacer-un-ingeniero-de-cloudops-para-resolver-este-problema) |
| 77 | [Una empresa tiene un bucket de Amazon S3 que contiene datos sensibles. Los datos deben cifrarse en tránsito y en reposo. La empresa cifra los datos en el bucket de S3 usando una clave de AWS Key Management Service (AWS KMS). Un desarrollador necesita otorgar a varias otras cuentas de AWS el permiso para usar la operación `GetObject` de S3 para recuperar los datos del bucket de S3. ¿Cómo puede el desarrollador exigir que todas las solicitudes para recuperar los datos proporcionen cifrado en tránsito?](#una-empresa-tiene-un-bucket-de-amazon-s3-que-contiene-datos-sensibles-los-datos-deben-cifrarse-en-tránsito-y-en-reposo-la-empresa-cifra-los-datos-en-el-bucket-de-s3-usando-una-clave-de-aws-key-management-service-aws-kms-un-desarrollador-necesita-otorgar-a-varias-otras-cuentas-de-aws-el-permiso-para-usar-la-operación-getobject-de-s3-para-recuperar-los-datos-del-bucket-de-s3-cómo-puede-el-desarrollador-exigir-que-todas-las-solicitudes-para-recuperar-los-datos-proporcionen-cifrado-en-tránsito) |
| 78 | [Una empresa tiene dos cuentas de AWS: desarrollo y producción. Todas las aplicaciones envían registros a un bucket de Amazon S3 específico para cada cuenta, y los desarrolladores están solicitando acceso a los buckets de S3 de la cuenta de producción para ver los registros. ¿Cuál es la forma MÁS eficiente de proporcionar a los desarrolladores el acceso?](#una-empresa-tiene-dos-cuentas-de-aws-desarrollo-y-producción-todas-las-aplicaciones-envían-registros-a-un-bucket-de-amazon-s3-específico-para-cada-cuenta-y-los-desarrolladores-están-solicitando-acceso-a-los-buckets-de-s3-de-la-cuenta-de-producción-para-ver-los-registros-cuál-es-la-forma-más-eficiente-de-proporcionar-a-los-desarrolladores-el-acceso) |
| 79 | [Una organización almacena datos sensibles de clientes en buckets de S3 protegidos por políticas de bucket. Recientemente, ha habido reportes de que entidades no autorizadas dentro de la empresa han estado intentando acceder a los datos en esos buckets de S3. El director de seguridad de la información (CISO) quisiera saber qué buckets están siendo objetivo y determinar quién es responsable de intentar acceder a esa información. ¿Qué pasos debe tomar un ingeniero de CloudOps para cumplir con el requisito del CISO? (Elija dos.)](#una-organización-almacena-datos-sensibles-de-clientes-en-buckets-de-s3-protegidos-por-políticas-de-bucket-recientemente-ha-habido-reportes-de-que-entidades-no-autorizadas-dentro-de-la-empresa-han-estado-intentando-acceder-a-los-datos-en-esos-buckets-de-s3-el-director-de-seguridad-de-la-información-ciso-quisiera-saber-qué-buckets-están-siendo-objetivo-y-determinar-quién-es-responsable-de-intentar-acceder-a-esa-información-qué-pasos-debe-tomar-un-ingeniero-de-cloudops-para-cumplir-con-el-requisito-del-ciso-elija-dos) |
| 80 | [Una empresa tiene una aplicación web pública existente para `www.example.com`. El Application Load Balancer (ALB) está configurado con un único listener `HTTP` en el puerto `80`. Un ingeniero de CloudOps debe asegurarse de que todas las solicitudes web a `www.example.com` estén cifradas entre el cliente y el `ALB`. El ingeniero de CloudOps ya ha solicitado y validado un certificado público para `www.example.com` en AWS Certificate Manager (ACM). Los usuarios existentes de la aplicación no deben tener que cambiar el endpoint al que se conectan. ¿Qué conjunto adicional de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?](#una-empresa-tiene-una-aplicación-web-pública-existente-para-wwwexamplecom-el-application-load-balancer-alb-está-configurado-con-un-único-listener-http-en-el-puerto-80-un-ingeniero-de-cloudops-debe-asegurarse-de-que-todas-las-solicitudes-web-a-wwwexamplecom-estén-cifradas-entre-el-cliente-y-el-alb-el-ingeniero-de-cloudops-ya-ha-solicitado-y-validado-un-certificado-público-para-wwwexamplecom-en-aws-certificate-manager-acm-los-usuarios-existentes-de-la-aplicación-no-deben-tener-que-cambiar-el-endpoint-al-que-se-conectan-qué-conjunto-adicional-de-pasos-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |

### El sitio web público de una empresa está alojado en un bucket de Amazon S3 en la región `us-east-1`, detrás de una distribución de Amazon CloudFront. La empresa quiere asegurarse de que el sitio web esté protegido contra ataques DDoS. Un ingeniero de CloudOps necesita implementar una solución que le dé a la empresa la capacidad de mantener control sobre el límite de velocidad (rate limit) con el que se aplican las protecciones contra DDoS. ¿Qué solución cumple con estos requisitos?

- [x] Implementar una `ACL` web de AWS WAF con alcance global, con una acción predeterminada de permitir. Configurar una regla de AWS WAF basada en tasa (rate-based) para bloquear el tráfico que coincida. Asociar la `ACL` web con la distribución de CloudFront.
- [ ] Implementar una `ACL` web de AWS WAF con una acción predeterminada de permitir en `us-east-1`. Configurar una regla de AWS WAF basada en tasa para bloquear el tráfico que coincida. Asociar la `ACL` web con el bucket de S3.
- [ ] Implementar una `ACL` web de AWS WAF con alcance global, con una acción predeterminada de bloquear. Configurar una regla de AWS WAF basada en tasa para permitir el tráfico que coincida. Asociar la `ACL` web con la distribución de CloudFront.
- [ ] Implementar una `ACL` web de AWS WAF con una acción predeterminada de bloquear en `us-east-1`. Configurar una regla de AWS WAF basada en tasa para permitir el tráfico que coincida. Asociar la `ACL` web con el bucket de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja un portal de compras en línea en la nube de AWS. El portal ofrece seguridad `HTTPS` mediante un certificado TLS en un Elastic Load Balancer (ELB). Recientemente, el portal sufrió una interrupción porque el certificado TLS expiró. Un ingeniero de CloudOps debe crear una solución para renovar automáticamente los certificados y evitar este problema en el futuro. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Solicitar un certificado público mediante AWS Certificate Manager (ACM). Asociar el certificado de ACM con el ELB. Escribir una función de AWS Lambda programada para renovar el certificado cada 18 meses.
- [x] Solicitar un certificado público mediante AWS Certificate Manager (ACM). Asociar el certificado de ACM con el ELB. ACM administrará automáticamente la renovación del certificado.
- [ ] Registrar un certificado con una autoridad certificadora (CA) externa. Importar este certificado a AWS Certificate Manager (ACM). Asociar el certificado de ACM con el ELB. ACM administrará automáticamente la renovación del certificado.
- [ ] Registrar un certificado con una autoridad certificadora (CA) externa. Configurar el ELB para importar el certificado directamente desde la CA. Establecer el ciclo de actualización del certificado en el ELB para que se renueve cuando falten 3 meses para la fecha de vencimiento.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Ante la amenaza de virus de ransomware que cifran y retienen como rehenes los datos de la empresa, ¿qué acción se debe tomar para proteger un bucket de Amazon S3?

- [ ] Denegar las acciones Post, Put y Delete en el bucket.
- [x] Habilitar el cifrado del lado del servidor en el bucket.
- [ ] Habilitar el versionado de Amazon S3 en el bucket.
- [ ] Habilitar instantáneas (snapshots) en el bucket.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa se está asociando con un proveedor externo para brindar servicios de procesamiento de datos. Para esta integración, el proveedor debe alojar los datos de la empresa en un bucket de Amazon S3 dentro de la cuenta de AWS del proveedor. El proveedor permite que la empresa proporcione una clave de AWS Key Management Service (AWS KMS) para cifrar los datos de la empresa. El proveedor le ha entregado a la empresa el Amazon Resource Name (ARN) de un rol de IAM para esta integración. ¿Qué debe hacer un ingeniero de CloudOps para configurar esta integración?

- [x] Crear una nueva clave de KMS. Agregar el ARN del rol de IAM del proveedor a la política de la clave de KMS. Entregar el ARN de la nueva clave de KMS al proveedor.
- [ ] Crear una nueva clave de KMS. Crear un nuevo usuario de IAM. Agregar el ARN del rol de IAM del proveedor a una política en línea adjunta al usuario de IAM. Entregar el ARN del nuevo usuario de IAM al proveedor.
- [ ] Configurar el cifrado usando la clave de S3 administrada por KMS. Agregar el ARN del rol de IAM del proveedor a la política de la clave de S3 administrada por KMS. Entregar el ARN de la clave de S3 administrada por KMS al proveedor.
- [ ] Configurar el cifrado usando la clave de S3 administrada por KMS. Crear un bucket de S3. Agregar el ARN del rol de IAM del proveedor a la política del bucket de S3. Entregar el ARN del bucket de S3 al proveedor.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una base de datos se ejecuta en una instancia de Amazon RDS Multi-AZ. Una auditoría de seguridad reciente encontró que la base de datos no cumple con la normativa porque no está cifrada. ¿Qué enfoque resolverá el requisito de cifrado?

- [ ] Iniciar sesión en la consola de RDS y seleccionar la casilla de cifrado para cifrar la base de datos.
- [ ] Crear un nuevo volumen de Amazon EBS cifrado y adjuntarlo a la instancia.
- [ ] Cifrar la réplica en espera (standby) en la Zona de disponibilidad secundaria y promoverla a instancia principal.
- [x] Tomar una instantánea de la instancia de RDS, copiarla y cifrar la copia, y luego restaurarla en una nueva instancia de RDS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps recibe una alerta de Amazon GuardDuty sobre actividad de red sospechosa en una instancia de Amazon EC2. El hallazgo de GuardDuty indica una nueva dirección IP externa como destino del tráfico. El ingeniero de CloudOps no reconoce esa dirección IP externa y debe bloquear el tráfico hacia la dirección IP externa identificada por GuardDuty. ¿Qué solución cumple con este requisito?

- [ ] Crear un nuevo grupo de seguridad para bloquear el tráfico hacia la dirección IP externa. Asignar el nuevo grupo de seguridad a la instancia de EC2.
- [ ] Usar los registros de flujo (flow logs) de `VPC` con Amazon Athena para bloquear el tráfico hacia la dirección IP externa.
- [x] Crear una `ACL` de red. Agregar una regla de denegación de salida para el tráfico hacia la dirección IP externa.
- [ ] Crear un nuevo grupo de seguridad para bloquear el tráfico hacia la dirección IP externa. Asignar el nuevo grupo de seguridad a toda la `VPC`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita permitir que los usuarios carguen objetos a un bucket de Amazon S3. El ingeniero de CloudOps crea una URL prefirmada (presigned URL) y se la entrega a un usuario, pero el usuario no puede cargar un objeto al bucket de S3. La URL prefirmada no ha expirado y no hay ninguna política de bucket aplicada al bucket de S3. ¿Cuál de las siguientes podría ser la causa de este problema?

- [ ] El usuario no ha configurado correctamente la AWS CLI con su clave de acceso y su clave de acceso secreta.
- [x] El ingeniero de CloudOps no tiene los permisos necesarios para cargar el objeto al bucket de S3.
- [ ] El ingeniero de CloudOps debe aplicar una política de bucket al bucket de S3 para permitir que el usuario cargue el objeto.
- [ ] El objeto ya fue cargado mediante el uso de la URL prefirmada, por lo que la URL prefirmada ya no es válida.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa necesita restringir el acceso a un bucket de Amazon S3 únicamente a instancias de Amazon EC2 que estén dentro de una `VPC`. Todo el tráfico debe transitar por la red privada de AWS. ¿Qué acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear un endpoint de `VPC` para el bucket de S3, y crear una política de IAM que limite condicionalmente todas las acciones de S3 sobre el bucket para que el origen sea el endpoint de `VPC`.
- [x] Crear un endpoint de `VPC` para el bucket de S3, y crear una política de bucket de S3 que limite condicionalmente todas las acciones de S3 sobre el bucket para que el origen sea el endpoint de `VPC`.
- [ ] Crear un rol vinculado a servicio (service-linked role) para Amazon EC2 que permita a las instancias de EC2 interactuar directamente con Amazon S3, y adjuntar al rol una política de IAM que dé a las instancias de EC2 acceso completo al bucket de S3.
- [ ] Crear una puerta de enlace `NAT` en la `VPC`, y modificar la tabla de enrutamiento de la `VPC` para enrutar todo el tráfico destinado a Amazon S3 a través de la puerta de enlace `NAT`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa administra múltiples cuentas de AWS mediante una sola organización en AWS Organizations. La empresa está revisando la seguridad interna de su entorno de AWS. El ingeniero de seguridad de la empresa tiene su propia cuenta de AWS y quiere revisar la configuración de `VPC` de las cuentas de AWS de los desarrolladores. ¿Qué solución cumple con estos requisitos de la manera MÁS segura?

- [ ] Crear una política de IAM en cada cuenta de desarrollador con acceso de solo lectura relacionado con recursos de `VPC`. Asignar la política a un usuario de IAM. Compartir las credenciales del usuario con el ingeniero de seguridad.
- [ ] Crear una política de IAM en cada cuenta de desarrollador con acceso de administrador a todas las acciones de Amazon EC2, incluidas las acciones de `VPC`. Asignar la política a un usuario de IAM. Compartir las credenciales del usuario con el ingeniero de seguridad.
- [ ] Crear una política de IAM en cada cuenta de desarrollador con acceso de administrador relacionado con recursos de `VPC`. Asignar la política a un rol de IAM entre cuentas (cross-account). Pedirle al ingeniero de seguridad que asuma el rol desde su cuenta.
- [x] Crear una política de IAM en cada cuenta de desarrollador con acceso de solo lectura relacionado con recursos de `VPC`. Asignar la política a un rol de IAM entre cuentas (cross-account). Pedirle al ingeniero de seguridad que asuma el rol desde su cuenta.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene múltiples conexiones AWS Site-to-Site `VPN` entre una `VPC` y sus oficinas remotas. La empresa administra un dominio de Amazon Elasticsearch Service (Amazon ES) configurado con acceso público. El dominio de Amazon ES tiene una política de acceso al dominio abierta. Un ingeniero de CloudOps necesita asegurarse de que Amazon ES solo pueda ser accedido desde las oficinas remotas, preservando los datos existentes. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar una política de acceso basada en identidad en Amazon ES. Agregar una declaración de permiso (allow) a la política que incluya el Amazon Resource Name (ARN) de cada conexión `VPN` de las oficinas remotas.
- [x] Configurar una política de acceso al dominio basada en IP en Amazon ES. Agregar una declaración de permiso (allow) a la política que incluya los bloques `CIDR` de IP privada de cada red de oficina remota.
- [ ] Implementar un nuevo dominio de Amazon ES en subredes privadas dentro de una `VPC`, e importar una instantánea del dominio anterior. Crear un grupo de seguridad que permita tráfico de entrada desde los bloques `CIDR` de las oficinas remotas.
- [ ] Reconfigurar el dominio de Amazon ES en subredes privadas dentro de una `VPC`. Crear un grupo de seguridad que permita tráfico de entrada desde los bloques `CIDR` de las oficinas remotas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un equipo de desarrollo implementó recientemente una nueva versión de una aplicación web en producción. Después del lanzamiento, una prueba de penetración reveló una vulnerabilidad de cross-site scripting que podría exponer datos de usuarios. ¿Qué servicio de AWS mitigará este problema?

- [ ] AWS Shield Standard.
- [x] AWS WAF.
- [ ] Elastic Load Balancing.
- [ ] Amazon Cognito.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una instancia de Amazon EC2 ejecuta una aplicación que utiliza colas de Amazon Simple Queue Service (Amazon SQS). Un ingeniero de CloudOps debe asegurarse de que la aplicación pueda leer, escribir y eliminar mensajes de las colas de SQS. ¿Qué solución cumple con estos requisitos de la manera MÁS segura?

- [ ] Crear un usuario de IAM con una política de IAM que permita el permiso `sqs:SendMessage`, el permiso `sqs:ReceiveMessage` y el permiso `sqs:DeleteMessage` sobre las colas correspondientes. Incrustar las credenciales del usuario de IAM en la configuración de la aplicación.
- [ ] Crear un usuario de IAM con una política de IAM que permita el permiso `sqs:SendMessage`, el permiso `sqs:ReceiveMessage` y el permiso `sqs:DeleteMessage` sobre las colas correspondientes. Exportar la clave de acceso y la clave de acceso secreta del usuario de IAM como variables de entorno en la instancia de EC2.
- [ ] Crear y asociar un rol de IAM que permita a las instancias de EC2 invocar servicios de AWS. Adjuntar al rol una política de IAM que permita todos los permisos `sqs:*` sobre las colas correspondientes.
- [x] Crear y asociar un rol de IAM que permita a las instancias de EC2 invocar servicios de AWS. Adjuntar al rol una política de IAM que permita el permiso `sqs:SendMessage`, el permiso `sqs:ReceiveMessage` y el permiso `sqs:DeleteMessage` sobre las colas correspondientes.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa le pide a un ingeniero de CloudOps que garantice que los archivos de AWS CloudTrail no sean alterados después de su creación. Actualmente, la empresa usa AWS Identity and Access Management (IAM) para restringir el acceso a rutas de seguimiento (trails) específicas. El equipo de seguridad de la empresa necesita poder rastrear la integridad de cada archivo. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que invoque una función de AWS Lambda cuando se entregue un nuevo archivo. Configurar la función Lambda para calcular un hash MD5 del archivo y almacenar el resultado en una tabla de Amazon DynamoDB. El equipo de seguridad puede usar los valores almacenados en DynamoDB para verificar la integridad de los archivos entregados.
- [ ] Crear una función de AWS Lambda que se invoque cada vez que se entregue un nuevo archivo al bucket de CloudTrail. Configurar la función Lambda para calcular un hash MD5 del archivo y almacenar el resultado como una etiqueta (tag) en un objeto de Amazon S3. El equipo de seguridad puede usar la información de la etiqueta para verificar la integridad de los archivos entregados.
- [ ] Habilitar la función de integridad de archivos de CloudTrail en un bucket de Amazon S3. Crear una política de IAM que otorgue al equipo de seguridad acceso a los registros de integridad de archivos almacenados en el bucket de S3.
- [x] Habilitar la función de integridad de archivos de CloudTrail en la ruta de seguimiento (trail). El equipo de seguridad puede usar el archivo resumen (digest file) creado por CloudTrail para verificar la integridad de los archivos entregados.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa Amazon Elasticsearch Service (Amazon ES) para analizar datos de ventas y de uso de clientes. Los miembros del equipo de ventas de la empresa, geográficamente dispersos, están de viaje. Necesitan iniciar sesión en Kibana usando sus credenciales corporativas existentes, almacenadas en Active Directory. La empresa ha implementado Active Directory Federation Services (AD FS) para habilitar la autenticación hacia servicios en la nube. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar Active Directory como proveedor de autenticación en Amazon ES. Agregar el nombre de dominio del servidor de Active Directory a Amazon ES. Configurar Kibana para usar la autenticación de Amazon ES.
- [x] Implementar un grupo de usuarios (user pool) de Amazon Cognito. Configurar Active Directory como proveedor de identidad externo del grupo de usuarios. Habilitar la autenticación de Amazon Cognito para Kibana en Amazon ES.
- [ ] Habilitar la autenticación de usuarios de Active Directory en Kibana. Crear una política de acceso al dominio personalizada basada en IP en Amazon ES que incluya la dirección IP del servidor de Active Directory.
- [ ] Establecer una relación de confianza (trust) con Kibana en el servidor de Active Directory. Habilitar la autenticación de usuarios de Active Directory en Kibana. Agregar la dirección IP del servidor de Active Directory a Kibana.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una gran empresa utiliza AWS Organizations para administrar su entorno multi-cuenta de AWS. Según la política de la empresa, todos los usuarios deben tener acceso de solo lectura a un bucket de Amazon S3 en particular, ubicado en una cuenta central. Los datos del bucket de S3 no deben estar disponibles fuera de la organización. Un ingeniero de CloudOps debe configurar los permisos y agregar una política de bucket al bucket de S3. ¿Qué parámetros se deben especificar para lograr esto de la manera MÁS eficiente?

- [x] Especificar `"*"` como principal y `PrincipalOrgld` como condición.
- [ ] Especificar todos los números de cuenta como principal.
- [ ] Especificar `PrincipalOrgld` como principal.
- [ ] Especificar la cuenta de administración de la organización como principal.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa actualiza su política de seguridad para prohibir la exposición pública de cualquier dato en los buckets de Amazon S3 de la cuenta de la empresa. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [x] Activar S3 Block Public Access a nivel de cuenta.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para hacer cumplir que todos los objetos de S3 sean privados.
- [ ] Usar Amazon Inspector para buscar buckets de S3 y restablecer automáticamente las `ACL`s de S3 si se encuentran buckets públicos de S3.
- [ ] Usar S3 Object Lambda para examinar las `ACL`s de S3 y cambiar cualquier `ACL` pública de S3 a privada.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un informe de Amazon S3 Inventory revela que más de 1 millón de objetos en un bucket de S3 no están cifrados. Estos objetos deben cifrarse, y todos los objetos futuros deben cifrarse en el momento en que se escriben. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Seleccione DOS)

- [ ] Crear una regla de AWS Config que ejecute evaluaciones sobre los cambios de configuración del bucket de S3. Cuando se encuentre un objeto sin cifrar, ejecutar un documento de Automation de AWS Systems Manager para cifrar el objeto en su lugar.
- [x] Editar las propiedades del bucket de S3 para habilitar el cifrado predeterminado del lado del servidor.
- [x] Filtrar el informe de S3 Inventory usando S3 Select para encontrar todos los objetos que no estén cifrados. Crear un trabajo de S3 Batch Operations para copiar cada objeto en su lugar con el cifrado habilitado.
- [ ] Filtrar el informe de S3 Inventory usando S3 Select para encontrar todos los objetos que no estén cifrados. Enviar el nombre de cada objeto como un mensaje a una cola de Amazon Simple Queue Service (Amazon SQS). Usar la cola de SQS para invocar una función de AWS Lambda que etiquete cada objeto con una clave `Encryption` y un valor `SSE-KMS`.
- [ ] Usar S3 Event Notifications para invocar una función de AWS Lambda en todos los eventos de creación de nuevos objetos del bucket de S3. Configurar la función Lambda para verificar si el objeto está cifrado y ejecutar un documento de Automation de AWS Systems Manager para cifrar el objeto en su lugar cuando se encuentre uno sin cifrar.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha adjuntado la siguiente política a un usuario de IAM. ¿Cuál de las siguientes acciones está permitida para el usuario de IAM?

![Question 62](images/question62.png)

- [ ] La acción `DescribeDBInstances` de Amazon RDS en la región `us-east-1`.
- [ ] La operación `Putobject` de Amazon S3 en un bucket llamado testbucket.
- [x] La acción `DescribeInstances` de Amazon EC2 en la región `us-east-1`.
- [ ] La acción `AttachNetworkinterface` de Amazon EC2 en la región `eu-west-1`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps no puede autenticar una llamada de la AWS CLI a un servicio de AWS. ¿Cuál de las siguientes es la causa de este problema?

- [ ] La contraseña de IAM es incorrecta.
- [ ] Falta el certificado del servidor.
- [ ] El par de claves `SSH` es incorrecto.
- [x] No hay una clave de acceso (access key).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita proteger las credenciales de una base de datos de Amazon RDS que se crea mediante una plantilla de AWS CloudFormation. La solución debe cifrar las credenciales y debe admitir rotación automática. ¿Qué solución cumple con estos requisitos?

- [x] Crear un recurso `AWS::SecretsManager::Secret` en la plantilla de CloudFormation. Referenciar las credenciales en el recurso `AWS::RDS::DBInstance` usando la referencia dinámica `resolve:secretsmanager`.
- [ ] Crear un recurso `AWS::SecretsManager::Secret` en la plantilla de CloudFormation. Referenciar las credenciales en el recurso `AWS::RDS::DBInstance` usando la referencia dinámica `resolve:ssm-secure`.
- [ ] Crear un recurso `AWS::SSM::Parameter` en la plantilla de CloudFormation. Referenciar las credenciales en el recurso `AWS::RDS::DBInstance` usando la referencia dinámica `resolve:ssm`.
- [ ] Crear parámetros para las credenciales de la base de datos en la plantilla de CloudFormation. Usar la función intrínseca Ref para proporcionar las credenciales al recurso `AWS::RDS::DBInstance`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa debe garantizar que todos los objetos cargados a un bucket de S3 estén cifrados. ¿Cuáles de las siguientes acciones cumplen con este requisito? (Elija dos.)

- [ ] Implementar AWS Shield para proteger contra objetos sin cifrar almacenados en buckets de S3.
- [ ] Implementar una Lista de Control de Acceso a Objetos (`ACL`) para denegar la carga de objetos sin cifrar al bucket de S3.
- [x] Implementar el cifrado predeterminado de Amazon S3 para asegurar que cualquier objeto cargado se cifre antes de almacenarse.
- [ ] Implementar Amazon Inspector para inspeccionar los objetos cargados al bucket de S3 y asegurar que estén cifrados.
- [x] Implementar políticas de bucket de S3 para denegar la carga de objetos sin cifrar a los buckets.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa manufacturera usa una instancia de base de datos de Amazon RDS para almacenar el inventario de todos los artículos en stock. La empresa mantiene varias funciones de AWS Lambda que interactúan con la base de datos para agregar, actualizar y eliminar artículos. Las funciones Lambda usan credenciales embebidas (hardcoded) para conectarse a la base de datos. Un ingeniero de CloudOps debe asegurarse de que las credenciales de la base de datos nunca se almacenen en texto plano y de que la contraseña se rote cada 30 días. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Almacenar la contraseña de la base de datos como variable de entorno en cada función Lambda. Crear una nueva función Lambda llamada `PasswordRotate`. Usar Amazon EventBridge (Amazon CloudWatch Events) para programar la función `PasswordRotate` cada 30 días, de modo que cambie la contraseña de la base de datos y actualice la variable de entorno de cada función Lambda.
- [ ] Usar AWS Key Management Service (AWS KMS) para cifrar la contraseña de la base de datos y almacenarla cifrada como variable de entorno en cada función Lambda. Otorgar a cada función Lambda acceso a la clave de KMS para que la contraseña de la base de datos pueda descifrarse cuando sea necesario. Crear una nueva función Lambda llamada `PasswordRotate` para cambiar la contraseña cada 30 días.
- [x] Usar AWS Secrets Manager para almacenar las credenciales de la base de datos. Crear un secreto en Secrets Manager y seleccionar la base de datos para que Secrets Manager use una función Lambda que actualice automáticamente la contraseña de la base de datos. Especificar un cronograma de rotación automática de 30 días. Actualizar cada función Lambda para que acceda a la contraseña de la base de datos desde Secrets Manager.
- [ ] Usar AWS Systems Manager Parameter Store para crear una cadena segura (secure string) que almacene las credenciales de la base de datos. Crear una nueva función Lambda llamada `PasswordRotate`. Usar Amazon EventBridge (Amazon CloudWatch Events) para programar la función `PasswordRotate` cada 30 días, de modo que cambie la contraseña de la base de datos y actualice el secreto en Parameter Store. Actualizar cada función Lambda para que acceda a la contraseña de la base de datos desde Parameter Store.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita configurar la rotación automática de las credenciales de una base de datos de Amazon RDS. Las credenciales deben rotarse cada 30 días. La solución debe integrarse con Amazon RDS. ¿Qué solución cumple con estos requisitos con el MENOR esfuerzo operativo?

- [ ] Almacenar las credenciales en AWS Systems Manager Parameter Store como una cadena segura (secure string). Configurar la rotación automática con un intervalo de 30 días.
- [x] Almacenar las credenciales en AWS Secrets Manager. Configurar la rotación automática con un intervalo de 30 días.
- [ ] Almacenar las credenciales en un archivo dentro de un bucket de Amazon S3. Desplegar una función de AWS Lambda para rotar automáticamente las credenciales cada 30 días.
- [ ] Almacenar las credenciales en AWS Secrets Manager. Desplegar una función de AWS Lambda para rotar automáticamente las credenciales cada 30 días.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa almacena sus datos en un bucket de Amazon S3. La empresa necesita clasificar los datos y encontrar cualquier información personal sensible en sus archivos de S3. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una regla de AWS Config para descubrir información personal sensible en los archivos de S3 y marcarlos como no conformes.
- [ ] Crear un pipeline de inteligencia artificial/aprendizaje automático (IA/ML) activado por eventos de S3 para clasificar información personal sensible usando Amazon Recognition.
- [ ] Habilitar Amazon GuardDuty. Configurar la protección de S3 para monitorear todos los datos dentro de Amazon S3.
- [x] Habilitar Amazon Macie. Crear un trabajo de descubrimiento (discovery job) que use el identificador de datos administrado (managed data identifier).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe crear una política de IAM para un desarrollador que necesita acceso a servicios específicos de AWS. Con base en los requisitos, el ingeniero de CloudOps crea la siguiente política. ¿Qué acciones permite esta política? (Seleccione DOS.)

![Question 98](images/question98.png)

- [ ] Crear un AWS Storage Gateway.
- [ ] Crear un rol de IAM para una función de AWS Lambda.
- [ ] Eliminar una cola de Amazon Simple Queue Service (Amazon SQS).
- [x] Describir los balanceadores de carga de AWS.
- [x] Invocar una función de AWS Lambda.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps usa instancias de Amazon EC2 para alojar una aplicación. El ingeniero de CloudOps necesita otorgar permisos para que la aplicación acceda a una tabla de Amazon DynamoDB. ¿Qué solución cumple con este requisito?

- [ ] Crear claves de acceso para acceder a la tabla de DynamoDB. Asignar las claves de acceso al perfil de instancia de EC2.
- [ ] Crear un par de claves de EC2 para acceder a la tabla de DynamoDB. Asignar el par de claves al perfil de instancia de EC2.
- [ ] Crear un usuario de IAM para acceder a la tabla de DynamoDB. Asignar el usuario de IAM al perfil de instancia de EC2.
- [x] Crear un rol de IAM para acceder a la tabla de DynamoDB. Asignar el rol de IAM al perfil de instancia de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El propietario de una cuenta raíz (root) le ha dado acceso completo a su bucket de S3 a uno de los usuarios de IAM usando la `ACL` del bucket. Cuando el usuario de IAM inicia sesión en la consola de S3, ¿qué acciones puede realizar?

- [ ] Solo puede ver el contenido del bucket.
- [ ] Puede realizar todas las operaciones en el bucket.
- [x] No es posible otorgar acceso a un usuario de IAM usando una `ACL`.
- [ ] El usuario de IAM puede realizar todas las operaciones en el bucket únicamente mediante API/SDK.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un bucket de Amazon S3 en la cuenta de un ingeniero de CloudOps puede ser accedido por usuarios de otras cuentas de AWS. ¿Cómo puede el ingeniero asegurarse de que el bucket sea accesible únicamente para los miembros de su propia cuenta de AWS?

- [ ] Mover el bucket de S3 de una subred pública a una subred privada en la `VPC` de Amazon.
- [x] Cambiar la Lista de Control de Acceso (`ACL`) del bucket para restringir el acceso únicamente al propietario del bucket.
- [ ] Habilitar el cifrado del lado del servidor para todos los objetos del bucket.
- [ ] Usar únicamente URLs prefirmadas de Amazon S3 para acceder a los objetos del bucket.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está ayudando a un equipo de desarrollo a desplegar una aplicación en AWS. La plantilla de AWS CloudFormation incluye una instancia de EC2 con Amazon Linux, un clúster de base de datos de Amazon Aurora y una contraseña de base de datos embebida (hard-coded) que debe rotarse cada 90 días. ¿Cuál es la forma MÁS segura de administrar la contraseña de la base de datos?

- [x] Usar el recurso Secret de AWS Secrets Manager con la propiedad `GenerateSecretString` para generar automáticamente una contraseña. Usar el recurso `RotationSchedule` de AWS Secrets Manager para definir un cronograma de rotación de la contraseña. Configurar la aplicación para que recupere el secreto desde AWS Secrets Manager al acceder a la base de datos.
- [ ] Usar el recurso Secret de AWS Secrets Manager con la propiedad `SecretString`. Aceptar una contraseña como parámetro de `CloudFormation`. Usar la propiedad `AllowedPattern` del parámetro de `CloudFormation` para exigir una longitud mínima, letras mayúsculas y minúsculas y caracteres especiales. Configurar la aplicación para que recupere el secreto desde AWS Secrets Manager al acceder a la base de datos.
- [ ] Usar el recurso `AWS::SSM::Parameter`. Aceptar la entrada como parámetro de `CloudFormation` para almacenar el parámetro como una cadena segura (secure string). Configurar la aplicación para que recupere el parámetro desde AWS Systems Manager Parameter Store al acceder a la base de datos.
- [ ] Usar el recurso `AWS::SSM::Parameter`. Aceptar la entrada como parámetro de `CloudFormation` para almacenar el parámetro como una cadena (string). Configurar la aplicación para que recupere el parámetro desde AWS Systems Manager Parameter Store al acceder a la base de datos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El ingeniero de CloudOps de una empresa ha creado una instancia de Amazon EC2 con software personalizado que se usará como plantilla para todas las nuevas instancias de EC2 en múltiples cuentas de AWS. Los volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos a la instancia de EC2 están cifrados con claves administradas por AWS. El ingeniero de CloudOps crea una Amazon Machine Image (AMI) de la instancia de EC2 personalizada y planea compartir la AMI con las demás cuentas de AWS de la empresa. La empresa exige que todas las AMIs estén cifradas con claves de AWS Key Management Service (AWS KMS) y que solo las cuentas de AWS autorizadas puedan acceder a las AMIs compartidas. ¿Qué solución compartirá la AMI de forma segura con las demás cuentas de AWS?

- [ ] En la cuenta donde se creó la AMI, crear una clave de KMS administrada por el cliente. Modificar la política de la clave para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Modificar los permisos de la AMI para especificar los números de cuenta de AWS con los que se compartirá.
- [x] En la cuenta donde se creó la AMI, crear una clave de KMS administrada por el cliente. Modificar la política de la clave para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Crear una copia de la AMI y especificar la clave de KMS. Modificar los permisos de la AMI copiada para especificar los números de cuenta de AWS con los que se compartirá.
- [ ] En la cuenta donde se creó la AMI, crear una clave de KMS administrada por el cliente. Modificar la política de la clave para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Crear una copia de la AMI y especificar la clave de KMS. Modificar los permisos de la AMI copiada para hacerla pública.
- [ ] En la cuenta donde se creó la AMI, modificar la política de la clave administrada por AWS para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Modificar los permisos de la AMI para especificar los números de cuenta de AWS con los que se compartirá.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa monitorea la actividad de su cuenta usando AWS CloudTrail, y le preocupa que algunos archivos de registro estén siendo alterados después de que los registros se entregan al bucket de Amazon S3 de la cuenta. De ahora en adelante, ¿cómo puede el ingeniero de CloudOps confirmar que los archivos de registro no han sido modificados después de ser entregados al bucket de S3?

- [ ] Transmitir los registros de CloudTrail a Amazon CloudWatch Logs para almacenar los registros en una ubicación secundaria.
- [x] Habilitar la validación de integridad de archivos de registro y usar archivos resumen (digest files) para verificar el valor hash del archivo de registro.
- [ ] Replicar el bucket de registros de S3 entre regiones y cifrar los archivos de registro con claves administradas por S3.
- [ ] Habilitar el registro de acceso al servidor de S3 (S3 server access logging) para rastrear las solicitudes realizadas al bucket de registros para auditorías de seguridad.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un equipo de ingenieros de guardia (on-call) necesita conectarse frecuentemente a instancias de Amazon EC2 en una subred privada para solucionar problemas y ejecutar comandos. Las instancias usan las últimas Amazon Machine Images (AMIs) de Windows o Amazon Linux proporcionadas por AWS. El equipo tiene un rol de IAM existente para autorización. Un ingeniero de CloudOps debe proporcionar al equipo acceso a las instancias otorgando permisos de IAM a este rol. ¿Qué solución cumple con este requisito?

- [x] Agregar una declaración a la política del rol de IAM para permitir la acción `ssm:StartSession` en las instancias. Indicar al equipo que use AWS Systems Manager Session Manager para conectarse a las instancias usando el rol de IAM asumido.
- [ ] Asociar una dirección IP elástica y un grupo de seguridad a cada instancia. Agregar las direcciones IP de los ingenieros a las reglas de entrada del grupo de seguridad. Agregar una declaración a la política del rol de IAM para permitir la acción `ec2:AuthorizeSecurityGroupIngress`, de modo que el equipo pueda conectarse a las instancias.
- [ ] Crear un host bastión con una instancia de EC2 y asociar el host bastión con la `VPC`. Agregar una declaración a la política del rol de IAM para permitir la acción `ec2:CreateVpnConnection` en el host bastión. Indicar al equipo que use el endpoint del host bastión para conectarse a las instancias.
- [ ] Crear un Network Load Balancer orientado a internet. Usar dos listeners. Reenviar el puerto `22` a un grupo de destino de instancias Linux. Reenviar el puerto `3389` a un grupo de destino de instancias Windows. Agregar una declaración a la política del rol de IAM para permitir la acción `ec2:CreateRoute`, de modo que el equipo pueda conectarse a las instancias.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una plantilla de AWS CloudFormation que crea un bucket de Amazon S3. Un usuario se autentica en la cuenta corporativa de AWS con sus credenciales de Active Directory e intenta desplegar la plantilla de CloudFormation. Sin embargo, la creación del stack falla. ¿Qué factores podrían causar este fallo? (Seleccione DOS.)

- [x] La política de IAM del usuario no permite la acción `cloudformation:CreateStack`.
- [ ] La política de IAM del usuario no permite la acción `cloudformation:CreateStackSet`.
- [x] La política de IAM del usuario no permite la acción `s3:CreateBucket`.
- [ ] La política de IAM del usuario deniega explícitamente la acción `s3:ListBucket`.
- [ ] La política de IAM del usuario deniega explícitamente la acción `s3:PutObject`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene un nuevo requisito que establece que todos los recursos en AWS deben etiquetarse según una política definida. ¿Qué servicio de AWS se debe usar para hacer cumplir e identificar continuamente todos los recursos que no cumplan con la política?

- [ ] AWS CloudTrail.
- [ ] Amazon Inspector.
- [x] AWS Config.
- [ ] AWS Systems Manager.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha desplegado AWS Security Hub y AWS Config en una organización recién implementada en AWS Organizations. Un ingeniero de CloudOps debe implementar una solución para restringir que todas las cuentas miembro de la organización desplieguen recursos de Amazon EC2 en la región `ap-southeast-2`. La solución debe implementarse desde un único punto y debe gobernar tanto las cuentas actuales como las futuras. El uso de credenciales raíz (root) también debe restringirse en las cuentas miembro. ¿Qué función de AWS debe usar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Agregador de AWS Config.
- [ ] Límites de permisos de usuario de IAM (permissions boundaries).
- [x] Políticas de Control de Servicio (SCP) de AWS Organizations.
- [ ] Paquetes de conformidad (conformance packs) de AWS Security Hub.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una solución existente y ya desplegada usa instancias de Amazon EC2 con volúmenes de Amazon EBS General Purpose SSD, una base de datos de Amazon RDS PostgreSQL, un sistema de archivos de Amazon EFS y objetos estáticos almacenados en un bucket de Amazon S3. El equipo de seguridad ahora exige que se active el cifrado en reposo (at-rest) de inmediato para todos los aspectos de la aplicación, sin crear nuevos recursos y sin tiempo de inactividad. Para cumplir con los requisitos, ¿en cuál de estos servicios puede el ingeniero de CloudOps habilitar el cifrado en reposo?

- [ ] Volúmenes de EBS General Purpose SSD.
- [ ] Base de datos RDS PostgreSQL.
- [ ] Sistemas de archivos de Amazon EFS.
- [x] Objetos de S3 dentro de un bucket.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una organización creó un volumen de Amazon Elastic File System (Amazon EFS) con un ID de sistema de archivos fs-85ba41fc, y es usado activamente por 10 hosts de Amazon EC2. A la organización le preocupa que el sistema de archivos no esté cifrado. ¿Cómo se puede resolver esto?

- [ ] Habilitar el cifrado en la conexión de cada host al volumen de Amazon EFS. Cada conexión debe recrearse para que el cifrado surta efecto.
- [ ] Habilitar el cifrado en el volumen de EFS existente usando la interfaz de línea de comandos de AWS.
- [ ] Habilitar el cifrado en el disco local de cada host. Reiniciar cada host para cifrar el disco.
- [x] Habilitar el cifrado en un volumen recién creado y copiar todos los datos del volumen original. Reconectar cada host al nuevo volumen.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una organización con un departamento de TI grande ha decidido migrar a AWS. Con diferentes funciones de trabajo en el departamento de TI, no es deseable dar a todos los usuarios acceso a todos los recursos de AWS. Actualmente, la organización maneja el acceso mediante membresía a grupos de LDAP. ¿Cuál es el MEJOR método para permitir el acceso usando las credenciales de LDAP actuales?

- [ ] Crear un AWS Directory Service Simple AD. Replicar el directorio LDAP on-premises hacia Simple AD.
- [ ] Crear una función Lambda para leer los grupos de LDAP y automatizar la creación de usuarios de IAM.
- [ ] Usar AWS CloudFormation para crear roles de IAM. Desplegar Direct Connect para permitir el acceso al servidor LDAP on-premises.
- [x] Federar el directorio LDAP con IAM usando SAML. Crear diferentes roles de IAM que correspondan a los diferentes grupos de LDAP para limitar los permisos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está usando una Clave Maestra del Cliente (CMK) de AWS KMS con material de clave importado. La empresa referencia la CMK por su alias en la aplicación Java para cifrar datos. La CMK debe rotarse cada 6 meses. ¿Cuál es el proceso para rotar la clave?

- [ ] Habilitar la rotación automática de claves para la CMK y especificar un período de 6 meses.
- [x] Crear una nueva CMK con nuevo material importado, y actualizar el alias de la clave para que apunte a la nueva CMK.
- [ ] Eliminar el material de clave actual e importar nuevo material en la CMK existente.
- [ ] Importar una copia del material de clave existente en una nueva CMK como respaldo, y establecer el cronograma de rotación en 6 meses.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está construyendo un proceso para compartir instantáneas de bases de datos de Amazon RDS entre diferentes cuentas asociadas con distintas unidades de negocio dentro de la misma empresa. Todos los datos deben estar cifrados en reposo. ¿Cómo debe implementar el ingeniero este proceso?

- [ ] Escribir un script para descargar la instantánea cifrada, descifrarla usando la clave de cifrado de AWS KMS usada para cifrar la instantánea, y luego crear un nuevo volumen en cada cuenta.
- [x] Actualizar la política de la clave para otorgar permiso sobre la clave de cifrado de AWS KMS usada para cifrar la instantánea a todas las cuentas relevantes, y luego compartir la instantánea con esas cuentas.
- [ ] Crear una instancia de Amazon EC2 basada en la instantánea, luego guardar el volumen de Amazon EBS de la instancia como una instantánea y compartirla con las otras cuentas. Exigir que cada propietario de cuenta cree un nuevo volumen a partir de esa instantánea y lo cifre.
- [ ] Crear una nueva instancia de RDS sin cifrar a partir de la instantánea cifrada, conectarse a la instancia mediante `SSH`/`RDP`, exportar el contenido de la base de datos a un archivo, y luego compartir este archivo con las otras cuentas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja una aplicación interna en instancias de Amazon EC2. Todos los datos y solicitudes de la aplicación se enrutan a través de una conexión AWS Site-to-Site `VPN` entre la red on-premises y AWS. La empresa debe monitorear la aplicación en busca de cambios que permitan acceso de red fuera de la red corporativa. Cualquier cambio que exponga la aplicación externamente debe restringirse automáticamente. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear una función de AWS Lambda que actualice los grupos de seguridad asociados a la interfaz de red elástica para eliminar reglas de entrada con rangos `CIDR` no corporativos. Activar los `VPC` Flow Logs y enviar los registros a Amazon CloudWatch Logs. Crear una alarma de Amazon CloudWatch que coincida con tráfico de rangos `CIDR` no corporativos y publique un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) con la función Lambda como destino.
- [ ] Crear una regla programada de Amazon EventBridge (Amazon CloudWatch Events) que apunte a un documento de Automation de AWS Systems Manager para verificar direcciones IP públicas en las instancias de EC2. Si se encuentran direcciones IP públicas en las instancias de EC2, iniciar otro documento de Automation de Systems Manager para terminar las instancias.
- [x] Configurar AWS Config y una regla personalizada para monitorear si un grupo de seguridad permite solicitudes de entrada desde rangos `CIDR` no corporativos. Crear un documento de Automation de AWS Systems Manager para eliminar cualquier rango `CIDR` no corporativo de los grupos de seguridad de la aplicación.
- [ ] Configurar AWS Config y la regla administrada para monitorear asociaciones de IP públicas con las instancias de EC2 por etiqueta. Etiquetar las instancias de EC2 con un identificador. Crear un documento de Automation de AWS Systems Manager para eliminar la asociación de IP pública de las instancias de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta miles de instancias de Amazon EC2 basadas en la Amazon Machine Image (AMI) de Amazon Linux 2. Un ingeniero de CloudOps debe implementar una solución para registrar comandos y salida de cualquier usuario que necesite una sesión interactiva en una de las instancias de EC2. La solución debe registrar los datos en una ubicación de almacenamiento duradero. La solución también debe proporcionar notificaciones y alarmas automatizadas basadas en los datos de registro. ¿Qué solución cumple con estos requisitos con la MAYOR eficiencia operativa?

- [ ] Configurar el registro de sesiones de comandos en cada instancia de EC2. Configurar el agente unificado de Amazon CloudWatch para enviar registros de sesión a Amazon CloudWatch Logs. Configurar filtros de consulta y alertas usando Amazon Athena.
- [ ] Exigir que todos los usuarios usen un host bastión centralizado cuando necesiten acceso de línea de comandos a una instancia de EC2. Configurar el agente unificado de Amazon CloudWatch en el host bastión para enviar registros de sesión a Amazon CloudWatch Logs. Configurar un filtro de métricas y una alarma de métricas para hallazgos de seguridad relevantes en CloudWatch Logs.
- [x] Exigir que todos los usuarios usen AWS Systems Manager Session Manager cuando necesiten acceso de línea de comandos a una instancia de EC2. Configurar Session Manager para transmitir registros de sesión a Amazon CloudWatch Logs. Configurar un filtro de métricas y una alarma de métricas para hallazgos de seguridad relevantes en CloudWatch Logs.
- [ ] Configurar el registro de sesiones de comandos en cada instancia de EC2. Exigir que todos los usuarios usen documentos de AWS Systems Manager Run Command cuando necesiten acceso de línea de comandos a una instancia de EC2. Configurar el agente unificado de Amazon CloudWatch para enviar registros de sesión a Amazon CloudWatch Logs. Configurar alarmas de CloudWatch basadas en resultados de consultas de Amazon Athena.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Los usuarios de la cuenta de AWS de una empresa están lanzando instancias de Amazon EC2 sin las etiquetas de asignación de costos requeridas. Un ingeniero de CloudOps necesita evitar que los usuarios dentro de una organización en AWS Organizations lancen nuevas instancias de EC2 que no tengan las etiquetas requeridas. La solución debe requerir el menor esfuerzo operativo posible. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar una función de AWS Lambda que inicie un evento de ejecución de instancia y verifique las etiquetas requeridas. Configurar la función para evitar el lanzamiento de instancias de EC2 si faltan las etiquetas.
- [ ] Configurar una regla de AWS Config para monitorear instancias de EC2 que carezcan de las etiquetas requeridas.
- [x] Configurar una Política de Control de Servicio (SCP) que evite el lanzamiento de instancias de EC2 que carezcan de las etiquetas requeridas. Adjuntar la SCP a la raíz de la organización.
- [ ] Configurar una alarma de Amazon CloudWatch para detener cualquier instancia de EC2 que carezca de las etiquetas requeridas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está cargando archivos importantes como objetos a Amazon S3. La empresa necesita ser informada si un objeto se corrompe durante la carga. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Pasar el valor `Content-Disposition` como cuerpo de la solicitud durante la carga del objeto.
- [x] Pasar el valor `Content-MD5` como encabezado de la solicitud durante la carga del objeto.
- [ ] Pasar `x-amz-object-lock-mode` como encabezado de la solicitud durante la carga del objeto.
- [ ] Pasar `x-amz-server-side-encryption-customer-algorithm` como cuerpo de la solicitud durante la carga del objeto.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe configurar Amazon S3 para alojar una página web simple de no producción. El ingeniero de CloudOps ha creado un bucket de S3 vacío desde la consola de administración de AWS. El bucket de S3 tiene la configuración predeterminada. ¿Qué combinación de acciones debe tomar el ingeniero de CloudOps para completar este proceso? (Elija dos.)

- [ ] Configurar el bucket de S3 usando la funcionalidad `Redirect requests for an object` para apuntar a la URL raíz del bucket.
- [ ] Desactivar la configuración `Block all public access`. Permitir acceso público usando una `ACL` de bucket que contenga `<Permission>WEBSITE</Permission>`.
- [ ] Desactivar la configuración `Block all public access`. Permitir acceso público usando una `ACL` de bucket que permita acceso al grantee AuthenticatedUsers.
- [x] Desactivar la configuración `Block all public access`. Configurar una política de bucket que permita la acción `s3:GetObject` para `Principal:` `*`.
- [x] Crear un documento `index.html`. Configurar el alojamiento de sitio web estático y subir el documento index al bucket de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa AWS Organizations para administrar múltiples cuentas de AWS. La política corporativa exige que solo se puedan usar regiones específicas de AWS para almacenar y procesar datos de clientes. Un ingeniero de CloudOps debe evitar el aprovisionamiento de instancias de Amazon EC2 en regiones no autorizadas por parte de cualquier persona en la empresa. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Configurar AWS CloudTrail en todas las regiones para registrar toda la actividad de la API. Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) en todas las regiones no autorizadas para eventos `ec2:RunInstances`. Usar AWS Lambda para terminar las instancias de EC2 lanzadas.
- [ ] En cada cuenta de AWS, crear una política administrada de IAM que use una condición de región para denegar la acción `ec2:RunInstances` en todas las regiones no autorizadas. Adjuntar esta política a todos los grupos de IAM en cada cuenta de AWS.
- [ ] En cada cuenta de AWS, crear una política de límite de permisos (permissions boundary) de IAM que use una condición `Region` para denegar la acción `ec2:RunInstances` en todas las regiones no autorizadas. Adjuntar la política de límite de permisos a todos los usuarios de IAM en cada cuenta de AWS.
- [x] Crear una Política de Control de Servicio (SCP) en AWS Organizations para denegar la acción `ec2:RunInstances` en todas las regiones no autorizadas. Adjuntar esta política al nivel raíz de la organización.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene un bucket privado de Amazon S3 que contiene información confidencial. Un ingeniero de CloudOps necesita mantener registros de las direcciones IP de los fallos de autenticación resultantes de intentos de acceder a objetos en el bucket. Los registros deben almacenarse de manera que no puedan sobrescribirse ni eliminarse durante 90 días. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un trail de AWS CloudTrail. Configurar los archivos de registro para que se guarden en Amazon CloudWatch Logs. Configurar el grupo de registro con un período de retención de 90 días.
- [ ] Crear un trail de AWS CloudTrail. Configurar los archivos de registro para que se guarden en un bucket de S3 diferente. Activar la validación de integridad de archivos de registro de CloudTrail durante 90 días.
- [ ] Activar el registro de acceso (access logging) para el bucket de S3. Configurar los registros de acceso para que se guarden en Amazon CloudWatch Logs. Configurar el grupo de registro con un período de retención de 90 días.
- [x] Activar el registro de acceso (access logging) para el bucket de S3. Configurar los registros de acceso para que se guarden en un segundo bucket de S3. Activar S3 Object Lock en el segundo bucket de S3, y configurar un período de retención predeterminado de 90 días.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un equipo de cumplimiento normativo requiere que todas las contraseñas de administrador de las instancias de base de datos de Amazon RDS se cambien al menos una vez al año. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?

- [x] Almacenar las credenciales de la base de datos en AWS Secrets Manager. Configurar la rotación automática del secreto cada 365 días.
- [ ] Almacenar las credenciales de la base de datos como un parámetro en el grupo de parámetros de RDS. Crear un disparador (trigger) de base de datos para rotar la contraseña cada 365 días.
- [ ] Almacenar las credenciales de la base de datos en un bucket privado de Amazon S3. Programar una función de AWS Lambda para generar un nuevo conjunto de credenciales cada 365 días.
- [ ] Almacenar las credenciales de la base de datos en AWS Systems Manager Parameter Store como un parámetro de tipo secure string. Configurar la rotación automática del parámetro cada 365 días.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa una distribución de Amazon CloudFront para entregar su sitio web. Los registros de tráfico del sitio web deben almacenarse de forma centralizada, y todos los datos deben estar cifrados en reposo. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) con acceso a internet y cifrado del lado del servidor que use la Customer Master Key (CMK) administrada por AWS predeterminada. Configurar CloudFront para usar el dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) como destino de registros.
- [ ] Crear un dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) con acceso `VPC` y cifrado del lado del servidor que use `AES-256`. Configurar CloudFront para usar el dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) como destino de registros.
- [x] Crear un bucket de Amazon S3 configurado con cifrado del lado del servidor predeterminado que use `AES-256`. Configurar CloudFront para usar el bucket de S3 como destino de registros.
- [ ] Crear un bucket de Amazon S3 configurado sin cifrado predeterminado. Habilitar el cifrado en la distribución de CloudFront, y usar el bucket de S3 como destino de registros.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta un sitio web minorista en múltiples instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa debe asegurar el tráfico hacia el sitio web mediante una conexión `HTTPS`. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Adjuntar el certificado a cada instancia de EC2.
- [x] Adjuntar el certificado al `ALB`.
- [ ] Crear un certificado privado en AWS Certificate Manager (ACM).
- [x] Crear un certificado público en AWS Certificate Manager (ACM).
- [ ] Exportar el certificado y adjuntarlo al sitio web.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps administra políticas para muchas cuentas miembro de AWS en una estructura de AWS Organizations. Ingenieros de otros equipos tienen acceso a las credenciales de usuario raíz de las cuentas miembro. El ingeniero de CloudOps debe impedir que todos los equipos, incluyendo sus administradores, usen Amazon DynamoDB. La solución no debe afectar la capacidad de los equipos para acceder a otros servicios de AWS. ¿Qué solución cumple con estos requisitos?

- [ ] En todas las cuentas miembro, configurar políticas de IAM que denieguen el acceso a todos los recursos de DynamoDB para todos los usuarios, incluyendo el usuario raíz.
- [x] Crear una Política de Control de Servicio (SCP) en la cuenta de administración para denegar todas las acciones de DynamoDB. Aplicar la SCP a la raíz de la organización.
- [ ] En todas las cuentas miembro, configurar políticas de IAM que denieguen `AmazonDynamoDBFullAccess` a todos los usuarios, incluyendo el usuario raíz.
- [ ] Eliminar la Política de Control de Servicio (SCP) predeterminada en la cuenta de administración. Crear una SCP de reemplazo que incluya una única declaración que deniegue todas las acciones de DynamoDB.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa quiere crear una solución automatizada para todas las cuentas administradas por AWS Organizations que detecte cualquier grupo de seguridad que use `0.0.0.0/0` como dirección de origen para tráfico entrante. La empresa también quiere remediar automáticamente cualquier grupo de seguridad no conforme restringiendo el acceso a un bloque `CIDR` específico que corresponda con la intranet de la empresa. ¿Qué conjunto de acciones debe tomar el ingeniero de CloudOps para crear una solución?

- [x] Crear una regla de AWS Config para detectar grupos de seguridad no conformes. Configurar la remediación automática para cambiar la dirección de origen `0.0.0.0/0` al bloque `CIDR` aprobado.
- [ ] Crear una política de IAM para denegar la creación de grupos de seguridad que tengan `0.0.0.0/0` como dirección de origen. Adjuntar esta política de IAM a todos los usuarios de la empresa.
- [ ] Crear una función de AWS Lambda para inspeccionar grupos de seguridad nuevos y existentes. Verificar una dirección de origen `0.0.0.0/0` no conforme y cambiar la dirección de origen al bloque `CIDR` aprobado.
- [ ] Crear una Política de Control de Servicio (SCP) para la unidad organizacional (OU) que deniegue la creación de grupos de seguridad que tengan la dirección de origen `0.0.0.0/0`. Configurar la remediación automática para cambiar la dirección de origen `0.0.0.0/0` al bloque `CIDR` aprobado.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa requiere que toda la actividad en su cuenta de AWS se registre usando AWS CloudTrail. Además, un ingeniero de CloudOps debe saber cuándo se modifican o eliminan los archivos de registro de CloudTrail. ¿Cómo debe el ingeniero de CloudOps cumplir con estos requisitos?

- [x] Habilitar la validación de integridad de archivos de registro. Usar la AWS CLI para validar los archivos de registro.
- [ ] Habilitar la validación de integridad de archivos de registro. Usar la AWS CloudTrail Processing Library para validar los archivos de registro.
- [ ] Usar CloudTrail Insights para monitorear los archivos de registro en busca de modificaciones.
- [ ] Usar Amazon CloudWatch Logs para monitorear los archivos de registro en busca de modificaciones.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación que aloja datos críticos para varios clientes. La empresa usa AWS CloudTrail para rastrear las actividades de los usuarios en varios recursos de AWS. Para cumplir con nuevos requisitos de seguridad, la empresa necesita proteger los archivos de registro de CloudTrail contra modificación, eliminación o falsificación. ¿Qué solución cumple con este requisito?

- [x] Habilitar la validación de integridad de archivos de registro de CloudTrail.
- [ ] Usar `MFA Delete` de Amazon S3 en el bucket de S3 donde se almacenan los archivos de registro de CloudTrail.
- [ ] Usar el versionado de Amazon S3 para conservar todas las versiones de los archivos de registro de CloudTrail.
- [ ] Usar claves de seguridad de AWS Key Management Service (AWS KMS) para asegurar los archivos de registro de CloudTrail.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps mantiene la seguridad y el cumplimiento normativo de la cuenta de AWS de una empresa. Para asegurar que las instancias de Amazon EC2 de la empresa sigan la política de la empresa, un ingeniero de CloudOps quiere terminar cualquier instancia de EC2 que no contenga una etiqueta de departamento. Los recursos no conformes deben terminarse casi en tiempo real. ¿Qué solución cumple con estos requisitos?

- [x] Crear una regla de AWS Config con la regla administrada `required-tags` para identificar recursos no conformes. Configurar la remediación automática para ejecutar el documento de automatización `TerminateEC2Instance` de AWS para terminar los recursos no conformes.
- [ ] Crear una nueva regla de Amazon EventBridge (Amazon CloudWatch Events) para monitorear cuándo se crean nuevas instancias de EC2. Enviar el evento a un tema de Simple Notification Service (Amazon SNS) para remediación automática.
- [ ] Asegurarse de que todos los usuarios que pueden crear instancias de EC2 también tengan los permisos para usar las acciones `ec2:CreateTags` y `ec2:DescribeTags`. Cambiar el comportamiento de apagado (shutdown behavior) de la instancia a terminate.
- [ ] Asegurarse de que AWS Systems Manager Compliance esté configurado para administrar las instancias de EC2. Llamar al documento de automatización AWS-StopEC2Instances para detener los recursos no conformes.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa quiere prohibir que sus desarrolladores usen una familia particular de instancias de Amazon EC2. La empresa usa AWS Organizations y quiere aplicar la restricción en múltiples cuentas. ¿Cuál es la forma MÁS eficiente operativamente para que la empresa aplique Políticas de Control de Servicio (SCP) y cumpla con estos requisitos?

- [x] Agregar las cuentas a una unidad organizacional (OU). Aplicar las SCP a la OU.
- [ ] Agregar las cuentas a grupos de recursos en AWS Resource Groups. Aplicar las SCP a los grupos de recursos.
- [ ] Aplicar las SCP a cada cuenta de desarrollador.
- [ ] Inscribir las cuentas en AWS Control Tower. Aplicar las SCP a la cuenta de administración de AWS Control Tower.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps quiere proporcionar acceso a servicios de AWS adjuntando una política de IAM a múltiples usuarios de IAM. El ingeniero de CloudOps también quiere poder cambiar la política y crear nuevas versiones. ¿Qué combinación de acciones cumple con estos requisitos? (Elija dos.)

- [ ] Agregar los usuarios a un rol vinculado a servicio (service-linked role) de IAM. Adjuntar la política al rol.
- [x] Agregar los usuarios a un grupo de usuarios de IAM. Adjuntar la política al grupo.
- [ ] Crear una política administrada por AWS.
- [x] Crear una política administrada por el cliente (customer managed policy).
- [ ] Crear una política en línea (inline policy).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa almacena datos críticos en buckets de Amazon S3. Un ingeniero de CloudOps debe construir una solución para registrar toda la actividad de la API de S3. ¿Qué acción cumplirá con este requisito?

- [ ] Configurar métricas del bucket de S3 para registrar los registros de acceso a objetos.
- [x] Crear un trail de AWS CloudTrail para registrar eventos de datos para todos los objetos de S3.
- [ ] Habilitar el registro de acceso del servidor (server access logging) de S3 para cada bucket de S3.
- [ ] Usar AWS IAM Access Analyzer para Amazon S3 para almacenar los registros de acceso a objetos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita controlar el acceso a grupos de instancias de Amazon EC2 usando AWS Systems Manager Session Manager. Ya se han agregado etiquetas específicas a las instancias de EC2. ¿Qué acciones adicionales debe tomar el ingeniero para controlar el acceso? (Elija dos.)

- [x] Adjuntar una política de IAM a los usuarios o grupos que requieren acceso a las instancias de EC2.
- [ ] Adjuntar un rol de IAM para controlar el acceso a las instancias de EC2.
- [ ] Crear un grupo de ubicación (placement group) para las instancias de EC2 y agregar una etiqueta específica.
- [ ] Crear una cuenta de servicio y adjuntarla a las instancias de EC2 que necesitan ser controladas.
- [x] Crear una política de IAM que otorgue acceso a cualquier instancia de EC2 con una etiqueta especificada en el elemento `Condition`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una función de AWS Lambda en la Cuenta A. La función Lambda necesita leer los objetos en un bucket de Amazon S3 en la Cuenta B. Un ingeniero de CloudOps debe crear los roles de IAM correspondientes en ambas cuentas. ¿Qué solución cumple con estos requisitos?

- [x] En la Cuenta A, crear un rol de ejecución de Lambda para asumir el rol en la Cuenta B. En la Cuenta B, crear un rol que la función pueda asumir para obtener acceso al bucket de S3.
- [ ] En la Cuenta A, crear un rol de ejecución de Lambda que proporcione acceso al bucket de S3. En la Cuenta B, crear un rol que la función pueda asumir.
- [ ] En la Cuenta A, crear un rol que la función pueda asumir. En la Cuenta B, crear un rol de ejecución de Lambda que proporcione acceso al bucket de S3.
- [ ] En la Cuenta A, crear un rol que la función pueda asumir para obtener acceso al bucket de S3. En la Cuenta B, crear un rol de ejecución de Lambda para asumir el rol en la Cuenta A.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está diseñando una solución para una instancia de base de datos de Amazon RDS para PostgreSQL. Las credenciales de la base de datos deben almacenarse y rotarse mensualmente. Las aplicaciones que se conectan a la instancia de base de datos envían tráfico intensivo en escritura con conexiones de cliente variables que a veces aumentan significativamente en un corto período de tiempo. ¿Qué solución debe elegir un ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Configurar AWS Key Management Service (AWS KMS) para rotar automáticamente las claves de la instancia de base de datos. Usar RDS Proxy para manejar los aumentos en las conexiones a la base de datos.
- [ ] Configurar AWS Key Management Service (AWS KMS) para rotar automáticamente las claves de la instancia de base de datos. Usar réplicas de lectura de RDS para manejar los aumentos en las conexiones a la base de datos.
- [x] Configurar AWS Secrets Manager para rotar automáticamente las credenciales de la instancia de base de datos. Usar RDS Proxy para manejar los aumentos en las conexiones a la base de datos.
- [ ] Configurar AWS Secrets Manager para rotar automáticamente las credenciales de la instancia de base de datos. Usar réplicas de lectura de RDS para manejar los aumentos en las conexiones a la base de datos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa mantiene un gran conjunto de datos sensibles en un bucket de Amazon S3. El equipo de seguridad de la empresa le pide a un ingeniero de CloudOps que ayude a verificar que todos los objetos actuales en el bucket de S3 estén cifrados. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear un script que se ejecute contra el bucket de S3 y muestre el estado de cada objeto.
- [x] Crear una configuración de S3 Inventory en el bucket de S3. Incluir los campos de estado apropiados.
- [ ] Proporcionar al equipo de seguridad un usuario de IAM con acceso de lectura al bucket de S3.
- [ ] Usar la AWS CLI para mostrar una lista de todos los objetos en el bucket de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa realizó recientemente una auditoría de seguridad de todas sus aplicaciones internas desarrolladas internamente. Ciertas aplicaciones críticas para el negocio que manejan datos sensibles fueron marcadas porque usan clústeres de Amazon ES que están abiertos para lectura/escritura a un grupo de usuarios más amplio del previsto. ¿Quién es responsable de corregir el problema?

- [ ] AWS Premium Support.
- [ ] El equipo de Amazon ES.
- [ ] El equipo de AWS IAM.
- [x] El ingeniero de CloudOps.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación que usa un bucket de Amazon S3 para almacenamiento de objetos. Un desarrollador necesita configurar el cifrado en tránsito para el bucket de S3. Todos los objetos de S3 que contienen datos personales deben cifrarse en reposo con claves de AWS Key Management Service (AWS KMS), las cuales se pueden rotar bajo demanda. ¿Qué combinación de pasos cumple con estos requisitos? (Elija dos.)

- [ ] Escribir una política de bucket de S3 para permitir solo conexiones cifradas sobre `HTTPS` usando un límite de permisos (permissions boundary).
- [ ] Configurar una política de bucket de S3 para habilitar el cifrado del lado del cliente para los objetos que contienen datos personales usando una clave administrada por el cliente de AWS KMS.
- [x] Configurar la aplicación para cifrar los objetos usando una clave administrada por el cliente de AWS KMS antes de subir los objetos que contienen datos personales a Amazon S3.
- [x] Escribir una política de bucket de S3 para permitir solo conexiones cifradas sobre `HTTPS` usando la condición `aws:SecureTransport`.
- [ ] Configurar la configuración de S3 Block Public Access para el bucket de S3 para permitir solo conexiones cifradas sobre `HTTPS`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está usando credenciales de IAM para intentar subir un archivo al bucket de Amazon S3 de un cliente llamado `DOC-EXAMPLE-BUCKET`. El ingeniero de CloudOps está recibiendo un mensaje `AccessDenied`. ¿Qué combinación de cambios de configuración corregirá este problema? (Elija dos.)

- [x] Agregar esta política de IAM al usuario del ingeniero de CloudOps.
![Question 288 option A](images/question288_A.png)
- [x] Agregar esta política de IAM al bucket de S3 del cliente.
![Question 288 option B](images/question288_B.png)
- [ ] Agregar esta política de IAM al usuario del ingeniero de CloudOps.
![Question 288 option C](images/question288_C.png)
- [ ] Agregar esta política de IAM al usuario raíz de la cuenta del cliente.
![Question 288 option D](images/question288_D.png)
- [ ] Agregar esta política de IAM al usuario raíz de la cuenta del ingeniero de CloudOps.
![Question 288 option E](images/question288_E.png)

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha exigido el uso de autenticación multifactor (MFA) para todos los usuarios de IAM, y requiere que los usuarios hagan todas las llamadas de API usando la CLI. Sin embargo, no se les pide a los usuarios que ingresen tokens de MFA, y pueden ejecutar comandos de la CLI sin MFA. En un intento por hacer cumplir MFA, la empresa adjuntó una política de IAM a todos los usuarios que deniega las llamadas de API que no se hayan autenticado con MFA. ¿Qué paso adicional se debe tomar para asegurar que las llamadas de API se autentiquen usando MFA?

- [ ] Habilitar MFA en roles de IAM, y requerir que los usuarios de IAM usen credenciales de rol para firmar las llamadas de API.
- [ ] Pedir a los usuarios de IAM que inicien sesión en la consola de administración de AWS con MFA antes de hacer llamadas de API usando la CLI.
- [ ] Restringir a los usuarios de IAM al uso de la consola, ya que MFA no es compatible para uso de la CLI.
- [x] Requerir que los usuarios usen credenciales temporales del comando `get-session-token` para firmar las llamadas de API.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa que usa AWS Organizations requiere que ningún bucket de Amazon S3 en sus cuentas de producción sea eliminado jamás. ¿Cuál es el enfoque MÁS SIMPLE que puede tomar el ingeniero de CloudOps para asegurar que los buckets de S3 en esas cuentas nunca puedan eliminarse?

- [ ] Configurar `MFA Delete` en todos los buckets de S3 para evitar que se eliminen los buckets.
- [x] Usar Políticas de Control de Servicio para denegar la acción `s3:DeleteBucket` en todos los buckets de las cuentas de producción.
- [ ] Crear un grupo de IAM que tenga una política de IAM para denegar la acción `s3:DeleteBucket` en todos los buckets de las cuentas de producción.
- [ ] Usar AWS Shield para denegar la acción `s3:DeleteBucket` en la cuenta de AWS en lugar de en todos los buckets de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa AWS Organizations para alojar varias aplicaciones en múltiples cuentas de AWS. Varios equipos son responsables de construir y mantener la infraestructura de las aplicaciones en las cuentas de AWS. Un ingeniero de CloudOps debe implementar una solución para asegurar que las cuentas de usuario y los permisos se administren centralizadamente. La solución debe integrarse con el entorno de Active Directory local (on-premises) existente de la empresa. El ingeniero de CloudOps ya ha habilitado AWS IAM Identity Center (AWS Single Sign-On) y ha configurado una conexión de AWS Direct Connect. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear un dominio Simple AD, y establecer una relación de confianza de bosque (forest trust) con el dominio de Active Directory local. Establecer el dominio Simple AD como el origen de identidad para IAM Identity Center. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.
- [ ] Crear un controlador de dominio de Active Directory en una instancia de Amazon EC2 unida al dominio de Active Directory local. Establecer el controlador de dominio de Active Directory como el origen de identidad para IAM Identity Center. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.
- [x] Crear un AD Connector asociado con el dominio de Active Directory local. Establecer el AD Connector como el origen de identidad para IAM Identity Center. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.
- [ ] Usar el directorio SSO integrado como el origen de identidad para IAM Identity Center. Copiar los usuarios y grupos desde el dominio de Active Directory local. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Recientemente, varios archivos críticos se eliminaron por error de un bucket compartido de Amazon S3. Un ingeniero de CloudOps necesita prevenir que ocurran eliminaciones accidentales en el futuro habilitando `MFA Delete`. Una vez habilitado, ¿qué actividades del bucket requerirán autenticación MFA? (Elija dos.)

- [x] Eliminar permanentemente una versión de objeto del bucket.
- [ ] Deshabilitar el cifrado predeterminado de objetos para el bucket.
- [ ] Listar todas las versiones de objetos eliminados en el bucket.
- [x] Suspender el versionado en el bucket.
- [ ] Habilitar `MFA Add` en el bucket.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene varias cuentas miembro que forman parte de una organización en AWS Organizations. La empresa descubrió recientemente que los administradores han estado usando credenciales de usuario raíz de la cuenta. La empresa debe evitar que los ingenieros usen credenciales de usuario raíz para realizar cualquier acción en instancias de Amazon EC2. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Crear una política de IAM basada en identidad en cada cuenta miembro para denegar acciones en instancias de EC2 por parte del usuario raíz.
- [x] En la cuenta de administración de la organización, crear una Política de Control de Servicio (SCP) para denegar acciones en instancias de EC2 por parte del usuario raíz en todas las cuentas miembro.
- [ ] Usar AWS Config para prevenir cualquier acción en instancias de EC2 por parte del usuario raíz.
- [ ] Usar Amazon Inspector en cada cuenta miembro para escanear inicios de sesión de usuario raíz y prevenir cualquier acción en instancias de EC2 por parte del usuario raíz.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa crea una nueva cuenta miembro usando AWS Organizations. Un ingeniero de CloudOps necesita agregar AWS Business Support a la nueva cuenta. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con este requisito? (Elija dos.)

- [x] Iniciar sesión en la nueva cuenta usando credenciales de IAM. Cambiar el plan de soporte.
- [ ] Iniciar sesión en la nueva cuenta usando credenciales de usuario raíz. Cambiar el plan de soporte.
- [ ] Usar la API de AWS Support para cambiar el plan de soporte.
- [ ] Restablecer la contraseña del usuario raíz de la cuenta.
- [x] Crear un usuario de IAM que tenga privilegios de administrador en la nueva cuenta.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps es responsable de la seguridad de la cuenta de AWS de una empresa. La empresa tiene una política según la cual un usuario solo puede detener o terminar instancias de Amazon EC2 cuando el usuario está autenticado usando un dispositivo de autenticación multifactor (MFA). ¿Qué política debe aplicar el ingeniero de CloudOps para cumplir con este requisito?

- [x] Opción A.
![Question 331 option A](images/question331_A.png)
- [ ] Opción B.
![Question 331 option B](images/question331_B.png)
- [ ] Opción C.
![Question 331 option C](images/question331_C.png)
- [ ] Opción D.
![Question 331 option D](images/question331_D.png)

**[⬆ Volver arriba](#tabla-de-contenidos)**

### La aplicación de una empresa actualmente usa un rol de IAM que permite acceso total a todos los servicios de AWS. Un ingeniero de CloudOps debe asegurarse de que las políticas de IAM de la empresa permitan solo los permisos que la aplicación requiere. ¿Cómo puede el ingeniero de CloudOps crear una política que cumpla con este requisito?

- [ ] Activar AWS CloudTrail. Generar una política usando AWS Security Hub.
- [ ] Activar Amazon EventBridge (Amazon CloudWatch Events). Generar una política usando AWS Identity and Access Management Access Analyzer.
- [ ] Usar la AWS CLI para ejecutar el comando `get-generated-policy` en AWS Identity and Access Management Access Analyzer.
- [x] Activar AWS CloudTrail. Generar una política usando AWS Identity and Access Management Access Analyzer.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa almacena datos sensibles en un bucket de Amazon S3. La empresa debe registrar todos los intentos de acceso al bucket de S3. El equipo de riesgos de la empresa debe recibir notificación inmediata sobre cualquier evento de eliminación. ¿Qué solución cumple con estos requisitos?

- [x] Habilitar el registro de acceso del servidor (S3 server access logging) de S3 para los registros de auditoría. Configurar una notificación de Amazon Simple Notification Service (Amazon SNS) para el bucket de S3. Seleccionar `DeleteObject` como el tipo de evento para el sistema de alertas.
- [ ] Habilitar el registro de acceso del servidor de S3 para los registros de auditoría. Lanzar una instancia de Amazon EC2 para el sistema de alertas. Ejecutar un cron job en la instancia de EC2 para descargar los registros de acceso cada día y buscar un evento `DeleteObject`.
- [ ] Usar Amazon CloudWatch Logs para los registros de auditoría. Usar alarmas de Amazon CloudWatch con una notificación de Amazon Simple Notification Service (Amazon SNS) para el sistema de alertas.
- [ ] Usar Amazon CloudWatch Logs para los registros de auditoría. Lanzar una instancia de Amazon EC2 para el sistema de alertas. Ejecutar un cron job en la instancia de EC2 cada día para comparar la lista de elementos con la lista del día anterior. Configurar el cron job para enviar una notificación si falta un elemento.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está escribiendo una función de AWS Lambda en la Cuenta A de AWS para colocar objetos en un bucket de Amazon S3 en la Cuenta B de AWS. La función Lambda puede escribir exitosamente nuevos objetos en el bucket de S3, pero los usuarios de IAM en la Cuenta B no pueden eliminar objetos escritos en el bucket por la Cuenta A. ¿Qué paso corregirá este problema?

- [ ] Agregar el permiso `s3:DeleteObject` al rol de ejecución de IAM de la función de AWS Lambda en la Cuenta A.
- [ ] Cambiar la política del bucket de S3 en la Cuenta B para permitir el permiso `s3:DeleteObject` para la Cuenta A.
- [ ] Deshabilitar el cifrado del lado del servidor para los objetos escritos en el bucket de S3 por la función Lambda.
- [x] Modificar la función Lambda para llamar a la operación de API `s3:PutObjectAcl` y especificar bucket owner, full control.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### La política de seguridad de una empresa establece que no está permitido conectarse a instancias de Amazon EC2 mediante `SSH` y `RDP`. Si se requiere acceso, el personal autorizado puede conectarse a las instancias usando AWS Systems Manager Session Manager. Los usuarios reportan que no pueden conectarse a una instancia específica de Amazon EC2 que ejecuta Ubuntu y tiene preinstalado AWS Systems Manager Agent (SSM Agent). Estos usuarios pueden usar Session Manager para conectarse a otras instancias en la misma subred, y están en un grupo de IAM que tiene permiso de Session Manager para todas las instancias. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?

- [ ] Agregar una regla de entrada para el puerto `22` en el grupo de seguridad asociado con la instancia Ubuntu.
- [x] Asignar la política administrada `AmazonSSMManagedInstanceCore` al perfil de instancia de EC2 para la instancia Ubuntu.
- [ ] Configurar el SSM Agent para iniciar sesión con un nombre de usuario `ubuntu`.
- [ ] Generar un nuevo par de claves, configurar Session Manager para usar este nuevo par de claves, y proporcionar la clave privada a los usuarios.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene un bucket de Amazon S3 que contiene datos sensibles. Los datos deben cifrarse en tránsito y en reposo. La empresa cifra los datos en el bucket de S3 usando una clave de AWS Key Management Service (AWS KMS). Un desarrollador necesita otorgar a varias otras cuentas de AWS el permiso para usar la operación `GetObject` de S3 para recuperar los datos del bucket de S3. ¿Cómo puede el desarrollador exigir que todas las solicitudes para recuperar los datos proporcionen cifrado en tránsito?

- [x] Definir una política basada en recursos en el bucket de S3 para denegar el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.
- [ ] Definir una política basada en recursos en el bucket de S3 para permitir el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.
- [ ] Definir una política basada en roles en los roles de las otras cuentas para denegar el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.
- [ ] Definir una política basada en recursos en la clave KMS para denegar el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene dos cuentas de AWS: desarrollo y producción. Todas las aplicaciones envían registros a un bucket de Amazon S3 específico para cada cuenta, y los desarrolladores están solicitando acceso a los buckets de S3 de la cuenta de producción para ver los registros. ¿Cuál es la forma MÁS eficiente de proporcionar a los desarrolladores el acceso?

- [ ] Crear una función de AWS Lambda con un rol de IAM adjunto que tenga acceso a los buckets de S3 de ambas cuentas. Extraer los registros del bucket de S3 de producción al bucket de S3 de desarrollo.
- [ ] Crear usuarios de IAM para cada desarrollador en la cuenta de producción, y agregar a los desarrolladores a un grupo de IAM que proporcione acceso de solo lectura al bucket de registros de S3.
- [ ] Crear un bastion host de Amazon EC2 con un rol de IAM adjunto que tenga acceso al bucket de registros de S3 de producción, y luego aprovisionar acceso para los desarrolladores en el host.
- [x] Crear una política basada en recursos para el bucket de S3 en la cuenta de producción que otorgue acceso a la cuenta de desarrollo, y luego delegar el acceso en la cuenta de desarrollo.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una organización almacena datos sensibles de clientes en buckets de S3 protegidos por políticas de bucket. Recientemente, ha habido reportes de que entidades no autorizadas dentro de la empresa han estado intentando acceder a los datos en esos buckets de S3. El director de seguridad de la información (CISO) quisiera saber qué buckets están siendo objetivo y determinar quién es responsable de intentar acceder a esa información. ¿Qué pasos debe tomar un ingeniero de CloudOps para cumplir con el requisito del CISO? (Elija dos.)

- [ ] Habilitar Amazon S3 Analytics en todos los buckets de S3 afectados para obtener un informe de qué buckets están siendo accedidos sin autorización.
- [x] Habilitar el registro de acceso del servidor (S3 Server Access Logging) de Amazon S3 en todos los buckets de S3 afectados y hacer que los registros se almacenen en un bucket dedicado para registros.
- [ ] Usar Amazon Athena para consultar el informe de S3 Analytics en busca de errores `HTTP` `403`, y determinar el usuario o rol de IAM que hace las solicitudes.
- [x] Usar Amazon Athena para consultar los registros de acceso del servidor de S3 en busca de errores `HTTP` `403`, y determinar el usuario o rol de IAM que hace las solicitudes.
- [ ] Usar Amazon Athena para consultar los registros de acceso del servidor de S3 en busca de errores `HTTP` `503`, y determinar el usuario o rol de IAM que hace las solicitudes.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación web pública existente para `www.example.com`. El Application Load Balancer (ALB) está configurado con un único listener `HTTP` en el puerto `80`. Un ingeniero de CloudOps debe asegurarse de que todas las solicitudes web a `www.example.com` estén cifradas entre el cliente y el `ALB`. El ingeniero de CloudOps ya ha solicitado y validado un certificado público para `www.example.com` en AWS Certificate Manager (ACM). Los usuarios existentes de la aplicación no deben tener que cambiar el endpoint al que se conectan. ¿Qué conjunto adicional de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear un listener adicional del `ALB` para `HTTPS` en el puerto `443`. Establecer la acción predeterminada para reenviar todo el tráfico al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado.
- [ ] Crear un listener adicional del `ALB` para `HTTPS` en el puerto `443`. Establecer la acción predeterminada para reenviar todo el tráfico al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado. Eliminar el listener `HTTP` original en el puerto `80`.
- [ ] Modificar la regla predeterminada del `ALB` para el listener `HTTP` del puerto `80`. Crear una regla en el listener para reenviar todo el tráfico del host www.example.com al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado.
- [x] Modificar la regla predeterminada del `ALB` para el listener `HTTP` del puerto `80` para redirigir a `HTTPS` en el puerto `443`. Crear un listener adicional de `HTTPS` en el puerto `443`. Establecer la acción predeterminada para reenviar todo el tráfico al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado.

**[⬆ Volver arriba](#tabla-de-contenidos)**
