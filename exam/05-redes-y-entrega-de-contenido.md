# Dominio 5: Redes y entrega de contenido (18 %)

Preguntas de práctica AWS Certified CloudOps Engineer – Associate (SOA-C03) — 86 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [Una instancia de Amazon EC2 necesita ser accesible desde internet. La instancia de EC2 está en una subred con la siguiente tabla de enrutamiento. ¿Qué entrada debe agregar un ingeniero de CloudOps a la tabla de enrutamiento para cumplir con este requisito?](#una-instancia-de-amazon-ec2-necesita-ser-accesible-desde-internet-la-instancia-de-ec2-está-en-una-subred-con-la-siguiente-tabla-de-enrutamiento-qué-entrada-debe-agregar-un-ingeniero-de-cloudops-a-la-tabla-de-enrutamiento-para-cumplir-con-este-requisito) |
| 2 | [Un ingeniero de CloudOps lanza una instancia de Amazon EC2 en una subred privada de una `VPC`. Cuando el ingeniero de CloudOps intenta ejecutar un comando `curl` desde la línea de comandos de la instancia de EC2, no logra conectarse a `https:www.example.com`. ¿Qué debe hacer el ingeniero de CloudOps para resolver este problema?](#un-ingeniero-de-cloudops-lanza-una-instancia-de-amazon-ec2-en-una-subred-privada-de-una-vpc-cuando-el-ingeniero-de-cloudops-intenta-ejecutar-un-comando-curl-desde-la-línea-de-comandos-de-la-instancia-de-ec2-no-logra-conectarse-a-httpswwwexamplecom-qué-debe-hacer-el-ingeniero-de-cloudops-para-resolver-este-problema) |
| 3 | [Un ingeniero de CloudOps lanza una instancia de Amazon EC2 con Linux en una subred pública. Una vez que la instancia está en ejecución, el ingeniero de CloudOps obtiene la dirección IP pública e intenta conectarse remotamente a la instancia varias veces. Sin embargo, siempre recibe un error de tiempo de espera (timeout). ¿Qué acción permitirá al ingeniero de CloudOps conectarse remotamente a la instancia?](#un-ingeniero-de-cloudops-lanza-una-instancia-de-amazon-ec2-con-linux-en-una-subred-pública-una-vez-que-la-instancia-está-en-ejecución-el-ingeniero-de-cloudops-obtiene-la-dirección-ip-pública-e-intenta-conectarse-remotamente-a-la-instancia-varias-veces-sin-embargo-siempre-recibe-un-error-de-tiempo-de-espera-timeout-qué-acción-permitirá-al-ingeniero-de-cloudops-conectarse-remotamente-a-la-instancia) |
| 4 | [Una empresa quiere usar únicamente IPv6 para todas sus instancias de Amazon EC2. Las instancias de EC2 no deben ser accesibles desde internet, pero sí deben poder acceder a internet. La empresa crea una `VPC` de doble pila (dual-stack) y subredes exclusivas de IPv6. ¿Cómo debe configurar un ingeniero de CloudOps la `VPC` para cumplir con estos requisitos?](#una-empresa-quiere-usar-únicamente-ipv6-para-todas-sus-instancias-de-amazon-ec2-las-instancias-de-ec2-no-deben-ser-accesibles-desde-internet-pero-sí-deben-poder-acceder-a-internet-la-empresa-crea-una-vpc-de-doble-pila-dual-stack-y-subredes-exclusivas-de-ipv6-cómo-debe-configurar-un-ingeniero-de-cloudops-la-vpc-para-cumplir-con-estos-requisitos) |
| 5 | [Una empresa planea ejecutar una aplicación web pública en instancias de Amazon EC2 detrás de un Elastic Load Balancer (ELB). El equipo de seguridad de la empresa quiere proteger el sitio web usando certificados de AWS Certificate Manager (ACM). El ELB debe redirigir automáticamente todas las solicitudes `HTTP` a `HTTPS`. ¿Qué solución cumple con estos requisitos?](#una-empresa-planea-ejecutar-una-aplicación-web-pública-en-instancias-de-amazon-ec2-detrás-de-un-elastic-load-balancer-elb-el-equipo-de-seguridad-de-la-empresa-quiere-proteger-el-sitio-web-usando-certificados-de-aws-certificate-manager-acm-el-elb-debe-redirigir-automáticamente-todas-las-solicitudes-http-a-https-qué-solución-cumple-con-estos-requisitos) |
| 6 | [Una empresa migró recientemente su aplicación a una `VPC` en AWS. Una conexión AWS Site-to-Site `VPN` conecta la red on-premises de la empresa con la `VPC`. La aplicación obtiene datos de clientes desde otro sistema que reside on-premises. La aplicación usa un servidor `DNS` on-premises para resolver registros de dominio. Después de la migración, la aplicación no puede conectarse a los datos de clientes debido a errores de resolución de nombres. ¿Qué solución le dará a la aplicación la capacidad de resolver los nombres de dominio internos?](#una-empresa-migró-recientemente-su-aplicación-a-una-vpc-en-aws-una-conexión-aws-site-to-site-vpn-conecta-la-red-on-premises-de-la-empresa-con-la-vpc-la-aplicación-obtiene-datos-de-clientes-desde-otro-sistema-que-reside-on-premises-la-aplicación-usa-un-servidor-dns-on-premises-para-resolver-registros-de-dominio-después-de-la-migración-la-aplicación-no-puede-conectarse-a-los-datos-de-clientes-debido-a-errores-de-resolución-de-nombres-qué-solución-le-dará-a-la-aplicación-la-capacidad-de-resolver-los-nombres-de-dominio-internos) |
| 7 | [Un ingeniero de CloudOps crea una nueva `VPC` que incluye una subred pública y una subred privada. El ingeniero de CloudOps lanza con éxito 11 instancias de Amazon EC2 en la subred privada. El ingeniero de CloudOps intenta lanzar una instancia de EC2 adicional en la misma subred, pero recibe un mensaje de error que indica que no hay suficientes direcciones IP libres disponibles. ¿Qué debe hacer el ingeniero de CloudOps para desplegar más instancias de EC2?](#un-ingeniero-de-cloudops-crea-una-nueva-vpc-que-incluye-una-subred-pública-y-una-subred-privada-el-ingeniero-de-cloudops-lanza-con-éxito-11-instancias-de-amazon-ec2-en-la-subred-privada-el-ingeniero-de-cloudops-intenta-lanzar-una-instancia-de-ec2-adicional-en-la-misma-subred-pero-recibe-un-mensaje-de-error-que-indica-que-no-hay-suficientes-direcciones-ip-libres-disponibles-qué-debe-hacer-el-ingeniero-de-cloudops-para-desplegar-más-instancias-de-ec2) |
| 8 | [Un ingeniero de CloudOps está intentando descargar parches de internet hacia una instancia en una subred privada. Existe una puerta de enlace de internet para la `VPC`, y se ha desplegado una puerta de enlace `NAT` en la subred pública; sin embargo, la instancia no tiene conectividad a internet. Los recursos desplegados en la subred privada deben ser inaccesibles directamente desde internet público. Dada la información proporcionada, ¿qué se debe agregar a la tabla de enrutamiento de la subred privada para resolver este problema?](#un-ingeniero-de-cloudops-está-intentando-descargar-parches-de-internet-hacia-una-instancia-en-una-subred-privada-existe-una-puerta-de-enlace-de-internet-para-la-vpc-y-se-ha-desplegado-una-puerta-de-enlace-nat-en-la-subred-pública-sin-embargo-la-instancia-no-tiene-conectividad-a-internet-los-recursos-desplegados-en-la-subred-privada-deben-ser-inaccesibles-directamente-desde-internet-público-dada-la-información-proporcionada-qué-se-debe-agregar-a-la-tabla-de-enrutamiento-de-la-subred-privada-para-resolver-este-problema) |
| 9 | [Una empresa tiene una conexión AWS Site-to-Site `VPN` entre recursos on-premises y recursos alojados en una `VPC`. Un ingeniero de CloudOps lanza una instancia de Amazon EC2 que solo tiene una dirección IP privada en una subred privada de la `VPC`. La instancia de EC2 ejecuta Microsoft Windows Server. Un grupo de seguridad de la instancia de EC2 tiene reglas que permiten tráfico de entrada desde la red on-premises a través de la conexión `VPN`. El entorno on-premises contiene un firewall de red de un tercero. Las reglas de ese firewall permiten que el tráfico de Remote Desktop Protocol (RDP) fluya entre los usuarios on-premises a través de la conexión `VPN`. Los usuarios on-premises no pueden conectarse a la instancia de EC2 y reciben un error de tiempo de espera (timeout). ¿Qué debe hacer el ingeniero de CloudOps para solucionar este problema?](#una-empresa-tiene-una-conexión-aws-site-to-site-vpn-entre-recursos-on-premises-y-recursos-alojados-en-una-vpc-un-ingeniero-de-cloudops-lanza-una-instancia-de-amazon-ec2-que-solo-tiene-una-dirección-ip-privada-en-una-subred-privada-de-la-vpc-la-instancia-de-ec2-ejecuta-microsoft-windows-server-un-grupo-de-seguridad-de-la-instancia-de-ec2-tiene-reglas-que-permiten-tráfico-de-entrada-desde-la-red-on-premises-a-través-de-la-conexión-vpn-el-entorno-on-premises-contiene-un-firewall-de-red-de-un-tercero-las-reglas-de-ese-firewall-permiten-que-el-tráfico-de-remote-desktop-protocol-rdp-fluya-entre-los-usuarios-on-premises-a-través-de-la-conexión-vpn-los-usuarios-on-premises-no-pueden-conectarse-a-la-instancia-de-ec2-y-reciben-un-error-de-tiempo-de-espera-timeout-qué-debe-hacer-el-ingeniero-de-cloudops-para-solucionar-este-problema) |
| 10 | [Un ingeniero de CloudOps está desplegando un sitio de prueba que se ejecuta en instancias de Amazon EC2. La aplicación requiere conectividad tanto de entrada como de salida hacia internet. ¿Qué combinación de pasos se requiere para proporcionar conectividad a internet a las instancias de EC2? (Elija dos.)](#un-ingeniero-de-cloudops-está-desplegando-un-sitio-de-prueba-que-se-ejecuta-en-instancias-de-amazon-ec2-la-aplicación-requiere-conectividad-tanto-de-entrada-como-de-salida-hacia-internet-qué-combinación-de-pasos-se-requiere-para-proporcionar-conectividad-a-internet-a-las-instancias-de-ec2-elija-dos) |
| 11 | [Un ingeniero de CloudOps está investigando por qué un usuario no ha podido usar `RDP` para conectarse a través de internet desde su computadora personal a un servidor bastión que se ejecuta en una instancia de Amazon EC2 con Windows. ¿Cuáles de las siguientes son posibles causas de este problema? (Elija dos.)](#un-ingeniero-de-cloudops-está-investigando-por-qué-un-usuario-no-ha-podido-usar-rdp-para-conectarse-a-través-de-internet-desde-su-computadora-personal-a-un-servidor-bastión-que-se-ejecuta-en-una-instancia-de-amazon-ec2-con-windows-cuáles-de-las-siguientes-son-posibles-causas-de-este-problema-elija-dos) |
| 12 | [Mientras aseguraba la conexión entre la `VPC` de una empresa y su centro de datos on-premises, un ingeniero de seguridad envió un comando ping desde un host on-premises (dirección IP `203.0.113.12`) hacia una instancia de Amazon EC2 (dirección IP `172.31.16.139`). El comando ping no obtuvo respuesta. El registro de flujo (flow log) de la `VPC` mostró lo siguiente. ¿Qué acción se debe realizar para que el ping funcione?](#mientras-aseguraba-la-conexión-entre-la-vpc-de-una-empresa-y-su-centro-de-datos-on-premises-un-ingeniero-de-seguridad-envió-un-comando-ping-desde-un-host-on-premises-dirección-ip-203011312-hacia-una-instancia-de-amazon-ec2-dirección-ip-1723116139-el-comando-ping-no-obtuvo-respuesta-el-registro-de-flujo-flow-log-de-la-vpc-mostró-lo-siguiente-qué-acción-se-debe-realizar-para-que-el-ping-funcione) |
| 13 | [Una empresa global maneja una gran cantidad de información de identificación personal (PII, por sus siglas en inglés) a través de un portal web interno. La aplicación de la empresa se ejecuta en un centro de datos corporativo que está conectado a AWS mediante una conexión de AWS Direct Connect. La aplicación almacena la PII en Amazon S3. Según un requisito de cumplimiento normativo, el tráfico desde el portal web hacia Amazon S3 no debe transitar por internet. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con el requisito de cumplimiento?](#una-empresa-global-maneja-una-gran-cantidad-de-información-de-identificación-personal-pii-por-sus-siglas-en-inglés-a-través-de-un-portal-web-interno-la-aplicación-de-la-empresa-se-ejecuta-en-un-centro-de-datos-corporativo-que-está-conectado-a-aws-mediante-una-conexión-de-aws-direct-connect-la-aplicación-almacena-la-pii-en-amazon-s3-según-un-requisito-de-cumplimiento-normativo-el-tráfico-desde-el-portal-web-hacia-amazon-s3-no-debe-transitar-por-internet-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-el-requisito-de-cumplimiento) |
| 14 | [Una empresa usa Amazon Elastic Container Service (Amazon ECS) para ejecutar una aplicación en contenedores sobre instancias de Amazon EC2. Un ingeniero de CloudOps necesita monitorear únicamente los flujos de tráfico entre las tareas (tasks) de ECS. ¿Qué combinación de pasos debe seguir el ingeniero de CloudOps para cumplir con este requisito? (Seleccione DOS.)](#una-empresa-usa-amazon-elastic-container-service-amazon-ecs-para-ejecutar-una-aplicación-en-contenedores-sobre-instancias-de-amazon-ec2-un-ingeniero-de-cloudops-necesita-monitorear-únicamente-los-flujos-de-tráfico-entre-las-tareas-tasks-de-ecs-qué-combinación-de-pasos-debe-seguir-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito-seleccione-dos) |
| 15 | [Una empresa tiene una aplicación web con estado (stateful) alojada en instancias de Amazon EC2 dentro de un grupo de Auto Scaling. Las instancias se ejecutan detrás de un Application Load Balancer (ALB) que tiene un único grupo de destino. El `ALB` está configurado como origen en una distribución de Amazon CloudFront. Los usuarios reportan cierres de sesión aleatorios en la aplicación web. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para resolver este problema? (Seleccione DOS.)](#una-empresa-tiene-una-aplicación-web-con-estado-stateful-alojada-en-instancias-de-amazon-ec2-dentro-de-un-grupo-de-auto-scaling-las-instancias-se-ejecutan-detrás-de-un-application-load-balancer-alb-que-tiene-un-único-grupo-de-destino-el-alb-está-configurado-como-origen-en-una-distribución-de-amazon-cloudfront-los-usuarios-reportan-cierres-de-sesión-aleatorios-en-la-aplicación-web-qué-combinación-de-acciones-debe-tomar-un-ingeniero-de-cloudops-para-resolver-este-problema-seleccione-dos) |
| 16 | [Una `VPC` está conectada al centro de datos de una empresa mediante una `VPN`. Una instancia de Amazon EC2 con la dirección IP `172.31.16.139` está dentro de una subred privada de la `VPC`. Un ingeniero de CloudOps envió un comando ping a la instancia de EC2 desde una computadora on-premises con la dirección IP `203.0.113.12` y no recibió confirmación. Los registros de flujo (`VPC` Flow Logs) estaban habilitados y mostraron lo siguiente. ¿Qué acción resolverá el problema?](#una-vpc-está-conectada-al-centro-de-datos-de-una-empresa-mediante-una-vpn-una-instancia-de-amazon-ec2-con-la-dirección-ip-1723116139-está-dentro-de-una-subred-privada-de-la-vpc-un-ingeniero-de-cloudops-envió-un-comando-ping-a-la-instancia-de-ec2-desde-una-computadora-on-premises-con-la-dirección-ip-203011312-y-no-recibió-confirmación-los-registros-de-flujo-vpc-flow-logs-estaban-habilitados-y-mostraron-lo-siguiente-qué-acción-resolverá-el-problema) |
| 17 | [Un ingeniero de CloudOps mantiene varias instancias de Amazon EC2 que no tienen acceso a internet público. Para aplicar parches a los sistemas operativos, las instancias requieren conectividad de salida a internet. Por razones de seguridad, las instancias no deben ser accesibles desde internet público. El ingeniero despliega una instancia `NAT`, actualiza los grupos de seguridad y configura las rutas apropiadas en la tabla de enrutamiento. Sin embargo, las instancias aún no pueden llegar a internet. ¿Qué se debe hacer para resolver el problema?](#un-ingeniero-de-cloudops-mantiene-varias-instancias-de-amazon-ec2-que-no-tienen-acceso-a-internet-público-para-aplicar-parches-a-los-sistemas-operativos-las-instancias-requieren-conectividad-de-salida-a-internet-por-razones-de-seguridad-las-instancias-no-deben-ser-accesibles-desde-internet-público-el-ingeniero-despliega-una-instancia-nat-actualiza-los-grupos-de-seguridad-y-configura-las-rutas-apropiadas-en-la-tabla-de-enrutamiento-sin-embargo-las-instancias-aún-no-pueden-llegar-a-internet-qué-se-debe-hacer-para-resolver-el-problema) |
| 18 | [Una empresa necesita desplegar una aplicación web en dos instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). También se desplegarán dos instancias de EC2 para alojar la base de datos. La infraestructura debe diseñarse a través de Zonas de disponibilidad para alta disponibilidad y debe limitar el acceso público a las instancias tanto como sea posible. ¿Cómo se debe lograr esto dentro de una `VPC`?](#una-empresa-necesita-desplegar-una-aplicación-web-en-dos-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-alb-también-se-desplegarán-dos-instancias-de-ec2-para-alojar-la-base-de-datos-la-infraestructura-debe-diseñarse-a-través-de-zonas-de-disponibilidad-para-alta-disponibilidad-y-debe-limitar-el-acceso-público-a-las-instancias-tanto-como-sea-posible-cómo-se-debe-lograr-esto-dentro-de-una-vpc) |
| 19 | [Una empresa tiene una distribución de Amazon CloudFront que usa un bucket de Amazon S3 como origen. Durante una revisión de los registros de acceso, la empresa determina que algunas solicitudes van directamente al bucket de S3 usando el endpoint de alojamiento de sitio web (website hosting endpoint). Un ingeniero de CloudOps debe proteger el bucket de S3 para permitir solicitudes únicamente desde CloudFront. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-tiene-una-distribución-de-amazon-cloudfront-que-usa-un-bucket-de-amazon-s3-como-origen-durante-una-revisión-de-los-registros-de-acceso-la-empresa-determina-que-algunas-solicitudes-van-directamente-al-bucket-de-s3-usando-el-endpoint-de-alojamiento-de-sitio-web-website-hosting-endpoint-un-ingeniero-de-cloudops-debe-proteger-el-bucket-de-s3-para-permitir-solicitudes-únicamente-desde-cloudfront-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 20 | [Una empresa está intentando conectar dos aplicaciones. Una aplicación se ejecuta en un centro de datos on-premises con el nombre de host hostl.onprem.private. La otra aplicación se ejecuta en una instancia de Amazon EC2 con el nombre de host `hostl.awscloud.private`. Existe una conexión AWS Site-to-Site `VPN` entre la red on-premises y AWS. La aplicación que se ejecuta en el centro de datos intenta conectarse a la aplicación que se ejecuta en la instancia de EC2, pero la resolución `DNS` falla. Un ingeniero de CloudOps debe implementar resolución `DNS` entre los recursos on-premises y los de AWS. ¿Qué solución permite que la aplicación on-premises resuelva el nombre de host de la instancia de EC2?](#una-empresa-está-intentando-conectar-dos-aplicaciones-una-aplicación-se-ejecuta-en-un-centro-de-datos-on-premises-con-el-nombre-de-host-hostlonpremprivate-la-otra-aplicación-se-ejecuta-en-una-instancia-de-amazon-ec2-con-el-nombre-de-host-hostlawscloudprivate-existe-una-conexión-aws-site-to-site-vpn-entre-la-red-on-premises-y-aws-la-aplicación-que-se-ejecuta-en-el-centro-de-datos-intenta-conectarse-a-la-aplicación-que-se-ejecuta-en-la-instancia-de-ec2-pero-la-resolución-dns-falla-un-ingeniero-de-cloudops-debe-implementar-resolución-dns-entre-los-recursos-on-premises-y-los-de-aws-qué-solución-permite-que-la-aplicación-on-premises-resuelva-el-nombre-de-host-de-la-instancia-de-ec2) |
| 21 | [Al configurar una conexión `VPN` administrada por AWS, un ingeniero de CloudOps crea un recurso de gateway de cliente (customer gateway) en AWS. El dispositivo de gateway del cliente reside en un centro de datos con una puerta de enlace `NAT` frente a él. ¿Qué dirección se debe usar para crear el recurso de gateway del cliente?](#al-configurar-una-conexión-vpn-administrada-por-aws-un-ingeniero-de-cloudops-crea-un-recurso-de-gateway-de-cliente-customer-gateway-en-aws-el-dispositivo-de-gateway-del-cliente-reside-en-un-centro-de-datos-con-una-puerta-de-enlace-nat-frente-a-él-qué-dirección-se-debe-usar-para-crear-el-recurso-de-gateway-del-cliente) |
| 22 | [El sitio web de una empresa contiene una capa web y una capa de base de datos en AWS. La capa web consiste en instancias de Amazon EC2 que se ejecutan en un grupo de Auto Scaling distribuido en dos Zonas de disponibilidad. La capa de base de datos se ejecuta en una instancia de Amazon RDS for MySQL Multi-AZ. Las `ACL`s de red de la subred de base de datos están restringidas únicamente a las subredes web que necesitan acceso a la base de datos. Las subredes web usan la `ACL` de red predeterminada con las reglas por defecto. El equipo de operaciones de la empresa ha agregado una tercera subred a la configuración del grupo de Auto Scaling. Después de que ocurre un evento de Auto Scaling, algunos usuarios reportan que reciben intermitentemente un mensaje de error. El mensaje de error indica que el servidor no puede conectarse a la base de datos. El equipo de operaciones ha confirmado que las tablas de enrutamiento son correctas y que los puertos requeridos están abiertos en todos los grupos de seguridad. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para que los servidores web puedan comunicarse con la instancia de base de datos? (Seleccione DOS.)](#el-sitio-web-de-una-empresa-contiene-una-capa-web-y-una-capa-de-base-de-datos-en-aws-la-capa-web-consiste-en-instancias-de-amazon-ec2-que-se-ejecutan-en-un-grupo-de-auto-scaling-distribuido-en-dos-zonas-de-disponibilidad-la-capa-de-base-de-datos-se-ejecuta-en-una-instancia-de-amazon-rds-for-mysql-multi-az-las-acls-de-red-de-la-subred-de-base-de-datos-están-restringidas-únicamente-a-las-subredes-web-que-necesitan-acceso-a-la-base-de-datos-las-subredes-web-usan-la-acl-de-red-predeterminada-con-las-reglas-por-defecto-el-equipo-de-operaciones-de-la-empresa-ha-agregado-una-tercera-subred-a-la-configuración-del-grupo-de-auto-scaling-después-de-que-ocurre-un-evento-de-auto-scaling-algunos-usuarios-reportan-que-reciben-intermitentemente-un-mensaje-de-error-el-mensaje-de-error-indica-que-el-servidor-no-puede-conectarse-a-la-base-de-datos-el-equipo-de-operaciones-ha-confirmado-que-las-tablas-de-enrutamiento-son-correctas-y-que-los-puertos-requeridos-están-abiertos-en-todos-los-grupos-de-seguridad-qué-combinación-de-acciones-debe-tomar-un-ingeniero-de-cloudops-para-que-los-servidores-web-puedan-comunicarse-con-la-instancia-de-base-de-datos-seleccione-dos) |
| 23 | [La infraestructura backend de una empresa contiene una instancia de Amazon EC2 en una subred privada. La subred privada tiene una ruta a internet a través de una puerta de enlace `NAT` en una subred pública. La instancia debe permitir conectividad hacia un servidor web seguro en internet para recuperar datos a intervalos regulares. El software cliente agota el tiempo de espera con un mensaje de error que indica que no pudo establecer la conexión `TCP`. ¿Qué debe hacer un ingeniero de CloudOps para resolver este error?](#la-infraestructura-backend-de-una-empresa-contiene-una-instancia-de-amazon-ec2-en-una-subred-privada-la-subred-privada-tiene-una-ruta-a-internet-a-través-de-una-puerta-de-enlace-nat-en-una-subred-pública-la-instancia-debe-permitir-conectividad-hacia-un-servidor-web-seguro-en-internet-para-recuperar-datos-a-intervalos-regulares-el-software-cliente-agota-el-tiempo-de-espera-con-un-mensaje-de-error-que-indica-que-no-pudo-establecer-la-conexión-tcp-qué-debe-hacer-un-ingeniero-de-cloudops-para-resolver-este-error) |
| 24 | [Una empresa almacena archivos en 50 buckets de Amazon S3 dentro de la misma región de AWS. La empresa quiere conectarse a los buckets de S3 de forma segura a través de una conexión privada desde sus instancias de Amazon EC2. La empresa necesita una solución que no genere costo adicional. ¿Qué solución cumple con estos requisitos?](#una-empresa-almacena-archivos-en-50-buckets-de-amazon-s3-dentro-de-la-misma-región-de-aws-la-empresa-quiere-conectarse-a-los-buckets-de-s3-de-forma-segura-a-través-de-una-conexión-privada-desde-sus-instancias-de-amazon-ec2-la-empresa-necesita-una-solución-que-no-genere-costo-adicional-qué-solución-cumple-con-estos-requisitos) |
| 25 | [Un ingeniero de CloudOps está solucionando problemas de tiempo de espera de conexión hacia una instancia de Amazon EC2 que tiene una dirección IP pública. La instancia tiene una dirección IP privada `172.31.16.139`. Cuando el ingeniero de CloudOps intenta hacer ping a la dirección IP pública de la instancia desde la dirección IP remota `203.0.113.12`, la respuesta es `request timed out`. Los registros de flujo contienen la siguiente información. ¿Cuál es una causa del problema?](#un-ingeniero-de-cloudops-está-solucionando-problemas-de-tiempo-de-espera-de-conexión-hacia-una-instancia-de-amazon-ec2-que-tiene-una-dirección-ip-pública-la-instancia-tiene-una-dirección-ip-privada-1723116139-cuando-el-ingeniero-de-cloudops-intenta-hacer-ping-a-la-dirección-ip-pública-de-la-instancia-desde-la-dirección-ip-remota-203011312-la-respuesta-es-request-timed-out-los-registros-de-flujo-contienen-la-siguiente-información-cuál-es-una-causa-del-problema) |
| 26 | [Un ingeniero de CloudOps necesita configurar una solución que entregue contenido digital a un conjunto de usuarios autorizados a través de Amazon CloudFront. Los usuarios no autorizados deben quedar restringidos del acceso. ¿Qué solución cumple con estos requisitos?](#un-ingeniero-de-cloudops-necesita-configurar-una-solución-que-entregue-contenido-digital-a-un-conjunto-de-usuarios-autorizados-a-través-de-amazon-cloudfront-los-usuarios-no-autorizados-deben-quedar-restringidos-del-acceso-qué-solución-cumple-con-estos-requisitos) |
| 27 | [Una empresa ha desplegado una aplicación en instancias de Amazon EC2 dentro de una única `VPC`. La empresa ha colocado las instancias de EC2 en una subred privada de la `VPC`. Las instancias de EC2 necesitan acceso a buckets de Amazon S3 que están en la misma región de AWS que las instancias de EC2. Un ingeniero de CloudOps debe proporcionar a las instancias de EC2 acceso a los buckets de S3 sin requerir ningún cambio en las instancias de EC2 ni en la aplicación. Las instancias de EC2 no deben tener acceso a internet. ¿Qué solución cumple con estos requisitos?](#una-empresa-ha-desplegado-una-aplicación-en-instancias-de-amazon-ec2-dentro-de-una-única-vpc-la-empresa-ha-colocado-las-instancias-de-ec2-en-una-subred-privada-de-la-vpc-las-instancias-de-ec2-necesitan-acceso-a-buckets-de-amazon-s3-que-están-en-la-misma-región-de-aws-que-las-instancias-de-ec2-un-ingeniero-de-cloudops-debe-proporcionar-a-las-instancias-de-ec2-acceso-a-los-buckets-de-s3-sin-requerir-ningún-cambio-en-las-instancias-de-ec2-ni-en-la-aplicación-las-instancias-de-ec2-no-deben-tener-acceso-a-internet-qué-solución-cumple-con-estos-requisitos) |
| 28 | [Una empresa actualmente ejecuta su infraestructura dentro de una `VPC` en una sola Zona de disponibilidad. La `VPC` está conectada al centro de datos on-premises de la empresa a través de una conexión AWS Site-to-Site `VPN` adjunta a una puerta de enlace privada virtual. Las tablas de enrutamiento on-premises enrutan todas las redes de la `VPC` hacia la conexión `VPN`. La comunicación entre ambos entornos funciona correctamente. Un ingeniero de CloudOps creó nuevas subredes de `VPC` dentro de una nueva Zona de disponibilidad, y desplegó nuevos recursos dentro de esas subredes. Sin embargo, no se puede establecer comunicación entre los nuevos recursos y el entorno on-premises. ¿Qué pasos debe tomar el ingeniero de CloudOps para resolver el problema?](#una-empresa-actualmente-ejecuta-su-infraestructura-dentro-de-una-vpc-en-una-sola-zona-de-disponibilidad-la-vpc-está-conectada-al-centro-de-datos-on-premises-de-la-empresa-a-través-de-una-conexión-aws-site-to-site-vpn-adjunta-a-una-puerta-de-enlace-privada-virtual-las-tablas-de-enrutamiento-on-premises-enrutan-todas-las-redes-de-la-vpc-hacia-la-conexión-vpn-la-comunicación-entre-ambos-entornos-funciona-correctamente-un-ingeniero-de-cloudops-creó-nuevas-subredes-de-vpc-dentro-de-una-nueva-zona-de-disponibilidad-y-desplegó-nuevos-recursos-dentro-de-esas-subredes-sin-embargo-no-se-puede-establecer-comunicación-entre-los-nuevos-recursos-y-el-entorno-on-premises-qué-pasos-debe-tomar-el-ingeniero-de-cloudops-para-resolver-el-problema) |
| 29 | [Una empresa está ejecutando un sitio web en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa configuró una distribución de Amazon CloudFront y estableció el `ALB` como origen. La empresa creó un registro `CNAME` de Amazon Route 53 para enviar todo el tráfico a través de la distribución de CloudFront. Como efecto secundario no deseado, ahora se está sirviendo a los usuarios móviles la versión de escritorio del sitio web. ¿Qué acción debe tomar un ingeniero de CloudOps para resolver este problema?](#una-empresa-está-ejecutando-un-sitio-web-en-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-alb-la-empresa-configuró-una-distribución-de-amazon-cloudfront-y-estableció-el-alb-como-origen-la-empresa-creó-un-registro-cname-de-amazon-route-53-para-enviar-todo-el-tráfico-a-través-de-la-distribución-de-cloudfront-como-efecto-secundario-no-deseado-ahora-se-está-sirviendo-a-los-usuarios-móviles-la-versión-de-escritorio-del-sitio-web-qué-acción-debe-tomar-un-ingeniero-de-cloudops-para-resolver-este-problema) |
| 30 | [Una empresa aloja su sitio web en instancias de Amazon EC2 detrás de un Application Load Balancer. La empresa administra su `DNS` con Amazon Route 53, y quiere apuntar el ápice de zona (zone apex) de su dominio hacia el sitio web. ¿Qué tipo de registro se debe usar para cumplir con estos requisitos?](#una-empresa-aloja-su-sitio-web-en-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-la-empresa-administra-su-dns-con-amazon-route-53-y-quiere-apuntar-el-ápice-de-zona-zone-apex-de-su-dominio-hacia-el-sitio-web-qué-tipo-de-registro-se-debe-usar-para-cumplir-con-estos-requisitos) |
| 31 | [Un ingeniero de CloudOps ha creado una `VPC` que contiene una subred pública y una subred privada. Las instancias de Amazon EC2 que se lanzaron en la subred privada no pueden acceder a internet. La `ACL` de red predeterminada está activa en todas las subredes de la `VPC`, y todos los grupos de seguridad permiten todo el tráfico de salida. ¿Qué solución proporcionará a las instancias de EC2 en la subred privada acceso a internet?](#un-ingeniero-de-cloudops-ha-creado-una-vpc-que-contiene-una-subred-pública-y-una-subred-privada-las-instancias-de-amazon-ec2-que-se-lanzaron-en-la-subred-privada-no-pueden-acceder-a-internet-la-acl-de-red-predeterminada-está-activa-en-todas-las-subredes-de-la-vpc-y-todos-los-grupos-de-seguridad-permiten-todo-el-tráfico-de-salida-qué-solución-proporcionará-a-las-instancias-de-ec2-en-la-subred-privada-acceso-a-internet) |
| 32 | [Una empresa aloja un sitio web estático en Amazon S3. El sitio web es servido por una distribución de Amazon CloudFront con un `TTL` predeterminado de 86,400 segundos. La empresa recientemente subió una versión actualizada del sitio web a Amazon S3. Sin embargo, los usuarios siguen viendo el contenido antiguo cuando actualizan el sitio. Un ingeniero de CloudOps debe hacer visible la nueva versión del sitio web a los usuarios lo antes posible. ¿Qué solución cumple con estos requisitos?](#una-empresa-aloja-un-sitio-web-estático-en-amazon-s3-el-sitio-web-es-servido-por-una-distribución-de-amazon-cloudfront-con-un-ttl-predeterminado-de-86400-segundos-la-empresa-recientemente-subió-una-versión-actualizada-del-sitio-web-a-amazon-s3-sin-embargo-los-usuarios-siguen-viendo-el-contenido-antiguo-cuando-actualizan-el-sitio-un-ingeniero-de-cloudops-debe-hacer-visible-la-nueva-versión-del-sitio-web-a-los-usuarios-lo-antes-posible-qué-solución-cumple-con-estos-requisitos) |
| 33 | [Un nuevo sitio web se ejecutará en instancias de Amazon EC2 detrás de un Application Load Balancer. Amazon Route 53 se usará para administrar los registros `DNS`. ¿Qué tipo de registro se debe configurar en Route 53 para que el nombre de dominio raíz del sitio web (por ejemplo, `company.com`) apunte al Application Load Balancer?](#un-nuevo-sitio-web-se-ejecutará-en-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-amazon-route-53-se-usará-para-administrar-los-registros-dns-qué-tipo-de-registro-se-debe-configurar-en-route-53-para-que-el-nombre-de-dominio-raíz-del-sitio-web-por-ejemplo-companycom-apunte-al-application-load-balancer) |
| 34 | [Una empresa planea alojar una aplicación en un conjunto de instancias de Amazon EC2 distribuidas entre múltiples Zonas de disponibilidad. La aplicación debe poder escalar a millones de solicitudes por segundo. Un ingeniero de CloudOps debe diseñar una solución para distribuir el tráfico a las instancias de EC2. La solución debe estar optimizada para manejar patrones de tráfico repentinos y volátiles, usando una única dirección IP estática por cada Zona de disponibilidad. ¿Qué solución cumple con estos requisitos?](#una-empresa-planea-alojar-una-aplicación-en-un-conjunto-de-instancias-de-amazon-ec2-distribuidas-entre-múltiples-zonas-de-disponibilidad-la-aplicación-debe-poder-escalar-a-millones-de-solicitudes-por-segundo-un-ingeniero-de-cloudops-debe-diseñar-una-solución-para-distribuir-el-tráfico-a-las-instancias-de-ec2-la-solución-debe-estar-optimizada-para-manejar-patrones-de-tráfico-repentinos-y-volátiles-usando-una-única-dirección-ip-estática-por-cada-zona-de-disponibilidad-qué-solución-cumple-con-estos-requisitos) |
| 35 | [Un ingeniero de CloudOps migra instancias `NAT` a puertas de enlace `NAT`. Después de la migración, una aplicación alojada en instancias de Amazon EC2 en una subred privada no puede acceder a internet. ¿Cuáles de las siguientes son posibles razones para este problema? (Elija dos.)](#un-ingeniero-de-cloudops-migra-instancias-nat-a-puertas-de-enlace-nat-después-de-la-migración-una-aplicación-alojada-en-instancias-de-amazon-ec2-en-una-subred-privada-no-puede-acceder-a-internet-cuáles-de-las-siguientes-son-posibles-razones-para-este-problema-elija-dos) |
| 36 | [Una nueva aplicación se ejecuta en instancias de Amazon EC2 y accede a datos en una instancia de base de datos de Amazon RDS. Cuando se despliega completamente en producción, la aplicación falla. La base de datos puede consultarse desde una consola en un bastion host. Al revisar los registros del servidor web, se repite varias veces el siguiente error: `*** Error Establishing a Database Connection`. ¿Cuáles de las siguientes pueden ser causas de los problemas de conectividad? (Elija dos.)](#una-nueva-aplicación-se-ejecuta-en-instancias-de-amazon-ec2-y-accede-a-datos-en-una-instancia-de-base-de-datos-de-amazon-rds-cuando-se-despliega-completamente-en-producción-la-aplicación-falla-la-base-de-datos-puede-consultarse-desde-una-consola-en-un-bastion-host-al-revisar-los-registros-del-servidor-web-se-repite-varias-veces-el-siguiente-error--error-establishing-a-database-connection-cuáles-de-las-siguientes-pueden-ser-causas-de-los-problemas-de-conectividad-elija-dos) |
| 37 | [Un ingeniero de CloudOps es responsable de administrar una flota de instancias de Amazon EC2. Estas instancias de EC2 suben artefactos de compilación (build artifacts) a un servicio de terceros. El servicio de terceros implementó recientemente una lista estricta de IP permitidas que requiere que todas las cargas de compilación provengan de una única dirección IP. ¿Qué cambio debe hacer el ingeniero de sistemas en la flota de compilación existente para cumplir con este nuevo requisito?](#un-ingeniero-de-cloudops-es-responsable-de-administrar-una-flota-de-instancias-de-amazon-ec2-estas-instancias-de-ec2-suben-artefactos-de-compilación-build-artifacts-a-un-servicio-de-terceros-el-servicio-de-terceros-implementó-recientemente-una-lista-estricta-de-ip-permitidas-que-requiere-que-todas-las-cargas-de-compilación-provengan-de-una-única-dirección-ip-qué-cambio-debe-hacer-el-ingeniero-de-sistemas-en-la-flota-de-compilación-existente-para-cumplir-con-este-nuevo-requisito) |
| 38 | [Un ingeniero de CloudOps está intentando configurar un nombre de dominio de Amazon Route 53 para enrutar tráfico a un sitio web alojado en Amazon S3. El nombre de dominio del sitio web es `www.example.com` y el nombre del bucket de S3 es `DOC-EXAMPLE-BUCKET`. Después de configurar el conjunto de registros en Route 53, el nombre de dominio `www.anycompany.com` no parece funcionar, y el sitio web estático no se muestra en el navegador. ¿Cuál de las siguientes es una causa de esto?](#un-ingeniero-de-cloudops-está-intentando-configurar-un-nombre-de-dominio-de-amazon-route-53-para-enrutar-tráfico-a-un-sitio-web-alojado-en-amazon-s3-el-nombre-de-dominio-del-sitio-web-es-wwwexamplecom-y-el-nombre-del-bucket-de-s3-es-doc-example-bucket-después-de-configurar-el-conjunto-de-registros-en-route-53-el-nombre-de-dominio-wwwanycompanycom-no-parece-funcionar-y-el-sitio-web-estático-no-se-muestra-en-el-navegador-cuál-de-las-siguientes-es-una-causa-de-esto) |
| 39 | [Una empresa aloja su sitio web en instancias de Amazon EC2 en la región `us-east-1`. La empresa se está preparando para extender su sitio web a la región `eu-central-1`, pero la base de datos debe permanecer únicamente en `us-east-1`. Después del despliegue, las instancias de EC2 en `eu-central-1` no pueden conectarse a la base de datos en `us-east-1`. ¿Cuál es la solución MÁS eficiente operativamente que resolverá este problema de conectividad?](#una-empresa-aloja-su-sitio-web-en-instancias-de-amazon-ec2-en-la-región-us-east-1-la-empresa-se-está-preparando-para-extender-su-sitio-web-a-la-región-eu-central-1-pero-la-base-de-datos-debe-permanecer-únicamente-en-us-east-1-después-del-despliegue-las-instancias-de-ec2-en-eu-central-1-no-pueden-conectarse-a-la-base-de-datos-en-us-east-1-cuál-es-la-solución-más-eficiente-operativamente-que-resolverá-este-problema-de-conectividad) |
| 40 | [Una empresa subió los archivos de su sitio web a un bucket de Amazon S3 que tiene habilitado el versionado de S3. La empresa usa una distribución de Amazon CloudFront con el bucket de S3 como origen. La empresa modificó recientemente los archivos, pero los nombres de objeto permanecieron iguales. Los usuarios reportan que el contenido antiguo sigue apareciendo en el sitio web. ¿Cómo debe un ingeniero de CloudOps remediar este problema?](#una-empresa-subió-los-archivos-de-su-sitio-web-a-un-bucket-de-amazon-s3-que-tiene-habilitado-el-versionado-de-s3-la-empresa-usa-una-distribución-de-amazon-cloudfront-con-el-bucket-de-s3-como-origen-la-empresa-modificó-recientemente-los-archivos-pero-los-nombres-de-objeto-permanecieron-iguales-los-usuarios-reportan-que-el-contenido-antiguo-sigue-apareciendo-en-el-sitio-web-cómo-debe-un-ingeniero-de-cloudops-remediar-este-problema) |
| 41 | [Una empresa tiene dos redes `VPC` llamadas `VPC` A y `VPC` B. El bloque `CIDR` de `VPC` A es `10.0.0.0/16` y el bloque `CIDR` de `VPC` B es `172.31.0.0/16`. La empresa quiere establecer una conexión de emparejamiento (peering) de `VPC` llamada `pcx-12345` entre ambas `VPC`. ¿Qué reglas deben aparecer en la tabla de enrutamiento de `VPC` A después de la configuración? (Elija dos.)](#una-empresa-tiene-dos-redes-vpc-llamadas-vpc-a-y-vpc-b-el-bloque-cidr-de-vpc-a-es-1000016-y-el-bloque-cidr-de-vpc-b-es-172310016-la-empresa-quiere-establecer-una-conexión-de-emparejamiento-peering-de-vpc-llamada-pcx-12345-entre-ambas-vpc-qué-reglas-deben-aparecer-en-la-tabla-de-enrutamiento-de-vpc-a-después-de-la-configuración-elija-dos) |
| 42 | [Una aplicación se ejecuta en una instancia de Amazon EC2 en una `VPC` con el conjunto de opciones `DHCP` predeterminado. La aplicación se conecta a una base de datos Microsoft SQL Server local (on-premises) con el nombre `DNS` `mssql.example.com`. La aplicación no puede resolver el nombre `DNS` de la base de datos. ¿Qué solución solucionará este problema?](#una-aplicación-se-ejecuta-en-una-instancia-de-amazon-ec2-en-una-vpc-con-el-conjunto-de-opciones-dhcp-predeterminado-la-aplicación-se-conecta-a-una-base-de-datos-microsoft-sql-server-local-on-premises-con-el-nombre-dns-mssqlexamplecom-la-aplicación-no-puede-resolver-el-nombre-dns-de-la-base-de-datos-qué-solución-solucionará-este-problema) |
| 43 | [La aplicación de una empresa está alojada por un proveedor de internet en `app.example.com`. La empresa quiere acceder a la aplicación usando `www.company.com`, que la empresa posee y administra con Amazon Route 53. ¿Qué registro de Route 53 se debe crear para lograr esto?](#la-aplicación-de-una-empresa-está-alojada-por-un-proveedor-de-internet-en-appexamplecom-la-empresa-quiere-acceder-a-la-aplicación-usando-wwwcompanycom-que-la-empresa-posee-y-administra-con-amazon-route-53-qué-registro-de-route-53-se-debe-crear-para-lograr-esto) |
| 44 | [Una empresa aloja un sitio web estático en Amazon S3. Una distribución de Amazon CloudFront presenta este sitio a usuarios globales. La empresa usa la política de caché `Managed-CachingDisabled` de CloudFront. Los desarrolladores de la empresa confirman que actualizan con frecuencia un archivo en Amazon S3 con información nueva. Los usuarios reportan que el sitio web presenta la información correcta cuando el sitio carga el archivo por primera vez. Sin embargo, los navegadores de los usuarios no obtienen el archivo actualizado después de una actualización (refresh). ¿Qué debe recomendar un ingeniero de CloudOps para solucionar este problema?](#una-empresa-aloja-un-sitio-web-estático-en-amazon-s3-una-distribución-de-amazon-cloudfront-presenta-este-sitio-a-usuarios-globales-la-empresa-usa-la-política-de-caché-managed-cachingdisabled-de-cloudfront-los-desarrolladores-de-la-empresa-confirman-que-actualizan-con-frecuencia-un-archivo-en-amazon-s3-con-información-nueva-los-usuarios-reportan-que-el-sitio-web-presenta-la-información-correcta-cuando-el-sitio-carga-el-archivo-por-primera-vez-sin-embargo-los-navegadores-de-los-usuarios-no-obtienen-el-archivo-actualizado-después-de-una-actualización-refresh-qué-debe-recomendar-un-ingeniero-de-cloudops-para-solucionar-este-problema) |
| 45 | [Una empresa usa Amazon CloudFront para servir contenido estático de su aplicación web a sus usuarios. La distribución de CloudFront usa un sitio web local (on-premises) existente como origen personalizado. La empresa requiere el uso de TLS entre CloudFront y el servidor de origen. Esta configuración ha funcionado como se esperaba durante varios meses. Sin embargo, los usuarios ahora están experimentando errores `HTTP 502 (Bad Gateway)` al ver páginas web que incluyen contenido de la distribución de CloudFront. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?](#una-empresa-usa-amazon-cloudfront-para-servir-contenido-estático-de-su-aplicación-web-a-sus-usuarios-la-distribución-de-cloudfront-usa-un-sitio-web-local-on-premises-existente-como-origen-personalizado-la-empresa-requiere-el-uso-de-tls-entre-cloudfront-y-el-servidor-de-origen-esta-configuración-ha-funcionado-como-se-esperaba-durante-varios-meses-sin-embargo-los-usuarios-ahora-están-experimentando-errores-http-502-bad-gateway-al-ver-páginas-web-que-incluyen-contenido-de-la-distribución-de-cloudfront-qué-debe-hacer-un-ingeniero-de-cloudops-para-resolver-este-problema) |
| 46 | [Una distribución de Amazon CloudFront tiene un único bucket de Amazon S3 como su origen. Un ingeniero de CloudOps debe asegurarse de que los usuarios solo puedan acceder al bucket de S3 a través de solicitudes provenientes del endpoint de CloudFront. ¿Qué solución cumple con estos requisitos?](#una-distribución-de-amazon-cloudfront-tiene-un-único-bucket-de-amazon-s3-como-su-origen-un-ingeniero-de-cloudops-debe-asegurarse-de-que-los-usuarios-solo-puedan-acceder-al-bucket-de-s3-a-través-de-solicitudes-provenientes-del-endpoint-de-cloudfront-qué-solución-cumple-con-estos-requisitos) |
| 47 | [Una empresa tiene una aplicación que se ejecuta en instancias de Amazon EC2 en una `VPC`. La aplicación necesita acceso para descargar actualizaciones de software desde internet. La `VPC` tiene subredes públicas y subredes privadas. La política de seguridad de la empresa requiere que todas las instancias de EC2 se desplieguen en subredes privadas. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con estos requisitos?](#una-empresa-tiene-una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-en-una-vpc-la-aplicación-necesita-acceso-para-descargar-actualizaciones-de-software-desde-internet-la-vpc-tiene-subredes-públicas-y-subredes-privadas-la-política-de-seguridad-de-la-empresa-requiere-que-todas-las-instancias-de-ec2-se-desplieguen-en-subredes-privadas-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 48 | [Un ingeniero de CloudOps ha configurado una nueva instancia de Amazon EC2 como servidor web en una subred pública. La instancia usa el puerto `80` de `HTTP` y el puerto `443` de `HTTPS`. El ingeniero de CloudOps ha confirmado la conectividad a internet descargando actualizaciones del sistema operativo y software desde repositorios públicos. Sin embargo, el ingeniero de CloudOps no puede acceder a la instancia desde un navegador web en internet. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para solucionar este problema? (Elija tres.)](#un-ingeniero-de-cloudops-ha-configurado-una-nueva-instancia-de-amazon-ec2-como-servidor-web-en-una-subred-pública-la-instancia-usa-el-puerto-80-de-http-y-el-puerto-443-de-https-el-ingeniero-de-cloudops-ha-confirmado-la-conectividad-a-internet-descargando-actualizaciones-del-sistema-operativo-y-software-desde-repositorios-públicos-sin-embargo-el-ingeniero-de-cloudops-no-puede-acceder-a-la-instancia-desde-un-navegador-web-en-internet-qué-combinación-de-pasos-debe-tomar-el-ingeniero-de-cloudops-para-solucionar-este-problema-elija-tres) |
| 49 | [Los usuarios reportan cierres de sesión forzados constantes en una aplicación web con estado (stateful). Los cierres de sesión ocurren antes de la expiración de un temporizador de cierre de sesión de la aplicación de 15 minutos. La aplicación web está alojada en instancias de Amazon EC2 que están en un grupo de Auto Scaling. Las instancias se ejecutan detrás de un Application Load Balancer (ALB) que tiene un único grupo de destino (target group). El `ALB` está configurado como el origen en una distribución de Amazon CloudFront. La afinidad de sesión (sticky sessions) ya está habilitada en el grupo de destino del `ALB` y usa cookies basadas en duración. La aplicación web genera su propia cookie de aplicación. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para resolver el problema de cierre de sesión? (Elija dos.)](#los-usuarios-reportan-cierres-de-sesión-forzados-constantes-en-una-aplicación-web-con-estado-stateful-los-cierres-de-sesión-ocurren-antes-de-la-expiración-de-un-temporizador-de-cierre-de-sesión-de-la-aplicación-de-15-minutos-la-aplicación-web-está-alojada-en-instancias-de-amazon-ec2-que-están-en-un-grupo-de-auto-scaling-las-instancias-se-ejecutan-detrás-de-un-application-load-balancer-alb-que-tiene-un-único-grupo-de-destino-target-group-el-alb-está-configurado-como-el-origen-en-una-distribución-de-amazon-cloudfront-la-afinidad-de-sesión-sticky-sessions-ya-está-habilitada-en-el-grupo-de-destino-del-alb-y-usa-cookies-basadas-en-duración-la-aplicación-web-genera-su-propia-cookie-de-aplicación-qué-combinación-de-acciones-debe-tomar-un-ingeniero-de-cloudops-para-resolver-el-problema-de-cierre-de-sesión-elija-dos) |
| 50 | [Un ingeniero de CloudOps descubrió que un servidor de aplicación de Amazon EC2 recién desplegado no puede conectarse a una instancia de base de datos de Amazon RDS existente. Después de habilitar `VPC` Flow Logs y confirmar que el flow log está activo en la consola, el grupo de registro no se puede encontrar en Amazon CloudWatch. ¿Cuáles son las razones MÁS probables de esta situación? (Elija dos.)](#un-ingeniero-de-cloudops-descubrió-que-un-servidor-de-aplicación-de-amazon-ec2-recién-desplegado-no-puede-conectarse-a-una-instancia-de-base-de-datos-de-amazon-rds-existente-después-de-habilitar-vpc-flow-logs-y-confirmar-que-el-flow-log-está-activo-en-la-consola-el-grupo-de-registro-no-se-puede-encontrar-en-amazon-cloudwatch-cuáles-son-las-razones-más-probables-de-esta-situación-elija-dos) |
| 51 | [El ingeniero de CloudOps de una empresa está solucionando problemas de comunicación entre los componentes de una aplicación. La empresa configuró los flow logs de `VPC` para que se publiquen en Amazon CloudWatch Logs. Sin embargo, no hay registros en CloudWatch Logs. ¿Qué podría estar bloqueando que los flow logs de `VPC` se publiquen en CloudWatch Logs?](#el-ingeniero-de-cloudops-de-una-empresa-está-solucionando-problemas-de-comunicación-entre-los-componentes-de-una-aplicación-la-empresa-configuró-los-flow-logs-de-vpc-para-que-se-publiquen-en-amazon-cloudwatch-logs-sin-embargo-no-hay-registros-en-cloudwatch-logs-qué-podría-estar-bloqueando-que-los-flow-logs-de-vpc-se-publiquen-en-cloudwatch-logs) |
| 52 | [Un ingeniero de CloudOps configura los flow logs de `VPC` para que se publiquen en Amazon CloudWatch Logs. El ingeniero de CloudOps revisa los registros en CloudWatch Logs y nota menos tráfico del esperado. Después de que el ingeniero de CloudOps compara los flow logs de `VPC` con registros capturados localmente (on-premises), el ingeniero de CloudOps cree que los flow logs de `VPC` están incompletos. ¿Cuál de las siguientes es una posible razón para la diferencia en el tráfico?](#un-ingeniero-de-cloudops-configura-los-flow-logs-de-vpc-para-que-se-publiquen-en-amazon-cloudwatch-logs-el-ingeniero-de-cloudops-revisa-los-registros-en-cloudwatch-logs-y-nota-menos-tráfico-del-esperado-después-de-que-el-ingeniero-de-cloudops-compara-los-flow-logs-de-vpc-con-registros-capturados-localmente-on-premises-el-ingeniero-de-cloudops-cree-que-los-flow-logs-de-vpc-están-incompletos-cuál-de-las-siguientes-es-una-posible-razón-para-la-diferencia-en-el-tráfico) |
| 53 | [Un ingeniero de CloudOps está revisando los `VPC` Flow Logs para solucionar problemas de conectividad en una `VPC`. Al revisar los registros, el ingeniero de CloudOps nota que el tráfico rechazado no aparece listado. ¿Qué debe hacer el ingeniero de CloudOps para asegurarse de que todo el tráfico se registre?](#un-ingeniero-de-cloudops-está-revisando-los-vpc-flow-logs-para-solucionar-problemas-de-conectividad-en-una-vpc-al-revisar-los-registros-el-ingeniero-de-cloudops-nota-que-el-tráfico-rechazado-no-aparece-listado-qué-debe-hacer-el-ingeniero-de-cloudops-para-asegurarse-de-que-todo-el-tráfico-se-registre) |
| 54 | [Una empresa aloja una aplicación web en una instancia de Amazon EC2 en una `VPC` de producción. Las conexiones de clientes a la aplicación están fallando. Un ingeniero de CloudOps inspecciona los flow logs de `VPC` y encuentra la siguiente entrada. ¿Cuál es una posible causa de estas conexiones fallidas?](#una-empresa-aloja-una-aplicación-web-en-una-instancia-de-amazon-ec2-en-una-vpc-de-producción-las-conexiones-de-clientes-a-la-aplicación-están-fallando-un-ingeniero-de-cloudops-inspecciona-los-flow-logs-de-vpc-y-encuentra-la-siguiente-entrada-cuál-es-una-posible-causa-de-estas-conexiones-fallidas) |
| 55 | [Una empresa está ejecutando una aplicación en un grupo de instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias de EC2 se ejecutan en tres Zonas de disponibilidad. La empresa necesita proporcionar a los clientes un máximo de dos direcciones IP estáticas para sus aplicaciones. ¿Cómo debe un ingeniero de CloudOps cumplir con este requisito?](#una-empresa-está-ejecutando-una-aplicación-en-un-grupo-de-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-las-instancias-de-ec2-se-ejecutan-en-tres-zonas-de-disponibilidad-la-empresa-necesita-proporcionar-a-los-clientes-un-máximo-de-dos-direcciones-ip-estáticas-para-sus-aplicaciones-cómo-debe-un-ingeniero-de-cloudops-cumplir-con-este-requisito) |
| 56 | [Una empresa almacena contenido multimedia en un bucket de Amazon S3 y usa Amazon CloudFront para distribuir el contenido a sus usuarios. Debido a los términos de licencia, la empresa no está autorizada a distribuir el contenido en algunos países. Un ingeniero de CloudOps debe restringir el acceso a ciertos países. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-almacena-contenido-multimedia-en-un-bucket-de-amazon-s3-y-usa-amazon-cloudfront-para-distribuir-el-contenido-a-sus-usuarios-debido-a-los-términos-de-licencia-la-empresa-no-está-autorizada-a-distribuir-el-contenido-en-algunos-países-un-ingeniero-de-cloudops-debe-restringir-el-acceso-a-ciertos-países-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 57 | [Una aplicación se ejecuta en múltiples instancias de EC2. Como parte de una iniciativa para mejorar la seguridad general de la infraestructura, las instancias de EC2 se movieron a una subred privada. Sin embargo, desde que se movieron, las instancias de EC2 no han podido actualizarse automáticamente, y un ingeniero de CloudOps no ha podido conectarse a ellas remotamente por `SSH`. ¿Qué dos acciones podría tomar el ingeniero para resolver estos problemas de forma segura? (Elija dos.)](#una-aplicación-se-ejecuta-en-múltiples-instancias-de-ec2-como-parte-de-una-iniciativa-para-mejorar-la-seguridad-general-de-la-infraestructura-las-instancias-de-ec2-se-movieron-a-una-subred-privada-sin-embargo-desde-que-se-movieron-las-instancias-de-ec2-no-han-podido-actualizarse-automáticamente-y-un-ingeniero-de-cloudops-no-ha-podido-conectarse-a-ellas-remotamente-por-ssh-qué-dos-acciones-podría-tomar-el-ingeniero-para-resolver-estos-problemas-de-forma-segura-elija-dos) |
| 58 | [Un ingeniero de CloudOps está solucionando problemas de una `VPC` con subredes públicas y privadas que usan `ACL` de red personalizadas. Las instancias en la subred privada no pueden acceder a internet. Hay una puerta de enlace de internet adjunta a la subred pública. La subred privada tiene una ruta hacia una puerta de enlace `NAT` que también está adjunta a la subred pública. Las instancias de Amazon EC2 están asociadas con el grupo de seguridad predeterminado de la `VPC`. ¿Qué está causando el problema en este escenario?](#un-ingeniero-de-cloudops-está-solucionando-problemas-de-una-vpc-con-subredes-públicas-y-privadas-que-usan-acl-de-red-personalizadas-las-instancias-en-la-subred-privada-no-pueden-acceder-a-internet-hay-una-puerta-de-enlace-de-internet-adjunta-a-la-subred-pública-la-subred-privada-tiene-una-ruta-hacia-una-puerta-de-enlace-nat-que-también-está-adjunta-a-la-subred-pública-las-instancias-de-amazon-ec2-están-asociadas-con-el-grupo-de-seguridad-predeterminado-de-la-vpc-qué-está-causando-el-problema-en-este-escenario) |
| 59 | [Un ingeniero de CloudOps necesita configurar un bucket de Amazon S3 para alojar una aplicación web. El ingeniero de CloudOps ha creado el bucket de S3 y ha copiado los archivos estáticos de la aplicación web al bucket de S3. La empresa tiene una política de que ningún bucket de S3 debe ser público. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?](#un-ingeniero-de-cloudops-necesita-configurar-un-bucket-de-amazon-s3-para-alojar-una-aplicación-web-el-ingeniero-de-cloudops-ha-creado-el-bucket-de-s3-y-ha-copiado-los-archivos-estáticos-de-la-aplicación-web-al-bucket-de-s3-la-empresa-tiene-una-política-de-que-ningún-bucket-de-s3-debe-ser-público-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 60 | [Una empresa planea lanzar un sitio web estático en su dominio `example.com` y subdominio `www.example.com` usando Amazon S3. ¿Cómo debe el ingeniero de CloudOps cumplir con este requisito?](#una-empresa-planea-lanzar-un-sitio-web-estático-en-su-dominio-examplecom-y-subdominio-wwwexamplecom-usando-amazon-s3-cómo-debe-el-ingeniero-de-cloudops-cumplir-con-este-requisito) |
| 61 | [Una empresa aloja su sitio web en la región `us-east-1`. La empresa se está preparando para desplegar su sitio web en la región `eu-central-1`. Los visitantes del sitio web ubicados en Europa deben acceder al sitio web alojado en `eu-central-1`. Todos los demás visitantes acceden al sitio web alojado en `us-east-1`. La empresa usa Amazon Route 53 para administrar los registros `DNS` del sitio web. ¿Qué política de enrutamiento debe aplicar un ingeniero de CloudOps al conjunto de registros de Route 53 para cumplir con estos requisitos?](#una-empresa-aloja-su-sitio-web-en-la-región-us-east-1-la-empresa-se-está-preparando-para-desplegar-su-sitio-web-en-la-región-eu-central-1-los-visitantes-del-sitio-web-ubicados-en-europa-deben-acceder-al-sitio-web-alojado-en-eu-central-1-todos-los-demás-visitantes-acceden-al-sitio-web-alojado-en-us-east-1-la-empresa-usa-amazon-route-53-para-administrar-los-registros-dns-del-sitio-web-qué-política-de-enrutamiento-debe-aplicar-un-ingeniero-de-cloudops-al-conjunto-de-registros-de-route-53-para-cumplir-con-estos-requisitos) |
| 62 | [Una empresa está configurando una conexión de emparejamiento (peering) de `VPC` entre su `VPC` y la `VPC` de un cliente. La `VPC` de la empresa tiene un bloque `CIDR` IPv4 de `172.16.0.0/16`, y la del cliente tiene un bloque `CIDR` IPv4 de `10.0.0.0/16`. El ingeniero de CloudOps quiere poder hacer ping a la dirección IP privada de la base de datos del cliente desde una de las instancias de Amazon EC2 de la empresa. ¿Qué acción se debe tomar para cumplir con los requisitos?](#una-empresa-está-configurando-una-conexión-de-emparejamiento-peering-de-vpc-entre-su-vpc-y-la-vpc-de-un-cliente-la-vpc-de-la-empresa-tiene-un-bloque-cidr-ipv4-de-172160016-y-la-del-cliente-tiene-un-bloque-cidr-ipv4-de-1000016-el-ingeniero-de-cloudops-quiere-poder-hacer-ping-a-la-dirección-ip-privada-de-la-base-de-datos-del-cliente-desde-una-de-las-instancias-de-amazon-ec2-de-la-empresa-qué-acción-se-debe-tomar-para-cumplir-con-los-requisitos) |
| 63 | [Una empresa ejecuta una aplicación web a la que los usuarios acceden usando el nombre de dominio `www.example.com`. La empresa administra el nombre de dominio usando Amazon Route 53. La empresa creó una distribución de Amazon CloudFront delante de la aplicación y le gustaría que `www.example.com` acceda a la aplicación a través de CloudFront. ¿Cuál es la forma MÁS rentable de lograr esto?](#una-empresa-ejecuta-una-aplicación-web-a-la-que-los-usuarios-acceden-usando-el-nombre-de-dominio-wwwexamplecom-la-empresa-administra-el-nombre-de-dominio-usando-amazon-route-53-la-empresa-creó-una-distribución-de-amazon-cloudfront-delante-de-la-aplicación-y-le-gustaría-que-wwwexamplecom-acceda-a-la-aplicación-a-través-de-cloudfront-cuál-es-la-forma-más-rentable-de-lograr-esto) |
| 64 | [Un ingeniero de CloudOps tiene un sitio web de Amazon S3 y quiere restringir el acceso a una única distribución de Amazon CloudFront. Los visitantes del sitio web no deben poder eludir CloudFront ni ver el sitio web de S3 directamente desde el bucket. ¿Qué servicio o función de AWS cumple con estos requisitos?](#un-ingeniero-de-cloudops-tiene-un-sitio-web-de-amazon-s3-y-quiere-restringir-el-acceso-a-una-única-distribución-de-amazon-cloudfront-los-visitantes-del-sitio-web-no-deben-poder-eludir-cloudfront-ni-ver-el-sitio-web-de-s3-directamente-desde-el-bucket-qué-servicio-o-función-de-aws-cumple-con-estos-requisitos) |
| 65 | [Un ingeniero de CloudOps está creando un sitio web simple, orientado al público, que se ejecuta en Amazon EC2. El ingeniero de CloudOps creó la instancia de EC2 en una subred pública existente y asignó una dirección IP elástica a la instancia. Luego, el ingeniero de CloudOps creó y aplicó un nuevo grupo de seguridad a la instancia para permitir tráfico `HTTP` entrante desde `0.0.0.0/0`. Finalmente, el ingeniero de CloudOps creó una nueva `ACL` de red y la aplicó a la subred para permitir tráfico `HTTP` entrante desde `0.0.0.0/0`. Sin embargo, no se puede acceder al sitio web desde internet. ¿Cuál es la causa de este problema?](#un-ingeniero-de-cloudops-está-creando-un-sitio-web-simple-orientado-al-público-que-se-ejecuta-en-amazon-ec2-el-ingeniero-de-cloudops-creó-la-instancia-de-ec2-en-una-subred-pública-existente-y-asignó-una-dirección-ip-elástica-a-la-instancia-luego-el-ingeniero-de-cloudops-creó-y-aplicó-un-nuevo-grupo-de-seguridad-a-la-instancia-para-permitir-tráfico-http-entrante-desde-00000-finalmente-el-ingeniero-de-cloudops-creó-una-nueva-acl-de-red-y-la-aplicó-a-la-subred-para-permitir-tráfico-http-entrante-desde-00000-sin-embargo-no-se-puede-acceder-al-sitio-web-desde-internet-cuál-es-la-causa-de-este-problema) |
| 66 | [Después de un cambio de red, los servidores de aplicación no pueden conectarse a la base de datos correspondiente de Amazon RDS MySQL. ¿Qué debe analizar el ingeniero de CloudOps?](#después-de-un-cambio-de-red-los-servidores-de-aplicación-no-pueden-conectarse-a-la-base-de-datos-correspondiente-de-amazon-rds-mysql-qué-debe-analizar-el-ingeniero-de-cloudops) |
| 67 | [Un ingeniero de CloudOps configuró los flow logs de `VPC` usando el formato predeterminado. El ingeniero de CloudOps especificó Amazon CloudWatch Logs como destino. Esta solución ha funcionado exitosamente durante varios meses. Sin embargo, debido a requisitos adicionales de solución de problemas, el ingeniero de CloudOps necesita incluir el campo `tcp-flags` en los flow logs. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#un-ingeniero-de-cloudops-configuró-los-flow-logs-de-vpc-usando-el-formato-predeterminado-el-ingeniero-de-cloudops-especificó-amazon-cloudwatch-logs-como-destino-esta-solución-ha-funcionado-exitosamente-durante-varios-meses-sin-embargo-debido-a-requisitos-adicionales-de-solución-de-problemas-el-ingeniero-de-cloudops-necesita-incluir-el-campo-tcp-flags-en-los-flow-logs-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 68 | [Una empresa ejecuta una aplicación en cientos de instancias de Amazon EC2 en tres Zonas de disponibilidad. La aplicación llama a una API de terceros a través de internet público. Un ingeniero de CloudOps debe proporcionar al tercero una lista de direcciones IP estáticas para que el tercero pueda permitir el tráfico desde la aplicación. ¿Qué solución cumple con estos requisitos?](#una-empresa-ejecuta-una-aplicación-en-cientos-de-instancias-de-amazon-ec2-en-tres-zonas-de-disponibilidad-la-aplicación-llama-a-una-api-de-terceros-a-través-de-internet-público-un-ingeniero-de-cloudops-debe-proporcionar-al-tercero-una-lista-de-direcciones-ip-estáticas-para-que-el-tercero-pueda-permitir-el-tráfico-desde-la-aplicación-qué-solución-cumple-con-estos-requisitos) |
| 69 | [Un ingeniero de CloudOps está administrando una red `VPC` que consiste en subredes públicas y privadas. Las instancias en las subredes privadas acceden a internet a través de una puerta de enlace `NAT`. Una factura reciente de AWS muestra que los cargos de la puerta de enlace `NAT` se han duplicado. El ingeniero quiere identificar qué instancias están generando la mayor cantidad de tráfico de red. ¿Cómo se debe lograr esto?](#un-ingeniero-de-cloudops-está-administrando-una-red-vpc-que-consiste-en-subredes-públicas-y-privadas-las-instancias-en-las-subredes-privadas-acceden-a-internet-a-través-de-una-puerta-de-enlace-nat-una-factura-reciente-de-aws-muestra-que-los-cargos-de-la-puerta-de-enlace-nat-se-han-duplicado-el-ingeniero-quiere-identificar-qué-instancias-están-generando-la-mayor-cantidad-de-tráfico-de-red-cómo-se-debe-lograr-esto) |
| 70 | [Una empresa está almacenando informes mensuales en Amazon S3. El requisito de seguridad de la empresa establece que el tráfico desde la `VPC` del cliente hacia Amazon S3 no puede atravesar internet. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-está-almacenando-informes-mensuales-en-amazon-s3-el-requisito-de-seguridad-de-la-empresa-establece-que-el-tráfico-desde-la-vpc-del-cliente-hacia-amazon-s3-no-puede-atravesar-internet-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 71 | [Un ingeniero de CloudOps está rediseñando la arquitectura de una aplicación. El ingeniero de CloudOps ha movido la base de datos de una subred pública, donde la base de datos usaba un endpoint público, a una subred privada para restringir el acceso desde la red pública. Después de este cambio, una función de AWS Lambda que requiere acceso de lectura a la base de datos no puede conectarse a la base de datos. El ingeniero de CloudOps debe resolver este problema sin comprometer la seguridad. ¿Qué solución cumple con estos requisitos?](#un-ingeniero-de-cloudops-está-rediseñando-la-arquitectura-de-una-aplicación-el-ingeniero-de-cloudops-ha-movido-la-base-de-datos-de-una-subred-pública-donde-la-base-de-datos-usaba-un-endpoint-público-a-una-subred-privada-para-restringir-el-acceso-desde-la-red-pública-después-de-este-cambio-una-función-de-aws-lambda-que-requiere-acceso-de-lectura-a-la-base-de-datos-no-puede-conectarse-a-la-base-de-datos-el-ingeniero-de-cloudops-debe-resolver-este-problema-sin-comprometer-la-seguridad-qué-solución-cumple-con-estos-requisitos) |
| 72 | [Una instancia de Amazon EC2 en una subred privada necesita copiar datos a un bucket de Amazon S3. Por razones de seguridad, la conexión desde la instancia de EC2 a Amazon S3 no debe atravesar internet. ¿Qué acción debe tomar el ingeniero de CloudOps para lograr esto?](#una-instancia-de-amazon-ec2-en-una-subred-privada-necesita-copiar-datos-a-un-bucket-de-amazon-s3-por-razones-de-seguridad-la-conexión-desde-la-instancia-de-ec2-a-amazon-s3-no-debe-atravesar-internet-qué-acción-debe-tomar-el-ingeniero-de-cloudops-para-lograr-esto) |
| 73 | [Un ingeniero de CloudOps necesita configurar la zona alojada de Amazon Route 53 para `example.com` y `www.example.com` para que apunten a un Application Load Balancer (ALB). ¿Qué combinación de acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)](#un-ingeniero-de-cloudops-necesita-configurar-la-zona-alojada-de-amazon-route-53-para-examplecom-y-wwwexamplecom-para-que-apunten-a-un-application-load-balancer-alb-qué-combinación-de-acciones-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-elija-dos) |
| 74 | [Un ingeniero de CloudOps creó una función de AWS Lambda dentro de una `VPC` sin acceso a internet. La función Lambda extrae mensajes de una cola de Amazon SQS y los almacena en una instancia de Amazon RDS en la misma `VPC`. Después de ejecutar la función Lambda, los datos no aparecen en la instancia de RDS. ¿Cuáles de las siguientes son posibles causas de esto? (Elija dos.)](#un-ingeniero-de-cloudops-creó-una-función-de-aws-lambda-dentro-de-una-vpc-sin-acceso-a-internet-la-función-lambda-extrae-mensajes-de-una-cola-de-amazon-sqs-y-los-almacena-en-una-instancia-de-amazon-rds-en-la-misma-vpc-después-de-ejecutar-la-función-lambda-los-datos-no-aparecen-en-la-instancia-de-rds-cuáles-de-las-siguientes-son-posibles-causas-de-esto-elija-dos) |
| 75 | [Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. ¿Cuál de las siguientes afirmaciones NO es verdadera en este escenario?](#un-usuario-ha-creado-una-vpc-con-subredes-públicas-y-privadas-usando-el-asistente-de-vpc-cuál-de-las-siguientes-afirmaciones-no-es-verdadera-en-este-escenario) |
| 76 | [Una empresa tiene una aplicación que usa una función programada de AWS Lambda para recuperar conjuntos de datos de fuentes externas a través de internet. La función no está asociada con una `VPC`. La empresa está modificando la aplicación para almacenar la información que la función Lambda recupera en una instancia de base de datos de Amazon RDS en una subred privada. La `VPC` tiene dos subredes públicas y dos subredes privadas. Un ingeniero de CloudOps debe desplegar una solución que permita a la función Lambda acceder a la nueva base de datos y continuar accediendo a internet. ¿Qué solución cumple con estos requisitos?](#una-empresa-tiene-una-aplicación-que-usa-una-función-programada-de-aws-lambda-para-recuperar-conjuntos-de-datos-de-fuentes-externas-a-través-de-internet-la-función-no-está-asociada-con-una-vpc-la-empresa-está-modificando-la-aplicación-para-almacenar-la-información-que-la-función-lambda-recupera-en-una-instancia-de-base-de-datos-de-amazon-rds-en-una-subred-privada-la-vpc-tiene-dos-subredes-públicas-y-dos-subredes-privadas-un-ingeniero-de-cloudops-debe-desplegar-una-solución-que-permita-a-la-función-lambda-acceder-a-la-nueva-base-de-datos-y-continuar-accediendo-a-internet-qué-solución-cumple-con-estos-requisitos) |
| 77 | [Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred privada usa `CIDR` `20.0.0.0/24`. El ID de la instancia `NAT` es `i-a12345`. ¿Cuál de las siguientes entradas se requiere en la tabla de enrutamiento principal adjunta a la subred privada para permitir que las instancias se conecten a internet?](#un-usuario-ha-creado-una-vpc-con-subredes-públicas-y-privadas-usando-el-asistente-de-vpc-la-vpc-tiene-cidr-2000016-la-subred-privada-usa-cidr-2000024-el-id-de-la-instancia-nat-es-i-a12345-cuál-de-las-siguientes-entradas-se-requiere-en-la-tabla-de-enrutamiento-principal-adjunta-a-la-subred-privada-para-permitir-que-las-instancias-se-conecten-a-internet) |
| 78 | [Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. ¿Cuál de las siguientes afirmaciones es verdadera en este escenario?](#un-usuario-ha-creado-una-vpc-con-subredes-públicas-y-privadas-usando-el-asistente-de-vpc-cuál-de-las-siguientes-afirmaciones-es-verdadera-en-este-escenario) |
| 79 | [Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred privada usa `CIDR` `20.0.0.0/24`. ¿Cuál de las siguientes entradas se requiere en la tabla de enrutamiento principal para permitir que las instancias en la `VPC` se comuniquen entre sí?](#un-usuario-ha-creado-una-vpc-con-subredes-públicas-y-privadas-usando-el-asistente-de-vpc-la-vpc-tiene-cidr-2000016-la-subred-privada-usa-cidr-2000024-cuál-de-las-siguientes-entradas-se-requiere-en-la-tabla-de-enrutamiento-principal-para-permitir-que-las-instancias-en-la-vpc-se-comuniquen-entre-sí) |
| 80 | [Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. El usuario no ha lanzado ninguna instancia manualmente y está intentando eliminar la `VPC`. ¿Qué sucederá en este escenario?](#un-usuario-ha-creado-una-vpc-con-subredes-públicas-y-privadas-usando-el-asistente-de-vpc-el-usuario-no-ha-lanzado-ninguna-instancia-manualmente-y-está-intentando-eliminar-la-vpc-qué-sucederá-en-este-escenario) |
| 81 | [Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred pública usa `CIDR` `20.0.1.0/24`. El usuario planea alojar un servidor web en la subred pública (puerto `80`) y un servidor de base de datos en la subred privada (puerto `3306`). El usuario está configurando un grupo de seguridad para la subred pública (`WebSecGrp`) y la subred privada (`DBSecGrp`). ¿Cuál de las siguientes entradas se requiere en el grupo de seguridad del servidor web (`WebSecGrp`)?](#un-usuario-ha-creado-una-vpc-con-subredes-públicas-y-privadas-usando-el-asistente-de-vpc-la-vpc-tiene-cidr-2000016-la-subred-pública-usa-cidr-2001024-el-usuario-planea-alojar-un-servidor-web-en-la-subred-pública-puerto-80-y-un-servidor-de-base-de-datos-en-la-subred-privada-puerto-3306-el-usuario-está-configurando-un-grupo-de-seguridad-para-la-subred-pública-websecgrp-y-la-subred-privada-dbsecgrp-cuál-de-las-siguientes-entradas-se-requiere-en-el-grupo-de-seguridad-del-servidor-web-websecgrp) |
| 82 | [Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado una subred pública `CIDR` `20.0.0.0/24` y subredes solo `VPN` `CIDR` `20.0.1.0/24` junto con la puerta de enlace `VPN` `vgw-12345` para conectarse al centro de datos del usuario. ¿Cuál de las siguientes opciones es una entrada válida para la tabla de enrutamiento principal en este escenario?](#un-usuario-ha-creado-una-vpc-con-cidr-2000016-usando-el-asistente-el-usuario-ha-creado-una-subred-pública-cidr-2000024-y-subredes-solo-vpn-cidr-2001024-junto-con-la-puerta-de-enlace-vpn-vgw-12345-para-conectarse-al-centro-de-datos-del-usuario-cuál-de-las-siguientes-opciones-es-una-entrada-válida-para-la-tabla-de-enrutamiento-principal-en-este-escenario) |
| 83 | [Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred pública usa `CIDR` `20.0.1.0/24`. El usuario planea alojar un servidor web en la subred pública (puerto `80`) y un servidor de base de datos en la subred privada (puerto `3306`). El usuario está configurando un grupo de seguridad para la subred pública (`WebSecGrp`) y la subred privada (`DBSecGrp`). ¿Cuál de las siguientes entradas se requiere en el grupo de seguridad de la base de datos de la subred privada (`DBSecGrp`)?](#un-usuario-ha-creado-una-vpc-con-subredes-públicas-y-privadas-usando-el-asistente-de-vpc-la-vpc-tiene-cidr-2000016-la-subred-pública-usa-cidr-2001024-el-usuario-planea-alojar-un-servidor-web-en-la-subred-pública-puerto-80-y-un-servidor-de-base-de-datos-en-la-subred-privada-puerto-3306-el-usuario-está-configurando-un-grupo-de-seguridad-para-la-subred-pública-websecgrp-y-la-subred-privada-dbsecgrp-cuál-de-las-siguientes-entradas-se-requiere-en-el-grupo-de-seguridad-de-la-base-de-datos-de-la-subred-privada-dbsecgrp) |
| 84 | [Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente de `VPC`. El usuario ha creado un `CIDR` público `20.0.0.0/24` y una subred solo `VPN` `CIDR` `20.0.1.0/24` junto con el acceso `VPN` de hardware para conectarse al centro de datos del usuario. ¿Cuál de los siguientes componentes NO está presente cuando la `VPC` se configura con el asistente?](#un-usuario-ha-creado-una-vpc-con-cidr-2000016-usando-el-asistente-de-vpc-el-usuario-ha-creado-un-cidr-público-2000024-y-una-subred-solo-vpn-cidr-2001024-junto-con-el-acceso-vpn-de-hardware-para-conectarse-al-centro-de-datos-del-usuario-cuál-de-los-siguientes-componentes-no-está-presente-cuando-la-vpc-se-configura-con-el-asistente) |
| 85 | [Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado subredes públicas y solo `VPN` junto con acceso `VPN` de hardware para conectarse al centro de datos del usuario. El usuario aún no ha lanzado ninguna instancia ni ha modificado o eliminado ninguna configuración. Quiere eliminar esta `VPC` desde la consola. ¿La consola permitirá al usuario eliminar la `VPC`?](#un-usuario-ha-creado-una-vpc-con-cidr-2000016-usando-el-asistente-el-usuario-ha-creado-subredes-públicas-y-solo-vpn-junto-con-acceso-vpn-de-hardware-para-conectarse-al-centro-de-datos-del-usuario-el-usuario-aún-no-ha-lanzado-ninguna-instancia-ni-ha-modificado-o-eliminado-ninguna-configuración-quiere-eliminar-esta-vpc-desde-la-consola-la-consola-permitirá-al-usuario-eliminar-la-vpc) |
| 86 | [Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado una subred pública `CIDR` `20.0.0.0/24` y subredes solo `VPN` `CIDR` `20.0.1.0/24` junto con la puerta de enlace `VPN` `vgw-12345` para conectarse al centro de datos del usuario. El centro de datos del usuario tiene `CIDR` `172.28.0.0/12`. El usuario también ha configurado una instancia `NAT` `i-123456` para permitir tráfico a internet desde la subred `VPN`. ¿Cuál de las siguientes opciones NO es una entrada válida para la tabla de enrutamiento principal en este escenario?](#un-usuario-ha-creado-una-vpc-con-cidr-2000016-usando-el-asistente-el-usuario-ha-creado-una-subred-pública-cidr-2000024-y-subredes-solo-vpn-cidr-2001024-junto-con-la-puerta-de-enlace-vpn-vgw-12345-para-conectarse-al-centro-de-datos-del-usuario-el-centro-de-datos-del-usuario-tiene-cidr-172280012-el-usuario-también-ha-configurado-una-instancia-nat-i-123456-para-permitir-tráfico-a-internet-desde-la-subred-vpn-cuál-de-las-siguientes-opciones-no-es-una-entrada-válida-para-la-tabla-de-enrutamiento-principal-en-este-escenario) |

### Una instancia de Amazon EC2 necesita ser accesible desde internet. La instancia de EC2 está en una subred con la siguiente tabla de enrutamiento. ¿Qué entrada debe agregar un ingeniero de CloudOps a la tabla de enrutamiento para cumplir con este requisito?

![Question 1](images/question1.jpg)

- [ ] Una ruta para `0.0.0.0/0` que apunte a una puerta de enlace `NAT`.
- [ ] Una ruta para `0.0.0.0/0` que apunte a una puerta de enlace de internet solo de salida (egress-only).
- [x] Una ruta para `0.0.0.0/0` que apunte a una puerta de enlace de internet.
- [ ] Una ruta para `0.0.0.0/0` que apunte a una interfaz de red elástica.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps lanza una instancia de Amazon EC2 en una subred privada de una `VPC`. Cuando el ingeniero de CloudOps intenta ejecutar un comando `curl` desde la línea de comandos de la instancia de EC2, no logra conectarse a `https:www.example.com`. ¿Qué debe hacer el ingeniero de CloudOps para resolver este problema?

- [x] Asegurarse de que exista un grupo de seguridad de salida que permita el puerto `443` hacia `0.0.0.0/0`.
- [ ] Asegurarse de que exista un grupo de seguridad de entrada que permita el puerto `443` desde `0.0.0.0/0`.
- [ ] Asegurarse de que exista una `ACL` de red de salida para los puertos efímeros `1024-66535` hacia `0.0.0.0/0`.
- [ ] Asegurarse de que exista una `ACL` de red de salida para el puerto `80` hacia `0.0.0.0/0`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps lanza una instancia de Amazon EC2 con Linux en una subred pública. Una vez que la instancia está en ejecución, el ingeniero de CloudOps obtiene la dirección IP pública e intenta conectarse remotamente a la instancia varias veces. Sin embargo, siempre recibe un error de tiempo de espera (timeout). ¿Qué acción permitirá al ingeniero de CloudOps conectarse remotamente a la instancia?

- [ ] Agregar una entrada en la tabla de enrutamiento de la subred pública para la dirección IP del ingeniero de CloudOps.
- [ ] Agregar una regla de `ACL` de red de salida que permita el puerto `TCP` `22` para la dirección IP del ingeniero de CloudOps.
- [x] Modificar el grupo de seguridad de la instancia para permitir tráfico `SSH` de entrada desde la dirección IP del ingeniero de CloudOps.
- [ ] Modificar el grupo de seguridad de la instancia para permitir tráfico `SSH` de salida hacia la dirección IP del ingeniero de CloudOps.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa quiere usar únicamente IPv6 para todas sus instancias de Amazon EC2. Las instancias de EC2 no deben ser accesibles desde internet, pero sí deben poder acceder a internet. La empresa crea una `VPC` de doble pila (dual-stack) y subredes exclusivas de IPv6. ¿Cómo debe configurar un ingeniero de CloudOps la `VPC` para cumplir con estos requisitos?

- [ ] Crear y adjuntar una puerta de enlace `NAT`. Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace `NAT`. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.
- [ ] Crear y adjuntar una puerta de enlace de internet. Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace de internet. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.
- [x] Crear y adjuntar una puerta de enlace de internet solo de salida (egress-only). Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace de internet solo de salida. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.
- [ ] Crear y adjuntar una puerta de enlace de internet y una puerta de enlace `NAT`. Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace de internet y todo el tráfico IPv4 hacia la puerta de enlace `NAT`. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa planea ejecutar una aplicación web pública en instancias de Amazon EC2 detrás de un Elastic Load Balancer (ELB). El equipo de seguridad de la empresa quiere proteger el sitio web usando certificados de AWS Certificate Manager (ACM). El ELB debe redirigir automáticamente todas las solicitudes `HTTP` a `HTTPS`. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un Application Load Balancer con un listener `HTTPS` en el puerto `80`. Adjuntar un certificado SSL/TLS al listener del puerto `80`. Crear una regla para redirigir las solicitudes de `HTTP` a `HTTPS`.
- [x] Crear un Application Load Balancer con un listener `HTTP` en el puerto `80` y un listener con protocolo `HTTPS` en el puerto `443`. Adjuntar un certificado SSL/TLS al listener del puerto `443`. Crear una regla para redirigir las solicitudes del puerto `80` al puerto `443`.
- [ ] Crear un Application Load Balancer con dos listeners `TCP` en el puerto `80` y el puerto `443`. Adjuntar un certificado SSL/TLS al listener del puerto `443`. Crear una regla para redirigir las solicitudes del puerto `80` al puerto `443`.
- [ ] Crear un Network Load Balancer con dos listeners `TCP` en el puerto `80` y el puerto `443`. Adjuntar un certificado SSL/TLS al listener del puerto `443`. Crear una regla para redirigir las solicitudes del puerto `80` al puerto `443`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa migró recientemente su aplicación a una `VPC` en AWS. Una conexión AWS Site-to-Site `VPN` conecta la red on-premises de la empresa con la `VPC`. La aplicación obtiene datos de clientes desde otro sistema que reside on-premises. La aplicación usa un servidor `DNS` on-premises para resolver registros de dominio. Después de la migración, la aplicación no puede conectarse a los datos de clientes debido a errores de resolución de nombres. ¿Qué solución le dará a la aplicación la capacidad de resolver los nombres de dominio internos?

- [ ] Lanzar instancias de EC2 en la `VPC`. En las instancias de EC2, desplegar un reenviador (forwarder) `DNS` personalizado que envíe todas las solicitudes `DNS` al servidor `DNS` on-premises. Crear una zona alojada privada de Amazon Route 53 que use las instancias de EC2 como servidores de nombres.
- [x] Crear un endpoint de salida (outbound endpoint) de Amazon Route 53 Resolver. Configurar el endpoint de salida para reenviar las consultas `DNS` del dominio on-premises al servidor `DNS` on-premises.
- [ ] Configurar dos conexiones AWS Direct Connect entre el entorno de AWS y la red on-premises. Configurar un grupo de agregación de enlaces (LAG) que incluya ambas conexiones. Cambiar la dirección del resolver de la `VPC` para que apunte al servidor `DNS` on-premises.
- [ ] Crear una zona alojada pública de Amazon Route 53 para el dominio on-premises. Configurar las `ACL`s de red para reenviar las solicitudes `DNS` del dominio on-premises a la zona alojada pública de Route 53.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps crea una nueva `VPC` que incluye una subred pública y una subred privada. El ingeniero de CloudOps lanza con éxito 11 instancias de Amazon EC2 en la subred privada. El ingeniero de CloudOps intenta lanzar una instancia de EC2 adicional en la misma subred, pero recibe un mensaje de error que indica que no hay suficientes direcciones IP libres disponibles. ¿Qué debe hacer el ingeniero de CloudOps para desplegar más instancias de EC2?

- [ ] Editar la subred privada para cambiar el bloque `CIDR` a `/27`.
- [ ] Editar la subred privada para que se extienda a través de una segunda Zona de disponibilidad.
- [ ] Asignar direcciones IP elásticas adicionales a la subred privada.
- [x] Crear una nueva subred privada para alojar las instancias de EC2 requeridas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está intentando descargar parches de internet hacia una instancia en una subred privada. Existe una puerta de enlace de internet para la `VPC`, y se ha desplegado una puerta de enlace `NAT` en la subred pública; sin embargo, la instancia no tiene conectividad a internet. Los recursos desplegados en la subred privada deben ser inaccesibles directamente desde internet público. Dada la información proporcionada, ¿qué se debe agregar a la tabla de enrutamiento de la subred privada para resolver este problema?

![Question 42](images/question42.png)

- [ ] `0.0.0.0/0` `IGW`.
- [x] `0.0.0.0/0` `NAT`.
- [ ] `10.0.1.0/24` `IGW`.
- [ ] `10.0.1.0/24` `NAT`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una conexión AWS Site-to-Site `VPN` entre recursos on-premises y recursos alojados en una `VPC`. Un ingeniero de CloudOps lanza una instancia de Amazon EC2 que solo tiene una dirección IP privada en una subred privada de la `VPC`. La instancia de EC2 ejecuta Microsoft Windows Server. Un grupo de seguridad de la instancia de EC2 tiene reglas que permiten tráfico de entrada desde la red on-premises a través de la conexión `VPN`. El entorno on-premises contiene un firewall de red de un tercero. Las reglas de ese firewall permiten que el tráfico de Remote Desktop Protocol (RDP) fluya entre los usuarios on-premises a través de la conexión `VPN`. Los usuarios on-premises no pueden conectarse a la instancia de EC2 y reciben un error de tiempo de espera (timeout). ¿Qué debe hacer el ingeniero de CloudOps para solucionar este problema?

- [ ] Crear registros de Amazon CloudWatch para la instancia de EC2 y verificar si hay tráfico bloqueado.
- [ ] Crear registros de Amazon CloudWatch para la conexión Site-to-Site `VPN` y verificar si hay tráfico bloqueado.
- [x] Crear registros de flujo (`VPC` flow logs) para la interfaz de red elástica de la instancia de EC2 y verificar si hay tráfico rechazado.
- [ ] Indicar a los usuarios que usen EC2 Instance Connect como método de conexión.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está desplegando un sitio de prueba que se ejecuta en instancias de Amazon EC2. La aplicación requiere conectividad tanto de entrada como de salida hacia internet. ¿Qué combinación de pasos se requiere para proporcionar conectividad a internet a las instancias de EC2? (Elija dos.)

- [ ] Agregar una puerta de enlace `NAT` a una subred pública.
- [ ] Adjuntar una dirección privada a la interfaz de red elástica de la instancia de EC2.
- [ ] Adjuntar una dirección IP elástica a la puerta de enlace de internet.
- [x] Agregar una entrada en la tabla de enrutamiento de la subred que apunte a una puerta de enlace de internet.
- [x] Crear una puerta de enlace de internet y adjuntarla a una `VPC`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está investigando por qué un usuario no ha podido usar `RDP` para conectarse a través de internet desde su computadora personal a un servidor bastión que se ejecuta en una instancia de Amazon EC2 con Windows. ¿Cuáles de las siguientes son posibles causas de este problema? (Elija dos.)

- [x] Una `ACL` de red asociada a la subred del bastión está bloqueando el tráfico de red.
- [ ] La instancia no tiene una dirección IP privada.
- [x] La tabla de enrutamiento asociada a la subred del bastión no tiene una ruta hacia la puerta de enlace de internet.
- [ ] El grupo de seguridad de la instancia no tiene una regla de entrada en el puerto `22`.
- [ ] El grupo de seguridad de la instancia no tiene una regla de salida en el puerto `3389`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Mientras aseguraba la conexión entre la `VPC` de una empresa y su centro de datos on-premises, un ingeniero de seguridad envió un comando ping desde un host on-premises (dirección IP `203.0.113.12`) hacia una instancia de Amazon EC2 (dirección IP `172.31.16.139`). El comando ping no obtuvo respuesta. El registro de flujo (flow log) de la `VPC` mostró lo siguiente. ¿Qué acción se debe realizar para que el ping funcione?

![Question 58](images/question58_74_155.png)

- [ ] En el grupo de seguridad de la instancia de EC2, permitir tráfico `ICMP` de entrada.
- [ ] En el grupo de seguridad de la instancia de EC2, permitir tráfico `ICMP` de salida.
- [ ] En la `NACL` de la `VPC`, permitir tráfico `ICMP` de entrada.
- [x] En la `NACL` de la `VPC`, permitir tráfico `ICMP` de salida.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa global maneja una gran cantidad de información de identificación personal (PII, por sus siglas en inglés) a través de un portal web interno. La aplicación de la empresa se ejecuta en un centro de datos corporativo que está conectado a AWS mediante una conexión de AWS Direct Connect. La aplicación almacena la PII en Amazon S3. Según un requisito de cumplimiento normativo, el tráfico desde el portal web hacia Amazon S3 no debe transitar por internet. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con el requisito de cumplimiento?

- [x] Aprovisionar un endpoint de interfaz de `VPC` para Amazon S3. Modificar la aplicación para que use el endpoint de interfaz.
- [ ] Configurar AWS Network Firewall para redirigir el tráfico a la dirección interna de S3.
- [ ] Modificar la aplicación para que use el endpoint de estilo de ruta (path-style) de S3.
- [ ] Configurar un conjunto de `ACL`s de red de `VPC` para redirigir el tráfico a la dirección interna de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa Amazon Elastic Container Service (Amazon ECS) para ejecutar una aplicación en contenedores sobre instancias de Amazon EC2. Un ingeniero de CloudOps necesita monitorear únicamente los flujos de tráfico entre las tareas (tasks) de ECS. ¿Qué combinación de pasos debe seguir el ingeniero de CloudOps para cumplir con este requisito? (Seleccione DOS.)

- [ ] Configurar Amazon CloudWatch Logs en la interfaz de red elástica de cada tarea.
- [x] Configurar registros de flujo (`VPC` Flow Logs) en la interfaz de red elástica de cada tarea.
- [x] Especificar el modo de red `awsvpc` en la definición de la tarea.
- [ ] Especificar el modo de red `bridge` en la definición de la tarea.
- [ ] Especificar el modo de red `host` en la definición de la tarea.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación web con estado (stateful) alojada en instancias de Amazon EC2 dentro de un grupo de Auto Scaling. Las instancias se ejecutan detrás de un Application Load Balancer (ALB) que tiene un único grupo de destino. El `ALB` está configurado como origen en una distribución de Amazon CloudFront. Los usuarios reportan cierres de sesión aleatorios en la aplicación web. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para resolver este problema? (Seleccione DOS.)

- [ ] Cambiar al algoritmo de solicitudes pendientes mínimas (least outstanding requests) en el grupo de destino del `ALB`.
- [x] Configurar el reenvío de cookies (cookie forwarding) en el comportamiento de caché de la distribución de CloudFront.
- [ ] Configurar el reenvío de encabezados (header forwarding) en el comportamiento de caché de la distribución de CloudFront.
- [ ] Habilitar la persistencia a nivel de grupo (group-level stickiness) en la regla del listener del `ALB`.
- [x] Habilitar sesiones persistentes (sticky sessions) en el grupo de destino del `ALB`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una `VPC` está conectada al centro de datos de una empresa mediante una `VPN`. Una instancia de Amazon EC2 con la dirección IP `172.31.16.139` está dentro de una subred privada de la `VPC`. Un ingeniero de CloudOps envió un comando ping a la instancia de EC2 desde una computadora on-premises con la dirección IP `203.0.113.12` y no recibió confirmación. Los registros de flujo (`VPC` Flow Logs) estaban habilitados y mostraron lo siguiente. ¿Qué acción resolverá el problema?

![Question 74](images/question58_74_155.png)

- [ ] Modificar las reglas del grupo de seguridad de EC2 para permitir tráfico de entrada desde la computadora on-premises.
- [ ] Modificar las reglas del grupo de seguridad de EC2 para permitir tráfico de salida hacia la computadora on-premises.
- [ ] Modificar las reglas de la `ACL` de red de la `VPC` para permitir tráfico de entrada desde la computadora on-premises.
- [x] Modificar las reglas de la `ACL` de red de la `VPC` para permitir tráfico de salida hacia la computadora on-premises.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps mantiene varias instancias de Amazon EC2 que no tienen acceso a internet público. Para aplicar parches a los sistemas operativos, las instancias requieren conectividad de salida a internet. Por razones de seguridad, las instancias no deben ser accesibles desde internet público. El ingeniero despliega una instancia `NAT`, actualiza los grupos de seguridad y configura las rutas apropiadas en la tabla de enrutamiento. Sin embargo, las instancias aún no pueden llegar a internet. ¿Qué se debe hacer para resolver el problema?

- [ ] Asignar direcciones IP elásticas a las instancias y crear una ruta desde las subredes privadas hacia la puerta de enlace de internet.
- [ ] Eliminar la instancia `NAT` y reemplazarla con AWS WAF.
- [x] Deshabilitar las verificaciones de origen/destino (source/destination checks) en la instancia `NAT`.
- [ ] Detener e iniciar la instancia `NAT` para que se lance en un host diferente.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa necesita desplegar una aplicación web en dos instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). También se desplegarán dos instancias de EC2 para alojar la base de datos. La infraestructura debe diseñarse a través de Zonas de disponibilidad para alta disponibilidad y debe limitar el acceso público a las instancias tanto como sea posible. ¿Cómo se debe lograr esto dentro de una `VPC`?

- [ ] Crear una subred pública para el Application Load Balancer, una subred pública para los servidores web y una subred privada para los servidores de base de datos.
- [ ] Crear una subred pública para el Application Load Balancer, dos subredes públicas para los servidores web y dos subredes privadas para los servidores de base de datos.
- [x] Crear dos subredes públicas para el Application Load Balancer, dos subredes privadas para los servidores web y dos subredes privadas para los servidores de base de datos.
- [ ] Crear dos subredes públicas para el Application Load Balancer, dos subredes públicas para los servidores web y dos subredes públicas para los servidores de base de datos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una distribución de Amazon CloudFront que usa un bucket de Amazon S3 como origen. Durante una revisión de los registros de acceso, la empresa determina que algunas solicitudes van directamente al bucket de S3 usando el endpoint de alojamiento de sitio web (website hosting endpoint). Un ingeniero de CloudOps debe proteger el bucket de S3 para permitir solicitudes únicamente desde CloudFront. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [x] Crear una Identidad de Acceso de Origen (OAI) en CloudFront. Asociar la OAI con la distribución. Eliminar el acceso hacia y desde otros principales en la política del bucket de S3. Actualizar la política del bucket de S3 para permitir acceso únicamente desde la OAI.
- [ ] Crear una Identidad de Acceso de Origen (OAI) en CloudFront. Asociar la OAI con la distribución. Actualizar la política del bucket de S3 para permitir acceso únicamente desde la OAI. Crear un nuevo origen y especificar el bucket de S3 como el nuevo origen. Actualizar el comportamiento de la distribución para usar el nuevo origen. Eliminar el origen existente.
- [ ] Crear una Identidad de Acceso de Origen (OAI) en CloudFront. Asociar la OAI con la distribución. Actualizar la política del bucket de S3 para permitir acceso únicamente desde la OAI. Deshabilitar el alojamiento de sitio web. Crear un nuevo origen y especificar el bucket de S3 como el nuevo origen. Actualizar el comportamiento de la distribución para usar el nuevo origen. Eliminar el origen existente.
- [ ] Actualizar la política del bucket de S3 para permitir acceso únicamente desde la distribución de CloudFront. Eliminar el acceso hacia y desde otros principales en la política del bucket de S3. Deshabilitar el alojamiento de sitio web. Crear un nuevo origen y especificar el bucket de S3 como el nuevo origen. Actualizar el comportamiento de la distribución para usar el nuevo origen. Eliminar el origen existente.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está intentando conectar dos aplicaciones. Una aplicación se ejecuta en un centro de datos on-premises con el nombre de host hostl.onprem.private. La otra aplicación se ejecuta en una instancia de Amazon EC2 con el nombre de host `hostl.awscloud.private`. Existe una conexión AWS Site-to-Site `VPN` entre la red on-premises y AWS. La aplicación que se ejecuta en el centro de datos intenta conectarse a la aplicación que se ejecuta en la instancia de EC2, pero la resolución `DNS` falla. Un ingeniero de CloudOps debe implementar resolución `DNS` entre los recursos on-premises y los de AWS. ¿Qué solución permite que la aplicación on-premises resuelva el nombre de host de la instancia de EC2?

- [ ] Configurar un endpoint de resolución de entrada (inbound resolver) de Amazon Route 53 con una regla de reenvío para la zona alojada onprem.private. Asociar el resolver con la `VPC` de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de onprem.private al endpoint de resolución de entrada.
- [x] Configurar un endpoint de resolución de entrada de Amazon Route 53. Asociar el resolver con la `VPC` de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de awscloud.private al endpoint de resolución de entrada.
- [ ] Configurar un endpoint de resolución de salida (outbound resolver) de Amazon Route 53 con una regla de reenvío para la zona alojada onprem.private. Asociar el resolver con la región de AWS de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de onprem.private al endpoint de resolución de salida.
- [ ] Configurar un endpoint de resolución de salida de Amazon Route 53. Asociar el resolver con la región de AWS de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de awscloud.private al endpoint de resolución de salida.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Al configurar una conexión `VPN` administrada por AWS, un ingeniero de CloudOps crea un recurso de gateway de cliente (customer gateway) en AWS. El dispositivo de gateway del cliente reside en un centro de datos con una puerta de enlace `NAT` frente a él. ¿Qué dirección se debe usar para crear el recurso de gateway del cliente?

- [ ] La dirección IP privada del dispositivo de gateway del cliente.
- [ ] La dirección MAC del dispositivo `NAT` frente al dispositivo de gateway del cliente.
- [ ] La dirección IP pública del dispositivo de gateway del cliente.
- [x] La dirección IP pública del dispositivo `NAT` frente al dispositivo de gateway del cliente.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El sitio web de una empresa contiene una capa web y una capa de base de datos en AWS. La capa web consiste en instancias de Amazon EC2 que se ejecutan en un grupo de Auto Scaling distribuido en dos Zonas de disponibilidad. La capa de base de datos se ejecuta en una instancia de Amazon RDS for MySQL Multi-AZ. Las `ACL`s de red de la subred de base de datos están restringidas únicamente a las subredes web que necesitan acceso a la base de datos. Las subredes web usan la `ACL` de red predeterminada con las reglas por defecto. El equipo de operaciones de la empresa ha agregado una tercera subred a la configuración del grupo de Auto Scaling. Después de que ocurre un evento de Auto Scaling, algunos usuarios reportan que reciben intermitentemente un mensaje de error. El mensaje de error indica que el servidor no puede conectarse a la base de datos. El equipo de operaciones ha confirmado que las tablas de enrutamiento son correctas y que los puertos requeridos están abiertos en todos los grupos de seguridad. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para que los servidores web puedan comunicarse con la instancia de base de datos? (Seleccione DOS.)

- [ ] En la `ACL` predeterminada, crear una regla de entrada de tipo Allow para `TCP` con el rango de puertos efímeros y como origen las subredes de base de datos.
- [ ] En la `ACL` predeterminada, crear una regla de salida de tipo Allow para `MySQL/Aurora (3306)`. Especificar como destinos las subredes de base de datos.
- [x] En las `ACL`s de red de las subredes de base de datos, crear una regla de entrada de tipo Allow para `MySQL/Aurora (3306)`. Especificar como origen la tercera subred web.
- [x] En las `ACL`s de red de las subredes de base de datos, crear una regla de salida de tipo Allow para `TCP` con el rango de puertos efímeros y como destino la tercera subred web.
- [ ] En las `ACL`s de red de las subredes de base de datos, crear una regla de salida de tipo Allow para `MySQL/Aurora (3306)`. Especificar como destino la tercera subred web.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### La infraestructura backend de una empresa contiene una instancia de Amazon EC2 en una subred privada. La subred privada tiene una ruta a internet a través de una puerta de enlace `NAT` en una subred pública. La instancia debe permitir conectividad hacia un servidor web seguro en internet para recuperar datos a intervalos regulares. El software cliente agota el tiempo de espera con un mensaje de error que indica que no pudo establecer la conexión `TCP`. ¿Qué debe hacer un ingeniero de CloudOps para resolver este error?

- [ ] Agregar una regla de entrada al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTP`, `Source` – `0.0.0.0/0`.
- [ ] Agregar una regla de entrada al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTPS`, `Source` – `0.0.0.0/0`.
- [ ] Agregar una regla de salida al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTP`, `Destination` – `0.0.0.0/0`.
- [x] Agregar una regla de salida al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTPS`, `Destination` – `0.0.0.0/0`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa almacena archivos en 50 buckets de Amazon S3 dentro de la misma región de AWS. La empresa quiere conectarse a los buckets de S3 de forma segura a través de una conexión privada desde sus instancias de Amazon EC2. La empresa necesita una solución que no genere costo adicional. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un endpoint de `VPC` de tipo gateway para cada bucket de S3. Adjuntar los endpoints de `VPC` de tipo gateway a cada subred dentro de la `VPC`.
- [ ] Crear un endpoint de `VPC` de tipo interfaz para cada bucket de S3. Adjuntar los endpoints de `VPC` de tipo interfaz a cada subred dentro de la `VPC`.
- [x] Crear un único endpoint de `VPC` de tipo gateway para todos los buckets de S3. Agregar el endpoint de `VPC` de tipo gateway a la tabla de enrutamiento de la `VPC`.
- [ ] Crear un único endpoint de `VPC` de tipo interfaz para todos los buckets de S3. Agregar el endpoint de `VPC` de tipo interfaz a la tabla de enrutamiento de la `VPC`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está solucionando problemas de tiempo de espera de conexión hacia una instancia de Amazon EC2 que tiene una dirección IP pública. La instancia tiene una dirección IP privada `172.31.16.139`. Cuando el ingeniero de CloudOps intenta hacer ping a la dirección IP pública de la instancia desde la dirección IP remota `203.0.113.12`, la respuesta es `request timed out`. Los registros de flujo contienen la siguiente información. ¿Cuál es una causa del problema?

![Question 155](images/question58_74_155.png)

- [ ] Regla de denegación de entrada del grupo de seguridad.
- [ ] Regla de denegación de salida del grupo de seguridad.
- [ ] Reglas de entrada de la `ACL` de red.
- [x] Reglas de salida de la `ACL` de red.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita configurar una solución que entregue contenido digital a un conjunto de usuarios autorizados a través de Amazon CloudFront. Los usuarios no autorizados deben quedar restringidos del acceso. ¿Qué solución cumple con estos requisitos?

- [ ] Almacenar el contenido digital en un bucket de Amazon S3 que no tenga el acceso público bloqueado. Usar URLs firmadas para acceder al bucket de S3 a través de CloudFront.
- [x] Almacenar el contenido digital en un bucket de Amazon S3 que tenga el acceso público bloqueado. Usar una Identidad de Acceso de Origen (OAI) para entregar el contenido a través de CloudFront. Restringir el acceso al bucket de S3 con URLs firmadas en CloudFront.
- [ ] Almacenar el contenido digital en un bucket de Amazon S3 que tenga el acceso público bloqueado. Usar una Identidad de Acceso de Origen (OAI) para entregar el contenido a través de CloudFront. Habilitar el cifrado a nivel de campo (field-level encryption).
- [ ] Almacenar el contenido digital en un bucket de Amazon S3 que no tenga el acceso público bloqueado. Usar cookies firmadas para la entrega restringida del contenido a través de CloudFront.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha desplegado una aplicación en instancias de Amazon EC2 dentro de una única `VPC`. La empresa ha colocado las instancias de EC2 en una subred privada de la `VPC`. Las instancias de EC2 necesitan acceso a buckets de Amazon S3 que están en la misma región de AWS que las instancias de EC2. Un ingeniero de CloudOps debe proporcionar a las instancias de EC2 acceso a los buckets de S3 sin requerir ningún cambio en las instancias de EC2 ni en la aplicación. Las instancias de EC2 no deben tener acceso a internet. ¿Qué solución cumple con estos requisitos?

- [x] Crear un endpoint de gateway de S3 que use la política de endpoint de gateway predeterminada. Asociar la subred privada con el endpoint de gateway.
- [ ] Crear un endpoint de interfaz de S3. Asociar las instancias de EC2 con el endpoint de interfaz.
- [ ] Configurar una puerta de enlace `NAT`. Asociar la subred privada con la puerta de enlace `NAT`.
- [ ] Configurar una instancia de EC2 proxy. Actualizar las tablas de enrutamiento de la subred privada para enrutar el tráfico a través de la instancia de EC2 proxy. Configurar el proxy para enrutar todas las solicitudes de S3 al bucket de S3 objetivo.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa actualmente ejecuta su infraestructura dentro de una `VPC` en una sola Zona de disponibilidad. La `VPC` está conectada al centro de datos on-premises de la empresa a través de una conexión AWS Site-to-Site `VPN` adjunta a una puerta de enlace privada virtual. Las tablas de enrutamiento on-premises enrutan todas las redes de la `VPC` hacia la conexión `VPN`. La comunicación entre ambos entornos funciona correctamente. Un ingeniero de CloudOps creó nuevas subredes de `VPC` dentro de una nueva Zona de disponibilidad, y desplegó nuevos recursos dentro de esas subredes. Sin embargo, no se puede establecer comunicación entre los nuevos recursos y el entorno on-premises. ¿Qué pasos debe tomar el ingeniero de CloudOps para resolver el problema?

- [x] Agregar una ruta a las tablas de enrutamiento de las nuevas subredes que envíe el tráfico on-premises hacia la puerta de enlace privada virtual.
- [ ] Crear un ticket con AWS Support para solicitar agregar Zonas de disponibilidad a la configuración de ruta de la Site-to-Site `VPN`.
- [ ] Establecer una nueva conexión Site-to-Site `VPN` entre una puerta de enlace privada virtual adjunta a la nueva Zona de disponibilidad y el centro de datos on-premises.
- [ ] Reemplazar la conexión Site-to-Site `VPN` con una conexión de AWS Direct Connect.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está ejecutando un sitio web en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa configuró una distribución de Amazon CloudFront y estableció el `ALB` como origen. La empresa creó un registro `CNAME` de Amazon Route 53 para enviar todo el tráfico a través de la distribución de CloudFront. Como efecto secundario no deseado, ahora se está sirviendo a los usuarios móviles la versión de escritorio del sitio web. ¿Qué acción debe tomar un ingeniero de CloudOps para resolver este problema?

- [x] Configurar el comportamiento de la distribución de CloudFront para reenviar el encabezado `User-Agent`.
- [ ] Configurar la configuración de origen de la distribución de CloudFront. Agregar un encabezado `User-Agent` a la lista de encabezados personalizados de origen.
- [ ] Habilitar IPv6 en el `ALB`. Actualizar la configuración de origen de la distribución de CloudFront para usar el endpoint de doble pila (dualstack).
- [ ] Habilitar IPv6 en la distribución de CloudFront. Actualizar el registro de Route 53 para usar el endpoint de doble pila.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja su sitio web en instancias de Amazon EC2 detrás de un Application Load Balancer. La empresa administra su `DNS` con Amazon Route 53, y quiere apuntar el ápice de zona (zone apex) de su dominio hacia el sitio web. ¿Qué tipo de registro se debe usar para cumplir con estos requisitos?

- [ ] Un registro `AAAA` para el ápice de zona del dominio.
- [ ] Un registro `A` para el ápice de zona del dominio.
- [ ] Un registro `CNAME` para el ápice de zona del dominio.
- [x] Un registro de alias para el ápice de zona del dominio.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps ha creado una `VPC` que contiene una subred pública y una subred privada. Las instancias de Amazon EC2 que se lanzaron en la subred privada no pueden acceder a internet. La `ACL` de red predeterminada está activa en todas las subredes de la `VPC`, y todos los grupos de seguridad permiten todo el tráfico de salida. ¿Qué solución proporcionará a las instancias de EC2 en la subred privada acceso a internet?

- [x] Crear una puerta de enlace `NAT` en la subred pública. Crear una ruta desde la subred privada hacia la puerta de enlace `NAT`.
- [ ] Crear una puerta de enlace `NAT` en la subred pública. Crear una ruta desde la subred pública hacia la puerta de enlace `NAT`.
- [ ] Crear una puerta de enlace `NAT` en la subred privada. Crear una ruta desde la subred pública hacia la puerta de enlace `NAT`.
- [ ] Crear una puerta de enlace `NAT` en la subred privada. Crear una ruta desde la subred privada hacia la puerta de enlace `NAT`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja un sitio web estático en Amazon S3. El sitio web es servido por una distribución de Amazon CloudFront con un `TTL` predeterminado de 86,400 segundos. La empresa recientemente subió una versión actualizada del sitio web a Amazon S3. Sin embargo, los usuarios siguen viendo el contenido antiguo cuando actualizan el sitio. Un ingeniero de CloudOps debe hacer visible la nueva versión del sitio web a los usuarios lo antes posible. ¿Qué solución cumple con estos requisitos?

- [ ] Ajustar el valor de `TTL` para el registro `CNAME` de `DNS` que apunta a la distribución de CloudFront.
- [x] Crear una invalidación en la distribución de CloudFront para los objetos antiguos de S3.
- [ ] Crear una nueva distribución de CloudFront. Actualizar los registros `DNS` para que apunten a la nueva distribución de CloudFront.
- [ ] Actualizar el registro `DNS` del sitio web para que apunte al bucket de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un nuevo sitio web se ejecutará en instancias de Amazon EC2 detrás de un Application Load Balancer. Amazon Route 53 se usará para administrar los registros `DNS`. ¿Qué tipo de registro se debe configurar en Route 53 para que el nombre de dominio raíz del sitio web (por ejemplo, `company.com`) apunte al Application Load Balancer?

- [ ] `CNAME`.
- [ ] `SOA`.
- [ ] `TXT`.
- [x] `ALIAS`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa planea alojar una aplicación en un conjunto de instancias de Amazon EC2 distribuidas entre múltiples Zonas de disponibilidad. La aplicación debe poder escalar a millones de solicitudes por segundo. Un ingeniero de CloudOps debe diseñar una solución para distribuir el tráfico a las instancias de EC2. La solución debe estar optimizada para manejar patrones de tráfico repentinos y volátiles, usando una única dirección IP estática por cada Zona de disponibilidad. ¿Qué solución cumple con estos requisitos?

- [ ] Cola de Amazon Simple Queue Service (Amazon SQS).
- [ ] Application Load Balancer.
- [ ] AWS Global Accelerator.
- [x] Network Load Balancer.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps migra instancias `NAT` a puertas de enlace `NAT`. Después de la migración, una aplicación alojada en instancias de Amazon EC2 en una subred privada no puede acceder a internet. ¿Cuáles de las siguientes son posibles razones para este problema? (Elija dos.)

- [x] La aplicación está usando un protocolo que la puerta de enlace `NAT` no admite.
- [ ] La puerta de enlace `NAT` no está en un grupo de seguridad.
- [ ] La puerta de enlace `NAT` está en una Zona de disponibilidad no compatible.
- [x] La puerta de enlace `NAT` no está en el estado Available.
- [ ] La configuración de reenvío de puertos no permite el acceso a servicios internos desde internet.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una nueva aplicación se ejecuta en instancias de Amazon EC2 y accede a datos en una instancia de base de datos de Amazon RDS. Cuando se despliega completamente en producción, la aplicación falla. La base de datos puede consultarse desde una consola en un bastion host. Al revisar los registros del servidor web, se repite varias veces el siguiente error: `*** Error Establishing a Database Connection`. ¿Cuáles de las siguientes pueden ser causas de los problemas de conectividad? (Elija dos.)

- [ ] El grupo de seguridad de la base de datos no tiene la regla de salida (egress) apropiada desde la base de datos hacia el servidor web.
- [ ] El certificado usado por el servidor web no es de confianza para la instancia de RDS.
- [x] El grupo de seguridad de la base de datos no tiene la regla de entrada (ingress) apropiada desde el servidor web hacia la base de datos.
- [x] El puerto usado por el desarrollador de la aplicación no coincide con el puerto especificado en la configuración de RDS.
- [ ] La base de datos todavía se está creando y no está disponible para conectividad.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps es responsable de administrar una flota de instancias de Amazon EC2. Estas instancias de EC2 suben artefactos de compilación (build artifacts) a un servicio de terceros. El servicio de terceros implementó recientemente una lista estricta de IP permitidas que requiere que todas las cargas de compilación provengan de una única dirección IP. ¿Qué cambio debe hacer el ingeniero de sistemas en la flota de compilación existente para cumplir con este nuevo requisito?

- [x] Mover todas las instancias de EC2 detrás de una puerta de enlace `NAT` y proporcionar la dirección IP de la puerta de enlace al servicio.
- [ ] Mover todas las instancias de EC2 detrás de una puerta de enlace de internet y proporcionar la dirección IP de la puerta de enlace al servicio.
- [ ] Mover todas las instancias de EC2 a una sola Zona de disponibilidad y proporcionar la dirección IP de la Zona de disponibilidad al servicio.
- [ ] Mover todas las instancias de EC2 a una `VPC` emparejada (peered) y proporcionar la dirección IP de la `VPC` al servicio.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está intentando configurar un nombre de dominio de Amazon Route 53 para enrutar tráfico a un sitio web alojado en Amazon S3. El nombre de dominio del sitio web es `www.example.com` y el nombre del bucket de S3 es `DOC-EXAMPLE-BUCKET`. Después de configurar el conjunto de registros en Route 53, el nombre de dominio `www.anycompany.com` no parece funcionar, y el sitio web estático no se muestra en el navegador. ¿Cuál de las siguientes es una causa de esto?

- [ ] El bucket de S3 debe configurarse primero con Amazon CloudFront.
- [ ] El conjunto de registros de Route 53 debe tener un rol de IAM que permita el acceso al bucket de S3.
- [ ] El conjunto de registros de Route 53 debe estar en la misma región que el bucket de S3.
- [x] El nombre del bucket de S3 debe coincidir con el nombre del conjunto de registros en Route 53.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja su sitio web en instancias de Amazon EC2 en la región `us-east-1`. La empresa se está preparando para extender su sitio web a la región `eu-central-1`, pero la base de datos debe permanecer únicamente en `us-east-1`. Después del despliegue, las instancias de EC2 en `eu-central-1` no pueden conectarse a la base de datos en `us-east-1`. ¿Cuál es la solución MÁS eficiente operativamente que resolverá este problema de conectividad?

- [x] Crear una conexión de emparejamiento (peering) de `VPC` entre las dos regiones. Agregar el rango de direcciones IP privadas de las instancias a la regla de entrada del grupo de seguridad de la base de datos.
- [ ] Crear una conexión de emparejamiento de `VPC` entre las dos regiones. Agregar el grupo de seguridad de las instancias en `eu-central-1` a la regla de salida del grupo de seguridad de la base de datos.
- [ ] Crear una conexión `VPN` entre las dos regiones. Agregar el rango de direcciones IP privadas de las instancias a la regla de salida del grupo de seguridad de la base de datos.
- [ ] Crear una conexión `VPN` entre las dos regiones. Agregar el grupo de seguridad de las instancias en `eu-central-1` a la regla de entrada del grupo de seguridad de la base de datos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa subió los archivos de su sitio web a un bucket de Amazon S3 que tiene habilitado el versionado de S3. La empresa usa una distribución de Amazon CloudFront con el bucket de S3 como origen. La empresa modificó recientemente los archivos, pero los nombres de objeto permanecieron iguales. Los usuarios reportan que el contenido antiguo sigue apareciendo en el sitio web. ¿Cómo debe un ingeniero de CloudOps remediar este problema?

- [x] Crear una invalidación de CloudFront, y agregar la ruta de los archivos actualizados.
- [ ] Crear una URL firmada (signed URL) de CloudFront para actualizar cada objeto inmediatamente.
- [ ] Configurar un Origin Access Identity (OAI) de S3 para mostrar solo los archivos actualizados a los usuarios.
- [ ] Deshabilitar el versionado de S3 en el bucket de S3 para que los archivos actualizados puedan reemplazar a los antiguos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene dos redes `VPC` llamadas `VPC` A y `VPC` B. El bloque `CIDR` de `VPC` A es `10.0.0.0/16` y el bloque `CIDR` de `VPC` B es `172.31.0.0/16`. La empresa quiere establecer una conexión de emparejamiento (peering) de `VPC` llamada `pcx-12345` entre ambas `VPC`. ¿Qué reglas deben aparecer en la tabla de enrutamiento de `VPC` A después de la configuración? (Elija dos.)

- [x] `Destination`: `10.0.0.0/16`, `Target`: `Local`.
- [ ] `Destination`: `172.31.0.0/16`, `Target`: `Local`.
- [ ] `Destination`: `10.0.0.0/16`, `Target`: `pcx-12345`.
- [x] `Destination`: `172.31.0.0/16`, `Target`: `pcx-12345`.
- [ ] `Destination`: `10.0.0.0/16`, `Target`: `172.31.0.0/16`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una aplicación se ejecuta en una instancia de Amazon EC2 en una `VPC` con el conjunto de opciones `DHCP` predeterminado. La aplicación se conecta a una base de datos Microsoft SQL Server local (on-premises) con el nombre `DNS` `mssql.example.com`. La aplicación no puede resolver el nombre `DNS` de la base de datos. ¿Qué solución solucionará este problema?

- [ ] Crear un endpoint de entrada (inbound) de Amazon Route 53 Resolver. Agregar una regla de reenvío para el dominio `example.com`. Asociar la regla de reenvío con la `VPC`.
- [ ] Crear un endpoint de entrada de Amazon Route 53 Resolver. Agregar una regla de sistema para el dominio `example.com`. Asociar la regla de sistema con la `VPC`.
- [x] Crear un endpoint de salida (outbound) de Amazon Route 53 Resolver. Agregar una regla de reenvío para el dominio `example.com`. Asociar la regla de reenvío con la `VPC`.
- [ ] Crear un endpoint de salida de Amazon Route 53 Resolver. Agregar una regla de sistema para el dominio `example.com`. Asociar la regla de sistema con la `VPC`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### La aplicación de una empresa está alojada por un proveedor de internet en `app.example.com`. La empresa quiere acceder a la aplicación usando `www.company.com`, que la empresa posee y administra con Amazon Route 53. ¿Qué registro de Route 53 se debe crear para lograr esto?

- [ ] Registro `A`.
- [ ] Registro `Alias`.
- [x] Registro `CNAME`.
- [ ] Registro `Pointer (PTR)`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja un sitio web estático en Amazon S3. Una distribución de Amazon CloudFront presenta este sitio a usuarios globales. La empresa usa la política de caché `Managed-CachingDisabled` de CloudFront. Los desarrolladores de la empresa confirman que actualizan con frecuencia un archivo en Amazon S3 con información nueva. Los usuarios reportan que el sitio web presenta la información correcta cuando el sitio carga el archivo por primera vez. Sin embargo, los navegadores de los usuarios no obtienen el archivo actualizado después de una actualización (refresh). ¿Qué debe recomendar un ingeniero de CloudOps para solucionar este problema?

- [x] Agregar un campo de encabezado `Cache-Control` con `max-age=0` al objeto de S3.
- [ ] Cambiar la política de caché de CloudFront a `Managed-CachingOptimized`.
- [ ] Deshabilitar el versionado del bucket en la configuración del bucket de S3.
- [ ] Habilitar la compresión de contenido en la configuración de CloudFront.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa Amazon CloudFront para servir contenido estático de su aplicación web a sus usuarios. La distribución de CloudFront usa un sitio web local (on-premises) existente como origen personalizado. La empresa requiere el uso de TLS entre CloudFront y el servidor de origen. Esta configuración ha funcionado como se esperaba durante varios meses. Sin embargo, los usuarios ahora están experimentando errores `HTTP 502 (Bad Gateway)` al ver páginas web que incluyen contenido de la distribución de CloudFront. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?

- [x] Examinar la fecha de vencimiento del certificado en el sitio de origen. Validar que el certificado no haya expirado. Reemplazar el certificado si es necesario.
- [ ] Examinar el nombre de host en el certificado en el sitio de origen. Validar que el nombre de host coincida con uno de los nombres de host en la distribución de CloudFront. Reemplazar el certificado si es necesario.
- [ ] Examinar las reglas de firewall asociadas con el servidor de origen. Validar que el puerto `443` esté abierto para tráfico entrante desde internet. Crear una regla de entrada si es necesario.
- [ ] Examinar las reglas de `ACL` de red asociadas con la distribución de CloudFront. Validar que el puerto `443` esté abierto para tráfico de salida hacia el servidor de origen. Crear una regla de salida si es necesario.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una distribución de Amazon CloudFront tiene un único bucket de Amazon S3 como su origen. Un ingeniero de CloudOps debe asegurarse de que los usuarios solo puedan acceder al bucket de S3 a través de solicitudes provenientes del endpoint de CloudFront. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar S3 Block Public Access en el bucket de S3. Actualizar la política del bucket de S3 para permitir la acción `GetObject` únicamente desde la distribución de CloudFront.
- [ ] Configurar Origin Shield en la distribución de CloudFront. Actualizar el origen de CloudFront para incluir un encabezado personalizado `Origin_Shield`.
- [x] Crear una Origin Access Identity (OAI). Asignar la OAI a la distribución de CloudFront. Actualizar la política del bucket de S3 para restringir el acceso a la OAI.
- [ ] Crear una Origin Access Identity (OAI). Asignar la OAI al bucket de S3. Actualizar el origen de CloudFront para incluir un encabezado personalizado `Origin` con el valor de la OAI.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación que se ejecuta en instancias de Amazon EC2 en una `VPC`. La aplicación necesita acceso para descargar actualizaciones de software desde internet. La `VPC` tiene subredes públicas y subredes privadas. La política de seguridad de la empresa requiere que todas las instancias de EC2 se desplieguen en subredes privadas. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Agregar una puerta de enlace de internet a la `VPC`. En la tabla de enrutamiento de las subredes privadas, agregar una ruta a la puerta de enlace de internet.
- [ ] Agregar una puerta de enlace `NAT` a una subred privada. En la tabla de enrutamiento de las subredes privadas, agregar una ruta a la puerta de enlace `NAT`.
- [x] Agregar una puerta de enlace `NAT` a una subred pública. En la tabla de enrutamiento de las subredes privadas, agregar una ruta a la puerta de enlace `NAT`.
- [ ] Agregar dos puertas de enlace de internet a la `VPC`. En las tablas de enrutamiento de las subredes privadas y subredes públicas, agregar una ruta a cada puerta de enlace de internet.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps ha configurado una nueva instancia de Amazon EC2 como servidor web en una subred pública. La instancia usa el puerto `80` de `HTTP` y el puerto `443` de `HTTPS`. El ingeniero de CloudOps ha confirmado la conectividad a internet descargando actualizaciones del sistema operativo y software desde repositorios públicos. Sin embargo, el ingeniero de CloudOps no puede acceder a la instancia desde un navegador web en internet. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para solucionar este problema? (Elija tres.)

- [x] Asegurarse de que las reglas de entrada del grupo de seguridad de la instancia permitan tráfico en los puertos `80` y `443`.
- [ ] Asegurarse de que las reglas de salida del grupo de seguridad de la instancia permitan tráfico en los puertos `80` y `443`.
- [ ] Asegurarse de que los puertos efímeros `1024-65535` estén permitidos en las reglas de entrada de la `ACL` de red asociada con la subred de la instancia.
- [x] Asegurarse de que los puertos efímeros `1024-65535` estén permitidos en las reglas de salida de la `ACL` de red asociada con la subred de la instancia.
- [x] Asegurarse de que las reglas de filtrado de cualquier firewall que se ejecute en la instancia permitan tráfico entrante en los puertos `80` y `443`.
- [ ] Asegurarse de que AWS WAF esté activado para la instancia y esté bloqueando el tráfico web.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Los usuarios reportan cierres de sesión forzados constantes en una aplicación web con estado (stateful). Los cierres de sesión ocurren antes de la expiración de un temporizador de cierre de sesión de la aplicación de 15 minutos. La aplicación web está alojada en instancias de Amazon EC2 que están en un grupo de Auto Scaling. Las instancias se ejecutan detrás de un Application Load Balancer (ALB) que tiene un único grupo de destino (target group). El `ALB` está configurado como el origen en una distribución de Amazon CloudFront. La afinidad de sesión (sticky sessions) ya está habilitada en el grupo de destino del `ALB` y usa cookies basadas en duración. La aplicación web genera su propia cookie de aplicación. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para resolver el problema de cierre de sesión? (Elija dos.)

- [ ] Cambiar al algoritmo de solicitudes pendientes mínimas (least outstanding requests) en el grupo de destino del `ALB`.
- [x] Configurar el reenvío de cookies (cookie forwarding) en la configuración de comportamiento de caché de la distribución de CloudFront.
- [ ] Configurar la cookie basada en duración para que se llame AWSALB.
- [ ] Configurar el `ALB` para usar el encabezado de cookie de expiración.
- [x] Cambiar el `ALB` para usar cookies basadas en la aplicación.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps descubrió que un servidor de aplicación de Amazon EC2 recién desplegado no puede conectarse a una instancia de base de datos de Amazon RDS existente. Después de habilitar `VPC` Flow Logs y confirmar que el flow log está activo en la consola, el grupo de registro no se puede encontrar en Amazon CloudWatch. ¿Cuáles son las razones MÁS probables de esta situación? (Elija dos.)

- [ ] El ingeniero debe configurar los `VPC` Flow Logs para que se envíen a AWS CloudTrail.
- [x] El ingeniero ha esperado menos de diez minutos para que se cree el grupo de registro en CloudWatch.
- [ ] Los `VPC` Flow Logs de la cuenta han sido deshabilitados mediante una Política de Control de Servicio.
- [x] No se ha enviado tráfico relevante desde que se crearon los `VPC` Flow Logs.
- [ ] La cuenta tiene Amazon GuardDuty habilitado.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El ingeniero de CloudOps de una empresa está solucionando problemas de comunicación entre los componentes de una aplicación. La empresa configuró los flow logs de `VPC` para que se publiquen en Amazon CloudWatch Logs. Sin embargo, no hay registros en CloudWatch Logs. ¿Qué podría estar bloqueando que los flow logs de `VPC` se publiquen en CloudWatch Logs?

- [x] A la política de IAM adjunta al rol de IAM para el flow log le falta el permiso `CreateLogGroup` de logs.
- [ ] A la política de IAM adjunta al rol de IAM para el flow log le falta el permiso `CreateExportTask` de logs.
- [ ] La `VPC` está configurada para direcciones IPv6.
- [ ] La `VPC` está emparejada (peered) con otra `VPC` en la cuenta de AWS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps configura los flow logs de `VPC` para que se publiquen en Amazon CloudWatch Logs. El ingeniero de CloudOps revisa los registros en CloudWatch Logs y nota menos tráfico del esperado. Después de que el ingeniero de CloudOps compara los flow logs de `VPC` con registros capturados localmente (on-premises), el ingeniero de CloudOps cree que los flow logs de `VPC` están incompletos. ¿Cuál de las siguientes es una posible razón para la diferencia en el tráfico?

- [ ] Se ha aplicado limitación (throttling) a CloudWatch Logs.
- [ ] El rol de IAM de CloudWatch no tiene una relación de confianza con el servicio de flow logs de `VPC`.
- [ ] El flow log de `VPC` todavía está en proceso de creación.
- [x] Los flow logs de `VPC` no pueden capturar tráfico desde servidores locales (on-premises) hacia una `VPC`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está revisando los `VPC` Flow Logs para solucionar problemas de conectividad en una `VPC`. Al revisar los registros, el ingeniero de CloudOps nota que el tráfico rechazado no aparece listado. ¿Qué debe hacer el ingeniero de CloudOps para asegurarse de que todo el tráfico se registre?

- [x] Crear un nuevo flow log que tenga una configuración de filtro para capturar todo el tráfico.
- [ ] Crear un nuevo flow log. Configurar el formato de registro en un formato personalizado. Seleccionar los campos apropiados para incluir en el registro.
- [ ] Editar el flow log existente. Cambiar la configuración de filtro para capturar todo el tráfico.
- [ ] Editar el flow log existente. Configurar el formato de registro en un formato personalizado. Seleccionar los campos apropiados para incluir en el registro.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja una aplicación web en una instancia de Amazon EC2 en una `VPC` de producción. Las conexiones de clientes a la aplicación están fallando. Un ingeniero de CloudOps inspecciona los flow logs de `VPC` y encuentra la siguiente entrada. ¿Cuál es una posible causa de estas conexiones fallidas?

![Question 282](images/question282.png)

- [ ] Una regla de denegación del grupo de seguridad está bloqueando el tráfico en el puerto `443`.
- [ ] La instancia de EC2 está apagada.
- [x] La `ACL` de red está bloqueando el tráfico `HTTPS`.
- [ ] La `VPC` no tiene una puerta de enlace de internet adjunta.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está ejecutando una aplicación en un grupo de instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias de EC2 se ejecutan en tres Zonas de disponibilidad. La empresa necesita proporcionar a los clientes un máximo de dos direcciones IP estáticas para sus aplicaciones. ¿Cómo debe un ingeniero de CloudOps cumplir con este requisito?

- [x] Agregar AWS Global Accelerator delante del Application Load Balancer.
- [ ] Agregar un Network Load Balancer interno detrás del Application Load Balancer.
- [ ] Configurar el Application Load Balancer en solo dos Zonas de disponibilidad.
- [ ] Crear dos direcciones IP elásticas y asignarlas al Application Load Balancer.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa almacena contenido multimedia en un bucket de Amazon S3 y usa Amazon CloudFront para distribuir el contenido a sus usuarios. Debido a los términos de licencia, la empresa no está autorizada a distribuir el contenido en algunos países. Un ingeniero de CloudOps debe restringir el acceso a ciertos países. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Configurar la política del bucket de S3 para denegar la operación `GetObject` según la condición `s3:LocationConstraint`.
- [ ] Crear una Origin Access Identity (OAI) secundaria. Configurar la política del bucket de S3 para prevenir el acceso desde países no autorizados.
- [x] Habilitar la función de restricción geográfica (geo restriction) en la distribución de CloudFront para prevenir el acceso desde países no autorizados.
- [ ] Actualizar la aplicación para generar URLs firmadas de CloudFront solo para direcciones IP en países autorizados.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una aplicación se ejecuta en múltiples instancias de EC2. Como parte de una iniciativa para mejorar la seguridad general de la infraestructura, las instancias de EC2 se movieron a una subred privada. Sin embargo, desde que se movieron, las instancias de EC2 no han podido actualizarse automáticamente, y un ingeniero de CloudOps no ha podido conectarse a ellas remotamente por `SSH`. ¿Qué dos acciones podría tomar el ingeniero para resolver estos problemas de forma segura? (Elija dos.)

- [x] Configurar un bastion host en una subred pública, y configurar los grupos de seguridad y tablas de enrutamiento en consecuencia.
- [ ] Configurar un bastion host en la subred privada, y configurar los grupos de seguridad en consecuencia.
- [ ] Configurar un balanceador de carga en una subred pública, y configurar las tablas de enrutamiento en consecuencia.
- [x] Configurar una puerta de enlace `NAT` en una subred pública, y cambiar las tablas de enrutamiento de la subred privada en consecuencia.
- [ ] Configurar una puerta de enlace `NAT` en una subred privada, y asegurarse de que las tablas de enrutamiento estén configuradas en consecuencia.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está solucionando problemas de una `VPC` con subredes públicas y privadas que usan `ACL` de red personalizadas. Las instancias en la subred privada no pueden acceder a internet. Hay una puerta de enlace de internet adjunta a la subred pública. La subred privada tiene una ruta hacia una puerta de enlace `NAT` que también está adjunta a la subred pública. Las instancias de Amazon EC2 están asociadas con el grupo de seguridad predeterminado de la `VPC`. ¿Qué está causando el problema en este escenario?

- [x] Hay una `ACL` de red en la subred privada configurada para denegar todo el tráfico de salida.
- [ ] No hay ninguna puerta de enlace `NAT` desplegada en la subred privada de la `VPC`.
- [ ] El grupo de seguridad predeterminado de la `VPC` bloquea todo el tráfico entrante hacia las instancias de EC2.
- [ ] El grupo de seguridad predeterminado de la `VPC` bloquea todo el tráfico saliente desde las instancias de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita configurar un bucket de Amazon S3 para alojar una aplicación web. El ingeniero de CloudOps ha creado el bucket de S3 y ha copiado los archivos estáticos de la aplicación web al bucket de S3. La empresa tiene una política de que ningún bucket de S3 debe ser público. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Crear una distribución de Amazon CloudFront. Configurar el bucket de S3 como origen con una Origin Access Identity (OAI). Otorgar a la OAI el permiso `s3:GetObject` en la política del bucket de S3.
- [ ] Configurar el alojamiento de sitio web estático en el bucket de S3. Usar Amazon Route 53 para crear un `CNAME` de `DNS` que apunte al endpoint del sitio web de S3.
- [ ] Crear un Application Load Balancer (ALB). Cambiar el protocolo a `HTTPS` en la configuración del listener del `ALB`. Reenviar el tráfico al bucket de S3.
- [ ] Crear un accelerator en AWS Global Accelerator. Configurar una configuración de listener para el puerto `443`. Establecer el tipo de endpoint para reenviar el tráfico al bucket de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa planea lanzar un sitio web estático en su dominio `example.com` y subdominio `www.example.com` usando Amazon S3. ¿Cómo debe el ingeniero de CloudOps cumplir con este requisito?

- [ ] Crear un bucket de S3 llamado `example.com` para tanto el dominio como el subdominio.
- [ ] Crear un bucket de S3 con un comodín llamado `*.example.com` para tanto el dominio como el subdominio.
- [x] Crear dos buckets de S3 llamados `example.com` y `www.example.com`. Configurar el bucket del subdominio para redirigir las solicitudes al bucket del dominio.
- [ ] Crear dos buckets de S3 llamados `http://example.com` y `http://*.example.com`. Configurar el bucket comodín (`*`) para redirigir las solicitudes al bucket del dominio.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja su sitio web en la región `us-east-1`. La empresa se está preparando para desplegar su sitio web en la región `eu-central-1`. Los visitantes del sitio web ubicados en Europa deben acceder al sitio web alojado en `eu-central-1`. Todos los demás visitantes acceden al sitio web alojado en `us-east-1`. La empresa usa Amazon Route 53 para administrar los registros `DNS` del sitio web. ¿Qué política de enrutamiento debe aplicar un ingeniero de CloudOps al conjunto de registros de Route 53 para cumplir con estos requisitos?

- [x] Política de enrutamiento por geolocalización (Geolocation).
- [ ] Política de enrutamiento por geoproximidad (Geoproximity).
- [ ] Política de enrutamiento por latencia (Latency).
- [ ] Política de enrutamiento de respuesta múltiple (Multivalue answer).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está configurando una conexión de emparejamiento (peering) de `VPC` entre su `VPC` y la `VPC` de un cliente. La `VPC` de la empresa tiene un bloque `CIDR` IPv4 de `172.16.0.0/16`, y la del cliente tiene un bloque `CIDR` IPv4 de `10.0.0.0/16`. El ingeniero de CloudOps quiere poder hacer ping a la dirección IP privada de la base de datos del cliente desde una de las instancias de Amazon EC2 de la empresa. ¿Qué acción se debe tomar para cumplir con los requisitos?

- [ ] Asegurarse de que ambas cuentas estén vinculadas y sean parte de la facturación consolidada para crear una red de intercambio de archivos, y luego habilitar el emparejamiento de `VPC`.
- [x] Asegurarse de que ambos propietarios de `VPC` agreguen manualmente una ruta a las tablas de enrutamiento de la `VPC` que apunte al rango de direcciones IP de la otra `VPC`.
- [ ] Indicar al cliente que configure una `VPC` con el mismo bloque `CIDR` IPv4 que la `VPC` de origen: `172.16.0.0/16`.
- [ ] Indicar al cliente que cree una puerta de enlace privada virtual para vincular las dos `VPC`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación web a la que los usuarios acceden usando el nombre de dominio `www.example.com`. La empresa administra el nombre de dominio usando Amazon Route 53. La empresa creó una distribución de Amazon CloudFront delante de la aplicación y le gustaría que `www.example.com` acceda a la aplicación a través de CloudFront. ¿Cuál es la forma MÁS rentable de lograr esto?

- [ ] Crear un registro `CNAME` en Amazon Route 53 que apunte a la URL de la distribución de CloudFront.
- [x] Crear un registro `ALIAS` en Amazon Route 53 que apunte a la URL de la distribución de CloudFront.
- [ ] Crear un registro `A` en Amazon Route 53 que apunte a la dirección IP pública de la aplicación web.
- [ ] Crear un registro `PTR` en Amazon Route 53 que apunte a la dirección IP pública de la aplicación web.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps tiene un sitio web de Amazon S3 y quiere restringir el acceso a una única distribución de Amazon CloudFront. Los visitantes del sitio web no deben poder eludir CloudFront ni ver el sitio web de S3 directamente desde el bucket. ¿Qué servicio o función de AWS cumple con estos requisitos?

- [ ] `ACL` del bucket de S3.
- [ ] AWS Firewall Manager.
- [ ] Zona alojada privada de Amazon Route 53.
- [x] Origin Access Identity (OAI).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está creando un sitio web simple, orientado al público, que se ejecuta en Amazon EC2. El ingeniero de CloudOps creó la instancia de EC2 en una subred pública existente y asignó una dirección IP elástica a la instancia. Luego, el ingeniero de CloudOps creó y aplicó un nuevo grupo de seguridad a la instancia para permitir tráfico `HTTP` entrante desde `0.0.0.0/0`. Finalmente, el ingeniero de CloudOps creó una nueva `ACL` de red y la aplicó a la subred para permitir tráfico `HTTP` entrante desde `0.0.0.0/0`. Sin embargo, no se puede acceder al sitio web desde internet. ¿Cuál es la causa de este problema?

- [x] El ingeniero de CloudOps no creó una regla de salida que permita el tráfico de retorno de puertos efímeros en la nueva `ACL` de red.
- [ ] El ingeniero de CloudOps no creó una regla de salida en el grupo de seguridad que permita tráfico `HTTP` desde el puerto `80`.
- [ ] La dirección IP elástica asignada a la instancia de EC2 ha cambiado.
- [ ] Hay una `ACL` de red adicional asociada con la subred que incluye una regla que deniega el tráfico `HTTP` entrante desde el puerto `80`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Después de un cambio de red, los servidores de aplicación no pueden conectarse a la base de datos correspondiente de Amazon RDS MySQL. ¿Qué debe analizar el ingeniero de CloudOps?

- [x] `VPC` Flow Logs.
- [ ] Registros de Elastic Load Balancing.
- [ ] Registros de Amazon CloudFront.
- [ ] Registros de error de Amazon RDS MySQL.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps configuró los flow logs de `VPC` usando el formato predeterminado. El ingeniero de CloudOps especificó Amazon CloudWatch Logs como destino. Esta solución ha funcionado exitosamente durante varios meses. Sin embargo, debido a requisitos adicionales de solución de problemas, el ingeniero de CloudOps necesita incluir el campo `tcp-flags` en los flow logs. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [x] Crear un nuevo flow log. Incluir el campo `tcp-flags` en el formato de registro personalizado. Eliminar el flow log original.
- [ ] En el grupo de registro de CloudWatch Logs, modificar el filtro para incluir el campo `tcp-flags` y el campo type.
- [ ] En CloudWatch Metrics, modificar la configuración de métrica para incluir el campo `tcp-flags`.
- [ ] Modificar el flow log existente. Incluir el campo `tcp-flags` y el campo type en el formato de registro personalizado. Guardar la configuración.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación en cientos de instancias de Amazon EC2 en tres Zonas de disponibilidad. La aplicación llama a una API de terceros a través de internet público. Un ingeniero de CloudOps debe proporcionar al tercero una lista de direcciones IP estáticas para que el tercero pueda permitir el tráfico desde la aplicación. ¿Qué solución cumple con estos requisitos?

- [x] Agregar una puerta de enlace `NAT` en la subred pública de cada Zona de disponibilidad. Hacer que la puerta de enlace `NAT` sea la ruta predeterminada de todas las subredes privadas en esas Zonas de disponibilidad.
- [ ] Asignar una dirección IP elástica en cada Zona de disponibilidad. Asociar la dirección IP elástica con todas las instancias en la Zona de disponibilidad.
- [ ] Colocar las instancias detrás de un Network Load Balancer (NLB). Enviar el tráfico a internet a través de la dirección IP privada del NLB.
- [ ] Actualizar la tabla de enrutamiento principal para enviar el tráfico a internet a través de una dirección IP elástica asignada a cada instancia.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está administrando una red `VPC` que consiste en subredes públicas y privadas. Las instancias en las subredes privadas acceden a internet a través de una puerta de enlace `NAT`. Una factura reciente de AWS muestra que los cargos de la puerta de enlace `NAT` se han duplicado. El ingeniero quiere identificar qué instancias están generando la mayor cantidad de tráfico de red. ¿Cómo se debe lograr esto?

- [x] Habilitar flow logs en la interfaz de red elástica de la puerta de enlace `NAT` y usar Amazon CloudWatch Insights para filtrar los datos según las direcciones IP de origen.
- [ ] Ejecutar un informe de AWS Cost and Usage y agrupar los hallazgos por ID de instancia.
- [ ] Usar la función de duplicación de tráfico (`VPC` traffic mirroring) para enviar tráfico a Amazon QuickSight.
- [ ] Usar las métricas de Amazon CloudWatch generadas por la puerta de enlace `NAT` para cada instancia individual.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está almacenando informes mensuales en Amazon S3. El requisito de seguridad de la empresa establece que el tráfico desde la `VPC` del cliente hacia Amazon S3 no puede atravesar internet. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Usar AWS Direct Connect y una interfaz virtual pública para conectarse a Amazon S3.
- [ ] Usar una puerta de enlace `NAT` administrada para conectarse a Amazon S3.
- [x] Desplegar un endpoint de `VPC` para conectarse a Amazon S3.
- [ ] Desplegar una puerta de enlace de internet para conectarse a Amazon S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está rediseñando la arquitectura de una aplicación. El ingeniero de CloudOps ha movido la base de datos de una subred pública, donde la base de datos usaba un endpoint público, a una subred privada para restringir el acceso desde la red pública. Después de este cambio, una función de AWS Lambda que requiere acceso de lectura a la base de datos no puede conectarse a la base de datos. El ingeniero de CloudOps debe resolver este problema sin comprometer la seguridad. ¿Qué solución cumple con estos requisitos?

- [x] Crear un endpoint de interfaz de AWS PrivateLink para la función Lambda. Conectarse a la base de datos usando su endpoint privado.
- [ ] Conectar la función Lambda a la `VPC` de la base de datos. Conectarse a la base de datos usando su endpoint privado.
- [ ] Adjuntar un rol de IAM a la función Lambda con permisos de lectura a la base de datos.
- [ ] Mover la base de datos a una subred pública. Usar grupos de seguridad para acceso seguro.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una instancia de Amazon EC2 en una subred privada necesita copiar datos a un bucket de Amazon S3. Por razones de seguridad, la conexión desde la instancia de EC2 a Amazon S3 no debe atravesar internet. ¿Qué acción debe tomar el ingeniero de CloudOps para lograr esto?

- [ ] Crear una instancia `NAT` y enrutar el tráfico destinado a Amazon S3 a través de ella.
- [ ] Crear una conexión `VPN` entre la instancia de EC2 y Amazon S3.
- [x] Crear un endpoint de `VPC` de S3 en la `VPC` donde reside la instancia de EC2.
- [ ] Usar AWS Direct Connect para maximizar el rendimiento y mantener el tráfico privado.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita configurar la zona alojada de Amazon Route 53 para `example.com` y `www.example.com` para que apunten a un Application Load Balancer (ALB). ¿Qué combinación de acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Configurar un registro `A` para `example.com` que apunte a la dirección IP del `ALB`.
- [ ] Configurar un registro `A` para `www.example.com` que apunte a la dirección IP del `ALB`.
- [x] Configurar un registro alias para `example.com` que apunte al `CNAME` del `ALB`.
- [x] Configurar un registro alias para `www.example.com` que apunte al registro `example.com` de Route 53.
- [ ] Configurar un registro `CNAME` para `example.com` que apunte al `CNAME` del `ALB`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps creó una función de AWS Lambda dentro de una `VPC` sin acceso a internet. La función Lambda extrae mensajes de una cola de Amazon SQS y los almacena en una instancia de Amazon RDS en la misma `VPC`. Después de ejecutar la función Lambda, los datos no aparecen en la instancia de RDS. ¿Cuáles de las siguientes son posibles causas de esto? (Elija dos.)

- [ ] No se ha creado un endpoint de `VPC` para Amazon RDS.
- [x] No se ha creado un endpoint de `VPC` para Amazon SQS.
- [x] El grupo de seguridad de RDS no permite conexiones desde la función Lambda.
- [ ] La subred asociada con la función Lambda no tiene una puerta de enlace de internet adjunta.
- [ ] La subred asociada con la función Lambda tiene una puerta de enlace `NAT`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. ¿Cuál de las siguientes afirmaciones NO es verdadera en este escenario?

- [x] La `VPC` creará una instancia de enrutamiento y la adjuntará a una subred pública.
- [ ] La `VPC` creará dos subredes.
- [ ] La `VPC` creará una puerta de enlace de internet y la adjuntará a la `VPC`.
- [ ] La `VPC` lanzará una instancia NAT con una IP elástica.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación que usa una función programada de AWS Lambda para recuperar conjuntos de datos de fuentes externas a través de internet. La función no está asociada con una `VPC`. La empresa está modificando la aplicación para almacenar la información que la función Lambda recupera en una instancia de base de datos de Amazon RDS en una subred privada. La `VPC` tiene dos subredes públicas y dos subredes privadas. Un ingeniero de CloudOps debe desplegar una solución que permita a la función Lambda acceder a la nueva base de datos y continuar accediendo a internet. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una nueva función Lambda con acceso `VPC` y una dirección IP elástica. Adjuntar la función a subredes públicas en dos Zonas de disponibilidad. Asociar un grupo de seguridad con la dirección IP elástica. Configurar las reglas de salida del grupo de seguridad para permitir que Lambda acceda a los recursos requeridos.
- [ ] Crear una nueva función Lambda con acceso `VPC` y dos direcciones IP públicas. Adjuntar la función a subredes públicas en las mismas Zonas de disponibilidad que usa la base de datos. Asociar un grupo de seguridad con la función. Configurar las reglas de entrada del grupo de seguridad para permitir que Lambda acceda a los recursos requeridos.
- [x] Reconfigurar la función Lambda para acceso `VPC`. Agregar puertas de enlace `NAT` a las subredes públicas en la `VPC`. Agregar entradas de tabla de enrutamiento en las subredes privadas para enrutar a través de las puertas de enlace `NAT` hacia internet. Adjuntar la función a las subredes privadas que soportan la base de datos. Asociar un grupo de seguridad con la función. Configurar las reglas de salida del grupo de seguridad para permitir que Lambda acceda a internet.
- [ ] Reconfigurar la función Lambda para acceso `VPC`. Adjuntar la función a las subredes privadas. Agregar entradas de tabla de enrutamiento en las subredes privadas para enrutar a través de la puerta de enlace de internet hacia internet. Asociar un grupo de seguridad con las subredes. Configurar las reglas de entrada del grupo de seguridad para permitir que Lambda acceda a los recursos requeridos a través de la puerta de enlace de internet.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred privada usa `CIDR` `20.0.0.0/24`. El ID de la instancia `NAT` es `i-a12345`. ¿Cuál de las siguientes entradas se requiere en la tabla de enrutamiento principal adjunta a la subred privada para permitir que las instancias se conecten a internet?

- [x] Destino: `0.0.0.0/0` y Destino: `i-a12345`.
- [ ] Destino: `20.0.0.0/0` y Destino: `80`.
- [ ] Destino: `20.0.0.0/0` y Destino: `i-a12345`.
- [ ] Destino: `20.0.0.0/24` y Destino: `i-a12345`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. ¿Cuál de las siguientes afirmaciones es verdadera en este escenario?

- [ ] La `VPC` de AWS creará automáticamente una instancia `NAT` de tamaño micro.
- [x] La `VPC` vincula la tabla de enrutamiento principal con una subred privada y una tabla de enrutamiento personalizada con una subred pública.
- [ ] El usuario debe crear manualmente una instancia `NAT`.
- [ ] La `VPC` vincula la tabla de enrutamiento principal con una subred pública y una tabla de enrutamiento personalizada con una subred privada.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred privada usa `CIDR` `20.0.0.0/24`. ¿Cuál de las siguientes entradas se requiere en la tabla de enrutamiento principal para permitir que las instancias en la `VPC` se comuniquen entre sí?

- [ ] Destino: `20.0.0.0/24` y Destino: `VPC`.
- [x] Destino: `20.0.0.0/16` y Destino: `Local`.
- [ ] Destino: `20.0.0.0/0` y Destino: `ALL`.
- [ ] Destino: `20.0.0.0/24` y Destino: `Local`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. El usuario no ha lanzado ninguna instancia manualmente y está intentando eliminar la `VPC`. ¿Qué sucederá en este escenario?

- [ ] No permitirá eliminar la `VPC` ya que tiene subredes con tablas de enrutamiento.
- [ ] No permitirá eliminar la `VPC` ya que tiene una instancia de enrutamiento en ejecución.
- [ ] Terminará la `VPC` junto con todas las instancias lanzadas por el asistente.
- [x] No permitirá eliminar la `VPC` ya que tiene una instancia `NAT` en ejecución.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred pública usa `CIDR` `20.0.1.0/24`. El usuario planea alojar un servidor web en la subred pública (puerto `80`) y un servidor de base de datos en la subred privada (puerto `3306`). El usuario está configurando un grupo de seguridad para la subred pública (`WebSecGrp`) y la subred privada (`DBSecGrp`). ¿Cuál de las siguientes entradas se requiere en el grupo de seguridad del servidor web (`WebSecGrp`)?

- [ ] Configurar `Destination` como el ID del grupo de seguridad de la base de datos (`DbSecGrp`) para el puerto `3306` de salida.
- [ ] `80` para `Destination` `0.0.0.0/0` de salida.
- [ ] Configurar el puerto `3306` para origen `20.0.0.0/24` de entrada.
- [x] Configurar el puerto `80` de entrada para origen `20.0.0.0/16`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado una subred pública `CIDR` `20.0.0.0/24` y subredes solo `VPN` `CIDR` `20.0.1.0/24` junto con la puerta de enlace `VPN` `vgw-12345` para conectarse al centro de datos del usuario. ¿Cuál de las siguientes opciones es una entrada válida para la tabla de enrutamiento principal en este escenario?

- [ ] Destino: `20.0.0.0/24` y Destino: `vgw-12345`.
- [ ] Destino: `20.0.0.0/16` y Destino: `ALL`.
- [ ] Destino: `20.0.1.0/16` y Destino: `vgw-12345`.
- [x] Destino: `0.0.0.0/0` y Destino: `vgw-12345`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred pública usa `CIDR` `20.0.1.0/24`. El usuario planea alojar un servidor web en la subred pública (puerto `80`) y un servidor de base de datos en la subred privada (puerto `3306`). El usuario está configurando un grupo de seguridad para la subred pública (`WebSecGrp`) y la subred privada (`DBSecGrp`). ¿Cuál de las siguientes entradas se requiere en el grupo de seguridad de la base de datos de la subred privada (`DBSecGrp`)?

- [x] Permitir entrada en el puerto `3306` para origen el grupo de seguridad del servidor web (`WebSecGrp`).
- [ ] Permitir entrada en el puerto `3306` desde origen `20.0.0.0/16`.
- [ ] Permitir salida en el puerto `3306` para destino el grupo de seguridad del servidor web (`WebSecGrp`).
- [ ] Permitir salida en el puerto `80` para destino la IP de la instancia `NAT`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente de `VPC`. El usuario ha creado un `CIDR` público `20.0.0.0/24` y una subred solo `VPN` `CIDR` `20.0.1.0/24` junto con el acceso `VPN` de hardware para conectarse al centro de datos del usuario. ¿Cuál de los siguientes componentes NO está presente cuando la `VPC` se configura con el asistente?

- [ ] Tabla de enrutamiento principal adjunta con una subred solo `VPN`.
- [x] Una instancia `NAT` configurada para permitir que las instancias de la subred `VPN` se conecten a internet.
- [ ] Tabla de enrutamiento personalizada adjunta con una subred pública.
- [ ] Una puerta de enlace de internet para una subred pública.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado subredes públicas y solo `VPN` junto con acceso `VPN` de hardware para conectarse al centro de datos del usuario. El usuario aún no ha lanzado ninguna instancia ni ha modificado o eliminado ninguna configuración. Quiere eliminar esta `VPC` desde la consola. ¿La consola permitirá al usuario eliminar la `VPC`?

- [ ] Sí, la consola eliminará todas las configuraciones y también eliminará la puerta de enlace privada virtual.
- [x] No, la consola le pedirá al usuario que desconecte manualmente la puerta de enlace privada virtual primero y luego permitirá eliminar la `VPC`.
- [ ] Sí, la consola eliminará todas las configuraciones y desconectará la puerta de enlace privada virtual.
- [ ] No, ya que la instancia `NAT` está en ejecución.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado una subred pública `CIDR` `20.0.0.0/24` y subredes solo `VPN` `CIDR` `20.0.1.0/24` junto con la puerta de enlace `VPN` `vgw-12345` para conectarse al centro de datos del usuario. El centro de datos del usuario tiene `CIDR` `172.28.0.0/12`. El usuario también ha configurado una instancia `NAT` `i-123456` para permitir tráfico a internet desde la subred `VPN`. ¿Cuál de las siguientes opciones NO es una entrada válida para la tabla de enrutamiento principal en este escenario?

- [x] Destino: `20.0.1.0/24` y Destino: `i-12345`.
- [ ] Destino: `0.0.0.0/0` y Destino: `i-12345`.
- [ ] Destino: `172.28.0.0/12` y Destino: `vgw-12345`.
- [ ] Destino: `20.0.0.0/16` y Destino: `local`.

**[⬆ Volver arriba](#tabla-de-contenidos)**
