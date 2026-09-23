### Una instancia de Amazon EC2 necesita ser accesible desde internet. La instancia de EC2 está en una subred con la siguiente tabla de enrutamiento. ¿Qué entrada debe agregar un ingeniero de CloudOps a la tabla de enrutamiento para cumplir con este requisito?

![Question 1](images/question1.jpg)

- [ ] Una ruta para `0.0.0.0/0` que apunte a una puerta de enlace `NAT`.
- [ ] Una ruta para `0.0.0.0/0` que apunte a una puerta de enlace de internet solo de salida (egress-only).
- [x] Una ruta para `0.0.0.0/0` que apunte a una puerta de enlace de internet.
- [ ] Una ruta para `0.0.0.0/0` que apunte a una interfaz de red elástica.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps lanza una instancia de Amazon EC2 en una subred privada de una `VPC`. Cuando el ingeniero de CloudOps intenta ejecutar un comando `curl` desde la línea de comandos de la instancia de EC2, no logra conectarse a `https:www.example.com`. ¿Qué debe hacer el ingeniero de CloudOps para resolver este problema?

- [x] Asegurarse de que exista un grupo de seguridad de salida que permita el puerto `443` hacia `0.0.0.0/0`.
- [ ] Asegurarse de que exista un grupo de seguridad de entrada que permita el puerto `443` desde `0.0.0.0/0`.
- [ ] Asegurarse de que exista una `ACL` de red de salida para los puertos efímeros `1024-66535` hacia `0.0.0.0/0`.
- [ ] Asegurarse de que exista una `ACL` de red de salida para el puerto `80` hacia `0.0.0.0/0`.

**[⬆ Volver arriba](#table-of-contents)**

### El sitio web público de una empresa está alojado en un bucket de Amazon S3 en la región `us-east-1`, detrás de una distribución de Amazon CloudFront. La empresa quiere asegurarse de que el sitio web esté protegido contra ataques DDoS. Un ingeniero de CloudOps necesita implementar una solución que le dé a la empresa la capacidad de mantener control sobre el límite de velocidad (rate limit) con el que se aplican las protecciones contra DDoS. ¿Qué solución cumple con estos requisitos?

- [x] Implementar una `ACL` web de AWS WAF con alcance global, con una acción predeterminada de permitir. Configurar una regla de AWS WAF basada en tasa (rate-based) para bloquear el tráfico que coincida. Asociar la `ACL` web con la distribución de CloudFront.
- [ ] Implementar una `ACL` web de AWS WAF con una acción predeterminada de permitir en `us-east-1`. Configurar una regla de AWS WAF basada en tasa para bloquear el tráfico que coincida. Asociar la `ACL` web con el bucket de S3.
- [ ] Implementar una `ACL` web de AWS WAF con alcance global, con una acción predeterminada de bloquear. Configurar una regla de AWS WAF basada en tasa para permitir el tráfico que coincida. Asociar la `ACL` web con la distribución de CloudFront.
- [ ] Implementar una `ACL` web de AWS WAF con una acción predeterminada de bloquear en `us-east-1`. Configurar una regla de AWS WAF basada en tasa para permitir el tráfico que coincida. Asociar la `ACL` web con el bucket de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja un portal de compras en línea en la nube de AWS. El portal ofrece seguridad `HTTPS` mediante un certificado TLS en un Elastic Load Balancer (ELB). Recientemente, el portal sufrió una interrupción porque el certificado TLS expiró. Un ingeniero de CloudOps debe crear una solución para renovar automáticamente los certificados y evitar este problema en el futuro. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Solicitar un certificado público mediante AWS Certificate Manager (ACM). Asociar el certificado de ACM con el ELB. Escribir una función de AWS Lambda programada para renovar el certificado cada 18 meses.
- [x] Solicitar un certificado público mediante AWS Certificate Manager (ACM). Asociar el certificado de ACM con el ELB. ACM administrará automáticamente la renovación del certificado.
- [ ] Registrar un certificado con una autoridad certificadora (CA) externa. Importar este certificado a AWS Certificate Manager (ACM). Asociar el certificado de ACM con el ELB. ACM administrará automáticamente la renovación del certificado.
- [ ] Registrar un certificado con una autoridad certificadora (CA) externa. Configurar el ELB para importar el certificado directamente desde la CA. Establecer el ciclo de actualización del certificado en el ELB para que se renueve cuando falten 3 meses para la fecha de vencimiento.

**[⬆ Volver arriba](#table-of-contents)**

### Ante la amenaza de virus de ransomware que cifran y retienen como rehenes los datos de la empresa, ¿qué acción se debe tomar para proteger un bucket de Amazon S3?

- [ ] Denegar las acciones Post, Put y Delete en el bucket.
- [x] Habilitar el cifrado del lado del servidor en el bucket.
- [ ] Habilitar el versionado de Amazon S3 en el bucket.
- [ ] Habilitar instantáneas (snapshots) en el bucket.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa se está asociando con un proveedor externo para brindar servicios de procesamiento de datos. Para esta integración, el proveedor debe alojar los datos de la empresa en un bucket de Amazon S3 dentro de la cuenta de AWS del proveedor. El proveedor permite que la empresa proporcione una clave de AWS Key Management Service (AWS KMS) para cifrar los datos de la empresa. El proveedor le ha entregado a la empresa el Amazon Resource Name (ARN) de un rol de IAM para esta integración. ¿Qué debe hacer un ingeniero de CloudOps para configurar esta integración?

- [x] Crear una nueva clave de KMS. Agregar el ARN del rol de IAM del proveedor a la política de la clave de KMS. Entregar el ARN de la nueva clave de KMS al proveedor.
- [ ] Crear una nueva clave de KMS. Crear un nuevo usuario de IAM. Agregar el ARN del rol de IAM del proveedor a una política en línea adjunta al usuario de IAM. Entregar el ARN del nuevo usuario de IAM al proveedor.
- [ ] Configurar el cifrado usando la clave de S3 administrada por KMS. Agregar el ARN del rol de IAM del proveedor a la política de la clave de S3 administrada por KMS. Entregar el ARN de la clave de S3 administrada por KMS al proveedor.
- [ ] Configurar el cifrado usando la clave de S3 administrada por KMS. Crear un bucket de S3. Agregar el ARN del rol de IAM del proveedor a la política del bucket de S3. Entregar el ARN del bucket de S3 al proveedor.

**[⬆ Volver arriba](#table-of-contents)**

### Una base de datos se ejecuta en una instancia de Amazon RDS Multi-AZ. Una auditoría de seguridad reciente encontró que la base de datos no cumple con la normativa porque no está cifrada. ¿Qué enfoque resolverá el requisito de cifrado?

- [ ] Iniciar sesión en la consola de RDS y seleccionar la casilla de cifrado para cifrar la base de datos.
- [ ] Crear un nuevo volumen de Amazon EBS cifrado y adjuntarlo a la instancia.
- [ ] Cifrar la réplica en espera (standby) en la Zona de disponibilidad secundaria y promoverla a instancia principal.
- [x] Tomar una instantánea de la instancia de RDS, copiarla y cifrar la copia, y luego restaurarla en una nueva instancia de RDS.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps recibe una alerta de Amazon GuardDuty sobre actividad de red sospechosa en una instancia de Amazon EC2. El hallazgo de GuardDuty indica una nueva dirección IP externa como destino del tráfico. El ingeniero de CloudOps no reconoce esa dirección IP externa y debe bloquear el tráfico hacia la dirección IP externa identificada por GuardDuty. ¿Qué solución cumple con este requisito?

- [ ] Crear un nuevo grupo de seguridad para bloquear el tráfico hacia la dirección IP externa. Asignar el nuevo grupo de seguridad a la instancia de EC2.
- [ ] Usar los registros de flujo (flow logs) de `VPC` con Amazon Athena para bloquear el tráfico hacia la dirección IP externa.
- [x] Crear una `ACL` de red. Agregar una regla de denegación de salida para el tráfico hacia la dirección IP externa.
- [ ] Crear un nuevo grupo de seguridad para bloquear el tráfico hacia la dirección IP externa. Asignar el nuevo grupo de seguridad a toda la `VPC`.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación web se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Las instancias se ejecutan en un grupo de Auto Scaling distribuido en varias Zonas de disponibilidad. Un ingeniero de CloudOps observa que algunas de estas instancias de EC2 aparecen como saludables en el grupo de Auto Scaling, pero aparecen como no saludables en el grupo de destino del `ALB`. ¿Cuál es una posible razón de este problema?

- [ ] Los grupos de seguridad no están permitiendo el tráfico entre el `ALB` y las instancias de EC2 que están fallando.
- [ ] La verificación de estado del grupo de Auto Scaling está configurada para usar verificaciones de estado de EC2.
- [ ] Las instancias de EC2 están fallando al iniciarse y no pasan las verificaciones de estado de EC2.
- [x] La verificación de estado del grupo de destino está configurada con un puerto o una ruta incorrectos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha habilitado AWS CloudTrail en una cuenta de AWS. Si CloudTrail se deshabilita, debe volver a habilitarse de inmediato. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos SIN escribir código personalizado?

- [ ] Agregar la cuenta de AWS a AWS Organizations. Habilitar CloudTrail en la cuenta de administración (management account).
- [x] Crear una regla de AWS Config que se invoque cuando cambie la configuración de CloudTrail.
Aplicar la acción de remediación automática `AWS-ConfigureCloudTrailLogging`.
- [ ] Crear una regla de AWS Config que se invoque cuando cambie la configuración de CloudTrail.
Configurar la regla para que invoque una función de AWS Lambda que habilite CloudTrail.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) programada cada hora para ejecutar un documento de Automation de AWS Systems Manager que habilite CloudTrail.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita permitir que los usuarios carguen objetos a un bucket de Amazon S3. El ingeniero de CloudOps crea una URL prefirmada (presigned URL) y se la entrega a un usuario, pero el usuario no puede cargar un objeto al bucket de S3. La URL prefirmada no ha expirado y no hay ninguna política de bucket aplicada al bucket de S3. ¿Cuál de las siguientes podría ser la causa de este problema?

- [ ] El usuario no ha configurado correctamente la AWS CLI con su clave de acceso y su clave de acceso secreta.
- [x] El ingeniero de CloudOps no tiene los permisos necesarios para cargar el objeto al bucket de S3.
- [ ] El ingeniero de CloudOps debe aplicar una política de bucket al bucket de S3 para permitir que el usuario cargue el objeto.
- [ ] El objeto ya fue cargado mediante el uso de la URL prefirmada, por lo que la URL prefirmada ya no es válida.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación web en tres instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa observa que períodos aleatorios de mayor tráfico causan una degradación en el rendimiento de la aplicación. Un ingeniero de CloudOps debe escalar la aplicación para hacer frente al aumento de tráfico. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una alarma de Amazon CloudWatch para monitorear la latencia de la aplicación y aumentar el tamaño de cada instancia de EC2 si se alcanza el umbral deseado.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para monitorear la latencia de la aplicación y agregar una instancia de EC2 al `ALB` si se alcanza el umbral deseado.
- [x] Implementar la aplicación en un grupo de Auto Scaling de instancias de EC2 con una política de escalado por seguimiento de destino (target tracking). Adjuntar el `ALB` al grupo de Auto Scaling.
- [ ] Implementar la aplicación en un grupo de Auto Scaling de instancias de EC2 con una política de escalado programado. Adjuntar el `ALB` al grupo de Auto Scaling.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa utiliza un sistema de archivos de Amazon Elastic File System (Amazon EFS) para compartir archivos entre muchas instancias de Amazon EC2 con Linux. Un ingeniero de CloudOps observa que la métrica `PercentIOLimit` del sistema de archivos se mantiene consistentemente en `100%` durante 15 minutos o más. El ingeniero de CloudOps también observa que la aplicación que lee y escribe en ese sistema de archivos tiene un rendimiento deficiente. La aplicación requiere alto throughput y muchas IOPS al acceder al sistema de archivos. ¿Qué debe hacer el ingeniero de CloudOps para remediar la métrica `PercentIOLimit` consistentemente alta?

- [ ] Crear un nuevo sistema de archivos EFS que use el modo de rendimiento Max I/O. Usar AWS DataSync para migrar los datos al nuevo sistema de archivos EFS.
- [ ] Crear una política de ciclo de vida en EFS para transicionar los archivos futuros a la clase de almacenamiento de Acceso Infrecuente (IA) y mejorar el rendimiento. Usar AWS DataSync para migrar los datos existentes al almacenamiento IA.
- [ ] Modificar el sistema de archivos EFS existente y activar el modo de rendimiento Max I/O.
- [x] Modificar el sistema de archivos EFS existente y activar el modo `Provisioned Throughput` (rendimiento aprovisionado).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa necesita restringir el acceso a un bucket de Amazon S3 únicamente a instancias de Amazon EC2 que estén dentro de una `VPC`. Todo el tráfico debe transitar por la red privada de AWS. ¿Qué acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear un endpoint de `VPC` para el bucket de S3, y crear una política de IAM que limite condicionalmente todas las acciones de S3 sobre el bucket para que el origen sea el endpoint de `VPC`.
- [x] Crear un endpoint de `VPC` para el bucket de S3, y crear una política de bucket de S3 que limite condicionalmente todas las acciones de S3 sobre el bucket para que el origen sea el endpoint de `VPC`.
- [ ] Crear un rol vinculado a servicio (service-linked role) para Amazon EC2 que permita a las instancias de EC2 interactuar directamente con Amazon S3, y adjuntar al rol una política de IAM que dé a las instancias de EC2 acceso completo al bucket de S3.
- [ ] Crear una puerta de enlace `NAT` en la `VPC`, y modificar la tabla de enrutamiento de la `VPC` para enrutar todo el tráfico destinado a Amazon S3 a través de la puerta de enlace `NAT`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa administra múltiples cuentas de AWS mediante una sola organización en AWS Organizations. La empresa está revisando la seguridad interna de su entorno de AWS. El ingeniero de seguridad de la empresa tiene su propia cuenta de AWS y quiere revisar la configuración de `VPC` de las cuentas de AWS de los desarrolladores. ¿Qué solución cumple con estos requisitos de la manera MÁS segura?

- [ ] Crear una política de IAM en cada cuenta de desarrollador con acceso de solo lectura relacionado con recursos de `VPC`. Asignar la política a un usuario de IAM. Compartir las credenciales del usuario con el ingeniero de seguridad.
- [ ] Crear una política de IAM en cada cuenta de desarrollador con acceso de administrador a todas las acciones de Amazon EC2, incluidas las acciones de `VPC`. Asignar la política a un usuario de IAM. Compartir las credenciales del usuario con el ingeniero de seguridad.
- [ ] Crear una política de IAM en cada cuenta de desarrollador con acceso de administrador relacionado con recursos de `VPC`. Asignar la política a un rol de IAM entre cuentas (cross-account). Pedirle al ingeniero de seguridad que asuma el rol desde su cuenta.
- [x] Crear una política de IAM en cada cuenta de desarrollador con acceso de solo lectura relacionado con recursos de `VPC`. Asignar la política a un rol de IAM entre cuentas (cross-account). Pedirle al ingeniero de seguridad que asuma el rol desde su cuenta.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa migró una aplicación intensiva en operaciones de E/S a una instancia de Amazon EC2 de propósito general. La instancia de EC2 tiene adjunto un único volumen de Amazon Elastic Block Store (Amazon EBS) de tipo General Purpose SSD. Los usuarios de la aplicación reportan que ciertas acciones que requieren lectura y escritura intensivas en disco tardan mucho más de lo normal o fallan por completo. Al revisar las métricas de rendimiento del volumen de EBS, un ingeniero de CloudOps observa que la métrica `VolumeQueueLength` se mantiene consistentemente alta durante los mismos períodos en los que los usuarios reportan problemas. El ingeniero de CloudOps necesita resolver este problema para restaurar el rendimiento completo de la aplicación. ¿Qué acción cumple con estos requisitos?

- [ ] Modificar el tipo de instancia a uno optimizado para almacenamiento.
- [ ] Modificar las propiedades del volumen desmarcando la opción Auto-Enable Volume I/O.
- [x] Modificar las propiedades del volumen para aumentar las IOPS.
- [ ] Modificar la instancia para habilitar redes mejoradas (enhanced networking).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene múltiples conexiones AWS Site-to-Site `VPN` entre una `VPC` y sus oficinas remotas. La empresa administra un dominio de Amazon Elasticsearch Service (Amazon ES) configurado con acceso público. El dominio de Amazon ES tiene una política de acceso al dominio abierta. Un ingeniero de CloudOps necesita asegurarse de que Amazon ES solo pueda ser accedido desde las oficinas remotas, preservando los datos existentes. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar una política de acceso basada en identidad en Amazon ES. Agregar una declaración de permiso (allow) a la política que incluya el Amazon Resource Name (ARN) de cada conexión `VPN` de las oficinas remotas.
- [x] Configurar una política de acceso al dominio basada en IP en Amazon ES. Agregar una declaración de permiso (allow) a la política que incluya los bloques `CIDR` de IP privada de cada red de oficina remota.
- [ ] Implementar un nuevo dominio de Amazon ES en subredes privadas dentro de una `VPC`, e importar una instantánea del dominio anterior. Crear un grupo de seguridad que permita tráfico de entrada desde los bloques `CIDR` de las oficinas remotas.
- [ ] Reconfigurar el dominio de Amazon ES en subredes privadas dentro de una `VPC`. Crear un grupo de seguridad que permita tráfico de entrada desde los bloques `CIDR` de las oficinas remotas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa administra muchas cuentas mediante una única organización en AWS Organizations. La organización tiene todas las funciones habilitadas. La empresa quiere activar AWS Config en todas las cuentas de la organización y en todas las regiones de AWS. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?

- [x] Usar `StackSets` de AWS CloudFormation para implementar instancias de stack que activen AWS Config en todas las cuentas y en todas las regiones.
- [ ] Usar `StackSets` de AWS CloudFormation para implementar políticas de stack que activen AWS Config en todas las cuentas y en todas las regiones.
- [ ] Usar Políticas de Control de Servicio (SCP) para configurar AWS Config en todas las cuentas y en todas las regiones.
- [ ] Crear un script que use la AWS CLI para activar AWS Config en todas las cuentas de la organización. Ejecutar el script desde la cuenta de administración de la organización.

**[⬆ Volver arriba](#table-of-contents)**

### El ingeniero de CloudOps de una empresa implementa cuatro nuevas instancias de Amazon EC2 utilizando la Amazon Machine Image (AMI) estándar de Amazon Linux 2. La empresa necesita poder usar AWS Systems Manager para administrar las instancias. El ingeniero de CloudOps observa que las instancias no aparecen en la consola de Systems Manager. ¿Qué debe hacer el ingeniero de CloudOps para resolver este problema?

- [ ] Conectarse a cada instancia mediante `SSH`. Instalar el Systems Manager Agent en cada instancia. Configurar el Systems Manager Agent para que se inicie automáticamente cuando las instancias arranquen.
- [ ] Usar AWS Certificate Manager (ACM) para crear un certificado TLS. Importar el certificado a cada instancia. Configurar el Systems Manager Agent para que use el certificado TLS en las comunicaciones seguras.
- [ ] Conectarse a cada instancia mediante `SSH`. Crear una cuenta `ssm-user`. Agregar la cuenta `ssm-user` al directorio `/etcsudoers`.
- [x] Adjuntar un perfil de instancia de IAM a las instancias. Asegurarse de que el perfil de instancia contenga la política `AmazonSSMManagedinstanceCore`.

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo de desarrollo implementó recientemente una nueva versión de una aplicación web en producción. Después del lanzamiento, una prueba de penetración reveló una vulnerabilidad de cross-site scripting que podría exponer datos de usuarios. ¿Qué servicio de AWS mitigará este problema?

- [ ] AWS Shield Standard.
- [x] AWS WAF.
- [ ] Elastic Load Balancing.
- [ ] Amazon Cognito.

**[⬆ Volver arriba](#table-of-contents)**

### Una instancia de Amazon EC2 ejecuta una aplicación que utiliza colas de Amazon Simple Queue Service (Amazon SQS). Un ingeniero de CloudOps debe asegurarse de que la aplicación pueda leer, escribir y eliminar mensajes de las colas de SQS. ¿Qué solución cumple con estos requisitos de la manera MÁS segura?

- [ ] Crear un usuario de IAM con una política de IAM que permita el permiso `sqs:SendMessage`, el permiso `sqs:ReceiveMessage` y el permiso `sqs:DeleteMessage` sobre las colas correspondientes. Incrustar las credenciales del usuario de IAM en la configuración de la aplicación.
- [ ] Crear un usuario de IAM con una política de IAM que permita el permiso `sqs:SendMessage`, el permiso `sqs:ReceiveMessage` y el permiso `sqs:DeleteMessage` sobre las colas correspondientes. Exportar la clave de acceso y la clave de acceso secreta del usuario de IAM como variables de entorno en la instancia de EC2.
- [ ] Crear y asociar un rol de IAM que permita a las instancias de EC2 invocar servicios de AWS. Adjuntar al rol una política de IAM que permita todos los permisos `sqs:*` sobre las colas correspondientes.
- [x] Crear y asociar un rol de IAM que permita a las instancias de EC2 invocar servicios de AWS. Adjuntar al rol una política de IAM que permita el permiso `sqs:SendMessage`, el permiso `sqs:ReceiveMessage` y el permiso `sqs:DeleteMessage` sobre las colas correspondientes.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una política que exige que todas las instancias de Amazon EC2 tengan un conjunto específico de etiquetas (tags). Si una instancia de EC2 no tiene las etiquetas requeridas, la instancia no conforme debe terminarse. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que envíe todos los cambios de estado de las instancias de EC2 a una función de AWS Lambda para determinar si cada instancia es conforme. Terminar cualquier instancia no conforme.
- [ ] Crear una política de IAM que haga cumplir todos los requisitos de etiquetado de instancias de EC2. Si una instancia no tiene las etiquetas requeridas, la política terminará la instancia no conforme.
- [ ] Crear una función de AWS Lambda para determinar si cada instancia de EC2 es conforme y terminar una instancia si no lo es. Programar la función Lambda para que se invoque cada 5 minutos.
- [x] Crear una regla de AWS Config para verificar si están presentes las etiquetas requeridas. Si una instancia de EC2 no es conforme, invocar un documento de Automation de AWS Systems Manager para terminar la instancia.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps quiere cargar un archivo de 1 TB de tamaño desde un entorno on-premises a un bucket de Amazon S3 usando cargas multiparte (multipart uploads). ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Cargar el archivo usando la consola de S3.
- [ ] Usar el comando `s3api copy-object`.
- [ ] Usar el comando `s3api put-object`.
- [x] Usar el comando `s3 cp`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps lanza una instancia de Amazon EC2 con Linux en una subred pública. Una vez que la instancia está en ejecución, el ingeniero de CloudOps obtiene la dirección IP pública e intenta conectarse remotamente a la instancia varias veces. Sin embargo, siempre recibe un error de tiempo de espera (timeout). ¿Qué acción permitirá al ingeniero de CloudOps conectarse remotamente a la instancia?

- [ ] Agregar una entrada en la tabla de enrutamiento de la subred pública para la dirección IP del ingeniero de CloudOps.
- [ ] Agregar una regla de `ACL` de red de salida que permita el puerto `TCP` `22` para la dirección IP del ingeniero de CloudOps.
- [x] Modificar el grupo de seguridad de la instancia para permitir tráfico `SSH` de entrada desde la dirección IP del ingeniero de CloudOps.
- [ ] Modificar el grupo de seguridad de la instancia para permitir tráfico `SSH` de salida hacia la dirección IP del ingeniero de CloudOps.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere usar únicamente IPv6 para todas sus instancias de Amazon EC2. Las instancias de EC2 no deben ser accesibles desde internet, pero sí deben poder acceder a internet. La empresa crea una `VPC` de doble pila (dual-stack) y subredes exclusivas de IPv6. ¿Cómo debe configurar un ingeniero de CloudOps la `VPC` para cumplir con estos requisitos?

- [ ] Crear y adjuntar una puerta de enlace `NAT`. Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace `NAT`. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.
- [ ] Crear y adjuntar una puerta de enlace de internet. Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace de internet. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.
- [x] Crear y adjuntar una puerta de enlace de internet solo de salida (egress-only). Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace de internet solo de salida. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.
- [ ] Crear y adjuntar una puerta de enlace de internet y una puerta de enlace `NAT`. Crear una tabla de enrutamiento personalizada que incluya una entrada para dirigir todo el tráfico IPv6 hacia la puerta de enlace de internet y todo el tráfico IPv4 hacia la puerta de enlace `NAT`. Adjuntar la tabla de enrutamiento personalizada a las subredes exclusivas de IPv6.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps quiere administrar una aplicación de servidor web con AWS Elastic Beanstalk. El servicio de Elastic Beanstalk debe mantener siempre la capacidad completa durante las nuevas implementaciones. ¿Qué políticas de despliegue satisfacen este requisito? (Seleccione DOS.)

- [ ] Todo a la vez (All at once).
- [x] Inmutable (Immutable).
- [ ] Reconstrucción (Rebuild).
- [ ] Continuo (Rolling).
- [x] Continuo con lote adicional (Rolling with additional batch).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa le pide a un ingeniero de CloudOps que garantice que los archivos de AWS CloudTrail no sean alterados después de su creación. Actualmente, la empresa usa AWS Identity and Access Management (IAM) para restringir el acceso a rutas de seguimiento (trails) específicas. El equipo de seguridad de la empresa necesita poder rastrear la integridad de cada archivo. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que invoque una función de AWS Lambda cuando se entregue un nuevo archivo. Configurar la función Lambda para calcular un hash MD5 del archivo y almacenar el resultado en una tabla de Amazon DynamoDB. El equipo de seguridad puede usar los valores almacenados en DynamoDB para verificar la integridad de los archivos entregados.
- [ ] Crear una función de AWS Lambda que se invoque cada vez que se entregue un nuevo archivo al bucket de CloudTrail. Configurar la función Lambda para calcular un hash MD5 del archivo y almacenar el resultado como una etiqueta (tag) en un objeto de Amazon S3. El equipo de seguridad puede usar la información de la etiqueta para verificar la integridad de los archivos entregados.
- [ ] Habilitar la función de integridad de archivos de CloudTrail en un bucket de Amazon S3. Crear una política de IAM que otorgue al equipo de seguridad acceso a los registros de integridad de archivos almacenados en el bucket de S3.
- [x] Habilitar la función de integridad de archivos de CloudTrail en la ruta de seguimiento (trail). El equipo de seguridad puede usar el archivo resumen (digest file) creado por CloudTrail para verificar la integridad de los archivos entregados.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene múltiples instancias de Amazon EC2 que ejecutan una aplicación intensiva en recursos en un entorno de desarrollo. Un ingeniero de CloudOps está implementando una solución para detener estas instancias de EC2 cuando no están en uso. ¿Qué solución cumple con este requisito?

- [ ] Evaluar los registros de AWS CloudTrail para verificar que no haya actividad de la API de EC2. Invocar una función de AWS Lambda para detener las instancias de EC2.
- [x] Crear una alarma de Amazon CloudWatch para detener las instancias de EC2 cuando el uso promedio de CPU sea inferior al `5%` durante un período de 30 minutos.
- [ ] Crear una métrica de Amazon CloudWatch para detener las instancias de EC2 cuando la métrica `VolumeReadBytes` sea inferior a `500` durante un período de 30 minutos.
- [ ] Usar AWS Config para invocar una función de AWS Lambda que detenga las instancias de EC2 según los cambios de configuración de recursos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa crea imágenes AMI personalizadas lanzando nuevas instancias de Amazon EC2 desde una plantilla de AWS CloudFormation; instala y configura el software necesario mediante AWS OpsWorks y luego toma imágenes de cada instancia de EC2. El proceso de instalación y configuración del software puede tardar entre 2 y 3 horas, pero a veces el proceso se detiene por errores de instalación. El ingeniero de CloudOps debe modificar la plantilla de CloudFormation para que, si el proceso se detiene, todo el stack falle y se revierta (rollback). Con base en estos requisitos, ¿qué se debe agregar a la plantilla?

- [ ] `Conditions` con un tiempo de espera (timeout) configurado en 4 horas.
- [x] `CreationPolicy` con un tiempo de espera configurado en 4 horas.
- [ ] `DependsOn` con un tiempo de espera configurado en 4 horas.
- [ ] `Metadata` con un tiempo de espera configurado en 4 horas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa planea ejecutar una aplicación web pública en instancias de Amazon EC2 detrás de un Elastic Load Balancer (ELB). El equipo de seguridad de la empresa quiere proteger el sitio web usando certificados de AWS Certificate Manager (ACM). El ELB debe redirigir automáticamente todas las solicitudes `HTTP` a `HTTPS`. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un Application Load Balancer con un listener `HTTPS` en el puerto `80`. Adjuntar un certificado SSL/TLS al listener del puerto `80`. Crear una regla para redirigir las solicitudes de `HTTP` a `HTTPS`.
- [x] Crear un Application Load Balancer con un listener `HTTP` en el puerto `80` y un listener con protocolo `HTTPS` en el puerto `443`. Adjuntar un certificado SSL/TLS al listener del puerto `443`. Crear una regla para redirigir las solicitudes del puerto `80` al puerto `443`.
- [ ] Crear un Application Load Balancer con dos listeners `TCP` en el puerto `80` y el puerto `443`. Adjuntar un certificado SSL/TLS al listener del puerto `443`. Crear una regla para redirigir las solicitudes del puerto `80` al puerto `443`.
- [ ] Crear un Network Load Balancer con dos listeners `TCP` en el puerto `80` y el puerto `443`. Adjuntar un certificado SSL/TLS al listener del puerto `443`. Crear una regla para redirigir las solicitudes del puerto `80` al puerto `443`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps es responsable de una aplicación heredada (legacy) intensiva en CPU. La aplicación solo puede escalarse verticalmente. Actualmente, la aplicación está desplegada en una única instancia de Amazon EC2 `t2.large`. El sistema muestra un uso de CPU del `90%` y una latencia de rendimiento significativa después de unos minutos. ¿Qué cambio se debe hacer para aliviar el problema de rendimiento?

- [ ] Cambiar el volumen de Amazon EBS a Provisioned IOPS.
- [x] Actualizar a una instancia optimizada para cómputo (compute-optimized).
- [ ] Agregar instancias `t2.large` adicionales a la aplicación.
- [ ] Comprar Instancias Reservadas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa migró recientemente su aplicación a una `VPC` en AWS. Una conexión AWS Site-to-Site `VPN` conecta la red on-premises de la empresa con la `VPC`. La aplicación obtiene datos de clientes desde otro sistema que reside on-premises. La aplicación usa un servidor `DNS` on-premises para resolver registros de dominio. Después de la migración, la aplicación no puede conectarse a los datos de clientes debido a errores de resolución de nombres. ¿Qué solución le dará a la aplicación la capacidad de resolver los nombres de dominio internos?

- [ ] Lanzar instancias de EC2 en la `VPC`. En las instancias de EC2, desplegar un reenviador (forwarder) `DNS` personalizado que envíe todas las solicitudes `DNS` al servidor `DNS` on-premises. Crear una zona alojada privada de Amazon Route 53 que use las instancias de EC2 como servidores de nombres.
- [x] Crear un endpoint de salida (outbound endpoint) de Amazon Route 53 Resolver. Configurar el endpoint de salida para reenviar las consultas `DNS` del dominio on-premises al servidor `DNS` on-premises.
- [ ] Configurar dos conexiones AWS Direct Connect entre el entorno de AWS y la red on-premises. Configurar un grupo de agregación de enlaces (LAG) que incluya ambas conexiones. Cambiar la dirección del resolver de la `VPC` para que apunte al servidor `DNS` on-premises.
- [ ] Crear una zona alojada pública de Amazon Route 53 para el dominio on-premises. Configurar las `ACL`s de red para reenviar las solicitudes `DNS` del dominio on-premises a la zona alojada pública de Route 53.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps crea una nueva `VPC` que incluye una subred pública y una subred privada. El ingeniero de CloudOps lanza con éxito 11 instancias de Amazon EC2 en la subred privada. El ingeniero de CloudOps intenta lanzar una instancia de EC2 adicional en la misma subred, pero recibe un mensaje de error que indica que no hay suficientes direcciones IP libres disponibles. ¿Qué debe hacer el ingeniero de CloudOps para desplegar más instancias de EC2?

- [ ] Editar la subred privada para cambiar el bloque `CIDR` a `/27`.
- [ ] Editar la subred privada para que se extienda a través de una segunda Zona de disponibilidad.
- [ ] Asignar direcciones IP elásticas adicionales a la subred privada.
- [x] Crear una nueva subred privada para alojar las instancias de EC2 requeridas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación crítica sin servidor (serverless) que utiliza múltiples funciones de AWS Lambda. Cada función Lambda genera `1 GB` de datos de registro diariamente en su propio grupo de registros (log group) de Amazon CloudWatch Logs. El equipo de seguridad de la empresa solicita un conteo de errores de la aplicación, agrupados por tipo, en todos los grupos de registros. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [x] Realizar una consulta de CloudWatch Logs Insights que use el comando `stats` y la función `count`.
- [ ] Realizar una búsqueda en CloudWatch Logs que use la palabra clave `groupby` y la función `count`.
- [ ] Realizar una consulta de Amazon Athena que use las palabras clave `SELECT` y `GROUP BY`.
- [ ] Realizar una consulta de Amazon RDS que use las palabras clave `SELECT` y `GROUP BY`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps aplica la siguiente política a un stack de AWS CloudFormation. ¿Cuál es el resultado de esta política?

![Question 35](images/question35.jpg)

- [ ] Los usuarios que asuman un rol de IAM con un ID lógico que comience con `Production` no podrán ejecutar el comando `update-stack`.
- [x] Los usuarios pueden actualizar todos los recursos del stack, excepto los recursos cuyo ID lógico comience con `Production`.
- [ ] Los usuarios pueden actualizar todos los recursos del stack, excepto los recursos cuyo atributo comience con `Production`.
- [ ] Los usuarios de un grupo de IAM con un ID lógico que comience con `Production` no podrán ejecutar el comando `update-stack`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está desplegando una aplicación en 10 instancias de Amazon EC2. La aplicación debe tener alta disponibilidad. Las instancias deben ubicarse en hardware físico distinto entre sí. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Lanzar las instancias en un grupo de ubicación (placement group) de tipo clúster en una sola región de AWS.
- [ ] Lanzar las instancias en un grupo de ubicación de tipo partición en múltiples regiones de AWS.
- [ ] Lanzar las instancias en un grupo de ubicación de tipo distribuido (spread) en múltiples regiones de AWS.
- [x] Lanzar las instancias en un grupo de ubicación de tipo distribuido (spread) en una sola región de AWS.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta un sitio web en instancias de Amazon EC2 dentro de un grupo de Auto Scaling. Cuando aumenta el tráfico del sitio web, las instancias adicionales tardan varios minutos en estar disponibles debido a un script de datos de usuario (user data) de larga duración que instala software. Un ingeniero de CloudOps debe reducir el tiempo necesario para que las nuevas instancias estén disponibles. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Reducir los umbrales de escalado para que las instancias se agreguen antes de que aumente el tráfico.
- [ ] Comprar Instancias Reservadas para cubrir el `100%` de la capacidad máxima del grupo de Auto Scaling.
- [ ] Actualizar el grupo de Auto Scaling para lanzar instancias de un tipo optimizado para almacenamiento.
- [x] Usar EC2 Image Builder para preparar una Amazon Machine Image (AMI) con el software preinstalado.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha lanzado una instancia de Amazon EC2 de propósito general de tamaño grande para procesar regularmente archivos de datos de gran tamaño. La instancia tiene adjunto un volumen de Amazon Elastic Block Store (Amazon EBS) de 1 TB de tipo `General Purpose SSD (gp2)`. La instancia también está optimizada para EBS. Para ahorrar costos, el ingeniero de CloudOps detiene la instancia cada noche y la reinicia cada mañana. Cuando el procesamiento de datos está activo, las métricas de Amazon CloudWatch de la instancia muestran consistentemente 3.000 `VolumeReadOps`. El ingeniero de CloudOps debe mejorar el rendimiento de E/S garantizando la integridad de los datos. ¿Qué acción cumple con estos requisitos?

- [ ] Cambiar el tipo de instancia a una de propósito general grande y con ráfagas (burstable).
- [ ] Cambiar el tipo de instancia a una de propósito general extra grande.
- [ ] Aumentar el volumen de EBS a un volumen `General Purpose SSD (gp2)` de 2 TB.
- [x] Mover los datos que residen en el volumen de EBS al almacenamiento de instancia (instance store).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta cargas de trabajo en 90 instancias de Amazon EC2 en la región `eu-west-1` dentro de una cuenta de AWS. En 2 meses, la empresa migrará las cargas de trabajo de `eu-west-1` a la región `eu-west-3`. La empresa necesita reducir el costo de las instancias de EC2. La empresa está dispuesta a asumir un compromiso de 1 año que comenzará la próxima semana. La empresa debe elegir una opción de compra de instancias de EC2 que proporcione descuentos para las 90 instancias de EC2 sin importar la región durante el período de 1 año. ¿Qué solución cumple con estos requisitos?

- [ ] Comprar Instancias Reservadas Estándar de EC2.
- [ ] Comprar un Savings Plan de instancias de EC2.
- [ ] Comprar Instancias Reservadas Convertibles de EC2.
- [x] Comprar un Compute Savings Plan.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa Amazon Elasticsearch Service (Amazon ES) para analizar datos de ventas y de uso de clientes. Los miembros del equipo de ventas de la empresa, geográficamente dispersos, están de viaje. Necesitan iniciar sesión en Kibana usando sus credenciales corporativas existentes, almacenadas en Active Directory. La empresa ha implementado Active Directory Federation Services (AD FS) para habilitar la autenticación hacia servicios en la nube. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar Active Directory como proveedor de autenticación en Amazon ES. Agregar el nombre de dominio del servidor de Active Directory a Amazon ES. Configurar Kibana para usar la autenticación de Amazon ES.
- [x] Implementar un grupo de usuarios (user pool) de Amazon Cognito. Configurar Active Directory como proveedor de identidad externo del grupo de usuarios. Habilitar la autenticación de Amazon Cognito para Kibana en Amazon ES.
- [ ] Habilitar la autenticación de usuarios de Active Directory en Kibana. Crear una política de acceso al dominio personalizada basada en IP en Amazon ES que incluya la dirección IP del servidor de Active Directory.
- [ ] Establecer una relación de confianza (trust) con Kibana en el servidor de Active Directory. Habilitar la autenticación de usuarios de Active Directory en Kibana. Agregar la dirección IP del servidor de Active Directory a Kibana.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa AWS Organizations. Un ingeniero de CloudOps quiere usar AWS Compute Optimizer y políticas de etiquetas (tag policies) de AWS en la cuenta de administración para gobernar todas las cuentas miembro de la familia de facturación. El ingeniero de CloudOps navega a la consola de AWS Organizations pero no puede activar las políticas de etiquetas desde la cuenta de administración. ¿Cuál podría ser la razón de este problema?

- [x] No se han habilitado todas las funciones (all features) en la organización.
- [ ] No se ha habilitado la facturación consolidada.
- [ ] Las cuentas miembro no tienen etiquetas habilitadas para la asignación de costos.
- [ ] Las cuentas miembro no han habilitado manualmente el acceso de confianza (trusted access) para Compute Optimizer.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está intentando descargar parches de internet hacia una instancia en una subred privada. Existe una puerta de enlace de internet para la `VPC`, y se ha desplegado una puerta de enlace `NAT` en la subred pública; sin embargo, la instancia no tiene conectividad a internet. Los recursos desplegados en la subred privada deben ser inaccesibles directamente desde internet público. Dada la información proporcionada, ¿qué se debe agregar a la tabla de enrutamiento de la subred privada para resolver este problema?

![Question 42](images/question42.png)

- [ ] `0.0.0.0/0` `IGW`.
- [x] `0.0.0.0/0` `NAT`.
- [ ] `10.0.1.0/24` `IGW`.
- [ ] `10.0.1.0/24` `NAT`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación sin estado (stateless) alojada en una flota de 10 instancias de Amazon EC2 On-Demand dentro de un grupo de Auto Scaling. Se necesitan un mínimo de 6 instancias para cumplir con los requisitos del servicio. ¿Qué acción mantendrá el tiempo de actividad de la aplicación de la manera MÁS rentable?

- [x] Usar una Spot Fleet con una capacidad On-Demand de 6 instancias.
- [ ] Actualizar el grupo de Auto Scaling con un mínimo de 6 instancias On-Demand y un máximo de 10 instancias On-Demand.
- [ ] Actualizar el grupo de Auto Scaling con un mínimo de 1 instancia On-Demand y un máximo de 6 instancias On-Demand.
- [ ] Usar una Spot Fleet con una capacidad objetivo (target capacity) de 6 instancias.

**[⬆ Volver arriba](#table-of-contents)**

### Una gran empresa utiliza AWS Organizations para administrar su entorno multi-cuenta de AWS. Según la política de la empresa, todos los usuarios deben tener acceso de solo lectura a un bucket de Amazon S3 en particular, ubicado en una cuenta central. Los datos del bucket de S3 no deben estar disponibles fuera de la organización. Un ingeniero de CloudOps debe configurar los permisos y agregar una política de bucket al bucket de S3. ¿Qué parámetros se deben especificar para lograr esto de la manera MÁS eficiente?

- [x] Especificar `"*"` como principal y `PrincipalOrgld` como condición.
- [ ] Especificar todos los números de cuenta como principal.
- [ ] Especificar `PrincipalOrgld` como principal.
- [ ] Especificar la cuenta de administración de la organización como principal.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita crear alertas basadas en las métricas de lectura y escritura de volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos a una instancia de Amazon EC2. El ingeniero de CloudOps crea y habilita alarmas de Amazon CloudWatch para la métrica `DiskReadBytes` y la métrica `DiskWriteBytes`. Una herramienta de monitoreo personalizada instalada en la instancia de EC2, con la misma configuración de alarma, indica que las métricas del volumen han superado el umbral. Sin embargo, las alarmas de CloudWatch no entraron en estado `ALARM`. ¿Qué acción garantizará que las alarmas de CloudWatch funcionen correctamente?

- [ ] Instalar y configurar el agente de CloudWatch en la instancia de EC2 para capturar las métricas deseadas.
- [ ] Instalar y configurar el AWS Systems Manager Agent en la instancia de EC2 para capturar las métricas deseadas.
- [x] Reconfigurar las alarmas de CloudWatch para usar la métrica `VolumeReadBytes` y la métrica `VolumeWriteBytes` de los volúmenes de EBS.
- [ ] Reconfigurar las alarmas de CloudWatch para usar la métrica `VolumeReadBytes` y la métrica `VolumeWriteBytes` de la instancia de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa actualiza su política de seguridad para prohibir la exposición pública de cualquier dato en los buckets de Amazon S3 de la cuenta de la empresa. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [x] Activar S3 Block Public Access a nivel de cuenta.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para hacer cumplir que todos los objetos de S3 sean privados.
- [ ] Usar Amazon Inspector para buscar buckets de S3 y restablecer automáticamente las `ACL`s de S3 si se encuentran buckets públicos de S3.
- [ ] Usar S3 Object Lambda para examinar las `ACL`s de S3 y cambiar cualquier `ACL` pública de S3 a privada.

**[⬆ Volver arriba](#table-of-contents)**

### Un informe de Amazon S3 Inventory revela que más de 1 millón de objetos en un bucket de S3 no están cifrados. Estos objetos deben cifrarse, y todos los objetos futuros deben cifrarse en el momento en que se escriben. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Seleccione DOS)

- [ ] Crear una regla de AWS Config que ejecute evaluaciones sobre los cambios de configuración del bucket de S3. Cuando se encuentre un objeto sin cifrar, ejecutar un documento de Automation de AWS Systems Manager para cifrar el objeto en su lugar.
- [x] Editar las propiedades del bucket de S3 para habilitar el cifrado predeterminado del lado del servidor.
- [x] Filtrar el informe de S3 Inventory usando S3 Select para encontrar todos los objetos que no estén cifrados. Crear un trabajo de S3 Batch Operations para copiar cada objeto en su lugar con el cifrado habilitado.
- [ ] Filtrar el informe de S3 Inventory usando S3 Select para encontrar todos los objetos que no estén cifrados. Enviar el nombre de cada objeto como un mensaje a una cola de Amazon Simple Queue Service (Amazon SQS). Usar la cola de SQS para invocar una función de AWS Lambda que etiquete cada objeto con una clave `Encryption` y un valor `SSE-KMS`.
- [ ] Usar S3 Event Notifications para invocar una función de AWS Lambda en todos los eventos de creación de nuevos objetos del bucket de S3. Configurar la función Lambda para verificar si el objeto está cifrado y ejecutar un documento de Automation de AWS Systems Manager para cifrar el objeto en su lugar cuando se encuentre uno sin cifrar.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación web se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB) de Elastic Load Balancing. Las instancias se ejecutan en un grupo de Auto Scaling distribuido en varias Zonas de disponibilidad. Un ingeniero de CloudOps ha notado que algunas instancias de EC2 aparecen como saludables en la consola de Auto Scaling, pero aparecen como no saludables en la consola de destino del `ALB`. ¿Cuál podría ser el problema?

- [ ] El período de gracia de la verificación de estado (health check grace period) del grupo de Auto Scaling está configurado demasiado bajo; hay que aumentarlo.
- [ ] La verificación de estado del grupo de destino está configurada incorrectamente y debe ajustarse.
- [ ] Los datos de usuario (user data) o la AMI usados en la configuración de lanzamiento del grupo de Auto Scaling son incorrectos.
- [x] El tipo de verificación de estado del grupo de Auto Scaling se basa en el estado de la instancia de EC2 en lugar de en las verificaciones de estado de Elastic Load Balancing.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación accede a datos a través de una interfaz de sistema de archivos. La aplicación se ejecuta en instancias de Amazon EC2 en múltiples Zonas de disponibilidad, todas las cuales deben compartir los mismos datos. Aunque la cantidad de datos es actualmente pequeña, la empresa anticipa que crecerá a decenas de terabytes durante la vida útil de la aplicación. ¿Cuál es la solución de almacenamiento MÁS escalable para cumplir con este requisito?

- [ ] Conectar un volumen grande de Amazon EBS a múltiples instancias y programar instantáneas.
- [x] Desplegar Amazon EFS en la `VPC` y crear puntos de montaje (mount targets) en múltiples subredes.
- [ ] Lanzar una instancia de EC2 y compartir los datos mediante SMB/CIFS o NFS.
- [ ] Desplegar un volumen en caché (cached volume) de AWS Storage Gateway en Amazon EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ampliando su uso de servicios de AWS en toda su cartera. La empresa quiere aprovisionar cuentas de AWS para cada equipo, con el fin de garantizar la separación de los procesos de negocio por motivos de cumplimiento de seguridad y facturación. La creación y configuración inicial (bootstrapping) de las cuentas debe realizarse de forma escalable y eficiente, de modo que las nuevas cuentas se creen con una línea base definida y con barreras de gobernanza (guardrails) implementadas. Un ingeniero de CloudOps necesita diseñar un proceso de aprovisionamiento que ahorre tiempo y recursos. ¿Qué acción se debe tomar para cumplir con estos requisitos?

- [ ] Automatizar usando AWS Elastic Beanstalk para aprovisionar las cuentas de AWS, configurar la infraestructura e integrarse con AWS Organizations.
- [ ] Crear scripts de configuración inicial (bootstrapping) en AWS OpsWorks y combinarlos con plantillas de AWS CloudFormation para aprovisionar cuentas e infraestructura.
- [ ] Usar AWS Config para aprovisionar cuentas y desplegar instancias usando AWS Service Catalog.
- [x] Usar AWS Control Tower para crear una plantilla en Account Factory y usar la plantilla para aprovisionar nuevas cuentas.

**[⬆ Volver arriba](#table-of-contents)**


### Una empresa aloja un portal web en instancias de Amazon EC2. El portal web usa un Elastic Load Balancer (ELB) y Amazon Route 53 como servicio `DNS` público. El ELB y las instancias de EC2 se despliegan mediante un único stack de AWS CloudFormation en la región `us-east-1`. El portal web debe tener alta disponibilidad en múltiples regiones. ¿Qué configuración cumple con estos requisitos?

- [ ] Desplegar una copia del stack en la región `us-west-2`. Crear un único registro de inicio de autoridad (`SOA`) en Route 53 que incluya la dirección IP de cada ELB. Configurar el registro `SOA` con verificaciones de estado. Usar el ELB de `us-east-1` como registro primario y el ELB de `us-west-2` como registro secundario.
- [x] Desplegar una copia del stack en la región `us-west-2`. Crear un registro `A` adicional en Route 53 que incluya el ELB de `us-west-2` como destino de alias. Configurar los registros `A` con una política de enrutamiento por conmutación por error (failover) y verificaciones de estado. Usar el ELB de `us-east-1` como registro primario y el ELB de `us-west-2` como registro secundario.
- [ ] Desplegar un nuevo grupo de instancias de EC2 en la región `us-west-2`. Asociar las nuevas instancias de EC2 con el ELB existente y configurar verificaciones de estado del balanceador de carga en todas las instancias de EC2. Configurar el ELB para actualizar Route 53 cuando las instancias de EC2 en `us-west-2` fallen las verificaciones de estado.
- [ ] Desplegar un nuevo grupo de instancias de EC2 en la región `us-west-2`. Configurar verificaciones de estado de EC2 en todas las instancias de EC2 de cada región. Configurar una conexión de emparejamiento (peering) entre las `VPC`s. Usar la `VPC` de `us-east-1` como registro primario y la `VPC` de `us-west-2` como registro secundario.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa necesita ver una lista de grupos de seguridad que están abiertos a internet en el puerto `3389`. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Configurar Amazon GuardDuty para escanear los grupos de seguridad y reportar acceso sin restricciones en el puerto `3389`.
- [ ] Configurar una Política de Control de Servicio (SCP) para identificar los grupos de seguridad que permiten acceso sin restricciones en el puerto `3389`.
- [ ] Usar AWS Identity and Access Management Access Analyzer para encontrar instancias que tengan acceso sin restricciones en el puerto `3389`.
- [x] Usar AWS Trusted Advisor para encontrar grupos de seguridad que permitan acceso sin restricciones en el puerto `3389`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una conexión AWS Site-to-Site `VPN` entre recursos on-premises y recursos alojados en una `VPC`. Un ingeniero de CloudOps lanza una instancia de Amazon EC2 que solo tiene una dirección IP privada en una subred privada de la `VPC`. La instancia de EC2 ejecuta Microsoft Windows Server. Un grupo de seguridad de la instancia de EC2 tiene reglas que permiten tráfico de entrada desde la red on-premises a través de la conexión `VPN`. El entorno on-premises contiene un firewall de red de un tercero. Las reglas de ese firewall permiten que el tráfico de Remote Desktop Protocol (RDP) fluya entre los usuarios on-premises a través de la conexión `VPN`. Los usuarios on-premises no pueden conectarse a la instancia de EC2 y reciben un error de tiempo de espera (timeout). ¿Qué debe hacer el ingeniero de CloudOps para solucionar este problema?

- [ ] Crear registros de Amazon CloudWatch para la instancia de EC2 y verificar si hay tráfico bloqueado.
- [ ] Crear registros de Amazon CloudWatch para la conexión Site-to-Site `VPN` y verificar si hay tráfico bloqueado.
- [x] Crear registros de flujo (`VPC` flow logs) para la interfaz de red elástica de la instancia de EC2 y verificar si hay tráfico rechazado.
- [ ] Indicar a los usuarios que usen EC2 Instance Connect como método de conexión.

**[⬆ Volver arriba](#table-of-contents)**

### Una auditoría organizacional reciente descubrió una base de datos existente de Amazon RDS que actualmente no está configurada para alta disponibilidad. Dada la naturaleza crítica de esta base de datos, debe configurarse para alta disponibilidad lo antes posible. ¿Cómo se puede cumplir con este requisito?

- [ ] Cambiar a un par de bases de datos activo/pasivo usando `create-db-instance-read-replica` con la marca `–availability-zone`.
- [ ] Especificar alta disponibilidad al crear una nueva instancia de RDS, y realizar una `live-migrate` de los datos.
- [x] Modificar la instancia de RDS usando la consola para incluir la opción Multi-AZ.
- [ ] Usar el comando `modify-db-instance` con la marca `–na`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está desplegando un sitio de prueba que se ejecuta en instancias de Amazon EC2. La aplicación requiere conectividad tanto de entrada como de salida hacia internet. ¿Qué combinación de pasos se requiere para proporcionar conectividad a internet a las instancias de EC2? (Elija dos.)

- [ ] Agregar una puerta de enlace `NAT` a una subred pública.
- [ ] Adjuntar una dirección privada a la interfaz de red elástica de la instancia de EC2.
- [ ] Adjuntar una dirección IP elástica a la puerta de enlace de internet.
- [x] Agregar una entrada en la tabla de enrutamiento de la subred que apunte a una puerta de enlace de internet.
- [x] Crear una puerta de enlace de internet y adjuntarla a una `VPC`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está probando Amazon Elasticsearch Service (Amazon ES) como solución para analizar registros del sistema provenientes de una flota de instancias de Amazon EC2. Durante la fase de prueba, el dominio opera en un clúster de un solo nodo. Un ingeniero de CloudOps necesita transformar el dominio de prueba en un despliegue de grado producción y alta disponibilidad. ¿Qué configuración de Amazon ES debe usar el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Usar un clúster de cuatro nodos de datos distribuidos en dos regiones de AWS. Desplegar cuatro nodos maestros dedicados en cada región.
- [x] Usar un clúster de seis nodos de datos distribuidos en tres Zonas de disponibilidad. Usar tres nodos maestros dedicados.
- [ ] Usar un clúster de seis nodos de datos distribuidos en tres Zonas de disponibilidad. Usar seis nodos maestros dedicados.
- [ ] Usar un clúster de ocho nodos de datos distribuidos en dos Zonas de disponibilidad. Desplegar cuatro nodos maestros en una región de AWS de conmutación por error.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está investigando por qué un usuario no ha podido usar `RDP` para conectarse a través de internet desde su computadora personal a un servidor bastión que se ejecuta en una instancia de Amazon EC2 con Windows. ¿Cuáles de las siguientes son posibles causas de este problema? (Elija dos.)

- [x] Una `ACL` de red asociada a la subred del bastión está bloqueando el tráfico de red.
- [ ] La instancia no tiene una dirección IP privada.
- [x] La tabla de enrutamiento asociada a la subred del bastión no tiene una ruta hacia la puerta de enlace de internet.
- [ ] El grupo de seguridad de la instancia no tiene una regla de entrada en el puerto `22`.
- [ ] El grupo de seguridad de la instancia no tiene una regla de salida en el puerto `3389`.

**[⬆ Volver arriba](#table-of-contents)**

### Mientras aseguraba la conexión entre la `VPC` de una empresa y su centro de datos on-premises, un ingeniero de seguridad envió un comando ping desde un host on-premises (dirección IP `203.0.113.12`) hacia una instancia de Amazon EC2 (dirección IP `172.31.16.139`). El comando ping no obtuvo respuesta. El registro de flujo (flow log) de la `VPC` mostró lo siguiente. ¿Qué acción se debe realizar para que el ping funcione?

![Question 58](images/question58_74_155.png)

- [ ] En el grupo de seguridad de la instancia de EC2, permitir tráfico `ICMP` de entrada.
- [ ] En el grupo de seguridad de la instancia de EC2, permitir tráfico `ICMP` de salida.
- [ ] En la `NACL` de la `VPC`, permitir tráfico `ICMP` de entrada.
- [x] En la `NACL` de la `VPC`, permitir tráfico `ICMP` de salida.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa global maneja una gran cantidad de información de identificación personal (PII, por sus siglas en inglés) a través de un portal web interno. La aplicación de la empresa se ejecuta en un centro de datos corporativo que está conectado a AWS mediante una conexión de AWS Direct Connect. La aplicación almacena la PII en Amazon S3. Según un requisito de cumplimiento normativo, el tráfico desde el portal web hacia Amazon S3 no debe transitar por internet. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con el requisito de cumplimiento?

- [x] Aprovisionar un endpoint de interfaz de `VPC` para Amazon S3. Modificar la aplicación para que use el endpoint de interfaz.
- [ ] Configurar AWS Network Firewall para redirigir el tráfico a la dirección interna de S3.
- [ ] Modificar la aplicación para que use el endpoint de estilo de ruta (path-style) de S3.
- [ ] Configurar un conjunto de `ACL`s de red de `VPC` para redirigir el tráfico a la dirección interna de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación se ejecuta en múltiples instancias de Amazon EC2 dentro de un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para usar la versión más reciente de una plantilla de lanzamiento (launch template). Un ingeniero de CloudOps debe diseñar una solución que administre de forma centralizada los registros de la aplicación y los conserve durante no más de 90 días. ¿Qué solución cumple con estos requisitos?

- [ ] Lanzar una Amazon Machine Image (AMI) preconfigurada con el agente de Amazon CloudWatch Logs para enviar registros a un bucket de Amazon S3. Aplicar una política de ciclo de vida de S3 de 90 días en el bucket de S3 para que los registros de la aplicación expiren.
- [ ] Lanzar una Amazon Machine Image (AMI) preconfigurada con el agente de Amazon CloudWatch Logs para enviar registros a un grupo de registros (log group). Crear una regla programada de Amazon EventBridge (Amazon CloudWatch Events) para realizar una actualización de instancias (instance refresh) cada 90 días.
- [x] Actualizar los datos de usuario (user data) de la plantilla de lanzamiento para instalar y configurar el agente de Amazon CloudWatch Logs, de modo que envíe los registros a un grupo de registros. Configurar el período de retención del grupo de registros en 90 días.
- [ ] Actualizar los datos de usuario de la plantilla de lanzamiento para instalar y configurar el agente de Amazon CloudWatch Logs, de modo que envíe los registros a un grupo de registros. Establecer la configuración de rotación de registros de las instancias de EC2 en 90 días.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está realizando una venta relámpago (flash sale) en su sitio web. El sitio web está alojado en instancias de Amazon EC2 de rendimiento con ráfagas (burstable) dentro de un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para lanzar instancias cuando el uso de CPU supera el `70%`. Un par de horas después de iniciada la venta, los usuarios reportan tiempos de carga lentos y mensajes de error por conexiones rechazadas. Un ingeniero de CloudOps revisa las métricas de Amazon CloudWatch y observa que el uso de CPU está en `20%` en toda la flota de instancias. El ingeniero de CloudOps debe restaurar la funcionalidad del sitio web sin hacer cambios en la infraestructura de red. ¿Qué solución cumple con estos requisitos?

- [x] Activar el modo ilimitado (unlimited mode) para las instancias del grupo de Auto Scaling.
- [ ] Implementar una distribución de Amazon CloudFront para descargar el tráfico del grupo de Auto Scaling.
- [ ] Mover el sitio web a otra región de AWS que esté más cerca de los usuarios.
- [ ] Reducir el tamaño deseado del grupo de Auto Scaling para aumentar artificialmente el promedio de uso de CPU.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha adjuntado la siguiente política a un usuario de IAM. ¿Cuál de las siguientes acciones está permitida para el usuario de IAM?

![Question 62](images/question62.png)

- [ ] La acción `DescribeDBInstances` de Amazon RDS en la región `us-east-1`.
- [ ] La operación `Putobject` de Amazon S3 en un bucket llamado testbucket.
- [x] La acción `DescribeInstances` de Amazon EC2 en la región `us-east-1`.
- [ ] La acción `AttachNetworkinterface` de Amazon EC2 en la región `eu-west-1`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha lanzado un sitio web de redes sociales que permite a los usuarios subir imágenes directamente a un bucket centralizado de Amazon S3. El sitio web es popular en zonas geográficamente distantes de la región de AWS donde se encuentra el bucket de S3. Los usuarios reportan que las cargas son lentas. Un ingeniero de CloudOps debe mejorar la velocidad de carga. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear puntos de acceso de S3 en regiones más cercanas a los usuarios.
- [ ] Crear un acelerador en AWS Global Accelerator para el bucket de S3.
- [x] Habilitar S3 Transfer Acceleration en el bucket de S3.
- [ ] Habilitar el intercambio de recursos de origen cruzado (CORS) en el bucket de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está usando AWS Systems Manager Patch Manager para aplicar parches a una flota de instancias de Amazon EC2. El ingeniero de CloudOps ha configurado una línea base de parches (patch baseline) y una ventana de mantenimiento. El ingeniero de CloudOps también ha usado una etiqueta de instancia para identificar cuáles instancias parchear. El ingeniero de CloudOps debe darle a Systems Manager la capacidad de acceder a las instancias de EC2. ¿Qué acción adicional debe realizar el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Agregar una regla de entrada al grupo de seguridad de las instancias.
- [x] Adjuntar un perfil de instancia de IAM con acceso a Systems Manager a las instancias.
- [ ] Crear una activación de Systems Manager y luego activar la flota de instancias.
- [ ] Especificar manualmente las instancias a parchear en lugar de usar selección basada en etiquetas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa Amazon Elastic Container Service (Amazon ECS) para ejecutar una aplicación en contenedores sobre instancias de Amazon EC2. Un ingeniero de CloudOps necesita monitorear únicamente los flujos de tráfico entre las tareas (tasks) de ECS. ¿Qué combinación de pasos debe seguir el ingeniero de CloudOps para cumplir con este requisito? (Seleccione DOS.)

- [ ] Configurar Amazon CloudWatch Logs en la interfaz de red elástica de cada tarea.
- [x] Configurar registros de flujo (`VPC` Flow Logs) en la interfaz de red elástica de cada tarea.
- [x] Especificar el modo de red `awsvpc` en la definición de la tarea.
- [ ] Especificar el modo de red `bridge` en la definición de la tarea.
- [ ] Especificar el modo de red `host` en la definición de la tarea.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación móvil que usa Amazon S3 para almacenar imágenes. Las imágenes son populares durante una semana, y luego el número de solicitudes de acceso disminuye con el tiempo. Las imágenes deben tener alta disponibilidad y ser accesibles de inmediato cuando se soliciten. Un ingeniero de CloudOps debe reducir los costos de almacenamiento en S3 para la empresa. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?

- [ ] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 Glacier después de 7 días.
- [ ] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 One Zone-Infrequent Access (S3 One Zone-IA) después de 7 días.
- [ ] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 Standard después de 7 días.
- [x] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 Standard-Infrequent Access (S3 Standard-IA) después de 7 días.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps no puede autenticar una llamada de la AWS CLI a un servicio de AWS. ¿Cuál de las siguientes es la causa de este problema?

- [ ] La contraseña de IAM es incorrecta.
- [ ] Falta el certificado del servidor.
- [ ] El par de claves `SSH` es incorrecto.
- [x] No hay una clave de acceso (access key).

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está configurando una flota de instancias de Amazon EC2 en un grupo de Auto Scaling para una aplicación. La flota debe tener `50%` de CPU disponible en todo momento para acomodar ráfagas de tráfico. La carga aumentará significativamente entre las 09:00 y las 17:00, los 7 días de la semana. ¿Cómo debe configurar el ingeniero de CloudOps el escalado de las instancias de EC2 para cumplir con estos requisitos?

- [ ] Crear una política de escalado por seguimiento de destino (target tracking) que se ejecute cuando el uso de CPU sea superior al `90%`.
- [x] Crear una política de escalado por seguimiento de destino que se ejecute cuando el uso de CPU sea superior al `50%`. Crear una política de escalado programado que asegure que la flota esté disponible a las 09:00. Crear una segunda política de escalado programado que reduzca la flota a las 17:00.
- [ ] Configurar el grupo de Auto Scaling para que inicie con 2 instancias, estableciendo el número deseado de instancias, el máximo y el mínimo en 2. Crear una política de escalado programado que asegure que la flota esté disponible a las 09:00.
- [ ] Crear una política de escalado programado que asegure que la flota esté disponible a las 09:00. Crear una segunda política de escalado programado que reduzca la flota a las 17:00.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha creado un portafolio de AWS Service Catalog y lo ha compartido con una segunda cuenta de AWS de la empresa. La segunda cuenta está controlada por otro ingeniero. ¿Qué acción podrá realizar el ingeniero de la segunda cuenta?

- [x] Agregar un producto del portafolio importado a un portafolio local.
- [ ] Agregar nuevos productos al portafolio importado.
- [ ] Cambiar el rol de lanzamiento (launch role) de los productos contenidos en el portafolio importado.
- [ ] Personalizar los productos del portafolio importado.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa AWS Organizations para administrar múltiples cuentas de AWS con facturación consolidada habilitada. Los propietarios de las cuentas miembro de la organización quieren los beneficios de las Instancias Reservadas (RI) pero no quieren compartir las RI con otras cuentas. ¿Qué solución cumple con estos requisitos?

- [x] Comprar RI en cuentas miembro individuales. Deshabilitar el uso compartido del descuento de RI en la cuenta de administración.
- [ ] Comprar RI en cuentas miembro individuales. Deshabilitar el uso compartido del descuento de RI en las cuentas miembro.
- [ ] Comprar RI en la cuenta de administración. Deshabilitar el uso compartido del descuento de RI en la cuenta de administración.
- [ ] Comprar RI en la cuenta de administración. Deshabilitar el uso compartido del descuento de RI en las cuentas miembro.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación de videojuegos está desplegada en cuatro instancias de Amazon EC2 dentro de una `VPC` predeterminada. El ingeniero de CloudOps ha notado latencia consistentemente alta en las respuestas mientras se transfieren datos entre las cuatro instancias. El ingeniero no tiene manera de modificar el código de la aplicación. La forma MÁS efectiva de reducir la latencia es volver a lanzar las instancias de EC2 en:

- [ ] Una `VPC` dedicada.
- [ ] Una sola subred dentro de la `VPC`.
- [x] Un grupo de ubicación (placement group).
- [ ] Una sola Zona de disponibilidad.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación web con estado (stateful) alojada en instancias de Amazon EC2 dentro de un grupo de Auto Scaling. Las instancias se ejecutan detrás de un Application Load Balancer (ALB) que tiene un único grupo de destino. El `ALB` está configurado como origen en una distribución de Amazon CloudFront. Los usuarios reportan cierres de sesión aleatorios en la aplicación web. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para resolver este problema? (Seleccione DOS.)

- [ ] Cambiar al algoritmo de solicitudes pendientes mínimas (least outstanding requests) en el grupo de destino del `ALB`.
- [x] Configurar el reenvío de cookies (cookie forwarding) en el comportamiento de caché de la distribución de CloudFront.
- [ ] Configurar el reenvío de encabezados (header forwarding) en el comportamiento de caché de la distribución de CloudFront.
- [ ] Habilitar la persistencia a nivel de grupo (group-level stickiness) en la regla del listener del `ALB`.
- [x] Habilitar sesiones persistentes (sticky sessions) en el grupo de destino del `ALB`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está investigando problemas de rendimiento en la aplicación web de una empresa. La aplicación se ejecuta en instancias de Amazon EC2 dentro de un grupo de Auto Scaling. La aplicación recibe grandes aumentos de tráfico en momentos aleatorios a lo largo del día. Durante los períodos de aumento rápido de tráfico, el grupo de Auto Scaling no agrega capacidad con suficiente rapidez. Como resultado, los usuarios experimentan un rendimiento deficiente. La empresa quiere minimizar los costos sin afectar negativamente la experiencia del usuario cuando el tráfico web aumenta rápidamente. La empresa necesita una solución que agregue más capacidad al grupo de Auto Scaling en aumentos de tráfico grandes que en aumentos pequeños. ¿Cómo debe configurar el ingeniero de CloudOps el grupo de Auto Scaling para cumplir con estos requisitos?

- [ ] Crear una política de escalado simple (simple scaling) con ajustes que hagan cambios más grandes en la capacidad cuando el sistema esté bajo carga pesada.
- [x] Crear una política de escalado por pasos (step scaling) con ajustes que hagan cambios más grandes en la capacidad cuando el sistema esté bajo carga pesada.
- [ ] Crear una política de escalado por seguimiento de destino (target tracking) con ajustes que hagan cambios más grandes en la capacidad cuando el sistema esté bajo carga pesada.
- [ ] Usar los lifecycle hooks de Amazon EC2 Auto Scaling. Ajustar el número máximo de instancias del grupo de Auto Scaling después de cada evento de escalado.

**[⬆ Volver arriba](#table-of-contents)**

### Una `VPC` está conectada al centro de datos de una empresa mediante una `VPN`. Una instancia de Amazon EC2 con la dirección IP `172.31.16.139` está dentro de una subred privada de la `VPC`. Un ingeniero de CloudOps envió un comando ping a la instancia de EC2 desde una computadora on-premises con la dirección IP `203.0.113.12` y no recibió confirmación. Los registros de flujo (`VPC` Flow Logs) estaban habilitados y mostraron lo siguiente. ¿Qué acción resolverá el problema?

![Question 74](images/question58_74_155.png)

- [ ] Modificar las reglas del grupo de seguridad de EC2 para permitir tráfico de entrada desde la computadora on-premises.
- [ ] Modificar las reglas del grupo de seguridad de EC2 para permitir tráfico de salida hacia la computadora on-premises.
- [ ] Modificar las reglas de la `ACL` de red de la `VPC` para permitir tráfico de entrada desde la computadora on-premises.
- [x] Modificar las reglas de la `ACL` de red de la `VPC` para permitir tráfico de salida hacia la computadora on-premises.

**[⬆ Volver arriba](#table-of-contents)**

### El departamento financiero de una empresa necesita ver los detalles de costos de cada proyecto en una cuenta de AWS. Un ingeniero de CloudOps debe realizar la configuración inicial requerida para ver el costo de cada proyecto en Cost Explorer. ¿Qué solución cumple con este requisito?

- [x] Activar las etiquetas de asignación de costos (cost allocation tags). Agregar una etiqueta de proyecto a los recursos correspondientes.
- [ ] Configurar la facturación consolidada. Crear Informes de Costos y Uso de AWS (AWS Cost and Usage Reports).
- [ ] Usar AWS Budgets. Crear informes de AWS Budgets.
- [ ] Usar categorías de costos para definir grupos personalizados basados en dimensiones de costo y uso de AWS.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps necesita proteger las credenciales de una base de datos de Amazon RDS que se crea mediante una plantilla de AWS CloudFormation. La solución debe cifrar las credenciales y debe admitir rotación automática. ¿Qué solución cumple con estos requisitos?

- [x] Crear un recurso `AWS::SecretsManager::Secret` en la plantilla de CloudFormation. Referenciar las credenciales en el recurso `AWS::RDS::DBInstance` usando la referencia dinámica `resolve:secretsmanager`.
- [ ] Crear un recurso `AWS::SecretsManager::Secret` en la plantilla de CloudFormation. Referenciar las credenciales en el recurso `AWS::RDS::DBInstance` usando la referencia dinámica `resolve:ssm-secure`.
- [ ] Crear un recurso `AWS::SSM::Parameter` en la plantilla de CloudFormation. Referenciar las credenciales en el recurso `AWS::RDS::DBInstance` usando la referencia dinámica `resolve:ssm`.
- [ ] Crear parámetros para las credenciales de la base de datos en la plantilla de CloudFormation. Usar la función intrínseca Ref para proporcionar las credenciales al recurso `AWS::RDS::DBInstance`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ampliando su flota de instancias de Amazon EC2 antes de un aumento esperado de tráfico. Cuando un ingeniero de CloudOps intenta agregar más instancias, se devuelve un error `InstanceLimitExceeded`. ¿Qué debe hacer el ingeniero de CloudOps para resolver este error?

- [ ] Agregar un bloque `CIDR` adicional a la `VPC`.
- [ ] Lanzar las instancias de EC2 en una Zona de disponibilidad diferente.
- [ ] Lanzar nuevas instancias de EC2 en otra `VPC`.
- [x] Usar Service Quotas para solicitar un aumento de cuota de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps mantiene varias instancias de Amazon EC2 que no tienen acceso a internet público. Para aplicar parches a los sistemas operativos, las instancias requieren conectividad de salida a internet. Por razones de seguridad, las instancias no deben ser accesibles desde internet público. El ingeniero despliega una instancia `NAT`, actualiza los grupos de seguridad y configura las rutas apropiadas en la tabla de enrutamiento. Sin embargo, las instancias aún no pueden llegar a internet. ¿Qué se debe hacer para resolver el problema?

- [ ] Asignar direcciones IP elásticas a las instancias y crear una ruta desde las subredes privadas hacia la puerta de enlace de internet.
- [ ] Eliminar la instancia `NAT` y reemplazarla con AWS WAF.
- [x] Deshabilitar las verificaciones de origen/destino (source/destination checks) en la instancia `NAT`.
- [ ] Detener e iniciar la instancia `NAT` para que se lance en un host diferente.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe configurar una capa resiliente de instancias de Amazon EC2 para una aplicación de computación de alto rendimiento (HPC). La aplicación HPC requiere latencia mínima entre nodos. ¿Qué acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Crear un sistema de archivos de Amazon Elastic File System (Amazon EFS). Montar el sistema de archivos en las instancias de EC2 usando datos de usuario (user data).
- [ ] Crear un Network Load Balancer Multi-AZ frente a las instancias de EC2.
- [x] Colocar las instancias de EC2 en un grupo de Auto Scaling dentro de una única subred.
- [x] Lanzar las instancias de EC2 en un grupo de ubicación (placement group) de tipo clúster.
- [ ] Lanzar las instancias de EC2 en un grupo de ubicación de tipo partición.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa una cola estándar de Amazon Simple Queue Service (Amazon SQS) con su aplicación. La aplicación envía mensajes a la cola con cuerpos de mensaje únicos. La empresa decide cambiar a una cola SQS FIFO. ¿Qué debe hacer la empresa para migrar a una cola SQS FIFO?

- [x] Crear una nueva cola SQS FIFO. Activar la deduplicación basada en contenido en la nueva cola FIFO. Actualizar la aplicación para incluir un ID de grupo de mensajes (message group ID) en los mensajes.
- [ ] Crear una nueva cola SQS FIFO. Actualizar la aplicación para incluir el parámetro `DelaySeconds` en los mensajes.
- [ ] Modificar el tipo de cola de SQS estándar a SQS FIFO. Desactivar la deduplicación basada en contenido en la cola. Actualizar la aplicación para incluir un ID de grupo de mensajes en los mensajes.
- [ ] Modificar el tipo de cola de SQS estándar a SQS FIFO. Actualizar la aplicación para enviar mensajes con cuerpos de mensaje idénticos e incluir el parámetro `DelaySeconds` en los mensajes.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps creó una plantilla de AWS CloudFormation que aprovisiona instancias de Amazon EC2, un Elastic Load Balancer (ELB) y una instancia de base de datos de Amazon RDS. Durante la creación del stack, la creación de las instancias de EC2 y del ELB es exitosa. Sin embargo, la creación de la instancia de base de datos falla. ¿Cuál es el comportamiento predeterminado de CloudFormation en este escenario?

- [ ] CloudFormation revertirá (rollback) el stack y lo eliminará.
- [x] CloudFormation revertirá el stack pero no lo eliminará.
- [ ] CloudFormation le pedirá al usuario que decida entre revertir el stack o continuar.
- [ ] CloudFormation completará el stack exitosamente pero reportará un estado fallido para la instancia de base de datos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps administra los buckets de Amazon S3 de una empresa. El ingeniero de CloudOps ha identificado `5 GB` de cargas multiparte incompletas en un bucket de S3 de la cuenta de AWS de la empresa. El ingeniero de CloudOps necesita reducir la cantidad de objetos de cargas multiparte incompletas en el bucket de S3. ¿Qué solución cumple con este requisito?

- [x] Crear una regla de ciclo de vida de S3 en el bucket de S3 para eliminar marcadores expirados o cargas multiparte incompletas.
- [ ] Exigir a los usuarios que realizan cargas de archivos a Amazon S3 que usen el S3 TransferUtility.
- [ ] Habilitar el versionado de S3 en el bucket de S3 que contiene las cargas multiparte incompletas.
- [ ] Crear un S3 Object Lambda Access Point para eliminar las cargas multiparte incompletas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa Amazon Elastic File System (Amazon EFS) para compartir un sistema de archivos entre varias instancias de Amazon EC2. A medida que aumenta el uso, los usuarios reportan que la recuperación de archivos desde el sistema de archivos EFS es más lenta de lo normal. ¿Qué acción debe tomar un ingeniero de CloudOps para mejorar el rendimiento del sistema de archivos?

- [x] Configurar el sistema de archivos para usar `Provisioned Throughput` (rendimiento aprovisionado).
- [ ] Habilitar el cifrado en tránsito en el sistema de archivos.
- [ ] Identificar archivos no utilizados en el sistema de archivos y eliminarlos.
- [ ] Redimensionar el volumen de Amazon Elastic Block Store (Amazon EBS) de cada una de las instancias de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja varias aplicaciones intensivas en escritura. Estas aplicaciones usan una base de datos MySQL que se ejecuta en una única instancia de Amazon EC2. La empresa le pide a un ingeniero de CloudOps que implemente una solución de base de datos de alta disponibilidad que sea ideal para cargas de trabajo multi-tenant. ¿Qué solución debe implementar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear una segunda instancia de EC2 para MySQL. Configurar la segunda instancia como una réplica de lectura.
- [ ] Migrar la base de datos a un clúster de Amazon Aurora DB. Agregar una réplica de Aurora.
- [x] Migrar la base de datos a un clúster de Amazon Aurora multi-master.
- [ ] Migrar la base de datos a una instancia de Amazon RDS for MySQL.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está evaluando las opciones `DNS` de Amazon Route 53 para abordar preocupaciones sobre la alta disponibilidad de un sitio web on-premises. El sitio web consta de dos servidores: un servidor activo primario y un servidor pasivo secundario. Route 53 debe enrutar el tráfico al servidor primario si la verificación de estado asociada devuelve códigos `HTTP` 2xx o 3xx. Todo el demás tráfico debe dirigirse al servidor pasivo secundario. El tipo de registro de conmutación por error (failover), el ID de conjunto y la política de enrutamiento ya se han configurado apropiadamente tanto para el servidor primario como para el secundario. ¿Cuál es el siguiente paso para configurar Route 53?

- [x] Crear un registro `A` para cada servidor. Asociar los registros con la verificación de estado `HTTP` de Route 53.
- [ ] Crear un registro `A` para cada servidor. Asociar los registros con la verificación de estado `TCP` de Route 53.
- [ ] Crear un registro de alias para cada servidor con `Evaluate Target Health` configurado en `Yes`. Asociar los registros con la verificación de estado `HTTP` de Route 53.
- [ ] Crear un registro de alias para cada servidor con `Evaluate Target Health` configurado en `Yes`. Asociar los registros con la verificación de estado `TCP` de Route 53.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa debe garantizar que todos los objetos cargados a un bucket de S3 estén cifrados. ¿Cuáles de las siguientes acciones cumplen con este requisito? (Elija dos.)

- [ ] Implementar AWS Shield para proteger contra objetos sin cifrar almacenados en buckets de S3.
- [ ] Implementar una Lista de Control de Acceso a Objetos (`ACL`) para denegar la carga de objetos sin cifrar al bucket de S3.
- [x] Implementar el cifrado predeterminado de Amazon S3 para asegurar que cualquier objeto cargado se cifre antes de almacenarse.
- [ ] Implementar Amazon Inspector para inspeccionar los objetos cargados al bucket de S3 y asegurar que estén cifrados.
- [x] Implementar políticas de bucket de S3 para denegar la carga de objetos sin cifrar a los buckets.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa necesita desplegar una aplicación web en dos instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). También se desplegarán dos instancias de EC2 para alojar la base de datos. La infraestructura debe diseñarse a través de Zonas de disponibilidad para alta disponibilidad y debe limitar el acceso público a las instancias tanto como sea posible. ¿Cómo se debe lograr esto dentro de una `VPC`?

- [ ] Crear una subred pública para el Application Load Balancer, una subred pública para los servidores web y una subred privada para los servidores de base de datos.
- [ ] Crear una subred pública para el Application Load Balancer, dos subredes públicas para los servidores web y dos subredes privadas para los servidores de base de datos.
- [x] Crear dos subredes públicas para el Application Load Balancer, dos subredes privadas para los servidores web y dos subredes privadas para los servidores de base de datos.
- [ ] Crear dos subredes públicas para el Application Load Balancer, dos subredes públicas para los servidores web y dos subredes públicas para los servidores de base de datos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere recopilar datos de una aplicación para usarlos en análisis. Durante los primeros 90 días, los datos se accederán con poca frecuencia pero deben permanecer altamente disponibles. Durante este tiempo, el equipo de análisis de la empresa requiere acceso a los datos en milisegundos. Sin embargo, después de 90 días, la empresa debe conservar los datos a largo plazo a un costo menor. El tiempo de recuperación después de 90 días debe ser inferior a 5 horas. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?

- [x] Almacenar los datos en S3 Standard-Infrequent Access (S3 Standard-IA) durante los primeros 90 días. Configurar una regla de ciclo de vida de S3 para mover los datos a S3 Glacier Flexible Retrieval después de 90 días.
- [ ] Almacenar los datos en S3 One Zone-Infrequent Access (S3 One Zone-IA) durante los primeros 90 días. Configurar una regla de ciclo de vida de S3 para mover los datos a S3 Glacier Deep Archive después de 90 días.
- [ ] Almacenar los datos en S3 Standard durante los primeros 90 días. Configurar una regla de ciclo de vida de S3 para mover los datos a S3 Glacier Flexible Retrieval después de 90 días.
- [ ] Almacenar los datos en S3 Standard durante los primeros 90 días. Configurar una regla de ciclo de vida de S3 para mover los datos a S3 Glacier Deep Archive después de 90 días.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa manufacturera usa una instancia de base de datos de Amazon RDS para almacenar el inventario de todos los artículos en stock. La empresa mantiene varias funciones de AWS Lambda que interactúan con la base de datos para agregar, actualizar y eliminar artículos. Las funciones Lambda usan credenciales embebidas (hardcoded) para conectarse a la base de datos. Un ingeniero de CloudOps debe asegurarse de que las credenciales de la base de datos nunca se almacenen en texto plano y de que la contraseña se rote cada 30 días. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Almacenar la contraseña de la base de datos como variable de entorno en cada función Lambda. Crear una nueva función Lambda llamada `PasswordRotate`. Usar Amazon EventBridge (Amazon CloudWatch Events) para programar la función `PasswordRotate` cada 30 días, de modo que cambie la contraseña de la base de datos y actualice la variable de entorno de cada función Lambda.
- [ ] Usar AWS Key Management Service (AWS KMS) para cifrar la contraseña de la base de datos y almacenarla cifrada como variable de entorno en cada función Lambda. Otorgar a cada función Lambda acceso a la clave de KMS para que la contraseña de la base de datos pueda descifrarse cuando sea necesario. Crear una nueva función Lambda llamada `PasswordRotate` para cambiar la contraseña cada 30 días.
- [x] Usar AWS Secrets Manager para almacenar las credenciales de la base de datos. Crear un secreto en Secrets Manager y seleccionar la base de datos para que Secrets Manager use una función Lambda que actualice automáticamente la contraseña de la base de datos. Especificar un cronograma de rotación automática de 30 días. Actualizar cada función Lambda para que acceda a la contraseña de la base de datos desde Secrets Manager.
- [ ] Usar AWS Systems Manager Parameter Store para crear una cadena segura (secure string) que almacene las credenciales de la base de datos. Crear una nueva función Lambda llamada `PasswordRotate`. Usar Amazon EventBridge (Amazon CloudWatch Events) para programar la función `PasswordRotate` cada 30 días, de modo que cambie la contraseña de la base de datos y actualice el secreto en Parameter Store. Actualizar cada función Lambda para que acceda a la contraseña de la base de datos desde Parameter Store.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps crea un clúster de Amazon Elastic Kubernetes Service (Amazon EKS) que usa AWS Fargate. El clúster se despliega con éxito. El ingeniero de CloudOps necesita administrar el clúster usando la herramienta de línea de comandos `kubectl`. ¿Cuál de los siguientes debe configurarse en la máquina del ingeniero de CloudOps para que `kubectl` pueda comunicarse con el servidor de la API del clúster?

- [x] El archivo `kubeconfig`.
- [ ] El complemento de Amazon EKS `kube-proxy`.
- [ ] El perfil de Fargate.
- [ ] El archivo `eks-connector.yaml`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita configurar la rotación automática de las credenciales de una base de datos de Amazon RDS. Las credenciales deben rotarse cada 30 días. La solución debe integrarse con Amazon RDS. ¿Qué solución cumple con estos requisitos con el MENOR esfuerzo operativo?

- [ ] Almacenar las credenciales en AWS Systems Manager Parameter Store como una cadena segura (secure string). Configurar la rotación automática con un intervalo de 30 días.
- [x] Almacenar las credenciales en AWS Secrets Manager. Configurar la rotación automática con un intervalo de 30 días.
- [ ] Almacenar las credenciales en un archivo dentro de un bucket de Amazon S3. Desplegar una función de AWS Lambda para rotar automáticamente las credenciales cada 30 días.
- [ ] Almacenar las credenciales en AWS Secrets Manager. Desplegar una función de AWS Lambda para rotar automáticamente las credenciales cada 30 días.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que se ejecuta únicamente en instancias Spot de Amazon EC2. Las instancias se ejecutan en un grupo de Amazon EC2 Auto Scaling con acciones de escalado programado. Sin embargo, la capacidad no siempre aumenta en los horarios programados, y las instancias se terminan muchas veces al día. Un ingeniero de CloudOps debe asegurarse de que las instancias se lancen a tiempo y tengan menos interrupciones. ¿Qué acción cumple con estos requisitos?

- [x] Especificar la estrategia de asignación optimizada por capacidad (capacity-optimized) para instancias Spot. Agregar más tipos de instancia al grupo de Auto Scaling.
- [ ] Especificar la estrategia de asignación optimizada por capacidad para instancias Spot. Aumentar el tamaño de las instancias en el grupo de Auto Scaling.
- [ ] Especificar la estrategia de asignación de precio más bajo (lowest-price) para instancias Spot. Agregar más tipos de instancia al grupo de Auto Scaling.
- [ ] Especificar la estrategia de asignación de precio más bajo para instancias Spot. Aumentar el tamaño de las instancias en el grupo de Auto Scaling.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa almacena sus datos en un bucket de Amazon S3. La empresa necesita clasificar los datos y encontrar cualquier información personal sensible en sus archivos de S3. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una regla de AWS Config para descubrir información personal sensible en los archivos de S3 y marcarlos como no conformes.
- [ ] Crear un pipeline de inteligencia artificial/aprendizaje automático (IA/ML) activado por eventos de S3 para clasificar información personal sensible usando Amazon Recognition.
- [ ] Habilitar Amazon GuardDuty. Configurar la protección de S3 para monitorear todos los datos dentro de Amazon S3.
- [x] Habilitar Amazon Macie. Crear un trabajo de descubrimiento (discovery job) que use el identificador de datos administrado (managed data identifier).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que los clientes usan para buscar registros en un sitio web. Los datos de la aplicación se almacenan en un clúster de Amazon Aurora DB. El uso de la aplicación varía según la temporada y el día de la semana. La popularidad del sitio web está aumentando, y el sitio web experimenta un rendimiento más lento debido al aumento de carga en el clúster de base de datos durante los períodos de actividad pico. Los registros de la aplicación muestran que los problemas de rendimiento ocurren cuando los usuarios buscan información. Rara vez se realiza la misma búsqueda varias veces. Un ingeniero de CloudOps debe mejorar el rendimiento de la plataforma usando una solución que maximice la eficiencia de los recursos. ¿Qué solución cumple con estos requisitos?

- [ ] Desplegar un clúster de Amazon ElastiCache for Redis frente al clúster de base de datos. Modificar la aplicación para que verifique la caché antes de emitir nuevas consultas a la base de datos. Agregar los resultados de cualquier consulta a la caché.
- [x] Desplegar una réplica de Aurora para el clúster de base de datos. Modificar la aplicación para que use el endpoint de lector (reader endpoint) para las operaciones de búsqueda. Usar Aurora Auto Scaling para escalar el número de réplicas según la carga.
- [ ] Usar Provisioned IOPS en los volúmenes de almacenamiento que respaldan el clúster de base de datos para mejorar el rendimiento lo suficiente como para soportar la carga pico de la aplicación.
- [ ] Aumentar el tamaño de la instancia del clúster de base de datos a un tamaño suficiente para soportar la carga pico de la aplicación. Usar Aurora Auto Scaling para escalar el tamaño de la instancia según la carga.

**[⬆ Volver arriba](#table-of-contents)**

### El equipo de seguridad está preocupado porque el número de políticas de AWS Identity and Access Management (IAM) que se usan en el entorno está aumentando. El equipo le encargó a un ingeniero de CloudOps que reportara el número actual de políticas de IAM en uso y el total de políticas de IAM disponibles. ¿Qué servicio de AWS debe usar el ingeniero para verificar cómo se compara el uso actual de políticas de IAM con los límites de servicio actuales?

- [x] AWS Trusted Advisor.
- [ ] Amazon Inspector.
- [ ] AWS Config.
- [ ] AWS Organizations.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps notó que se está creando una gran cantidad de direcciones IP elásticas en la cuenta de AWS de la empresa, pero no se están asociando con instancias de Amazon EC2, y están generando cargos por direcciones IP elásticas en la factura mensual. ¿Cómo puede el ingeniero identificar quién está creando las direcciones IP elásticas?

- [ ] Adjuntar una etiqueta de asignación de costos (`cost-allocation`) a cada dirección IP elástica solicitada, con el nombre de usuario de IAM del desarrollador que la crea.
- [x] Consultar los registros de AWS CloudTrail usando Amazon Athena para buscar eventos de direcciones IP elásticas.
- [ ] Crear una alarma de CloudWatch sobre la métrica `EIPCreated` y enviar una notificación de Amazon SNS cuando se active la alarma.
- [ ] Usar Amazon Inspector para obtener un informe de todas las direcciones IP elásticas creadas en los últimos 30 días.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una distribución de Amazon CloudFront que usa un bucket de Amazon S3 como origen. Durante una revisión de los registros de acceso, la empresa determina que algunas solicitudes van directamente al bucket de S3 usando el endpoint de alojamiento de sitio web (website hosting endpoint). Un ingeniero de CloudOps debe proteger el bucket de S3 para permitir solicitudes únicamente desde CloudFront. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [x] Crear una Identidad de Acceso de Origen (OAI) en CloudFront. Asociar la OAI con la distribución. Eliminar el acceso hacia y desde otros principales en la política del bucket de S3. Actualizar la política del bucket de S3 para permitir acceso únicamente desde la OAI.
- [ ] Crear una Identidad de Acceso de Origen (OAI) en CloudFront. Asociar la OAI con la distribución. Actualizar la política del bucket de S3 para permitir acceso únicamente desde la OAI. Crear un nuevo origen y especificar el bucket de S3 como el nuevo origen. Actualizar el comportamiento de la distribución para usar el nuevo origen. Eliminar el origen existente.
- [ ] Crear una Identidad de Acceso de Origen (OAI) en CloudFront. Asociar la OAI con la distribución. Actualizar la política del bucket de S3 para permitir acceso únicamente desde la OAI. Deshabilitar el alojamiento de sitio web. Crear un nuevo origen y especificar el bucket de S3 como el nuevo origen. Actualizar el comportamiento de la distribución para usar el nuevo origen. Eliminar el origen existente.
- [ ] Actualizar la política del bucket de S3 para permitir acceso únicamente desde la distribución de CloudFront. Eliminar el acceso hacia y desde otros principales en la política del bucket de S3. Deshabilitar el alojamiento de sitio web. Crear un nuevo origen y especificar el bucket de S3 como el nuevo origen. Actualizar el comportamiento de la distribución para usar el nuevo origen. Eliminar el origen existente.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe crear una política de IAM para un desarrollador que necesita acceso a servicios específicos de AWS. Con base en los requisitos, el ingeniero de CloudOps crea la siguiente política. ¿Qué acciones permite esta política? (Seleccione DOS.)

![Question 98](images/question98.png)

- [ ] Crear un AWS Storage Gateway.
- [ ] Crear un rol de IAM para una función de AWS Lambda.
- [ ] Eliminar una cola de Amazon Simple Queue Service (Amazon SQS).
- [x] Describir los balanceadores de carga de AWS.
- [x] Invocar una función de AWS Lambda.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está intentando conectar dos aplicaciones. Una aplicación se ejecuta en un centro de datos on-premises con el nombre de host hostl.onprem.private. La otra aplicación se ejecuta en una instancia de Amazon EC2 con el nombre de host `hostl.awscloud.private`. Existe una conexión AWS Site-to-Site `VPN` entre la red on-premises y AWS. La aplicación que se ejecuta en el centro de datos intenta conectarse a la aplicación que se ejecuta en la instancia de EC2, pero la resolución `DNS` falla. Un ingeniero de CloudOps debe implementar resolución `DNS` entre los recursos on-premises y los de AWS. ¿Qué solución permite que la aplicación on-premises resuelva el nombre de host de la instancia de EC2?

- [ ] Configurar un endpoint de resolución de entrada (inbound resolver) de Amazon Route 53 con una regla de reenvío para la zona alojada onprem.private. Asociar el resolver con la `VPC` de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de onprem.private al endpoint de resolución de entrada.
- [x] Configurar un endpoint de resolución de entrada de Amazon Route 53. Asociar el resolver con la `VPC` de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de awscloud.private al endpoint de resolución de entrada.
- [ ] Configurar un endpoint de resolución de salida (outbound resolver) de Amazon Route 53 con una regla de reenvío para la zona alojada onprem.private. Asociar el resolver con la región de AWS de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de onprem.private al endpoint de resolución de salida.
- [ ] Configurar un endpoint de resolución de salida de Amazon Route 53. Asociar el resolver con la región de AWS de la instancia de EC2. Configurar el resolver `DNS` on-premises para reenviar las consultas `DNS` de awscloud.private al endpoint de resolución de salida.

**[⬆ Volver arriba](#table-of-contents)**

### Al configurar una conexión `VPN` administrada por AWS, un ingeniero de CloudOps crea un recurso de gateway de cliente (customer gateway) en AWS. El dispositivo de gateway del cliente reside en un centro de datos con una puerta de enlace `NAT` frente a él. ¿Qué dirección se debe usar para crear el recurso de gateway del cliente?

- [ ] La dirección IP privada del dispositivo de gateway del cliente.
- [ ] La dirección MAC del dispositivo `NAT` frente al dispositivo de gateway del cliente.
- [ ] La dirección IP pública del dispositivo de gateway del cliente.
- [x] La dirección IP pública del dispositivo `NAT` frente al dispositivo de gateway del cliente.

**[⬆ Volver arriba](#table-of-contents)**


### Una aplicación se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Las instancias están configuradas en un grupo de Amazon EC2 Auto Scaling. Un ingeniero de CloudOps debe configurar la aplicación para que escale según el número de solicitudes entrantes. ¿Qué solución logra esto con el MENOR esfuerzo?

- [ ] Usar una política de escalado simple (simple scaling) basada en una métrica personalizada que mida el promedio de solicitudes activas de todas las instancias de EC2.
- [ ] Usar una política de escalado simple basada en la métrica `GroupDesiredCapacity` del grupo de Auto Scaling.
- [ ] Usar una política de escalado por seguimiento de destino (target tracking) basada en la métrica `ActiveConnectionCount` del `ALB`.
- [x] Usar una política de escalado por seguimiento de destino basada en la métrica `RequestCountPerTarget` del `ALB`.

**[⬆ Volver arriba](#table-of-contents)**

### El departamento de TI de una empresa notó un aumento en el gasto de su cuenta de AWS para desarrolladores. Hay más de 50 desarrolladores usando la cuenta, y el equipo de finanzas quiere determinar los costos de servicio incurridos por cada desarrollador. ¿Qué debe hacer un ingeniero de CloudOps para recopilar esta información? (Seleccione DOS.)

- [x] Activar la etiqueta `createdBy` en la cuenta.
- [ ] Analizar el uso con dashboards de Amazon CloudWatch.
- [x] Analizar el uso con Cost Explorer.
- [ ] Configurar AWS Trusted Advisor para rastrear el uso de recursos.
- [ ] Crear una alarma de facturación en AWS Budgets.

**[⬆ Volver arriba](#table-of-contents)**

### El sitio web de una empresa contiene una capa web y una capa de base de datos en AWS. La capa web consiste en instancias de Amazon EC2 que se ejecutan en un grupo de Auto Scaling distribuido en dos Zonas de disponibilidad. La capa de base de datos se ejecuta en una instancia de Amazon RDS for MySQL Multi-AZ. Las `ACL`s de red de la subred de base de datos están restringidas únicamente a las subredes web que necesitan acceso a la base de datos. Las subredes web usan la `ACL` de red predeterminada con las reglas por defecto. El equipo de operaciones de la empresa ha agregado una tercera subred a la configuración del grupo de Auto Scaling. Después de que ocurre un evento de Auto Scaling, algunos usuarios reportan que reciben intermitentemente un mensaje de error. El mensaje de error indica que el servidor no puede conectarse a la base de datos. El equipo de operaciones ha confirmado que las tablas de enrutamiento son correctas y que los puertos requeridos están abiertos en todos los grupos de seguridad. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para que los servidores web puedan comunicarse con la instancia de base de datos? (Seleccione DOS.)

- [ ] En la `ACL` predeterminada, crear una regla de entrada de tipo Allow para `TCP` con el rango de puertos efímeros y como origen las subredes de base de datos.
- [ ] En la `ACL` predeterminada, crear una regla de salida de tipo Allow para `MySQL/Aurora (3306)`. Especificar como destinos las subredes de base de datos.
- [x] En las `ACL`s de red de las subredes de base de datos, crear una regla de entrada de tipo Allow para `MySQL/Aurora (3306)`. Especificar como origen la tercera subred web.
- [x] En las `ACL`s de red de las subredes de base de datos, crear una regla de salida de tipo Allow para `TCP` con el rango de puertos efímeros y como destino la tercera subred web.
- [ ] En las `ACL`s de red de las subredes de base de datos, crear una regla de salida de tipo Allow para `MySQL/Aurora (3306)`. Especificar como destino la tercera subred web.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación en una flota de instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Las instancias de EC2 son lanzadas por un grupo de Auto Scaling y se registran automáticamente en un grupo de destino. Un ingeniero de CloudOps debe configurar una notificación para alertar a los propietarios de la aplicación cuando los destinos fallen las verificaciones de estado. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Crear una alarma de Amazon CloudWatch sobre la métrica `UnHealthyHostCount`. Configurar una acción para enviar una notificación de Amazon Simple Notification Service (Amazon SNS) cuando la métrica sea mayor que 0.
- [ ] Configurar una acción de ciclo de vida personalizada (lifecycle hook) de Amazon EC2 Auto Scaling para enviar una notificación de Amazon SNS cuando una instancia esté en estado Pending:Wait.
- [ ] Actualizar el grupo de Auto Scaling. Configurar una notificación de actividad para enviar una notificación de Amazon SNS para el tipo de evento Unhealthy.
- [ ] Actualizar la verificación de estado del `ALB` para enviar una notificación de Amazon SNS cuando una instancia esté no saludable.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere construir una solución para su base de datos crítica de Amazon RDS for MySQL. La base de datos requiere alta disponibilidad en diferentes ubicaciones geográficas. Un ingeniero de CloudOps debe construir una solución para manejar un escenario de recuperación ante desastres (DR) con el menor Objetivo de Tiempo de Recuperación (RTO) y Objetivo de Punto de Recuperación (RPO). ¿Qué solución cumple con estos requisitos?

- [ ] Crear instantáneas automatizadas de la base de datos según un cronograma. Copiar las instantáneas a la región de DR.
- [x] Crear una réplica de lectura entre regiones (Cross-Region) para la base de datos.
- [ ] Crear una réplica de lectura Multi-AZ para la base de datos.
- [ ] Programar funciones de AWS Lambda para crear instantáneas de la base de datos de origen y copiarlas a una región de DR.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps usa instancias de Amazon EC2 para alojar una aplicación. El ingeniero de CloudOps necesita otorgar permisos para que la aplicación acceda a una tabla de Amazon DynamoDB. ¿Qué solución cumple con este requisito?

- [ ] Crear claves de acceso para acceder a la tabla de DynamoDB. Asignar las claves de acceso al perfil de instancia de EC2.
- [ ] Crear un par de claves de EC2 para acceder a la tabla de DynamoDB. Asignar el par de claves al perfil de instancia de EC2.
- [ ] Crear un usuario de IAM para acceder a la tabla de DynamoDB. Asignar el usuario de IAM al perfil de instancia de EC2.
- [x] Crear un rol de IAM para acceder a la tabla de DynamoDB. Asignar el rol de IAM al perfil de instancia de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación web con una capa de base de datos que consiste en una instancia de Amazon EC2 que ejecuta MySQL. Un ingeniero de CloudOps necesita minimizar la posible pérdida de datos y el tiempo requerido para recuperarse en caso de fallo de la base de datos. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una alarma de Amazon CloudWatch para la métrica `StatusCheckFailed_System` que invoque una función de AWS Lambda para detener e iniciar la instancia de EC2.
- [x] Crear una instancia de Amazon RDS for MySQL Multi-AZ. Usar un respaldo nativo de MySQL almacenado en Amazon S3 para restaurar los datos en la nueva base de datos. Actualizar la cadena de conexión en la aplicación web.
- [ ] Crear una instancia de Amazon RDS for MySQL Single-AZ con una réplica de lectura. Usar un respaldo nativo de MySQL almacenado en Amazon S3 para restaurar los datos en la nueva base de datos. Actualizar la cadena de conexión en la aplicación web.
- [ ] Usar Amazon Data Lifecycle Manager (Amazon DLM) para tomar una instantánea del volumen de Amazon Elastic Block Store (Amazon EBS) cada hora. En caso de fallo de la instancia de EC2, restaurar el volumen de EBS desde una instantánea.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que se ejecuta en una flota de instancias de Amazon EC2 detrás de un Elastic Load Balancer. Las instancias se ejecutan en un grupo de Auto Scaling. El rendimiento de la aplicación se mantiene consistente durante la mayor parte del día. Sin embargo, un aumento en el tráfico de usuarios ralentiza el rendimiento durante el mismo período de 4 horas cada día. ¿Cuál es la solución MÁS eficiente operativamente que resolverá este problema?

- [ ] Configurar un segundo Elastic Load Balancer frente al grupo de Auto Scaling con una política de enrutamiento ponderado (weighted).
- [ ] Configurar la flota de instancias de EC2 para que se ejecute en tipos de instancia más grandes que soporten el aumento de tráfico de usuarios.
- [x] Crear una acción de escalado programado para escalar el número de instancias de EC2 poco antes de que ocurra el aumento de tráfico de usuarios.
- [ ] Agregar manualmente más instancias de EC2 al grupo de Auto Scaling para soportar el aumento de tráfico de usuarios.

**[⬆ Volver arriba](#table-of-contents)**

### El propietario de una cuenta raíz (root) le ha dado acceso completo a su bucket de S3 a uno de los usuarios de IAM usando la `ACL` del bucket. Cuando el usuario de IAM inicia sesión en la consola de S3, ¿qué acciones puede realizar?

- [ ] Solo puede ver el contenido del bucket.
- [ ] Puede realizar todas las operaciones en el bucket.
- [x] No es posible otorgar acceso a un usuario de IAM usando una `ACL`.
- [ ] El usuario de IAM puede realizar todas las operaciones en el bucket únicamente mediante API/SDK.

**[⬆ Volver arriba](#table-of-contents)**

### Un bucket de Amazon S3 en la cuenta de un ingeniero de CloudOps puede ser accedido por usuarios de otras cuentas de AWS. ¿Cómo puede el ingeniero asegurarse de que el bucket sea accesible únicamente para los miembros de su propia cuenta de AWS?

- [ ] Mover el bucket de S3 de una subred pública a una subred privada en la `VPC` de Amazon.
- [x] Cambiar la Lista de Control de Acceso (`ACL`) del bucket para restringir el acceso únicamente al propietario del bucket.
- [ ] Habilitar el cifrado del lado del servidor para todos los objetos del bucket.
- [ ] Usar únicamente URLs prefirmadas de Amazon S3 para acceder a los objetos del bucket.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación sin estado (stateless) que se ejecuta en cuatro instancias de Amazon EC2. La aplicación requiere cuatro instancias en todo momento para soportar todo el tráfico. Un ingeniero de CloudOps debe diseñar una arquitectura de alta disponibilidad y tolerante a fallos que continúe soportando todo el tráfico si una Zona de disponibilidad deja de estar disponible. ¿Qué configuración cumple con estos requisitos?

- [ ] Desplegar dos grupos de Auto Scaling en dos Zonas de disponibilidad con una capacidad mínima de dos instancias en cada grupo.
- [ ] Desplegar un grupo de Auto Scaling a través de dos Zonas de disponibilidad con una capacidad mínima de cuatro instancias.
- [x] Desplegar un grupo de Auto Scaling a través de tres Zonas de disponibilidad con una capacidad mínima de cuatro instancias.
- [ ] Desplegar un grupo de Auto Scaling a través de tres Zonas de disponibilidad con una capacidad mínima de seis instancias.

**[⬆ Volver arriba](#table-of-contents)**

### La infraestructura backend de una empresa contiene una instancia de Amazon EC2 en una subred privada. La subred privada tiene una ruta a internet a través de una puerta de enlace `NAT` en una subred pública. La instancia debe permitir conectividad hacia un servidor web seguro en internet para recuperar datos a intervalos regulares. El software cliente agota el tiempo de espera con un mensaje de error que indica que no pudo establecer la conexión `TCP`. ¿Qué debe hacer un ingeniero de CloudOps para resolver este error?

- [ ] Agregar una regla de entrada al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTP`, `Source` – `0.0.0.0/0`.
- [ ] Agregar una regla de entrada al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTPS`, `Source` – `0.0.0.0/0`.
- [ ] Agregar una regla de salida al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTP`, `Destination` – `0.0.0.0/0`.
- [x] Agregar una regla de salida al grupo de seguridad de la instancia de EC2 con los siguientes parámetros: `Type` – `HTTPS`, `Destination` – `0.0.0.0/0`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa de desarrollo de software tiene varios desarrolladores que trabajan en el mismo producto. Cada desarrollador debe tener su propio entorno de desarrollo, y estos entornos de desarrollo deben ser idénticos. Cada entorno de desarrollo consiste en instancias de Amazon EC2 y una instancia de base de datos de Amazon RDS. Los entornos de desarrollo deben crearse solo cuando sea necesario y deben terminarse cada noche para minimizar costos. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Dar a los desarrolladores acceso a la misma plantilla de AWS CloudFormation para que puedan aprovisionar su entorno de desarrollo cuando sea necesario. Programar un cron job nocturno en cada instancia de desarrollo para detener todos los procesos en ejecución y reducir el uso de CPU a casi cero.
- [x] Dar a los desarrolladores acceso a la misma plantilla de AWS CloudFormation para que puedan aprovisionar su entorno de desarrollo cuando sea necesario. Programar una regla nocturna de Amazon EventBridge (Amazon CloudWatch Events) para invocar una función de AWS Lambda que elimine los stacks de AWS CloudFormation.
- [ ] Dar a los desarrolladores comandos de la CLI para que puedan aprovisionar su propio entorno de desarrollo cuando sea necesario. Programar una regla nocturna de Amazon EventBridge (Amazon CloudWatch Events) para invocar una función de AWS Lambda que termine todas las instancias de EC2 y la instancia de base de datos.
- [ ] Dar a los desarrolladores comandos de la CLI para que puedan aprovisionar su propio entorno de desarrollo cuando sea necesario. Programar una regla nocturna de Amazon EventBridge (Amazon CloudWatch Events) para que AWS CloudFormation elimine todos los recursos del entorno de desarrollo.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación sin estado (stateless) alojada en una instancia de Amazon EC2. Los usuarios reportan problemas de rendimiento. Un ingeniero de CloudOps revisa las métricas de Amazon CloudWatch de la aplicación y observa que el uso de CPU de la instancia frecuentemente alcanza `90%` durante el horario laboral. ¿Cuál es la solución MÁS eficiente operativamente que mejorará la capacidad de respuesta de la aplicación?

- [ ] Configurar el registro de CloudWatch en la instancia de EC2. Configurar una alarma de CloudWatch para el uso de CPU que alerte al ingeniero de CloudOps cuando el uso de CPU supere el `90%`.
- [ ] Configurar una conexión AWS Client `VPN` para permitir que los usuarios de la aplicación se conecten directamente a la dirección IP privada de la instancia de EC2 y reducir la latencia.
- [x] Crear un grupo de Auto Scaling y asignarlo a un Application Load Balancer. Configurar una política de escalado por seguimiento de destino (target tracking) basada en el uso promedio de CPU del grupo de Auto Scaling.
- [ ] Crear una alarma de CloudWatch que se active cuando el uso de CPU de la instancia de EC2 supere el `80%`. Configurar la alarma para invocar una función de AWS Lambda que escale verticalmente la instancia.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa adquirió recientemente otra corporación junto con todas las cuentas de AWS de esa corporación. Un analista financiero necesita los datos de costos de estas cuentas. Un ingeniero de CloudOps usa Cost Explorer para generar informes de costos y uso. El ingeniero de CloudOps observa que `No Tagkey` representa el `20%` del costo mensual. ¿Qué debe hacer el ingeniero de CloudOps para etiquetar los recursos de `No Tagkey`?

- [ ] Agregar las cuentas a AWS Organizations. Usar una Política de Control de Servicio (SCP) para etiquetar todos los recursos sin etiquetar.
- [ ] Usar una regla de AWS Config para encontrar los recursos sin etiquetar. Configurar la acción de remediación para terminar los recursos.
- [ ] Usar Cost Explorer para encontrar y etiquetar todos los recursos sin etiquetar.
- [x] Usar Tag Editor para encontrar y etiquetar todos los recursos sin etiquetar.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está ayudando a un equipo de desarrollo a desplegar una aplicación en AWS. La plantilla de AWS CloudFormation incluye una instancia de EC2 con Amazon Linux, un clúster de base de datos de Amazon Aurora y una contraseña de base de datos embebida (hard-coded) que debe rotarse cada 90 días. ¿Cuál es la forma MÁS segura de administrar la contraseña de la base de datos?

- [x] Usar el recurso Secret de AWS Secrets Manager con la propiedad `GenerateSecretString` para generar automáticamente una contraseña. Usar el recurso `RotationSchedule` de AWS Secrets Manager para definir un cronograma de rotación de la contraseña. Configurar la aplicación para que recupere el secreto desde AWS Secrets Manager al acceder a la base de datos.
- [ ] Usar el recurso Secret de AWS Secrets Manager con la propiedad `SecretString`. Aceptar una contraseña como parámetro de `CloudFormation`. Usar la propiedad `AllowedPattern` del parámetro de `CloudFormation` para exigir una longitud mínima, letras mayúsculas y minúsculas y caracteres especiales. Configurar la aplicación para que recupere el secreto desde AWS Secrets Manager al acceder a la base de datos.
- [ ] Usar el recurso `AWS::SSM::Parameter`. Aceptar la entrada como parámetro de `CloudFormation` para almacenar el parámetro como una cadena segura (secure string). Configurar la aplicación para que recupere el parámetro desde AWS Systems Manager Parameter Store al acceder a la base de datos.
- [ ] Usar el recurso `AWS::SSM::Parameter`. Aceptar la entrada como parámetro de `CloudFormation` para almacenar el parámetro como una cadena (string). Configurar la aplicación para que recupere el parámetro desde AWS Systems Manager Parameter Store al acceder a la base de datos.

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo de aplicaciones usa un clúster de base de datos de Amazon Aurora MySQL con una réplica de Aurora. El equipo de aplicaciones nota que el rendimiento de lectura de la aplicación se degrada cuando las conexiones de usuario superan `200`. El número de conexiones de usuario típicamente se mantiene alrededor de `180`, con aumentos súbitos ocasionales por encima de `200` conexiones. El equipo de aplicaciones quiere que la aplicación escale automáticamente a medida que aumente o disminuya la demanda de usuarios. ¿Qué solución cumple con estos requisitos?

- [ ] Migrar a un nuevo clúster de base de datos Aurora multi-master. Modificar la cadena de conexión de la base de datos de la aplicación.
- [ ] Modificar el clúster de base de datos cambiándolo a modo sin servidor (serverless) cada vez que las conexiones de usuario superen `200`.
- [x] Crear una política de escalado automático con una métrica objetivo de `195` `DatabaseConnections`.
- [ ] Modificar el clúster de base de datos aumentando el tamaño de instancia de la réplica de Aurora.

**[⬆ Volver arriba](#table-of-contents)**

### El ingeniero de CloudOps de una empresa ha creado una instancia de Amazon EC2 con software personalizado que se usará como plantilla para todas las nuevas instancias de EC2 en múltiples cuentas de AWS. Los volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos a la instancia de EC2 están cifrados con claves administradas por AWS. El ingeniero de CloudOps crea una Amazon Machine Image (AMI) de la instancia de EC2 personalizada y planea compartir la AMI con las demás cuentas de AWS de la empresa. La empresa exige que todas las AMIs estén cifradas con claves de AWS Key Management Service (AWS KMS) y que solo las cuentas de AWS autorizadas puedan acceder a las AMIs compartidas. ¿Qué solución compartirá la AMI de forma segura con las demás cuentas de AWS?

- [ ] En la cuenta donde se creó la AMI, crear una clave de KMS administrada por el cliente. Modificar la política de la clave para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Modificar los permisos de la AMI para especificar los números de cuenta de AWS con los que se compartirá.
- [x] En la cuenta donde se creó la AMI, crear una clave de KMS administrada por el cliente. Modificar la política de la clave para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Crear una copia de la AMI y especificar la clave de KMS. Modificar los permisos de la AMI copiada para especificar los números de cuenta de AWS con los que se compartirá.
- [ ] En la cuenta donde se creó la AMI, crear una clave de KMS administrada por el cliente. Modificar la política de la clave para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Crear una copia de la AMI y especificar la clave de KMS. Modificar los permisos de la AMI copiada para hacerla pública.
- [ ] En la cuenta donde se creó la AMI, modificar la política de la clave administrada por AWS para otorgar los permisos `kms:DescribeKey`, `kms:ReEncrypt*`, `kms:CreateGrant` y `kms:Decrypt` a las cuentas de AWS con las que se compartirá la AMI. Modificar los permisos de la AMI para especificar los números de cuenta de AWS con los que se compartirá.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que usa un sistema de archivos de Amazon Elastic File System (Amazon EFS). Un incidente reciente que involucró un error de lógica de la aplicación corrompió varios archivos. La empresa quiere mejorar su capacidad de respaldar y recuperar el sistema de archivos EFS. La empresa debe poder recuperar archivos individuales rápidamente. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?

- [ ] Configurar Amazon Data Lifecycle Manager (Amazon DLM) para archivar una copia de los datos en un vault de Amazon S3 Glacier. Usar solicitudes de recuperación de S3 Glacier para recuperar archivos individuales.
- [ ] Crear un segundo sistema de archivos EFS en otra región de AWS. Configurar AWS DataSync para copiar los datos al sistema de archivos de respaldo. Recuperar archivos copiándolos desde el sistema de archivos EFS de respaldo.
- [ ] Habilitar AWS Backup en Amazon EFS para respaldar el sistema de archivos en un vault de Amazon S3 Glacier. Usar solicitudes de recuperación de S3 Glacier para recuperar archivos individuales.
- [x] Habilitar AWS Backup en Amazon EFS para respaldar el sistema de archivos en un vault de respaldo (backup vault). Usar un trabajo de restauración parcial (partial restore) para recuperar archivos individuales.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está solucionando problemas de una plantilla de AWS CloudFormation mediante la cual se crean múltiples instancias de Amazon EC2. La plantilla funciona en `us-east-1`, pero falla en `us-west-2` con el código de error: `AMI [ami-12345678] does not exist`. ¿Cómo debe asegurarse el ingeniero de que la plantilla de AWS CloudFormation funcione en todas las regiones?

- [ ] Copiar la Amazon Machine Image (AMI) de la región de origen a la región de destino y asignarle el mismo ID.
- [ ] Editar la plantilla de AWS CloudFormation para especificar el código de región como parte del ID de AMI totalmente calificado.
- [ ] Editar la plantilla de AWS CloudFormation para ofrecer al usuario una lista desplegable de todas las AMIs usando el control `AWS::EC2::AMI::ImageID`.
- [x] Modificar la plantilla de AWS CloudFormation incluyendo los IDs de AMI en la sección `Mappings`. Referenciar el mapeo apropiado dentro de la plantilla para obtener el ID de AMI correcto.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta su infraestructura en instancias de Amazon EC2 que corren en un grupo de Auto Scaling. Recientemente, la empresa promovió código defectuoso a toda la flota de EC2. Este código defectuoso hizo que el grupo de Auto Scaling escalara las instancias antes de que se pudieran recuperar los registros de la aplicación. ¿Qué debe hacer un ingeniero de CloudOps para conservar los registros de la aplicación después de que las instancias sean terminadas?

- [ ] Configurar un lifecycle hook de Auto Scaling para crear una instantánea del almacenamiento efímero al terminar las instancias.
- [x] Crear una nueva Amazon Machine Image (AMI) que tenga instalado y configurado el agente de Amazon CloudWatch para enviar registros a Amazon CloudWatch Logs. Actualizar la plantilla de lanzamiento para usar la nueva AMI.
- [ ] Crear una nueva Amazon Machine Image (AMI) que tenga un script personalizado configurado para enviar registros a AWS CloudTrail. Actualizar la plantilla de lanzamiento para usar la nueva AMI.
- [ ] Instalar el agente de Amazon CloudWatch en la Amazon Machine Image (AMI) definida en la plantilla de lanzamiento. Configurar el agente de CloudWatch para respaldar los registros en almacenamiento efímero.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa monitorea la actividad de su cuenta usando AWS CloudTrail, y le preocupa que algunos archivos de registro estén siendo alterados después de que los registros se entregan al bucket de Amazon S3 de la cuenta. De ahora en adelante, ¿cómo puede el ingeniero de CloudOps confirmar que los archivos de registro no han sido modificados después de ser entregados al bucket de S3?

- [ ] Transmitir los registros de CloudTrail a Amazon CloudWatch Logs para almacenar los registros en una ubicación secundaria.
- [x] Habilitar la validación de integridad de archivos de registro y usar archivos resumen (digest files) para verificar el valor hash del archivo de registro.
- [ ] Replicar el bucket de registros de S3 entre regiones y cifrar los archivos de registro con claves administradas por S3.
- [ ] Habilitar el registro de acceso al servidor de S3 (S3 server access logging) para rastrear las solicitudes realizadas al bucket de registros para auditorías de seguridad.

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo de ingenieros de guardia (on-call) necesita conectarse frecuentemente a instancias de Amazon EC2 en una subred privada para solucionar problemas y ejecutar comandos. Las instancias usan las últimas Amazon Machine Images (AMIs) de Windows o Amazon Linux proporcionadas por AWS. El equipo tiene un rol de IAM existente para autorización. Un ingeniero de CloudOps debe proporcionar al equipo acceso a las instancias otorgando permisos de IAM a este rol. ¿Qué solución cumple con este requisito?

- [x] Agregar una declaración a la política del rol de IAM para permitir la acción `ssm:StartSession` en las instancias. Indicar al equipo que use AWS Systems Manager Session Manager para conectarse a las instancias usando el rol de IAM asumido.
- [ ] Asociar una dirección IP elástica y un grupo de seguridad a cada instancia. Agregar las direcciones IP de los ingenieros a las reglas de entrada del grupo de seguridad. Agregar una declaración a la política del rol de IAM para permitir la acción `ec2:AuthorizeSecurityGroupIngress`, de modo que el equipo pueda conectarse a las instancias.
- [ ] Crear un host bastión con una instancia de EC2 y asociar el host bastión con la `VPC`. Agregar una declaración a la política del rol de IAM para permitir la acción `ec2:CreateVpnConnection` en el host bastión. Indicar al equipo que use el endpoint del host bastión para conectarse a las instancias.
- [ ] Crear un Network Load Balancer orientado a internet. Usar dos listeners. Reenviar el puerto `22` a un grupo de destino de instancias Linux. Reenviar el puerto `3389` a un grupo de destino de instancias Windows. Agregar una declaración a la política del rol de IAM para permitir la acción `ec2:CreateRoute`, de modo que el equipo pueda conectarse a las instancias.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una plantilla de AWS CloudFormation que crea un bucket de Amazon S3. Un usuario se autentica en la cuenta corporativa de AWS con sus credenciales de Active Directory e intenta desplegar la plantilla de CloudFormation. Sin embargo, la creación del stack falla. ¿Qué factores podrían causar este fallo? (Seleccione DOS.)

- [x] La política de IAM del usuario no permite la acción `cloudformation:CreateStack`.
- [ ] La política de IAM del usuario no permite la acción `cloudformation:CreateStackSet`.
- [x] La política de IAM del usuario no permite la acción `s3:CreateBucket`.
- [ ] La política de IAM del usuario deniega explícitamente la acción `s3:ListBucket`.
- [ ] La política de IAM del usuario deniega explícitamente la acción `s3:PutObject`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene un nuevo requisito que establece que todos los recursos en AWS deben etiquetarse según una política definida. ¿Qué servicio de AWS se debe usar para hacer cumplir e identificar continuamente todos los recursos que no cumplan con la política?

- [ ] AWS CloudTrail.
- [ ] Amazon Inspector.
- [x] AWS Config.
- [ ] AWS Systems Manager.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps está configurando un proceso automatizado para recuperar una instancia de Amazon EC2 en caso de una falla de hardware subyacente. La instancia recuperada debe tener la misma dirección IP privada y la misma dirección IP elástica que tenía la instancia original. El equipo de SysOps debe recibir una notificación por correo electrónico cuando se inicie el proceso de recuperación. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una alarma de Amazon CloudWatch para la instancia de EC2, especificando la métrica `SiatusCheckFailedjnstance`. Agregar una acción de EC2 a la alarma para recuperar la instancia. Agregar una notificación de alarma para publicar un mensaje en un tema (topic) de Amazon Simple Notification Service (Amazon SNS). Suscribir la dirección de correo electrónico del equipo de SysOps al tema de SNS.
- [x] Crear una alarma de Amazon CloudWatch para la instancia de EC2, especificando la métrica `StatusCheckFailed_System`. Agregar una acción de EC2 a la alarma para recuperar la instancia. Agregar una notificación de alarma para publicar un mensaje en un tema de Amazon SNS. Suscribir la dirección de correo electrónico del equipo de SysOps al tema de SNS.
- [ ] Crear un grupo de Auto Scaling distribuido en tres subredes diferentes dentro de la misma Zona de disponibilidad, con un tamaño mínimo, máximo y deseado de `1`. Configurar el grupo de Auto Scaling para que use una plantilla de lanzamiento que especifique la dirección IP privada y la dirección IP elástica. Agregar una notificación de actividad al grupo de Auto Scaling para enviar un correo electrónico al equipo de SysOps a través de Amazon Simple Email Service (Amazon SES).
- [ ] Crear un grupo de Auto Scaling distribuido en tres Zonas de disponibilidad, con un tamaño mínimo, máximo y deseado de `1`. Configurar el grupo de Auto Scaling para que use una plantilla de lanzamiento que especifique la dirección IP privada y la dirección IP elástica. Agregar una notificación de actividad al grupo de Auto Scaling para publicar un mensaje en un tema de Amazon SNS. Suscribir la dirección de correo electrónico del equipo de SysOps al tema de SNS.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe crear una solución que notifique inmediatamente a los desarrolladores de software si una función de AWS Lambda presenta un error. ¿Qué solución cumple con este requisito?

- [x] Crear un tema (topic) de Amazon Simple Notification Service (Amazon SNS) con una suscripción de correo electrónico para cada desarrollador. Crear una alarma de Amazon CloudWatch usando la métrica `Errors` y el nombre de la función Lambda como dimensión. Configurar la alarma para enviar una notificación al tema de SNS cuando el estado de la alarma llegue a `ALARM`.
- [ ] Crear un tema de Amazon SNS con una suscripción móvil para cada desarrollador. Crear una alarma de Amazon EventBridge (Amazon CloudWatch Events) usando `LambdaError` como patrón de evento y el nombre del tema de SNS como recurso. Configurar la alarma para enviar una notificación al tema de SNS cuando el estado de la alarma llegue a `ALARM`.
- [ ] Verificar la dirección de correo electrónico de cada desarrollador en Amazon Simple Email Service (Amazon SES). Crear una regla de Amazon CloudWatch usando la métrica `LambdaError` y las direcciones de correo electrónico de los desarrolladores como dimensiones. Configurar la regla para enviar un correo electrónico a través de Amazon SES cuando el estado de la regla llegue a `ALARM`.
- [ ] Verificar el teléfono móvil de cada desarrollador en Amazon Simple Email Service (Amazon SES). Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) usando `Errors` como patrón de evento y el nombre de la función Lambda como recurso. Configurar la regla para enviar una notificación push a través de Amazon SES cuando el estado de la regla llegue a `ALARM`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps desarrolló un script de Python que usa el AWS SDK para realizar varias tareas de mantenimiento. El script necesita ejecutarse automáticamente cada noche. ¿Cuál es la solución MÁS eficiente operativamente que cumple con este requisito?

- [x] Convertir el script de Python en una función de AWS Lambda. Usar una regla de Amazon EventBridge (Amazon CloudWatch Events) para invocar la función cada noche.
- [ ] Convertir el script de Python en una función de AWS Lambda. Usar AWS CloudTrail para invocar la función cada noche.
- [ ] Desplegar el script de Python en una instancia de Amazon EC2. Usar Amazon EventBridge (Amazon CloudWatch Events) para programar el inicio y detención de la instancia cada noche.
- [ ] Desplegar el script de Python en una instancia de Amazon EC2. Usar AWS Systems Manager para programar el inicio y detención de la instancia cada noche.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe crear una solución que apague automáticamente cualquier instancia de Amazon EC2 que tenga menos del `10%` de uso promedio de CPU durante 60 minutos o más. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?

- [ ] Implementar un cron job en cada instancia de EC2 que se ejecute cada 60 minutos y calcule el uso actual de CPU. Iniciar el apagado de la instancia si el uso de CPU es menor al `10%`.
- [x] Implementar una alarma de Amazon CloudWatch para cada instancia de EC2 que monitoree el uso promedio de CPU. Establecer el período en 1 hora y el umbral en `10%`. Configurar una acción de EC2 en la alarma para detener la instancia.
- [ ] Instalar el agente unificado de Amazon CloudWatch en cada instancia de EC2 y habilitar el conjunto de métricas predefinidas de nivel Básico. Registrar el uso de CPU cada 60 minutos e iniciar el apagado de la instancia si el uso de CPU es menor al `10%`.
- [ ] Usar AWS Systems Manager Run Command para obtener el uso de CPU de cada instancia de EC2 cada 60 minutos. Iniciar el apagado de la instancia si el uso de CPU es menor al `10%`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa plantillas de AWS CloudFormation para desplegar infraestructura en la nube. Un análisis de todas las plantillas de la empresa muestra que la empresa ha declarado los mismos componentes en múltiples plantillas. Un ingeniero de CloudOps necesita crear plantillas dedicadas que tengan sus propios parámetros y condiciones para estos componentes comunes. ¿Qué solución cumple con este requisito?

- [ ] Desarrollar un conjunto de cambios (change set) de CloudFormation.
- [ ] Desarrollar macros de CloudFormation.
- [x] Desarrollar stacks anidados (nested stacks) de CloudFormation.
- [ ] Desarrollar conjuntos de stacks (stack sets) de CloudFormation.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha desplegado AWS Security Hub y AWS Config en una organización recién implementada en AWS Organizations. Un ingeniero de CloudOps debe implementar una solución para restringir que todas las cuentas miembro de la organización desplieguen recursos de Amazon EC2 en la región `ap-southeast-2`. La solución debe implementarse desde un único punto y debe gobernar tanto las cuentas actuales como las futuras. El uso de credenciales raíz (root) también debe restringirse en las cuentas miembro. ¿Qué función de AWS debe usar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Agregador de AWS Config.
- [ ] Límites de permisos de usuario de IAM (permissions boundaries).
- [x] Políticas de Control de Servicio (SCP) de AWS Organizations.
- [ ] Paquetes de conformidad (conformance packs) de AWS Security Hub.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta un proceso de trabajo (worker) en tres instancias de Amazon EC2. Las instancias están en un grupo de Auto Scaling configurado para usar una política de escalado simple. Las instancias procesan mensajes de una cola de Amazon Simple Queue Service (Amazon SQS). Períodos aleatorios de aumento de mensajes están causando una disminución en el rendimiento del proceso de trabajo. Un ingeniero de CloudOps debe escalar las instancias para acomodar el mayor número de mensajes. ¿Qué solución cumple con estos requisitos?

- [ ] Usar CloudWatch para crear una expresión matemática de métricas que calcule la antigüedad aproximada del mensaje más antiguo en la cola de SQS. Crear una política de escalado por seguimiento de destino (target tracking) para la expresión matemática de métricas que modifique el grupo de Auto Scaling.
- [x] Usar CloudWatch para crear una expresión matemática de métricas que calcule el número aproximado de mensajes visibles en la cola de SQS por cada instancia. Crear una política de escalado por seguimiento de destino para la expresión matemática de métricas que modifique el grupo de Auto Scaling.
- [ ] Crear un Application Load Balancer (ALB). Adjuntar el `ALB` al grupo de Auto Scaling. Crear una política de escalado por seguimiento de destino para la métrica `RequestCountPerTarget` del `ALB` que modifique el grupo de Auto Scaling.
- [ ] Crear un Application Load Balancer (ALB). Adjuntar el `ALB` al grupo de Auto Scaling. Crear una política de escalado programado para el grupo de Auto Scaling.

**[⬆ Volver arriba](#table-of-contents)**

### Se notifica a un ingeniero de CloudOps que una instancia de Amazon EC2 dejó de responder. La consola de administración de AWS indica que las verificaciones de sistema están fallando. ¿Qué debe hacer primero el ingeniero para resolver este problema?

- [ ] Reiniciar (reboot) la instancia de EC2 para que se pueda lanzar en un nuevo host.
- [x] Detener e iniciar (stop/start) la instancia de EC2 para que se pueda lanzar en un nuevo host.
- [ ] Terminar la instancia de EC2 y volver a lanzarla.
- [ ] Ver el registro de AWS CloudTrail para investigar qué cambió en la instancia de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una auditoría reciente encontró que la mayoría de los recursos pertenecientes al equipo de desarrollo estaban en violación de los estándares de cumplimiento de parches. Los recursos estaban correctamente etiquetados. ¿Qué servicio se debe usar para remediar rápidamente el problema y devolver los recursos al cumplimiento?

- [ ] AWS Config.
- [ ] Amazon Inspector.
- [ ] AWS Trusted Advisor.
- [x] AWS Systems Manager.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps tiene muchas instancias de Amazon EC2 con Windows que necesitan compartir un sistema de archivos entre nodos. El ingeniero de CloudOps crea un recurso compartido de archivos de Amazon Elastic File System (Amazon EFS). Después de crear el recurso compartido, el ingeniero de CloudOps tiene problemas para montarlo en las instancias de EC2. ¿Qué acción debe tomar el ingeniero de CloudOps para que las instancias de EC2 puedan compartir los archivos?

- [x] Eliminar el recurso compartido de EFS. Crear un recurso compartido de archivos de Amazon FSx for Windows File Server para las instancias de EC2.
- [ ] Usar las credenciales de IAM correctas para montar el recurso compartido de EFS.
- [ ] Configurar soporte para NFSv4 en el sistema operativo Windows que se ejecuta en las instancias de EC2.
- [ ] Permitir el puerto correcto para NFS a través del grupo de seguridad y la `ACL` de red.

**[⬆ Volver arriba](#table-of-contents)**

### Una solución existente y ya desplegada usa instancias de Amazon EC2 con volúmenes de Amazon EBS General Purpose SSD, una base de datos de Amazon RDS PostgreSQL, un sistema de archivos de Amazon EFS y objetos estáticos almacenados en un bucket de Amazon S3. El equipo de seguridad ahora exige que se active el cifrado en reposo (at-rest) de inmediato para todos los aspectos de la aplicación, sin crear nuevos recursos y sin tiempo de inactividad. Para cumplir con los requisitos, ¿en cuál de estos servicios puede el ingeniero de CloudOps habilitar el cifrado en reposo?

- [ ] Volúmenes de EBS General Purpose SSD.
- [ ] Base de datos RDS PostgreSQL.
- [ ] Sistemas de archivos de Amazon EFS.
- [x] Objetos de S3 dentro de un bucket.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa una plantilla de AWS CloudFormation para aprovisionar una instancia de Amazon EC2 y una instancia de base de datos de Amazon RDS. Un ingeniero de CloudOps debe actualizar la plantilla para asegurarse de que la instancia de base de datos se cree antes de que se lance la instancia de EC2. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Agregar una condición de espera (wait condition) a la plantilla. Actualizar el script de datos de usuario (user data) de la instancia de EC2 para enviar una señal después de que la instancia de EC2 se inicie.
- [x] Agregar el atributo `DependsOn` al recurso de la instancia de EC2, y proporcionar el nombre lógico del recurso de RDS.
- [ ] Cambiar el orden de los recursos en la plantilla para que el recurso de RDS se liste antes que el recurso de la instancia de EC2.
- [ ] Crear múltiples plantillas. Usar `StackSets` de AWS CloudFormation para esperar a que un stack se complete antes de crear el segundo stack.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación web existente que se ejecuta en dos instancias de Amazon EC2 detrás de un Application Load Balancer (ALB) a través de dos Zonas de disponibilidad. La aplicación usa una instancia de Amazon RDS Multi-AZ. Los conjuntos de registros de Amazon Route 53 enrutan las solicitudes de contenido dinámico al balanceador de carga y las solicitudes de contenido estático a un bucket de Amazon S3. Los visitantes del sitio reportan tiempos de carga extremadamente largos. ¿Qué acciones se deben tomar para mejorar el rendimiento del sitio web? (Seleccione DOS)

- [x] Agregar caché de Amazon CloudFront para el contenido estático.
- [ ] Cambiar el listener del balanceador de carga de `HTTPS` a `TCP`.
- [ ] Habilitar el enrutamiento basado en latencia de Amazon Route 53.
- [x] Implementar Amazon EC2 Auto Scaling para los servidores web.
- [ ] Mover el contenido estático de Amazon S3 a los servidores web.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ejecutando una aplicación on-premises y quiere usar AWS para respaldo de datos. Todos los datos deben estar disponibles localmente. La aplicación de respaldo solo puede escribir en almacenamiento basado en bloques que sea compatible con la Interfaz Portable de Sistema Operativo (POSIX). ¿Qué solución de respaldo cumple con estos requisitos?

- [ ] Configurar el software de respaldo para usar Amazon S3 como destino de los respaldos de datos.
- [ ] Configurar el software de respaldo para usar Amazon S3 Glacier como destino de los respaldos de datos.
- [ ] Usar AWS Storage Gateway y configurarlo para usar volúmenes en caché (gateway-cached volumes).
- [x] Usar AWS Storage Gateway y configurarlo para usar volúmenes almacenados (gateway-stored volumes).

**[⬆ Volver arriba](#table-of-contents)**

### Una organización creó un volumen de Amazon Elastic File System (Amazon EFS) con un ID de sistema de archivos fs-85ba41fc, y es usado activamente por 10 hosts de Amazon EC2. A la organización le preocupa que el sistema de archivos no esté cifrado. ¿Cómo se puede resolver esto?

- [ ] Habilitar el cifrado en la conexión de cada host al volumen de Amazon EFS. Cada conexión debe recrearse para que el cifrado surta efecto.
- [ ] Habilitar el cifrado en el volumen de EFS existente usando la interfaz de línea de comandos de AWS.
- [ ] Habilitar el cifrado en el disco local de cada host. Reiniciar cada host para cifrar el disco.
- [x] Habilitar el cifrado en un volumen recién creado y copiar todos los datos del volumen original. Reconectar cada host al nuevo volumen.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps configura una aplicación para que se ejecute en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB) dentro de un grupo de Auto Scaling con escalado simple y configuración predeterminada. El grupo de Auto Scaling está configurado para usar la métrica `RequestCountPerTarget` para el escalado. El ingeniero de CloudOps observa que la métrica `RequestCountPerTarget` superó el límite especificado dos veces en `180` segundos. ¿Cómo se verá afectado el número de instancias de EC2 en este grupo de Auto Scaling en este escenario?

- [ ] El grupo de Auto Scaling lanzará una instancia de EC2 adicional cada vez que la métrica `RequestCountPerTarget` supere el límite predefinido.
- [x] El grupo de Auto Scaling lanzará una instancia de EC2 y esperará el período de enfriamiento (cooldown) predeterminado antes de lanzar otra instancia.
- [ ] El grupo de Auto Scaling enviará una alerta al `ALB` para reequilibrar el tráfico y no agregará nuevas instancias de EC2 hasta que la carga se normalice.
- [ ] El grupo de Auto Scaling intentará distribuir el tráfico entre todas las instancias de EC2 antes de lanzar otra instancia.

**[⬆ Volver arriba](#table-of-contents)**

### Se sabe que un proceso errático usa todo un procesador y se ejecuta al `100%`. Un ingeniero de CloudOps quiere automatizar el reinicio de la instancia una vez que el problema ocurra durante más de 2 minutos. ¿Cómo se puede lograr esto?

- [ ] Crear una alarma de Amazon CloudWatch para la instancia de Amazon EC2 con monitoreo básico. Habilitar una acción para reiniciar la instancia.
- [x] Crear una alarma de CloudWatch para la instancia de EC2 con monitoreo detallado. Habilitar una acción para reiniciar la instancia.
- [ ] Crear una función de AWS Lambda para reiniciar la instancia de EC2, activada de forma programada cada 2 minutos.
- [ ] Crear una función Lambda para reiniciar la instancia de EC2, activada por verificaciones de estado de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps observa un evento de escalado (scale-up) para un grupo de Amazon EC2 Auto Scaling. Amazon CloudWatch muestra un pico en la métrica `RequestCount` del Application Load Balancer asociado. Al ingeniero le gustaría conocer las direcciones IP de origen de las solicitudes. ¿Dónde puede el ingeniero encontrar esta información?

- [ ] Registros de Auto Scaling.
- [ ] Registros de AWS CloudTrail.
- [ ] Registros de la instancia de EC2.
- [x] Registros de acceso del Elastic Load Balancer.

**[⬆ Volver arriba](#table-of-contents)**

### Una organización con un departamento de TI grande ha decidido migrar a AWS. Con diferentes funciones de trabajo en el departamento de TI, no es deseable dar a todos los usuarios acceso a todos los recursos de AWS. Actualmente, la organización maneja el acceso mediante membresía a grupos de LDAP. ¿Cuál es el MEJOR método para permitir el acceso usando las credenciales de LDAP actuales?

- [ ] Crear un AWS Directory Service Simple AD. Replicar el directorio LDAP on-premises hacia Simple AD.
- [ ] Crear una función Lambda para leer los grupos de LDAP y automatizar la creación de usuarios de IAM.
- [ ] Usar AWS CloudFormation para crear roles de IAM. Desplegar Direct Connect para permitir el acceso al servidor LDAP on-premises.
- [x] Federar el directorio LDAP con IAM usando SAML. Crear diferentes roles de IAM que correspondan a los diferentes grupos de LDAP para limitar los permisos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está usando una Clave Maestra del Cliente (CMK) de AWS KMS con material de clave importado. La empresa referencia la CMK por su alias en la aplicación Java para cifrar datos. La CMK debe rotarse cada 6 meses. ¿Cuál es el proceso para rotar la clave?

- [ ] Habilitar la rotación automática de claves para la CMK y especificar un período de 6 meses.
- [x] Crear una nueva CMK con nuevo material importado, y actualizar el alias de la clave para que apunte a la nueva CMK.
- [ ] Eliminar el material de clave actual e importar nuevo material en la CMK existente.
- [ ] Importar una copia del material de clave existente en una nueva CMK como respaldo, y establecer el cronograma de rotación en 6 meses.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ejecutando una aplicación sin servidor (serverless) en AWS Lambda. La aplicación almacena datos en una instancia de base de datos de Amazon RDS for MySQL. El uso ha aumentado constantemente, y recientemente han ocurrido numerosos errores de `too many connections` cuando la función Lambda intenta conectarse a la base de datos. La empresa ya ha configurado la base de datos para usar el valor máximo posible de `max_connections`. ¿Qué debe hacer un ingeniero de CloudOps para resolver estos errores?

- [ ] Crear una réplica de lectura de la base de datos. Usar Amazon Route 53 para crear un registro `DNS` ponderado que contenga ambas bases de datos.
- [x] Usar Amazon RDS Proxy para crear un proxy. Actualizar la cadena de conexión en la función Lambda.
- [ ] Aumentar el valor del parámetro `max_connect_errors` en el grupo de parámetros que usa la base de datos.
- [ ] Actualizar la concurrencia reservada (reserved concurrency) de la función Lambda a un valor más alto.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa almacena archivos en 50 buckets de Amazon S3 dentro de la misma región de AWS. La empresa quiere conectarse a los buckets de S3 de forma segura a través de una conexión privada desde sus instancias de Amazon EC2. La empresa necesita una solución que no genere costo adicional. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un endpoint de `VPC` de tipo gateway para cada bucket de S3. Adjuntar los endpoints de `VPC` de tipo gateway a cada subred dentro de la `VPC`.
- [ ] Crear un endpoint de `VPC` de tipo interfaz para cada bucket de S3. Adjuntar los endpoints de `VPC` de tipo interfaz a cada subred dentro de la `VPC`.
- [x] Crear un único endpoint de `VPC` de tipo gateway para todos los buckets de S3. Agregar el endpoint de `VPC` de tipo gateway a la tabla de enrutamiento de la `VPC`.
- [ ] Crear un único endpoint de `VPC` de tipo interfaz para todos los buckets de S3. Agregar el endpoint de `VPC` de tipo interfaz a la tabla de enrutamiento de la `VPC`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa AWS CloudFormation para desplegar la infraestructura de su aplicación. Recientemente, un usuario cambió accidentalmente una propiedad de una base de datos en una plantilla de CloudFormation y realizó una actualización del stack que causó una interrupción en la aplicación. Un ingeniero de CloudOps debe determinar cómo modificar el proceso de despliegue para permitir que el equipo de DevOps continúe desplegando la infraestructura, pero evitando modificaciones accidentales a recursos específicos. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar una regla de AWS Config para alertar según los cambios en cualquier stack de CloudFormation. Una función de AWS Lambda puede entonces describir el stack para determinar si se modificó algún recurso protegido y cancelar la operación.
- [ ] Configurar un evento de Amazon CloudWatch Events con una regla que se active según cualquier llamada a la API de CloudFormation. Una función de AWS Lambda puede entonces describir el stack para determinar si se modificó algún recurso protegido y cancelar la operación.
- [x] Lanzar las plantillas de CloudFormation usando una política de stack (stack policy) con un permiso explícito (allow) para todos los recursos y una denegación explícita (deny) de los recursos protegidos con una acción de `Update:*`.
- [ ] Adjuntar una política de IAM al rol del equipo de DevOps que impida que un stack de CloudFormation se actualice, con una condición basada en los Amazon Resource Names (ARNs) específicos de los recursos protegidos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps recibe una notificación de que una aplicación que se ejecuta en instancias de Amazon EC2 no ha podido autenticarse en una base de datos de Amazon RDS. Para solucionar el problema, el ingeniero de CloudOps necesita investigar la rotación de contraseñas de AWS Secrets Manager. ¿Qué registro de Amazon CloudWatch proporcionará información sobre la rotación de contraseñas?

- [ ] Registros de AWS CloudTrail.
- [ ] Registros de la aplicación de la instancia de EC2.
- [x] Registros de la función de AWS Lambda.
- [ ] Registros de la base de datos RDS.

**[⬆ Volver arriba](#table-of-contents)**

### Una función de AWS Lambda falla intermitentemente varias veces al día. Un ingeniero de CloudOps debe averiguar con qué frecuencia ha ocurrido este error en los últimos 7 días. ¿Qué acción cumple con este requisito de la manera MÁS eficiente operativamente?

- [ ] Usar Amazon Athena para consultar los registros de Amazon CloudWatch asociados con la función Lambda.
- [ ] Usar Amazon Athena para consultar los registros de AWS CloudTrail asociados con la función Lambda.
- [x] Usar Amazon CloudWatch Logs Insights para consultar los registros asociados de la función Lambda.
- [ ] Usar Amazon Elasticsearch Service (Amazon ES) para transmitir los registros de Amazon CloudWatch de la función Lambda.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps está construyendo un proceso para compartir instantáneas de bases de datos de Amazon RDS entre diferentes cuentas asociadas con distintas unidades de negocio dentro de la misma empresa. Todos los datos deben estar cifrados en reposo. ¿Cómo debe implementar el ingeniero este proceso?

- [ ] Escribir un script para descargar la instantánea cifrada, descifrarla usando la clave de cifrado de AWS KMS usada para cifrar la instantánea, y luego crear un nuevo volumen en cada cuenta.
- [x] Actualizar la política de la clave para otorgar permiso sobre la clave de cifrado de AWS KMS usada para cifrar la instantánea a todas las cuentas relevantes, y luego compartir la instantánea con esas cuentas.
- [ ] Crear una instancia de Amazon EC2 basada en la instantánea, luego guardar el volumen de Amazon EBS de la instancia como una instantánea y compartirla con las otras cuentas. Exigir que cada propietario de cuenta cree un nuevo volumen a partir de esa instantánea y lo cifre.
- [ ] Crear una nueva instancia de RDS sin cifrar a partir de la instantánea cifrada, conectarse a la instancia mediante `SSH`/`RDP`, exportar el contenido de la base de datos a un archivo, y luego compartir este archivo con las otras cuentas.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps tiene una plantilla de AWS CloudFormation de la infraestructura existente de la empresa en `us-west-2`. El ingeniero intenta usar la plantilla para lanzar un nuevo stack en `eu-west-1`, pero el stack solo se despliega parcialmente, recibe un mensaje de error y luego se revierte (rollback). ¿Por qué fallaría esta plantilla al desplegarse? (Seleccione DOS.)

- [ ] La plantilla referenciaba un usuario de IAM que no está disponible en `eu-west-1`.
- [x] La plantilla referenciaba una Amazon Machine Image (AMI) que no está disponible en `eu-west-1`.
- [ ] La plantilla no tenía el nivel adecuado de permisos para desplegar los recursos.
- [x] La plantilla solicitaba servicios que no existen en `eu-west-1`.
- [ ] Las plantillas de CloudFormation solo pueden usarse para actualizar servicios existentes.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa una tabla de Amazon DynamoDB para almacenar datos. Un ingeniero de CloudOps debe configurar la replicación de la tabla hacia otra región de AWS para recuperación ante desastres. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Habilitar DynamoDB Accelerator (DAX).
- [ ] Habilitar DynamoDB Streams y agregar un índice secundario global (GSI).
- [x] Habilitar DynamoDB Streams y agregar una región de tabla global (global table).
- [ ] Habilitar la recuperación a un punto en el tiempo (point-in-time recovery).

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe configurar notificaciones para cuando la facturación combinada supere un cierto umbral para todas las cuentas de AWS dentro de una empresa. El ingeniero ha configurado AWS Organizations y habilitado la facturación consolidada. ¿Qué pasos adicionales debe realizar el ingeniero para configurar las alertas de facturación?

- [ ] En la cuenta de pagador: habilitar las alertas de facturación en la consola de Billing and Cost Management; publicar un mensaje de Amazon SNS cuando se active la alerta de facturación.
- [ ] En cada cuenta: habilitar las alertas de facturación en la consola de Billing and Cost Management; configurar una alarma de facturación en Amazon CloudWatch; publicar un mensaje de SNS cuando se active la alarma.
- [ ] En la cuenta de pagador: habilitar las alertas de facturación en la consola de Billing and Cost Management; configurar una alarma de facturación en la consola de Billing and Cost Management para publicar un mensaje de SNS cuando se active la alarma.
- [x] En la cuenta de pagador: habilitar las alertas de facturación en la consola de Billing and Cost Management; configurar una alarma de facturación en Amazon CloudWatch; publicar un mensaje de SNS cuando se active la alarma.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está solucionando problemas de tiempo de espera de conexión hacia una instancia de Amazon EC2 que tiene una dirección IP pública. La instancia tiene una dirección IP privada `172.31.16.139`. Cuando el ingeniero de CloudOps intenta hacer ping a la dirección IP pública de la instancia desde la dirección IP remota `203.0.113.12`, la respuesta es `request timed out`. Los registros de flujo contienen la siguiente información. ¿Cuál es una causa del problema?

![Question 155](images/question58_74_155.png)

- [ ] Regla de denegación de entrada del grupo de seguridad.
- [ ] Regla de denegación de salida del grupo de seguridad.
- [ ] Reglas de entrada de la `ACL` de red.
- [x] Reglas de salida de la `ACL` de red.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita configurar una solución que entregue contenido digital a un conjunto de usuarios autorizados a través de Amazon CloudFront. Los usuarios no autorizados deben quedar restringidos del acceso. ¿Qué solución cumple con estos requisitos?

- [ ] Almacenar el contenido digital en un bucket de Amazon S3 que no tenga el acceso público bloqueado. Usar URLs firmadas para acceder al bucket de S3 a través de CloudFront.
- [x] Almacenar el contenido digital en un bucket de Amazon S3 que tenga el acceso público bloqueado. Usar una Identidad de Acceso de Origen (OAI) para entregar el contenido a través de CloudFront. Restringir el acceso al bucket de S3 con URLs firmadas en CloudFront.
- [ ] Almacenar el contenido digital en un bucket de Amazon S3 que tenga el acceso público bloqueado. Usar una Identidad de Acceso de Origen (OAI) para entregar el contenido a través de CloudFront. Habilitar el cifrado a nivel de campo (field-level encryption).
- [ ] Almacenar el contenido digital en un bucket de Amazon S3 que no tenga el acceso público bloqueado. Usar cookies firmadas para la entrega restringida del contenido a través de CloudFront.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una carga de trabajo Windows de alto rendimiento. La carga de trabajo requiere un volumen de almacenamiento que proporcione un rendimiento constante de 10,000 IOPS. La empresa no quiere pagar por capacidad adicional innecesaria para lograr este rendimiento. ¿Qué solución cumple con estos requisitos con el MENOR costo?

- [ ] Usar un volumen de Amazon Elastic Block Store (Amazon EBS) `Provisioned IOPS SSD (io1)` configurado con 10,000 IOPS aprovisionadas.
- [x] Usar un volumen de Amazon Elastic Block Store (Amazon EBS) `General Purpose SSD (gp3)` configurado con 10,000 IOPS aprovisionadas.
- [ ] Usar un sistema de archivos de Amazon Elastic File System (Amazon EFS) en modo Max I/O.
- [ ] Usar un sistema de archivos de Amazon FSx for Windows File Server configurado con 10,000 IOPS.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja una aplicación interna en instancias de Amazon EC2. Todos los datos y solicitudes de la aplicación se enrutan a través de una conexión AWS Site-to-Site `VPN` entre la red on-premises y AWS. La empresa debe monitorear la aplicación en busca de cambios que permitan acceso de red fuera de la red corporativa. Cualquier cambio que exponga la aplicación externamente debe restringirse automáticamente. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear una función de AWS Lambda que actualice los grupos de seguridad asociados a la interfaz de red elástica para eliminar reglas de entrada con rangos `CIDR` no corporativos. Activar los `VPC` Flow Logs y enviar los registros a Amazon CloudWatch Logs. Crear una alarma de Amazon CloudWatch que coincida con tráfico de rangos `CIDR` no corporativos y publique un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) con la función Lambda como destino.
- [ ] Crear una regla programada de Amazon EventBridge (Amazon CloudWatch Events) que apunte a un documento de Automation de AWS Systems Manager para verificar direcciones IP públicas en las instancias de EC2. Si se encuentran direcciones IP públicas en las instancias de EC2, iniciar otro documento de Automation de Systems Manager para terminar las instancias.
- [x] Configurar AWS Config y una regla personalizada para monitorear si un grupo de seguridad permite solicitudes de entrada desde rangos `CIDR` no corporativos. Crear un documento de Automation de AWS Systems Manager para eliminar cualquier rango `CIDR` no corporativo de los grupos de seguridad de la aplicación.
- [ ] Configurar AWS Config y la regla administrada para monitorear asociaciones de IP públicas con las instancias de EC2 por etiqueta. Etiquetar las instancias de EC2 con un identificador. Crear un documento de Automation de AWS Systems Manager para eliminar la asociación de IP pública de las instancias de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha desplegado una aplicación en instancias de Amazon EC2 dentro de una única `VPC`. La empresa ha colocado las instancias de EC2 en una subred privada de la `VPC`. Las instancias de EC2 necesitan acceso a buckets de Amazon S3 que están en la misma región de AWS que las instancias de EC2. Un ingeniero de CloudOps debe proporcionar a las instancias de EC2 acceso a los buckets de S3 sin requerir ningún cambio en las instancias de EC2 ni en la aplicación. Las instancias de EC2 no deben tener acceso a internet. ¿Qué solución cumple con estos requisitos?

- [x] Crear un endpoint de gateway de S3 que use la política de endpoint de gateway predeterminada. Asociar la subred privada con el endpoint de gateway.
- [ ] Crear un endpoint de interfaz de S3. Asociar las instancias de EC2 con el endpoint de interfaz.
- [ ] Configurar una puerta de enlace `NAT`. Asociar la subred privada con la puerta de enlace `NAT`.
- [ ] Configurar una instancia de EC2 proxy. Actualizar las tablas de enrutamiento de la subred privada para enrutar el tráfico a través de la instancia de EC2 proxy. Configurar el proxy para enrutar todas las solicitudes de S3 al bucket de S3 objetivo.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta miles de instancias de Amazon EC2 basadas en la Amazon Machine Image (AMI) de Amazon Linux 2. Un ingeniero de CloudOps debe implementar una solución para registrar comandos y salida de cualquier usuario que necesite una sesión interactiva en una de las instancias de EC2. La solución debe registrar los datos en una ubicación de almacenamiento duradero. La solución también debe proporcionar notificaciones y alarmas automatizadas basadas en los datos de registro. ¿Qué solución cumple con estos requisitos con la MAYOR eficiencia operativa?

- [ ] Configurar el registro de sesiones de comandos en cada instancia de EC2. Configurar el agente unificado de Amazon CloudWatch para enviar registros de sesión a Amazon CloudWatch Logs. Configurar filtros de consulta y alertas usando Amazon Athena.
- [ ] Exigir que todos los usuarios usen un host bastión centralizado cuando necesiten acceso de línea de comandos a una instancia de EC2. Configurar el agente unificado de Amazon CloudWatch en el host bastión para enviar registros de sesión a Amazon CloudWatch Logs. Configurar un filtro de métricas y una alarma de métricas para hallazgos de seguridad relevantes en CloudWatch Logs.
- [x] Exigir que todos los usuarios usen AWS Systems Manager Session Manager cuando necesiten acceso de línea de comandos a una instancia de EC2. Configurar Session Manager para transmitir registros de sesión a Amazon CloudWatch Logs. Configurar un filtro de métricas y una alarma de métricas para hallazgos de seguridad relevantes en CloudWatch Logs.
- [ ] Configurar el registro de sesiones de comandos en cada instancia de EC2. Exigir que todos los usuarios usen documentos de AWS Systems Manager Run Command cuando necesiten acceso de línea de comandos a una instancia de EC2. Configurar el agente unificado de Amazon CloudWatch para enviar registros de sesión a Amazon CloudWatch Logs. Configurar alarmas de CloudWatch basadas en resultados de consultas de Amazon Athena.

**[⬆ Volver arriba](#table-of-contents)**

### Los usuarios de la cuenta de AWS de una empresa están lanzando instancias de Amazon EC2 sin las etiquetas de asignación de costos requeridas. Un ingeniero de CloudOps necesita evitar que los usuarios dentro de una organización en AWS Organizations lancen nuevas instancias de EC2 que no tengan las etiquetas requeridas. La solución debe requerir el menor esfuerzo operativo posible. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar una función de AWS Lambda que inicie un evento de ejecución de instancia y verifique las etiquetas requeridas. Configurar la función para evitar el lanzamiento de instancias de EC2 si faltan las etiquetas.
- [ ] Configurar una regla de AWS Config para monitorear instancias de EC2 que carezcan de las etiquetas requeridas.
- [x] Configurar una Política de Control de Servicio (SCP) que evite el lanzamiento de instancias de EC2 que carezcan de las etiquetas requeridas. Adjuntar la SCP a la raíz de la organización.
- [ ] Configurar una alarma de Amazon CloudWatch para detener cualquier instancia de EC2 que carezca de las etiquetas requeridas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene científicos que cargan objetos de datos grandes a un bucket de Amazon S3. Los científicos cargan los objetos como cargas multiparte. Las cargas multiparte a menudo fallan debido a una mala conectividad del cliente final. La empresa quiere optimizar los costos de almacenamiento asociados con los datos. Un ingeniero de CloudOps debe implementar una solución que presente métricas para cargas incompletas. La solución también debe eliminar automáticamente cualquier carga incompleta después de 7 días. ¿Qué solución cumple con estos requisitos?

- [x] Revisar la métrica Incomplete Multipart Upload Bytes en el dashboard de S3 Storage Lens. Crear una política de ciclo de vida de S3 para eliminar automáticamente cualquier carga multiparte incompleta después de 7 días.
- [ ] Implementar S3 Intelligent-Tiering para mover los datos a clases de almacenamiento de menor costo después de 7 días. Crear una política de S3 Storage Lens para eliminar automáticamente cualquier carga multiparte incompleta después de 7 días.
- [ ] Acceder a la consola de S3. Revisar la pestaña de Métricas para verificar el almacenamiento que consumen las cargas multiparte incompletas. Crear una función de AWS Lambda para eliminar cualquier carga multiparte incompleta después de 7 días.
- [ ] Usar la herramienta de análisis de clase de almacenamiento de S3 analytics para identificar y medir las cargas multiparte incompletas. Configurar una política de bucket de S3 para hacer cumplir restricciones sobre las cargas multiparte y eliminar las incompletas después de 7 días.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está cargando archivos importantes como objetos a Amazon S3. La empresa necesita ser informada si un objeto se corrompe durante la carga. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Pasar el valor `Content-Disposition` como cuerpo de la solicitud durante la carga del objeto.
- [x] Pasar el valor `Content-MD5` como encabezado de la solicitud durante la carga del objeto.
- [ ] Pasar `x-amz-object-lock-mode` como encabezado de la solicitud durante la carga del objeto.
- [ ] Pasar `x-amz-server-side-encryption-customer-algorithm` como cuerpo de la solicitud durante la carga del objeto.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa actualmente ejecuta su infraestructura dentro de una `VPC` en una sola Zona de disponibilidad. La `VPC` está conectada al centro de datos on-premises de la empresa a través de una conexión AWS Site-to-Site `VPN` adjunta a una puerta de enlace privada virtual. Las tablas de enrutamiento on-premises enrutan todas las redes de la `VPC` hacia la conexión `VPN`. La comunicación entre ambos entornos funciona correctamente. Un ingeniero de CloudOps creó nuevas subredes de `VPC` dentro de una nueva Zona de disponibilidad, y desplegó nuevos recursos dentro de esas subredes. Sin embargo, no se puede establecer comunicación entre los nuevos recursos y el entorno on-premises. ¿Qué pasos debe tomar el ingeniero de CloudOps para resolver el problema?

- [x] Agregar una ruta a las tablas de enrutamiento de las nuevas subredes que envíe el tráfico on-premises hacia la puerta de enlace privada virtual.
- [ ] Crear un ticket con AWS Support para solicitar agregar Zonas de disponibilidad a la configuración de ruta de la Site-to-Site `VPN`.
- [ ] Establecer una nueva conexión Site-to-Site `VPN` entre una puerta de enlace privada virtual adjunta a la nueva Zona de disponibilidad y el centro de datos on-premises.
- [ ] Reemplazar la conexión Site-to-Site `VPN` con una conexión de AWS Direct Connect.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación web interna que se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias se ejecutan en un grupo de Amazon EC2 Auto Scaling en una única Zona de disponibilidad. Un ingeniero de CloudOps debe hacer que la aplicación tenga alta disponibilidad. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Aumentar el número máximo de instancias en el grupo de Auto Scaling para cumplir con la capacidad requerida en el uso pico.
- [ ] Aumentar el número mínimo de instancias en el grupo de Auto Scaling para cumplir con la capacidad requerida en el uso pico.
- [x] Actualizar el grupo de Auto Scaling para lanzar nuevas instancias en una segunda Zona de disponibilidad dentro de la misma región de AWS.
- [ ] Actualizar el grupo de Auto Scaling para lanzar nuevas instancias en una Zona de disponibilidad de una segunda región de AWS.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja un sitio web en múltiples instancias de Amazon EC2 que se ejecutan en un grupo de Auto Scaling. Los usuarios reportan respuestas lentas durante horas pico, entre las 6 PM y las 11 PM cada fin de semana. Un ingeniero de CloudOps debe implementar una solución para mejorar el rendimiento durante estos horarios pico. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una regla programada de Amazon EventBridge (Amazon CloudWatch Events) para invocar una función de AWS Lambda que aumente la capacidad deseada antes de las horas pico.
- [x] Configurar una acción de escalado programado con una opción de recurrencia para cambiar la capacidad deseada antes y después de las horas pico.
- [ ] Crear una política de escalado por seguimiento de destino (target tracking) para agregar más instancias cuando el uso de memoria supere el `70%`.
- [ ] Configurar el período de enfriamiento (cooldown) del grupo de Auto Scaling para modificar la capacidad deseada antes y después de las horas pico.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ejecutando un sitio web en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa configuró una distribución de Amazon CloudFront y estableció el `ALB` como origen. La empresa creó un registro `CNAME` de Amazon Route 53 para enviar todo el tráfico a través de la distribución de CloudFront. Como efecto secundario no deseado, ahora se está sirviendo a los usuarios móviles la versión de escritorio del sitio web. ¿Qué acción debe tomar un ingeniero de CloudOps para resolver este problema?

- [x] Configurar el comportamiento de la distribución de CloudFront para reenviar el encabezado `User-Agent`.
- [ ] Configurar la configuración de origen de la distribución de CloudFront. Agregar un encabezado `User-Agent` a la lista de encabezados personalizados de origen.
- [ ] Habilitar IPv6 en el `ALB`. Actualizar la configuración de origen de la distribución de CloudFront para usar el endpoint de doble pila (dualstack).
- [ ] Habilitar IPv6 en la distribución de CloudFront. Actualizar el registro de Route 53 para usar el endpoint de doble pila.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja su sitio web en instancias de Amazon EC2 detrás de un Application Load Balancer. La empresa administra su `DNS` con Amazon Route 53, y quiere apuntar el ápice de zona (zone apex) de su dominio hacia el sitio web. ¿Qué tipo de registro se debe usar para cumplir con estos requisitos?

- [ ] Un registro `AAAA` para el ápice de zona del dominio.
- [ ] Un registro `A` para el ápice de zona del dominio.
- [ ] Un registro `CNAME` para el ápice de zona del dominio.
- [x] Un registro de alias para el ápice de zona del dominio.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha creado una `VPC` que contiene una subred pública y una subred privada. Las instancias de Amazon EC2 que se lanzaron en la subred privada no pueden acceder a internet. La `ACL` de red predeterminada está activa en todas las subredes de la `VPC`, y todos los grupos de seguridad permiten todo el tráfico de salida. ¿Qué solución proporcionará a las instancias de EC2 en la subred privada acceso a internet?

- [x] Crear una puerta de enlace `NAT` en la subred pública. Crear una ruta desde la subred privada hacia la puerta de enlace `NAT`.
- [ ] Crear una puerta de enlace `NAT` en la subred pública. Crear una ruta desde la subred pública hacia la puerta de enlace `NAT`.
- [ ] Crear una puerta de enlace `NAT` en la subred privada. Crear una ruta desde la subred pública hacia la puerta de enlace `NAT`.
- [ ] Crear una puerta de enlace `NAT` en la subred privada. Crear una ruta desde la subred privada hacia la puerta de enlace `NAT`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa AWS CloudFormation para desplegar su infraestructura. La empresa recientemente retiró una aplicación. Un ingeniero de operaciones en la nube inicia la eliminación de un stack de CloudFormation, y el stack queda atascado en estado `DELETE_FAILED`. Un ingeniero de CloudOps descubre que el stack había desplegado un grupo de seguridad. Ese grupo de seguridad es referenciado por otros grupos de seguridad en el entorno. El ingeniero de CloudOps necesita eliminar el stack sin afectar otras aplicaciones. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear un nuevo grupo de seguridad con un nombre diferente. Aplicar reglas idénticas al nuevo grupo de seguridad. Reemplazar todos los demás grupos de seguridad que referencien al nuevo grupo de seguridad. Eliminar el stack.
- [ ] Crear un conjunto de cambios (change set) de CloudFormation para eliminar el grupo de seguridad. Desplegar el conjunto de cambios.
- [x] Eliminar el stack nuevamente. Especificar que el grupo de seguridad se conserve (retained).
- [ ] Realizar una detección de deriva (drift detection) de CloudFormation. Eliminar el stack.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps crea una plantilla de AWS CloudFormation para definir una pila de aplicación que puede desplegarse en múltiples regiones de AWS. El ingeniero de CloudOps también crea un dashboard de Amazon CloudWatch usando la consola de administración de AWS. Cada despliegue de la aplicación requiere su propio dashboard de CloudWatch. ¿Cómo puede el ingeniero de CloudOps automatizar la creación del dashboard de CloudWatch cada vez que se despliega la aplicación?

- [ ] Crear un script usando la AWS CLI para ejecutar el comando `aws cloudformation put-dashboard` con el nombre del dashboard. Ejecutar el comando cada vez que se cree un nuevo stack de CloudFormation.
- [x] Exportar el dashboard de CloudWatch existente como JSON. Actualizar la plantilla de CloudFormation para definir un recurso `AWS::CloudWatch::Dashboard`. Incluir el JSON exportado en la propiedad `DashboardBody` del recurso.
- [ ] Actualizar la plantilla de CloudFormation para definir un recurso `AWS::CloudWatch::Dashboard`. Usar la función intrínseca Ref para referenciar el ID del dashboard de CloudWatch existente.
- [ ] Actualizar la plantilla de CloudFormation para definir un recurso `AWS::CloudWatch::Dashboard`. Especificar el nombre del dashboard existente en la propiedad `DashboardName`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está aprovisionando un sistema de archivos de Amazon Elastic File System (Amazon EFS) para proporcionar almacenamiento compartido entre múltiples instancias de Amazon EC2. Las instancias existen en la misma `VPC` a través de múltiples Zonas de disponibilidad. Hay dos instancias en cada Zona de disponibilidad. El ingeniero de CloudOps debe hacer que el sistema de archivos sea accesible para cada instancia con la menor latencia posible. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un punto de montaje (mount target) para el sistema de archivos EFS en la `VPC`. Usar el punto de montaje para montar el sistema de archivos en cada una de las instancias.
- [ ] Crear un punto de montaje para el sistema de archivos EFS en una Zona de disponibilidad de la `VPC`. Usar el punto de montaje para montar el sistema de archivos en las instancias de esa Zona de disponibilidad. Compartir el directorio con las demás instancias.
- [ ] Crear un punto de montaje para cada instancia. Usar cada punto de montaje para montar el sistema de archivos EFS en su respectiva instancia.
- [x] Crear un punto de montaje en cada Zona de disponibilidad de la `VPC`. Usar el punto de montaje para montar el sistema de archivos EFS en las instancias de la Zona de disponibilidad respectiva.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha desplegado con éxito una `VPC` con una plantilla de AWS CloudFormation. El ingeniero de CloudOps quiere desplegar la misma plantilla en múltiples cuentas administradas a través de AWS Organizations. ¿Qué solución cumple con este requisito con el MENOR esfuerzo operativo?

- [ ] Asumir el rol de IAM `OrganizationAccountAccessRole` desde la cuenta de administración. Desplegar la plantilla en cada una de las cuentas.
- [ ] Crear una función de AWS Lambda para asumir un rol en cada cuenta. Desplegar la plantilla usando la llamada a la API `CreateStack` de AWS CloudFormation.
- [ ] Crear una función de AWS Lambda para consultar una lista de cuentas. Desplegar la plantilla usando la llamada a la API `CreateStack` de AWS CloudFormation.
- [x] Usar `StackSets` de AWS CloudFormation desde la cuenta de administración para desplegar la plantilla en cada una de las cuentas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ejecutando un software de computación distribuida para administrar una flota de 20 instancias de Amazon EC2 para cálculos. La flota incluye 2 nodos de control y 18 nodos de tareas para ejecutar los cálculos. Los nodos de control pueden iniciar automáticamente los nodos de tareas. Actualmente, todos los nodos se ejecutan bajo demanda (on-demand). Los nodos de control deben estar disponibles las 24 horas del día, los 7 días de la semana. Los nodos de tareas se ejecutan durante 4 horas cada día. Un ingeniero de CloudOps necesita optimizar el costo de esta solución. ¿Qué combinación de acciones cumple con estos requisitos? (Elija dos.)

- [x] Comprar Savings Plans de instancias de EC2 para los nodos de control.
- [ ] Usar Hosts Dedicados para los nodos de control.
- [ ] Usar Instancias Reservadas para los nodos de tareas.
- [ ] Usar instancias Spot para los nodos de control. Usar instancias On-Demand si no hay disponibilidad Spot.
- [x] Usar instancias Spot para los nodos de tareas. Usar instancias On-Demand si no hay disponibilidad Spot.

**[⬆ Volver arriba](#table-of-contents)**

### Se supone que una empresa recibe un archivo de datos cada hora en un bucket de Amazon S3. Una notificación de evento de S3 invoca una función de AWS Lambda cada vez que llega un archivo. La función procesa los datos para que los use una aplicación. El equipo de la aplicación nota que, a veces, el archivo no llega. El equipo de la aplicación quiere recibir una notificación siempre que el archivo no llegue. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Agregar una regla de ciclo de vida de S3 en el bucket de S3 con un alcance limitado a objetos creados en la última hora. Configurar otra notificación de evento de S3 para que se invoque mediante la transición de ciclo de vida cuando el número de objetos transicionados sea cero. Publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) para notificar al equipo de la aplicación.
- [ ] Configurar otra notificación de evento de S3 para invocar una función Lambda que publique un mensaje en una cola de Amazon Simple Queue Service (Amazon SQS). Crear una alarma de Amazon CloudWatch para publicar un mensaje en un tema de Amazon SNS y notificar al equipo de la aplicación cuando la métrica ApproximateAgeOfOldestMessage de la cola sea mayor a 1 hora.
- [x] Crear una alarma de Amazon CloudWatch para publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) que alerte al equipo de la aplicación cuando la métrica Invocations de la función Lambda sea cero durante una hora. Configurar la alarma para tratar los datos faltantes como incumplimiento (breaching).
- [ ] Crear una nueva función Lambda para obtener la marca de tiempo del archivo más reciente en el bucket de S3. Si la marca de tiempo tiene más de 1 hora de antigüedad, publicar un mensaje en un tema de Amazon SNS para notificar al equipo de la aplicación. Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para invocar la nueva función cada hora.

**[⬆ Volver arriba](#table-of-contents)**


### Una empresa tiene una aplicación web que experimenta problemas de rendimiento varias veces cada noche. Un análisis de causa raíz revela aumentos repentinos en el uso de CPU que duran 5 minutos en una instancia de Amazon EC2 Linux. Un ingeniero de CloudOps debe encontrar el ID de proceso (PID) del servicio o proceso que está consumiendo más CPU. ¿Qué debe hacer el ingeniero de CloudOps para recopilar la información de uso del proceso con el MENOR esfuerzo posible?

- [x] Configurar el plugin `procstat` del agente de Amazon CloudWatch para capturar métricas de procesos de CPU.
- [ ] Configurar una función de AWS Lambda que se ejecute cada minuto para capturar el PID y enviar una notificación.
- [ ] Iniciar sesión en la instancia de EC2 usando una clave `.pem` cada noche. Luego ejecutar el comando top.
- [ ] Usar la métrica predeterminada de uso de CPU de Amazon CloudWatch para capturar el PID en CloudWatch.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps configuró AWS Backup para capturar instantáneas de una sola instancia de Amazon EC2 que tiene un volumen de Amazon Elastic Block Store (Amazon EBS) adjunto. En la primera instantánea, el volumen EBS tiene 10 GiB de datos. En la segunda instantánea, el volumen EBS todavía contiene 10 GiB de datos, pero 4 GiB han cambiado. En la tercera instantánea, se han agregado 2 GiB de datos al volumen, para un total de 12 GiB. ¿Cuánto almacenamiento total se requiere para guardar estas instantáneas?

- [ ] 12 GiB.
- [x] 16 GiB.
- [ ] 26 GiB.
- [ ] 32 GiB.

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo administra una cuenta de AWS que es miembro de una organización en AWS Organizations. La organización tiene habilitadas las funciones de facturación consolidada. La cuenta aloja varias aplicaciones. Un ingeniero de CloudOps ha aplicado etiquetas (tags) a los recursos dentro de la cuenta para reflejar el entorno. El equipo necesita un informe del desglose de cargos por entorno. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Filtrar, mapear y categorizar grupos de recursos en Tag Editor.
- [ ] Asegurarse de que las Políticas de Control de Servicio (SCP) de la organización permitan el acceso a las etiquetas de asignación de costos.
- [ ] Asegurarse de que las credenciales de IAM utilizadas para acceder a Cost Explorer tengan permisos para agrupar costos por etiquetas.
- [x] Activar las claves de etiquetas para la asignación de costos en la cuenta de administración de la organización.

**[⬆ Volver arriba](#table-of-contents)**

### Se sabe que un proceso errático usa un procesador completo y se ejecuta al `100%`. Un ingeniero de CloudOps quiere automatizar el reinicio de una instancia de Amazon EC2 cuando el problema ocurre por más de 2 minutos. ¿Cómo se puede lograr esto?

- [ ] Crear una alarma de Amazon CloudWatch para la instancia de EC2 con monitoreo básico. Agregar una acción para reiniciar la instancia.
- [x] Crear una alarma de Amazon CloudWatch para la instancia de EC2 con monitoreo detallado. Agregar una acción para reiniciar la instancia.
- [ ] Crear una función de AWS Lambda para reiniciar la instancia de EC2, invocada de forma programada cada 2 minutos.
- [ ] Crear una función de AWS Lambda para reiniciar la instancia de EC2, invocada por verificaciones de salud (health checks) de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja un sitio web estático en Amazon S3. El sitio web es servido por una distribución de Amazon CloudFront con un `TTL` predeterminado de 86,400 segundos. La empresa recientemente subió una versión actualizada del sitio web a Amazon S3. Sin embargo, los usuarios siguen viendo el contenido antiguo cuando actualizan el sitio. Un ingeniero de CloudOps debe hacer visible la nueva versión del sitio web a los usuarios lo antes posible. ¿Qué solución cumple con estos requisitos?

- [ ] Ajustar el valor de `TTL` para el registro `CNAME` de `DNS` que apunta a la distribución de CloudFront.
- [x] Crear una invalidación en la distribución de CloudFront para los objetos antiguos de S3.
- [ ] Crear una nueva distribución de CloudFront. Actualizar los registros `DNS` para que apunten a la nueva distribución de CloudFront.
- [ ] Actualizar el registro `DNS` del sitio web para que apunte al bucket de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps es responsable de administrar la infraestructura en la nube de una empresa con AWS CloudFormation. El ingeniero de CloudOps necesita crear un único recurso que consista en múltiples servicios de AWS. El recurso debe admitir su creación y eliminación a través de la consola de CloudFormation. ¿Qué tipo de recurso de CloudFormation debe crear el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] `AWS::EC2::Instance` con un script de ayuda `cfn-init`.
- [ ] `AWS::OpsWorks::Instance`.
- [ ] `AWS::SSM::Document`.
- [x] `Custom::MyCustomType`.

**[⬆ Volver arriba](#table-of-contents)**

### Un nuevo sitio web se ejecutará en instancias de Amazon EC2 detrás de un Application Load Balancer. Amazon Route 53 se usará para administrar los registros `DNS`. ¿Qué tipo de registro se debe configurar en Route 53 para que el nombre de dominio raíz del sitio web (por ejemplo, `company.com`) apunte al Application Load Balancer?

- [ ] `CNAME`.
- [ ] `SOA`.
- [ ] `TXT`.
- [x] `ALIAS`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está implementando seguridad y cumplimiento normativo usando AWS Trusted Advisor. El equipo de SysOps de la empresa está validando la lista de verificaciones de Trusted Advisor a las que puede acceder. ¿Qué factor afectará la cantidad de verificaciones de Trusted Advisor disponibles?

- [ ] Si al menos una instancia de Amazon EC2 está en estado de ejecución.
- [x] El plan de soporte de AWS.
- [ ] Una Política de Control de Servicio (SCP) de AWS Organizations.
- [ ] Si el usuario raíz de la cuenta de AWS tiene habilitada la autenticación multifactor (MFA).

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está investigando problemas en una instancia de base de datos de Amazon RDS para MariaDB. El ingeniero de CloudOps quiere mostrar la carga de la base de datos categorizada por eventos de espera detallados. ¿Cómo puede el ingeniero de CloudOps lograr este objetivo?

- [ ] Crear un panel (dashboard) de Amazon CloudWatch.
- [x] Habilitar `Performance Insights` de Amazon RDS.
- [ ] Habilitar y configurar `Enhanced Monitoring`.
- [ ] Revisar los registros de la base de datos en Amazon CloudWatch Logs.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa planea alojar una aplicación en un conjunto de instancias de Amazon EC2 distribuidas entre múltiples Zonas de disponibilidad. La aplicación debe poder escalar a millones de solicitudes por segundo. Un ingeniero de CloudOps debe diseñar una solución para distribuir el tráfico a las instancias de EC2. La solución debe estar optimizada para manejar patrones de tráfico repentinos y volátiles, usando una única dirección IP estática por cada Zona de disponibilidad. ¿Qué solución cumple con estos requisitos?

- [ ] Cola de Amazon Simple Queue Service (Amazon SQS).
- [ ] Application Load Balancer.
- [ ] AWS Global Accelerator.
- [x] Network Load Balancer.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está usando `StackSets` de AWS CloudFormation para crear recursos de AWS en dos regiones de AWS dentro de la misma cuenta de AWS. Una operación de stack falla en una región y devuelve el estado de instancia de stack `OUTDATED`. ¿Cuál es la causa de esta falla?

- [ ] La plantilla de CloudFormation cambió en el disco local y no ha sido enviada a CloudFormation.
- [x] La plantilla de CloudFormation está intentando crear un recurso global que no es único.
- [ ] El stack aún no ha sido desplegado en la región.
- [ ] El ingeniero de CloudOps está usando una versión antigua de la API de CloudFormation.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe configurar Amazon S3 para alojar una página web simple de no producción. El ingeniero de CloudOps ha creado un bucket de S3 vacío desde la consola de administración de AWS. El bucket de S3 tiene la configuración predeterminada. ¿Qué combinación de acciones debe tomar el ingeniero de CloudOps para completar este proceso? (Elija dos.)

- [ ] Configurar el bucket de S3 usando la funcionalidad `Redirect requests for an object` para apuntar a la URL raíz del bucket.
- [ ] Desactivar la configuración `Block all public access`. Permitir acceso público usando una `ACL` de bucket que contenga `<Permission>WEBSITE</Permission>`.
- [ ] Desactivar la configuración `Block all public access`. Permitir acceso público usando una `ACL` de bucket que permita acceso al grantee AuthenticatedUsers.
- [x] Desactivar la configuración `Block all public access`. Configurar una política de bucket que permita la acción `s3:GetObject` para `Principal:` `*`.
- [x] Crear un documento `index.html`. Configurar el alojamiento de sitio web estático y subir el documento index al bucket de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está usando un clúster de base de datos Amazon Aurora MySQL que tiene habilitados recuperación a un punto en el tiempo, retroceso (backtracking) y respaldo automático. Un ingeniero de CloudOps necesita poder revertir el clúster de base de datos a un punto de recuperación específico dentro de las últimas 72 horas. Las restauraciones deben completarse en el mismo clúster de base de datos de producción. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una réplica de Aurora. Promover la réplica para reemplazar la instancia de base de datos principal.
- [ ] Crear una función de AWS Lambda para restaurar un respaldo automático al clúster de base de datos existente.
- [x] Usar el retroceso (backtracking) para rebobinar el clúster de base de datos existente hasta el punto de recuperación deseado.
- [ ] Usar la recuperación a un punto en el tiempo para restaurar el clúster de base de datos existente al punto de recuperación deseado.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario que trabaja en la consola de Amazon EC2 aumentó el tamaño de un volumen de Amazon Elastic Block Store (Amazon EBS) adjunto a una instancia de Amazon EC2 Windows. El cambio no se refleja en el sistema de archivos. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?

- [x] Extender el sistema de archivos con herramientas a nivel de sistema operativo para usar la nueva capacidad de almacenamiento.
- [ ] Volver a adjuntar el volumen EBS a la instancia de EC2.
- [ ] Reiniciar la instancia de EC2 que está adjunta al volumen EBS.
- [ ] Tomar una instantánea del volumen EBS. Reemplazar el volumen original por un volumen creado a partir de la instantánea.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps quiere proteger los objetos en un bucket de Amazon S3 contra sobrescritura y eliminación accidental. Los objetos no actuales deben conservarse durante 90 días y luego deben eliminarse permanentemente. Los objetos deben residir dentro de la misma región de AWS que el bucket de S3 original. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una política de ciclo de vida de Amazon Data Lifecycle Manager (Amazon DLM) para el bucket de S3. Agregar una regla a la política de ciclo de vida para eliminar los objetos no actuales después de 90 días.
- [ ] Crear una política de AWS Backup para el bucket de S3. Crear una regla de respaldo que incluya un ciclo de vida para expirar los objetos no actuales después de 90 días.
- [ ] Habilitar la replicación entre regiones (Cross-Region Replication) de S3 en el bucket de S3. Crear una política de ciclo de vida de S3 para el bucket que expire los objetos no actuales después de 90 días.
- [x] Habilitar el versionado (Versioning) de S3 en el bucket de S3. Crear una política de ciclo de vida de S3 para el bucket que expire los objetos no actuales después de 90 días.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa AWS Organizations para administrar múltiples cuentas de AWS. La política corporativa exige que solo se puedan usar regiones específicas de AWS para almacenar y procesar datos de clientes. Un ingeniero de CloudOps debe evitar el aprovisionamiento de instancias de Amazon EC2 en regiones no autorizadas por parte de cualquier persona en la empresa. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Configurar AWS CloudTrail en todas las regiones para registrar toda la actividad de la API. Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) en todas las regiones no autorizadas para eventos `ec2:RunInstances`. Usar AWS Lambda para terminar las instancias de EC2 lanzadas.
- [ ] En cada cuenta de AWS, crear una política administrada de IAM que use una condición de región para denegar la acción `ec2:RunInstances` en todas las regiones no autorizadas. Adjuntar esta política a todos los grupos de IAM en cada cuenta de AWS.
- [ ] En cada cuenta de AWS, crear una política de límite de permisos (permissions boundary) de IAM que use una condición `Region` para denegar la acción `ec2:RunInstances` en todas las regiones no autorizadas. Adjuntar la política de límite de permisos a todos los usuarios de IAM en cada cuenta de AWS.
- [x] Crear una Política de Control de Servicio (SCP) en AWS Organizations para denegar la acción `ec2:RunInstances` en todas las regiones no autorizadas. Adjuntar esta política al nivel raíz de la organización.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene un bucket privado de Amazon S3 que contiene información confidencial. Un ingeniero de CloudOps necesita mantener registros de las direcciones IP de los fallos de autenticación resultantes de intentos de acceder a objetos en el bucket. Los registros deben almacenarse de manera que no puedan sobrescribirse ni eliminarse durante 90 días. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un trail de AWS CloudTrail. Configurar los archivos de registro para que se guarden en Amazon CloudWatch Logs. Configurar el grupo de registro con un período de retención de 90 días.
- [ ] Crear un trail de AWS CloudTrail. Configurar los archivos de registro para que se guarden en un bucket de S3 diferente. Activar la validación de integridad de archivos de registro de CloudTrail durante 90 días.
- [ ] Activar el registro de acceso (access logging) para el bucket de S3. Configurar los registros de acceso para que se guarden en Amazon CloudWatch Logs. Configurar el grupo de registro con un período de retención de 90 días.
- [x] Activar el registro de acceso (access logging) para el bucket de S3. Configurar los registros de acceso para que se guarden en un segundo bucket de S3. Activar S3 Object Lock en el segundo bucket de S3, y configurar un período de retención predeterminado de 90 días.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps migra instancias `NAT` a puertas de enlace `NAT`. Después de la migración, una aplicación alojada en instancias de Amazon EC2 en una subred privada no puede acceder a internet. ¿Cuáles de las siguientes son posibles razones para este problema? (Elija dos.)

- [x] La aplicación está usando un protocolo que la puerta de enlace `NAT` no admite.
- [ ] La puerta de enlace `NAT` no está en un grupo de seguridad.
- [ ] La puerta de enlace `NAT` está en una Zona de disponibilidad no compatible.
- [x] La puerta de enlace `NAT` no está en el estado Available.
- [ ] La configuración de reenvío de puertos no permite el acceso a servicios internos desde internet.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación en una instancia de Amazon EC2. Un ingeniero de CloudOps crea un grupo de Auto Scaling y un Application Load Balancer (ALB) para manejar un aumento en la demanda. Sin embargo, las instancias de EC2 están fallando la verificación de salud (health check). ¿Qué debe hacer el ingeniero de CloudOps para solucionar este problema?

- [ ] Verificar que el grupo de Auto Scaling esté configurado para usar todas las regiones de AWS.
- [x] Verificar que la aplicación se esté ejecutando en el protocolo y el puerto que el listener espera.
- [ ] Verificar la prioridad del listener en el `ALB`. Cambiar la prioridad si es necesario.
- [ ] Verificar el número máximo de instancias en el grupo de Auto Scaling. Cambiar el número si es necesario.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha migrado su aplicación a AWS. La empresa alojará la aplicación en instancias de Amazon EC2 de múltiples familias de instancias. Durante las pruebas iniciales, un ingeniero de CloudOps identifica problemas de rendimiento en instancias de EC2 seleccionadas. La empresa tiene una política estricta de asignación de presupuesto, por lo que el ingeniero de CloudOps debe usar los tipos de recursos correctos con las características de rendimiento que coincidan con la carga de trabajo. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Comprar Instancias Reservadas (RI) regionales para ahorros de costos inmediatos. Revisar y actuar sobre las recomendaciones de rightsizing de EC2 en Cost Explorer. Intercambiar las RI por la familia de instancias óptima después del rightsizing.
- [ ] Comprar Instancias Reservadas (RI) zonales para las instancias existentes. Monitorear la utilización de RI en la consola de AWS Billing and Cost Management. Hacer ajustes en los tamaños de instancia para optimizar la utilización.
- [x] Revisar y actuar sobre las recomendaciones de AWS Compute Optimizer. Comprar Compute Savings Plans para reducir el costo requerido para ejecutar los recursos de cómputo.
- [ ] Revisar las métricas de utilización de recursos en el AWS Cost and Usage Report. Ajustar el tamaño (rightsize) de las instancias de EC2. Crear Reservas de Capacidad On-Demand para los recursos ajustados.

**[⬆ Volver arriba](#table-of-contents)**

### A un ingeniero de CloudOps se le asigna la tarea de desplegar la infraestructura de una empresa como código. El ingeniero de CloudOps quiere escribir una única plantilla que pueda reutilizarse para múltiples entornos. ¿Cómo debe el ingeniero de CloudOps usar AWS CloudFormation para crear una solución?

- [ ] Usar datos de usuario (user data) de Amazon EC2 en una plantilla de CloudFormation.
- [ ] Usar stacks anidados (nested stacks) para aprovisionar recursos.
- [x] Usar parámetros en una plantilla de CloudFormation.
- [ ] Usar políticas de stack para aprovisionar recursos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps es responsable de una gran flota de instancias de Amazon EC2 y debe saber si alguna instancia se verá afectada por el próximo mantenimiento de hardware. ¿Qué opción proporcionaría esta información con el MENOR esfuerzo administrativo?

- [ ] Desplegar una solución de monitoreo de terceros para proporcionar monitoreo en tiempo real de instancias EC2.
- [ ] Listar las instancias con verificaciones de estado del sistema fallidas usando la consola de administración de AWS.
- [ ] Monitorear AWS CloudTrail en busca de llamadas a la API `StopInstances`.
- [x] Revisar el AWS Personal Health Dashboard.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está intentando desplegar recursos usando una plantilla de AWS CloudFormation. Una instancia de Amazon EC2 que está definida en la plantilla no logra iniciarse y produce un error `InsufficientInstanceCapacity`. ¿Qué acciones debe tomar el ingeniero de CloudOps para resolver este error? (Elija dos.)

- [ ] Crear una plantilla de AWS CloudFormation separada para la instancia de EC2.
- [x] Modificar la plantilla de AWS CloudFormation para no especificar una Zona de disponibilidad para la instancia de EC2.
- [x] Modificar la plantilla de AWS CloudFormation para usar un tipo de instancia de EC2 diferente.
- [ ] Usar una Amazon Machine Image (AMI) diferente para la instancia de EC2.
- [ ] Usar el comando `validate-template` de la AWS CLI antes de crear un stack a partir de la plantilla.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja una aplicación web en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa usa Amazon Route 53 para enrutar el tráfico. La empresa también tiene un sitio web estático configurado en un bucket de Amazon S3. Un ingeniero de CloudOps debe usar el sitio web estático como respaldo de la aplicación web. La conmutación por error (failover) al sitio web estático debe ser completamente automatizada. ¿Qué combinación de acciones cumple con estos requisitos? (Elija dos.)

- [ ] Crear un registro de política de enrutamiento de failover primario. Configurar el valor para que sea el `ALB`.
- [ ] Crear una función de AWS Lambda para cambiar del sitio web primario al secundario cuando falle la verificación de salud.
- [x] Crear un registro de política de enrutamiento de failover primario. Configurar el valor para que sea el `ALB`. Asociar el registro con una verificación de salud de Route 53.
- [ ] Crear un registro de política de enrutamiento de failover secundario. Configurar el valor para que sea el sitio web estático. Asociar el registro con una verificación de salud de Route 53.
- [x] Crear un registro de política de enrutamiento de failover secundario. Configurar el valor para que sea el sitio web estático.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación de análisis de datos se está ejecutando en una instancia de Amazon EC2. Un ingeniero de CloudOps debe agregar dimensiones personalizadas a las métricas recopiladas por el agente de Amazon CloudWatch. ¿Cómo puede el ingeniero de CloudOps cumplir con este requisito?

- [ ] Crear un script de shell personalizado para extraer las dimensiones y recopilar las métricas usando el agente de Amazon CloudWatch.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para evaluar las dimensiones personalizadas requeridas y enviar las métricas a Amazon Simple Notification Service (Amazon SNS).
- [ ] Crear una función de AWS Lambda para recopilar las métricas de AWS CloudTrail y enviar las métricas a un grupo de Amazon CloudWatch Logs.
- [x] Crear un campo `append_dimensions` en el archivo de configuración del agente de Amazon CloudWatch para recopilar las métricas.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps está examinando la siguiente plantilla de AWS CloudFormation. ¿Por qué fallará la creación del stack?

![Question 201](images/question201.jpg)

- [ ] Se omitió la sección `Outputs` de la plantilla de CloudFormation.
- [ ] Se omitió la sección `Parameters` de la plantilla de CloudFormation.
- [x] `PrivateDnsName` no se puede configurar desde una plantilla de CloudFormation.
- [ ] No se especificó la `VPC` en la plantilla de CloudFormation.

**[⬆ Volver arriba](#table-of-contents)**

### Una nueva aplicación se ejecuta en instancias de Amazon EC2 y accede a datos en una instancia de base de datos de Amazon RDS. Cuando se despliega completamente en producción, la aplicación falla. La base de datos puede consultarse desde una consola en un bastion host. Al revisar los registros del servidor web, se repite varias veces el siguiente error: `*** Error Establishing a Database Connection`. ¿Cuáles de las siguientes pueden ser causas de los problemas de conectividad? (Elija dos.)

- [ ] El grupo de seguridad de la base de datos no tiene la regla de salida (egress) apropiada desde la base de datos hacia el servidor web.
- [ ] El certificado usado por el servidor web no es de confianza para la instancia de RDS.
- [x] El grupo de seguridad de la base de datos no tiene la regla de entrada (ingress) apropiada desde el servidor web hacia la base de datos.
- [x] El puerto usado por el desarrollador de la aplicación no coincide con el puerto especificado en la configuración de RDS.
- [ ] La base de datos todavía se está creando y no está disponible para conectividad.

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo de cumplimiento normativo requiere que todas las contraseñas de administrador de las instancias de base de datos de Amazon RDS se cambien al menos una vez al año. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?

- [x] Almacenar las credenciales de la base de datos en AWS Secrets Manager. Configurar la rotación automática del secreto cada 365 días.
- [ ] Almacenar las credenciales de la base de datos como un parámetro en el grupo de parámetros de RDS. Crear un disparador (trigger) de base de datos para rotar la contraseña cada 365 días.
- [ ] Almacenar las credenciales de la base de datos en un bucket privado de Amazon S3. Programar una función de AWS Lambda para generar un nuevo conjunto de credenciales cada 365 días.
- [ ] Almacenar las credenciales de la base de datos en AWS Systems Manager Parameter Store como un parámetro de tipo secure string. Configurar la rotación automática del parámetro cada 365 días.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps es responsable de administrar una flota de instancias de Amazon EC2. Estas instancias de EC2 suben artefactos de compilación (build artifacts) a un servicio de terceros. El servicio de terceros implementó recientemente una lista estricta de IP permitidas que requiere que todas las cargas de compilación provengan de una única dirección IP. ¿Qué cambio debe hacer el ingeniero de sistemas en la flota de compilación existente para cumplir con este nuevo requisito?

- [x] Mover todas las instancias de EC2 detrás de una puerta de enlace `NAT` y proporcionar la dirección IP de la puerta de enlace al servicio.
- [ ] Mover todas las instancias de EC2 detrás de una puerta de enlace de internet y proporcionar la dirección IP de la puerta de enlace al servicio.
- [ ] Mover todas las instancias de EC2 a una sola Zona de disponibilidad y proporcionar la dirección IP de la Zona de disponibilidad al servicio.
- [ ] Mover todas las instancias de EC2 a una `VPC` emparejada (peered) y proporcionar la dirección IP de la `VPC` al servicio.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa una distribución de Amazon CloudFront para entregar su sitio web. Los registros de tráfico del sitio web deben almacenarse de forma centralizada, y todos los datos deben estar cifrados en reposo. ¿Qué solución cumple con estos requisitos?

- [ ] Crear un dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) con acceso a internet y cifrado del lado del servidor que use la Customer Master Key (CMK) administrada por AWS predeterminada. Configurar CloudFront para usar el dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) como destino de registros.
- [ ] Crear un dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) con acceso `VPC` y cifrado del lado del servidor que use `AES-256`. Configurar CloudFront para usar el dominio de Amazon OpenSearch Service (Amazon Elasticsearch Service) como destino de registros.
- [x] Crear un bucket de Amazon S3 configurado con cifrado del lado del servidor predeterminado que use `AES-256`. Configurar CloudFront para usar el bucket de S3 como destino de registros.
- [ ] Crear un bucket de Amazon S3 configurado sin cifrado predeterminado. Habilitar el cifrado en la distribución de CloudFront, y usar el bucket de S3 como destino de registros.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa recibe una alerta de una alarma de Amazon CloudWatch. La alarma indica que una aplicación web que se ejecuta en instancias de Amazon EC2 no está respondiendo a las solicitudes. Las instancias de EC2 tienen un sistema operativo Red Hat Enterprise Linux y están en un grupo de Auto Scaling. El grupo de Auto Scaling tiene una capacidad mínima de 2 y una capacidad máxima de 5. Una investigación revela que la aplicación web está experimentando errores por falta de memoria (out-of-memory). La empresa agrega memoria a la aplicación web y quiere monitorear el uso de memoria del sistema operativo. Actualmente no existe una métrica de memoria de CloudWatch para las instancias de EC2 en el grupo de Auto Scaling. ¿Qué debe hacer un ingeniero de CloudOps para proporcionar una métrica de memoria de CloudWatch para las instancias de EC2?

- [x] Usar una Amazon Machine Image (AMI) que incluya el agente de CloudWatch.
- [ ] Activar el monitoreo detallado de CloudWatch.
- [ ] Activar Instance Metadata Service Version 2 (IMDSv2).
- [ ] Usar una Amazon Machine Image (AMI) basada en Amazon Linux.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa un portafolio de AWS Service Catalog para crear y administrar recursos. Un ingeniero de CloudOps debe crear una réplica de la infraestructura de AWS existente de la empresa en una nueva cuenta de AWS. ¿Cuál es la forma MÁS eficiente operativamente de cumplir con este requisito?

- [ ] Crear una plantilla de AWS CloudFormation para usar el portafolio de AWS Service Catalog en la nueva cuenta de AWS.
- [ ] En la nueva cuenta de AWS, crear manualmente un portafolio de AWS Service Catalog que duplique el portafolio original.
- [ ] Ejecutar una función de AWS Lambda para crear un nuevo portafolio de AWS Service Catalog basado en la salida de la operación de API `DescribePortfolio`.
- [x] Compartir el portafolio de AWS Service Catalog con la nueva cuenta de AWS. Importar el portafolio a la nueva cuenta de AWS.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe administrar la seguridad de una cuenta de AWS. Recientemente, la clave de acceso de un usuario de IAM se subió por error a un repositorio de código público. El ingeniero de CloudOps debe identificar todo lo que fue cambiado usando esta clave de acceso. ¿Cómo debe el ingeniero de CloudOps cumplir con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para enviar todos los eventos de IAM a una función de AWS Lambda para su análisis.
- [ ] Consultar los registros de Amazon EC2 usando Amazon CloudWatch Logs Insights para todos los eventos iniciados con la clave de acceso comprometida dentro del período de tiempo sospechoso.
- [x] Buscar en el historial de eventos de AWS CloudTrail todos los eventos iniciados con la clave de acceso comprometida dentro del período de tiempo sospechoso.
- [ ] Buscar en los `VPC` Flow Logs todos los eventos iniciados con la clave de acceso comprometida dentro del período de tiempo sospechoso.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta un sitio web minorista en múltiples instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). La empresa debe asegurar el tráfico hacia el sitio web mediante una conexión `HTTPS`. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Adjuntar el certificado a cada instancia de EC2.
- [x] Adjuntar el certificado al `ALB`.
- [ ] Crear un certificado privado en AWS Certificate Manager (ACM).
- [x] Crear un certificado público en AWS Certificate Manager (ACM).
- [ ] Exportar el certificado y adjuntarlo al sitio web.

**[⬆ Volver arriba](#table-of-contents)**

### Si el navegador de la consola de administración de AWS no muestra que ha iniciado sesión en una cuenta de AWS, cierre el navegador y vuelva a abrir la consola usando el acceso directo de la consola de administración de AWS desde el escritorio de la VM. Si la funcionalidad de copiar y pegar no funciona en su entorno, consulte el archivo de instrucciones en el escritorio de la VM y use `Ctrl+C`, `Ctrl+V` o `Command-C`, `Command-V`. Configure Amazon EventBridge para cumplir con los siguientes requisitos. 1. Use la región `us-east-2` para todos los recursos. 2. A menos que se especifique lo contrario a continuación, use la configuración predeterminada. 3. Use su propia nomenclatura de recursos a menos que se especifique un nombre de recurso a continuación. 4. Asegúrese de que todos los eventos de Amazon EC2 en el bus de eventos predeterminado sean reproducibles (replayable) durante los últimos 90 días. 5. Cree una regla llamada `RunFunction` para enviar el mensaje exacto `{"name":"example"}` cada 15 minutos a una función de AWS Lambda existente llamada LogEventFunction. 6. Cree una regla llamada `SpotWarning` para enviar una notificación a un nuevo tema estándar de Amazon SNS llamado `TopicEvents` cada vez que se interrumpa una instancia Spot de Amazon EC2. NO cree ninguna suscripción al tema. La notificación debe coincidir con la siguiente estructura: `Input path: {instance: detail.instance-id} Input template: The EC2 Spot Instance <instance> has been interrupted.` Importante: Haga clic en el botón Next para completar este laboratorio y continuar al siguiente. Una vez que haga clic en el botón Next, NO podrá volver a este laboratorio.

![Question 210](images/question210.png)

- [x] 1. Haga clic en `Event pattern form` en `Event patterns`. 2. Seleccione `AWS service`. 3. En `Step 1: Create rule`, seleccione `Event Pattern` bajo `Event Source`. 4. Asegúrese de que esté seleccionado `Build event pattern to match events by service`. 5. Asegúrese de que `Service Name` tenga seleccionado `EC2`. 6. Asegúrese de que `Event Type` tenga seleccionado `EC2 Spot Instance Interruption Warning`. 7. Seleccione `SNS topic` bajo `Targets`. 8. Asegúrese de que `TopicEvents` tenga seleccionado `Topic`. 9. Haga clic en `Input Transformer` y asegúrese de tener `{"instance":"$.detail-instance-id"}`. 10. Escriba una descripción y haga clic en `Configure details`. 11. En `Step 2: Configure rule details`, cree 2 reglas: `RunFunction` y `SpotWarning`. 12. Asegúrese de que el `State` de las reglas esté configurado como `Enabled` en ese paso. 13. Valide en CloudWatch Events o EventBridge.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una carga de trabajo con estado (stateful) de larga duración en una única instancia de Amazon EC2 On-Demand de propósito general xlarge. Las métricas muestran que el servicio siempre está usando `80%` de su memoria disponible y `40%` de su CPU disponible. Un ingeniero de CloudOps debe reducir el costo del servicio sin afectar negativamente el rendimiento. ¿Qué cambio en el tipo de instancia cumplirá con estos requisitos?

- [ ] Cambiar a una instancia On-Demand large optimizada para cómputo.
- [x] Cambiar a una instancia On-Demand large optimizada para memoria.
- [ ] Cambiar a una instancia Spot xlarge de propósito general.
- [ ] Cambiar a dos instancias On-Demand large de propósito general.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación en instancias de Amazon EC2 que están en un grupo de Amazon EC2 Auto Scaling. Las acciones de escalado hacia afuera (scale-out) tardan mucho en completarse debido a scripts de arranque de larga duración. Un ingeniero de CloudOps debe implementar una solución para reducir el tiempo requerido para las acciones de scale-out sin sobreaprovisionar el grupo de Auto Scaling. ¿Qué solución cumple con estos requisitos?

- [ ] Cambiar la configuración de lanzamiento (launch configuration) para usar un tamaño de instancia mayor.
- [ ] Aumentar el número mínimo de instancias en el grupo de Auto Scaling.
- [ ] Agregar una política de escalado predictivo al grupo de Auto Scaling.
- [x] Agregar un warm pool al grupo de Auto Scaling.

**[⬆ Volver arriba](#table-of-contents)**

### Cuando la infraestructura de la nube de AWS experimenta un evento que puede afectar a una organización, ¿qué servicio de AWS se puede usar para ver cuáles recursos de la organización están afectados?

- [ ] AWS Service Health Dashboard.
- [ ] AWS Trusted Advisor.
- [x] AWS Personal Health Dashboard.
- [ ] AWS Systems Manager.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias de EC2 están en un grupo de Auto Scaling. La aplicación a veces se vuelve lenta y no responde. Las métricas de Amazon CloudWatch muestran que algunas instancias de EC2 están experimentando alta carga de CPU. Un ingeniero de CloudOps necesita crear un panel (dashboard) de CloudWatch que pueda mostrar automáticamente las métricas de CPU de todas las instancias de EC2. Las métricas deben incluir las nuevas instancias que se lancen como parte del grupo de Auto Scaling. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear un panel de CloudWatch. Usar notificaciones de actividad del grupo de Auto Scaling para invocar una función personalizada de AWS Lambda. Usar la función Lambda para actualizar el panel de CloudWatch y monitorear la métrica `CPUUtilization` de los nuevos ID de instancia.
- [ ] Crear un panel de CloudWatch. Ejecutar un script personalizado en cada instancia de EC2 para transmitir el uso de CPU al panel.
- [x] Usar CloudWatch metrics explorer para filtrar por la etiqueta `aws:autoscaling:groupName` y crear una visualización para la métrica `CPUUtilization`. Agregar la visualización a un panel de CloudWatch.
- [ ] Usar CloudWatch metrics explorer para filtrar por estado de instancia y crear una visualización para la métrica `CPUUtilization`. Agregar la visualización a un panel de CloudWatch.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está intentando configurar un nombre de dominio de Amazon Route 53 para enrutar tráfico a un sitio web alojado en Amazon S3. El nombre de dominio del sitio web es `www.example.com` y el nombre del bucket de S3 es `DOC-EXAMPLE-BUCKET`. Después de configurar el conjunto de registros en Route 53, el nombre de dominio `www.anycompany.com` no parece funcionar, y el sitio web estático no se muestra en el navegador. ¿Cuál de las siguientes es una causa de esto?

- [ ] El bucket de S3 debe configurarse primero con Amazon CloudFront.
- [ ] El conjunto de registros de Route 53 debe tener un rol de IAM que permita el acceso al bucket de S3.
- [ ] El conjunto de registros de Route 53 debe estar en la misma región que el bucket de S3.
- [x] El nombre del bucket de S3 debe coincidir con el nombre del conjunto de registros en Route 53.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha usado AWS CloudFormation para desplegar una aplicación sin servidor (serverless) en una `VPC` de producción. La aplicación consiste en una función de AWS Lambda, una tabla de Amazon DynamoDB y una API de Amazon API Gateway. El ingeniero de CloudOps debe eliminar el stack de AWS CloudFormation sin eliminar la tabla de DynamoDB. ¿Qué acción debe tomar el ingeniero de CloudOps antes de eliminar el stack de AWS CloudFormation?

- [x] Agregar una política de eliminación `Retain` al recurso de DynamoDB en el stack de AWS CloudFormation.
- [ ] Agregar una política de eliminación `Snapshot` al recurso de DynamoDB en el stack de AWS CloudFormation.
- [ ] Habilitar la protección contra terminación en el stack de AWS CloudFormation.
- [ ] Actualizar la política de IAM de la aplicación con una declaración `Deny` para la acción `dynamodb:DeleteTable`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps debe idear una estrategia para hacer cumplir el etiquetado de todas las instancias de EC2 y volúmenes de Amazon Elastic Block Store (Amazon EBS). ¿Qué acción puede tomar el ingeniero para implementar esto en tiempo real?

- [ ] Usar el AWS Tag Editor para buscar manualmente recursos sin etiquetar y luego etiquetarlos correctamente en el editor.
- [x] Configurar AWS Service Catalog con la regla de biblioteca `TagOptions` que hace cumplir una taxonomía de etiquetado proactivamente cuando se lanzan instancias y volúmenes.
- [ ] En un script de PowerShell o shell, verificar elementos sin etiquetar usando la acción de API de etiquetado de recursos `GetResources`, y luego etiquetar manualmente los elementos reportados.
- [ ] Lanzar elementos usando la API de AWS. Usar la acción de API `TagResources` para aplicar las etiquetas requeridas cuando se lancen las instancias y volúmenes.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación de negocio alojada en instancias de Amazon EC2 detrás de un Application Load Balancer. Las métricas de Amazon CloudWatch muestran que el uso de CPU en las instancias de EC2 es muy alto. También hay reportes de usuarios que reciben errores `HTTP` `503` y `504` al intentar conectarse a la aplicación. ¿Qué acción resolverá estos problemas?

- [x] Colocar las instancias de EC2 en un grupo de AWS Auto Scaling.
- [ ] Configurar el Target Group del `ALB` para usar verificaciones de salud más frecuentes.
- [ ] Habilitar sesiones persistentes (sticky sessions) en el Application Load Balancer.
- [ ] Aumentar la configuración de tiempo de espera inactivo (idle timeout) del Application Load Balancer.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps administra políticas para muchas cuentas miembro de AWS en una estructura de AWS Organizations. Ingenieros de otros equipos tienen acceso a las credenciales de usuario raíz de las cuentas miembro. El ingeniero de CloudOps debe impedir que todos los equipos, incluyendo sus administradores, usen Amazon DynamoDB. La solución no debe afectar la capacidad de los equipos para acceder a otros servicios de AWS. ¿Qué solución cumple con estos requisitos?

- [ ] En todas las cuentas miembro, configurar políticas de IAM que denieguen el acceso a todos los recursos de DynamoDB para todos los usuarios, incluyendo el usuario raíz.
- [x] Crear una Política de Control de Servicio (SCP) en la cuenta de administración para denegar todas las acciones de DynamoDB. Aplicar la SCP a la raíz de la organización.
- [ ] En todas las cuentas miembro, configurar políticas de IAM que denieguen `AmazonDynamoDBFullAccess` a todos los usuarios, incluyendo el usuario raíz.
- [ ] Eliminar la Política de Control de Servicio (SCP) predeterminada en la cuenta de administración. Crear una SCP de reemplazo que incluya una única declaración que deniegue todas las acciones de DynamoDB.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta cientos de instancias de Amazon EC2 en una única región de AWS. Cada instancia de EC2 tiene dos volúmenes adjuntos de Amazon Elastic Block Store (Amazon EBS) de 1 GiB `General Purpose SSD (gp2)`. Una carga de trabajo crítica está usando toda la capacidad de IOPS disponible en los volúmenes EBS. Según la política de la empresa, esta no puede cambiar los tipos de instancia ni los tipos de volumen EBS sin completar extensas pruebas de aceptación para validar que las aplicaciones de la empresa funcionarán correctamente. Un ingeniero de CloudOps necesita aumentar el rendimiento de E/S de los volúmenes EBS lo más rápido posible. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Aumentar el tamaño de los volúmenes EBS de 1 GiB.
- [ ] Agregar dos interfaces de red elásticas adicionales en cada instancia de EC2.
- [ ] Activar Transfer Acceleration en los volúmenes EBS de la región.
- [ ] Agregar todas las instancias de EC2 a un grupo de ubicación (placement group) de tipo cluster.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja su sitio web en instancias de Amazon EC2 en la región `us-east-1`. La empresa se está preparando para extender su sitio web a la región `eu-central-1`, pero la base de datos debe permanecer únicamente en `us-east-1`. Después del despliegue, las instancias de EC2 en `eu-central-1` no pueden conectarse a la base de datos en `us-east-1`. ¿Cuál es la solución MÁS eficiente operativamente que resolverá este problema de conectividad?

- [x] Crear una conexión de emparejamiento (peering) de `VPC` entre las dos regiones. Agregar el rango de direcciones IP privadas de las instancias a la regla de entrada del grupo de seguridad de la base de datos.
- [ ] Crear una conexión de emparejamiento de `VPC` entre las dos regiones. Agregar el grupo de seguridad de las instancias en `eu-central-1` a la regla de salida del grupo de seguridad de la base de datos.
- [ ] Crear una conexión `VPN` entre las dos regiones. Agregar el rango de direcciones IP privadas de las instancias a la regla de salida del grupo de seguridad de la base de datos.
- [ ] Crear una conexión `VPN` entre las dos regiones. Agregar el grupo de seguridad de las instancias en `eu-central-1` a la regla de entrada del grupo de seguridad de la base de datos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere crear una solución automatizada para todas las cuentas administradas por AWS Organizations que detecte cualquier grupo de seguridad que use `0.0.0.0/0` como dirección de origen para tráfico entrante. La empresa también quiere remediar automáticamente cualquier grupo de seguridad no conforme restringiendo el acceso a un bloque `CIDR` específico que corresponda con la intranet de la empresa. ¿Qué conjunto de acciones debe tomar el ingeniero de CloudOps para crear una solución?

- [x] Crear una regla de AWS Config para detectar grupos de seguridad no conformes. Configurar la remediación automática para cambiar la dirección de origen `0.0.0.0/0` al bloque `CIDR` aprobado.
- [ ] Crear una política de IAM para denegar la creación de grupos de seguridad que tengan `0.0.0.0/0` como dirección de origen. Adjuntar esta política de IAM a todos los usuarios de la empresa.
- [ ] Crear una función de AWS Lambda para inspeccionar grupos de seguridad nuevos y existentes. Verificar una dirección de origen `0.0.0.0/0` no conforme y cambiar la dirección de origen al bloque `CIDR` aprobado.
- [ ] Crear una Política de Control de Servicio (SCP) para la unidad organizacional (OU) que deniegue la creación de grupos de seguridad que tengan la dirección de origen `0.0.0.0/0`. Configurar la remediación automática para cambiar la dirección de origen `0.0.0.0/0` al bloque `CIDR` aprobado.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa requiere que toda la actividad en su cuenta de AWS se registre usando AWS CloudTrail. Además, un ingeniero de CloudOps debe saber cuándo se modifican o eliminan los archivos de registro de CloudTrail. ¿Cómo debe el ingeniero de CloudOps cumplir con estos requisitos?

- [x] Habilitar la validación de integridad de archivos de registro. Usar la AWS CLI para validar los archivos de registro.
- [ ] Habilitar la validación de integridad de archivos de registro. Usar la AWS CloudTrail Processing Library para validar los archivos de registro.
- [ ] Usar CloudTrail Insights para monitorear los archivos de registro en busca de modificaciones.
- [ ] Usar Amazon CloudWatch Logs para monitorear los archivos de registro en busca de modificaciones.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa planea alojar sus aplicaciones web con estado (stateful) en AWS. Un ingeniero de CloudOps está usando un grupo de Auto Scaling de instancias de Amazon EC2. Las aplicaciones web se ejecutarán las 24 horas del día, los 7 días de la semana, durante todo el año. La empresa debe poder cambiar el tipo de instancia dentro de la misma familia de instancias más adelante en el año según los patrones de tráfico y uso. ¿Qué opción de compra de instancias EC2 cumplirá con estos requisitos de la manera MÁS rentable?

- [x] Instancias Reservadas Convertibles.
- [ ] Instancias On-Demand.
- [ ] Instancias Spot.
- [ ] Instancias Reservadas Estándar.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación se ejecuta en instancias de Amazon EC2 en un grupo de Auto Scaling. Después de desplegar una nueva funcionalidad en las instancias de EC2, algunas instancias fueron marcadas como no saludables y luego reemplazadas por el grupo de Auto Scaling. Las instancias de EC2 se terminaron antes de que un ingeniero de CloudOps pudiera determinar la causa de los cambios de estado de salud. Para solucionar este problema, el ingeniero de CloudOps quiere asegurarse de que se invoque una función de AWS Lambda en esta situación. ¿Cómo debe el ingeniero de CloudOps cumplir con estos requisitos?

- [ ] Activar la configuración de protección contra reducción de escala (scale-in protection) de instancias para el grupo de Auto Scaling. Invocar la función Lambda a través de Amazon EventBridge (Amazon CloudWatch Events).
- [ ] Activar la configuración de protección contra reducción de escala de instancias para el grupo de Auto Scaling. Invocar la función Lambda a través de Amazon Route 53.
- [x] Agregar un lifecycle hook al grupo de Auto Scaling para invocar la función Lambda a través de Amazon EventBridge (Amazon CloudWatch Events).
- [ ] Agregar un lifecycle hook al grupo de Auto Scaling para invocar la función Lambda a través de Amazon Route 53.

**[⬆ Volver arriba](#table-of-contents)**


### Una empresa ejecuta una aplicación que aloja datos críticos para varios clientes. La empresa usa AWS CloudTrail para rastrear las actividades de los usuarios en varios recursos de AWS. Para cumplir con nuevos requisitos de seguridad, la empresa necesita proteger los archivos de registro de CloudTrail contra modificación, eliminación o falsificación. ¿Qué solución cumple con este requisito?

- [x] Habilitar la validación de integridad de archivos de registro de CloudTrail.
- [ ] Usar `MFA Delete` de Amazon S3 en el bucket de S3 donde se almacenan los archivos de registro de CloudTrail.
- [ ] Usar el versionado de Amazon S3 para conservar todas las versiones de los archivos de registro de CloudTrail.
- [ ] Usar claves de seguridad de AWS Key Management Service (AWS KMS) para asegurar los archivos de registro de CloudTrail.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa global opera desde cinco regiones de AWS. Un ingeniero de CloudOps quiere identificar todas las instancias de Amazon EC2 de la empresa, tanto etiquetadas como sin etiquetar. La empresa requiere que la salida muestre el ID de instancia y las etiquetas. ¿Cuál es la forma MÁS eficiente operativamente para que el ingeniero de CloudOps cumpla con estos requisitos?

- [ ] Crear un grupo de recursos basado en etiquetas en AWS Resource Groups.
- [ ] Usar AWS Trusted Advisor. Exportar los resultados de la verificación de instancias On-Demand de EC2 desde Trusted Advisor.
- [ ] Usar Cost Explorer. Elegir un tipo de servicio de EC2-Instances, y agrupar por recurso.
- [x] Usar Tag Editor en AWS Resource Groups. Seleccionar todas las regiones, y elegir un tipo de recurso `AWS::EC2::Instance`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa necesita subir gigabytes de archivos todos los días. La empresa necesita lograr mayor rendimiento y velocidades de carga hacia Amazon S3. ¿Qué acción debe tomar un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Crear una distribución de Amazon CloudFront con el método `HTTP` GET permitido y el bucket de S3 como origen.
- [ ] Crear un clúster de Amazon ElastiCache y habilitar el almacenamiento en caché para el bucket de S3.
- [ ] Configurar AWS Global Accelerator con el bucket de S3.
- [x] Habilitar S3 Transfer Acceleration y usar el endpoint de aceleración al subir archivos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps mantiene la seguridad y el cumplimiento normativo de la cuenta de AWS de una empresa. Para asegurar que las instancias de Amazon EC2 de la empresa sigan la política de la empresa, un ingeniero de CloudOps quiere terminar cualquier instancia de EC2 que no contenga una etiqueta de departamento. Los recursos no conformes deben terminarse casi en tiempo real. ¿Qué solución cumple con estos requisitos?

- [x] Crear una regla de AWS Config con la regla administrada `required-tags` para identificar recursos no conformes. Configurar la remediación automática para ejecutar el documento de automatización `TerminateEC2Instance` de AWS para terminar los recursos no conformes.
- [ ] Crear una nueva regla de Amazon EventBridge (Amazon CloudWatch Events) para monitorear cuándo se crean nuevas instancias de EC2. Enviar el evento a un tema de Simple Notification Service (Amazon SNS) para remediación automática.
- [ ] Asegurarse de que todos los usuarios que pueden crear instancias de EC2 también tengan los permisos para usar las acciones `ec2:CreateTags` y `ec2:DescribeTags`. Cambiar el comportamiento de apagado (shutdown behavior) de la instancia a terminate.
- [ ] Asegurarse de que AWS Systems Manager Compliance esté configurado para administrar las instancias de EC2. Llamar al documento de automatización AWS-StopEC2Instances para detener los recursos no conformes.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa subió los archivos de su sitio web a un bucket de Amazon S3 que tiene habilitado el versionado de S3. La empresa usa una distribución de Amazon CloudFront con el bucket de S3 como origen. La empresa modificó recientemente los archivos, pero los nombres de objeto permanecieron iguales. Los usuarios reportan que el contenido antiguo sigue apareciendo en el sitio web. ¿Cómo debe un ingeniero de CloudOps remediar este problema?

- [x] Crear una invalidación de CloudFront, y agregar la ruta de los archivos actualizados.
- [ ] Crear una URL firmada (signed URL) de CloudFront para actualizar cada objeto inmediatamente.
- [ ] Configurar un Origin Access Identity (OAI) de S3 para mostrar solo los archivos actualizados a los usuarios.
- [ ] Deshabilitar el versionado de S3 en el bucket de S3 para que los archivos actualizados puedan reemplazar a los antiguos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene dos redes `VPC` llamadas `VPC` A y `VPC` B. El bloque `CIDR` de `VPC` A es `10.0.0.0/16` y el bloque `CIDR` de `VPC` B es `172.31.0.0/16`. La empresa quiere establecer una conexión de emparejamiento (peering) de `VPC` llamada `pcx-12345` entre ambas `VPC`. ¿Qué reglas deben aparecer en la tabla de enrutamiento de `VPC` A después de la configuración? (Elija dos.)

- [x] `Destination`: `10.0.0.0/16`, `Target`: `Local`.
- [ ] `Destination`: `172.31.0.0/16`, `Target`: `Local`.
- [ ] `Destination`: `10.0.0.0/16`, `Target`: `pcx-12345`.
- [x] `Destination`: `172.31.0.0/16`, `Target`: `pcx-12345`.
- [ ] `Destination`: `10.0.0.0/16`, `Target`: `172.31.0.0/16`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa analiza datos de ventas para sus clientes. Los clientes suben archivos a uno de los buckets de Amazon S3 de la empresa, y se publica un mensaje en una cola de Amazon Simple Queue Service (Amazon SQS) que contiene el Amazon Resource Name (ARN) del objeto. Una aplicación que se ejecuta en una instancia de Amazon EC2 sondea la cola y procesa los mensajes. El tiempo de procesamiento depende del tamaño del archivo. Los clientes reportan retrasos en el procesamiento de sus archivos. Un ingeniero de CloudOps decide configurar Amazon EC2 Auto Scaling como primer paso. El ingeniero de CloudOps crea una Amazon Machine Image (AMI) basada en la instancia de EC2 existente. El ingeniero de CloudOps también crea una plantilla de lanzamiento (launch template) que hace referencia a la AMI. ¿Cómo debe el ingeniero de CloudOps configurar la política de Auto Scaling para mejorar el tiempo de respuesta?

- [ ] Agregar varios tamaños de instancia diferentes en la plantilla de lanzamiento. Crear una política de Auto Scaling basada en la métrica `ApproximateNumberOfMessagesVisible` para seleccionar el tamaño de la instancia según el número de mensajes en la cola.
- [ ] Crear una política de Auto Scaling basada en la métrica ApproximateNumberOfMessagesDelayed para escalar el número de instancias según el número de mensajes retrasados en la cola.
- [ ] Crear una métrica personalizada basada en la métrica `ASGAverageCPUUtilization` y la métrica GroupPendingInstances del grupo de Auto Scaling. Modificar la aplicación para calcular la métrica y publicarla en Amazon CloudWatch cada minuto. Crear una política de Auto Scaling basada en esta métrica para escalar el número de instancias.
- [x] Crear una métrica personalizada basada en la métrica `ApproximateNumberOfMessagesVisible` y el número de instancias en estado `InService` en el grupo de Auto Scaling. Modificar la aplicación para calcular la métrica y publicarla en Amazon CloudWatch cada minuto. Crear una política de Auto Scaling basada en esta métrica para escalar el número de instancias.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación web multicapa con dos instancias de Amazon EC2 en una Zona de disponibilidad en la región `us-east-1`. Un ingeniero de CloudOps debe migrar una de las instancias de EC2 a una nueva Zona de disponibilidad. ¿Qué solución logrará esto?

- [ ] Copiar la instancia de EC2 a una Zona de disponibilidad diferente. Terminar la instancia original.
- [x] Crear una Amazon Machine Image (AMI) a partir de la instancia de EC2 y lanzarla en una Zona de disponibilidad diferente. Terminar la instancia original.
- [ ] Mover la instancia de EC2 a una Zona de disponibilidad diferente usando la AWS CLI.
- [ ] Detener la instancia de EC2, modificar la Zona de disponibilidad, e iniciar la instancia.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere prohibir que sus desarrolladores usen una familia particular de instancias de Amazon EC2. La empresa usa AWS Organizations y quiere aplicar la restricción en múltiples cuentas. ¿Cuál es la forma MÁS eficiente operativamente para que la empresa aplique Políticas de Control de Servicio (SCP) y cumpla con estos requisitos?

- [x] Agregar las cuentas a una unidad organizacional (OU). Aplicar las SCP a la OU.
- [ ] Agregar las cuentas a grupos de recursos en AWS Resource Groups. Aplicar las SCP a los grupos de recursos.
- [ ] Aplicar las SCP a cada cuenta de desarrollador.
- [ ] Inscribir las cuentas en AWS Control Tower. Aplicar las SCP a la cuenta de administración de AWS Control Tower.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación se ejecuta en una instancia de Amazon EC2 en una `VPC` con el conjunto de opciones `DHCP` predeterminado. La aplicación se conecta a una base de datos Microsoft SQL Server local (on-premises) con el nombre `DNS` `mssql.example.com`. La aplicación no puede resolver el nombre `DNS` de la base de datos. ¿Qué solución solucionará este problema?

- [ ] Crear un endpoint de entrada (inbound) de Amazon Route 53 Resolver. Agregar una regla de reenvío para el dominio `example.com`. Asociar la regla de reenvío con la `VPC`.
- [ ] Crear un endpoint de entrada de Amazon Route 53 Resolver. Agregar una regla de sistema para el dominio `example.com`. Asociar la regla de sistema con la `VPC`.
- [x] Crear un endpoint de salida (outbound) de Amazon Route 53 Resolver. Agregar una regla de reenvío para el dominio `example.com`. Asociar la regla de reenvío con la `VPC`.
- [ ] Crear un endpoint de salida de Amazon Route 53 Resolver. Agregar una regla de sistema para el dominio `example.com`. Asociar la regla de sistema con la `VPC`.

**[⬆ Volver arriba](#table-of-contents)**

### La aplicación de una empresa está alojada por un proveedor de internet en `app.example.com`. La empresa quiere acceder a la aplicación usando `www.company.com`, que la empresa posee y administra con Amazon Route 53. ¿Qué registro de Route 53 se debe crear para lograr esto?

- [ ] Registro `A`.
- [ ] Registro `Alias`.
- [x] Registro `CNAME`.
- [ ] Registro `Pointer (PTR)`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa expandió su aplicación web para atender a una audiencia mundial. Un ingeniero de CloudOps ha implementado un despliegue de AWS multi-región para toda la infraestructura de producción. El ingeniero de CloudOps debe enrutar el tráfico según la ubicación de los recursos. ¿Qué política de enrutamiento de Amazon Route 53 debe usar el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Política de enrutamiento por geolocalización (Geolocation).
- [x] Política de enrutamiento por geoproximidad (Geoproximity).
- [ ] Política de enrutamiento basada en latencia (Latency-based).
- [ ] Política de enrutamiento de respuesta múltiple (Multivalue answer).

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo de aplicación está trabajando con un ingeniero de CloudOps para definir alarmas de Amazon CloudWatch para una aplicación. El equipo de aplicación no conoce el uso esperado ni el crecimiento esperado de la aplicación. ¿Qué solución debe recomendar el ingeniero de CloudOps?

- [x] Crear alarmas de CloudWatch basadas en detección de anomalías (anomaly detection).
- [ ] Crear alarmas de CloudWatch usando un conjunto de alarmas compuestas.
- [ ] Crear alarmas de CloudWatch usando umbrales estáticos.
- [ ] Crear alarmas de CloudWatch que traten los datos faltantes como incumplimiento (breaching).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa de comercio electrónico usa un clúster de Amazon ElastiCache for Memcached para el almacenamiento en caché en memoria de consultas de productos populares en el sitio de compras. Al revisar los datos recientes de métricas de Amazon CloudWatch para el clúster de ElastiCache, el ingeniero de CloudOps nota una gran cantidad de desalojos (evictions). ¿Cuál de las siguientes acciones reducirá estos desalojos? (Elija dos.)

- [x] Agregar un nodo adicional al clúster de ElastiCache.
- [ ] Aumentar el tiempo de vida (TTL) de ElastiCache.
- [x] Aumentar el tamaño de los nodos individuales dentro del clúster de ElastiCache.
- [ ] Colocar un Elastic Load Balancer delante del clúster de ElastiCache.
- [ ] Usar Amazon Simple Queue Service (Amazon SQS) para desacoplar el clúster de ElastiCache.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps quiere proporcionar acceso a servicios de AWS adjuntando una política de IAM a múltiples usuarios de IAM. El ingeniero de CloudOps también quiere poder cambiar la política y crear nuevas versiones. ¿Qué combinación de acciones cumple con estos requisitos? (Elija dos.)

- [ ] Agregar los usuarios a un rol vinculado a servicio (service-linked role) de IAM. Adjuntar la política al rol.
- [x] Agregar los usuarios a un grupo de usuarios de IAM. Adjuntar la política al grupo.
- [ ] Crear una política administrada por AWS.
- [x] Crear una política administrada por el cliente (customer managed policy).
- [ ] Crear una política en línea (inline policy).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa almacena datos críticos en buckets de Amazon S3. Un ingeniero de CloudOps debe construir una solución para registrar toda la actividad de la API de S3. ¿Qué acción cumplirá con este requisito?

- [ ] Configurar métricas del bucket de S3 para registrar los registros de acceso a objetos.
- [x] Crear un trail de AWS CloudTrail para registrar eventos de datos para todos los objetos de S3.
- [ ] Habilitar el registro de acceso del servidor (server access logging) de S3 para cada bucket de S3.
- [ ] Usar AWS IAM Access Analyzer para Amazon S3 para almacenar los registros de acceso a objetos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación que usa una base de datos MySQL en una instancia de Amazon EC2. La instancia de EC2 tiene un volumen de Amazon Elastic Block Store (Amazon EBS) General Purpose SSD. La empresa hizo cambios en el código de la aplicación y ahora quiere realizar pruebas de carga para evaluar el impacto de los cambios de código. Un ingeniero de CloudOps debe crear una nueva instancia de MySQL a partir de una instantánea de la instancia de producción existente. Esta nueva instancia debe funcionar de la manera más similar posible a la instancia de producción. ¿Qué opción de restauración cumple con estos requisitos?

- [x] Usar la restauración rápida de instantáneas (EBS fast snapshot restore) de EBS para crear un nuevo volumen `General Purpose SSD EBS` a partir de la instantánea de producción.
- [ ] Usar la restauración rápida de instantáneas de EBS para crear un nuevo volumen `Provisioned IOPS SSD EBS` a partir de la instantánea de producción.
- [ ] Usar la restauración de instantáneas de EBS para crear un nuevo volumen `General Purpose SSD EBS` a partir de la instantánea de producción.
- [ ] Usar la restauración de instantáneas de EBS para crear un nuevo volumen `Provisioned IOPS SSD EBS` a partir de la instantánea de producción.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa AWS Organizations para administrar sus cuentas de AWS. Un ingeniero de CloudOps debe crear una estrategia de respaldo para todas las instancias de Amazon EC2 en todas las cuentas de AWS de la empresa. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Desplegar una función de AWS Lambda en cada cuenta para ejecutar instantáneas de instancias de EC2 de forma programada.
- [ ] Crear un stack set de AWS CloudFormation en la cuenta de administración para agregar una etiqueta `AutoBackup=True` a cada instancia de EC2.
- [x] Usar AWS Backup en la cuenta de administración para desplegar políticas para todas las cuentas y recursos.
- [ ] Usar una Política de Control de Servicio (SCP) para ejecutar instantáneas de instancias de EC2 de forma programada en cada cuenta.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa necesita garantizar un cumplimiento estricto de un presupuesto para 25 aplicaciones desplegadas en AWS. Equipos separados son responsables de los costos de almacenamiento, cómputo y base de datos. Un ingeniero de CloudOps debe implementar una solución automatizada para alertar a cada equipo cuando su gasto proyectado exceda un monto trimestral establecido por el departamento de finanzas. La solución no puede incurrir en costos adicionales de cómputo, almacenamiento o base de datos. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar AWS Cost and Usage Reports para enviar un informe diario a un bucket de Amazon S3. Crear una función de AWS Lambda que evalúe el gasto por servicio y notifique a cada equipo usando notificaciones de Amazon Simple Notification Service (Amazon SNS). Invocar la función Lambda cuando se coloque un informe en el bucket de S3.
- [ ] Configurar AWS Cost and Usage Reports para enviar un informe diario a un bucket de Amazon S3. Crear una regla en Amazon EventBridge (Amazon CloudWatch Events) para evaluar el gasto por servicio y notificar a cada equipo usando Amazon Simple Queue Service (Amazon SQS) cuando se supere el umbral de costo.
- [ ] Usar AWS Budgets para crear un presupuesto de costos y seleccionar cada uno de los servicios en uso. Especificar el monto del presupuesto definido por el departamento de finanzas junto con el umbral de costo proyectado. Ingresar los destinatarios de correo electrónico apropiados para el presupuesto.
- [x] Usar AWS Budgets para crear un presupuesto de costos para cada equipo, filtrando por los servicios que poseen. Especificar el monto del presupuesto definido por el departamento de finanzas junto con un umbral de costo proyectado. Ingresar los destinatarios de correo electrónico apropiados para cada presupuesto.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja un sitio web estático en Amazon S3. Una distribución de Amazon CloudFront presenta este sitio a usuarios globales. La empresa usa la política de caché `Managed-CachingDisabled` de CloudFront. Los desarrolladores de la empresa confirman que actualizan con frecuencia un archivo en Amazon S3 con información nueva. Los usuarios reportan que el sitio web presenta la información correcta cuando el sitio carga el archivo por primera vez. Sin embargo, los navegadores de los usuarios no obtienen el archivo actualizado después de una actualización (refresh). ¿Qué debe recomendar un ingeniero de CloudOps para solucionar este problema?

- [x] Agregar un campo de encabezado `Cache-Control` con `max-age=0` al objeto de S3.
- [ ] Cambiar la política de caché de CloudFront a `Managed-CachingOptimized`.
- [ ] Deshabilitar el versionado del bucket en la configuración del bucket de S3.
- [ ] Habilitar la compresión de contenido en la configuración de CloudFront.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita eliminar un stack de AWS CloudFormation que ya no está en uso. El stack de CloudFormation está en el estado `DELETE_FAILED`. El ingeniero de CloudOps ha validado los permisos requeridos para eliminar el stack de CloudFormation. ¿Cuáles de las siguientes son posibles causas del estado `DELETE_FAILED`? (Elija dos.)

- [ ] El tiempo de espera (timeout) configurado para eliminar el stack era demasiado bajo para que se completara la operación de eliminación.
- [ ] El stack contiene stacks anidados (nested stacks) que deben eliminarse manualmente primero.
- [ ] El stack se desplegó con la opción `--disable-rollback`.
- [x] Hay recursos adicionales asociados con un grupo de seguridad en el stack.
- [x] Hay buckets de Amazon S3 en el stack que todavía contienen objetos.

**[⬆ Volver arriba](#table-of-contents)**

### Se requiere que un ingeniero de CloudOps monitoree el espacio libre en volúmenes de Amazon EBS adjuntos a instancias de Amazon EC2 basadas en Microsoft Windows dentro de la cuenta de una empresa. El ingeniero debe recibir alertas sobre posibles problemas. ¿Qué debe hacer el ingeniero para recibir alertas por correo electrónico antes de que el poco espacio de almacenamiento afecte el rendimiento de la instancia de EC2?

- [ ] Usar métricas integradas de Amazon CloudWatch, y configurar alarmas de CloudWatch y un tema de Amazon SNS para notificaciones por correo electrónico.
- [ ] Usar registros de AWS CloudTrail y configurar el trail para enviar notificaciones a un tema de Amazon SNS.
- [x] Usar el agente de Amazon CloudWatch para enviar métricas de espacio en disco, luego configurar alarmas de CloudWatch usando un tema de Amazon SNS.
- [ ] Usar AWS Trusted Advisor y habilitar alertas de notificación por correo electrónico para el espacio en disco de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene un grupo de Auto Scaling de instancias de Amazon EC2 que escala según el uso promedio de CPU. El registro de eventos del grupo de Auto Scaling indica un error `InsufficientInstanceCapacity`. ¿Qué acciones debe tomar un ingeniero de CloudOps para remediar este problema? (Elija dos.)

- [x] Cambiar el tipo de instancia que está usando la empresa.
- [x] Configurar el grupo de Auto Scaling en diferentes Zonas de disponibilidad.
- [ ] Configurar el grupo de Auto Scaling para usar diferentes tamaños de volumen de Amazon Elastic Block Store (Amazon EBS).
- [ ] Aumentar el tamaño máximo del grupo de Auto Scaling.
- [ ] Solicitar un aumento en la cuota de servicio de instancias.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita controlar el acceso a grupos de instancias de Amazon EC2 usando AWS Systems Manager Session Manager. Ya se han agregado etiquetas específicas a las instancias de EC2. ¿Qué acciones adicionales debe tomar el ingeniero para controlar el acceso? (Elija dos.)

- [x] Adjuntar una política de IAM a los usuarios o grupos que requieren acceso a las instancias de EC2.
- [ ] Adjuntar un rol de IAM para controlar el acceso a las instancias de EC2.
- [ ] Crear un grupo de ubicación (placement group) para las instancias de EC2 y agregar una etiqueta específica.
- [ ] Crear una cuenta de servicio y adjuntarla a las instancias de EC2 que necesitan ser controladas.
- [x] Crear una política de IAM que otorgue acceso a cualquier instancia de EC2 con una etiqueta especificada en el elemento `Condition`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una función de AWS Lambda en la Cuenta A. La función Lambda necesita leer los objetos en un bucket de Amazon S3 en la Cuenta B. Un ingeniero de CloudOps debe crear los roles de IAM correspondientes en ambas cuentas. ¿Qué solución cumple con estos requisitos?

- [x] En la Cuenta A, crear un rol de ejecución de Lambda para asumir el rol en la Cuenta B. En la Cuenta B, crear un rol que la función pueda asumir para obtener acceso al bucket de S3.
- [ ] En la Cuenta A, crear un rol de ejecución de Lambda que proporcione acceso al bucket de S3. En la Cuenta B, crear un rol que la función pueda asumir.
- [ ] En la Cuenta A, crear un rol que la función pueda asumir. En la Cuenta B, crear un rol de ejecución de Lambda que proporcione acceso al bucket de S3.
- [ ] En la Cuenta A, crear un rol que la función pueda asumir para obtener acceso al bucket de S3. En la Cuenta B, crear un rol de ejecución de Lambda para asumir el rol en la Cuenta A.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps quiere monitorear el espacio libre en disco disponible en un conjunto de instancias de Amazon EC2 que tienen volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos. El ingeniero de CloudOps quiere recibir una notificación cuando el espacio de disco usado de los volúmenes EBS supere un valor umbral, pero solo cuando la métrica `DiskReadOps` también supere un valor umbral. El ingeniero de CloudOps ha configurado un tema de Amazon Simple Notification Service (Amazon SNS). ¿Cómo puede el ingeniero de CloudOps recibir la notificación solo cuando ambas métricas superen sus valores umbral?

- [x] Instalar el agente de Amazon CloudWatch en las instancias de EC2. Crear una alarma de métrica para el espacio en disco y una alarma de métrica para la métrica `DiskReadOps`. Crear una alarma compuesta que incluya las dos alarmas de métrica para publicar una notificación en el tema de SNS.
- [ ] Instalar el agente de Amazon CloudWatch en las instancias de EC2. Crear una alarma de métrica para el espacio en disco y una alarma de métrica para la métrica `DiskReadOps`. Configurar cada alarma para publicar una notificación en el tema de SNS.
- [ ] Crear una alarma de métrica para la métrica `EBSByteBalance%` y una alarma de métrica para la métrica `DiskReadOps`. Crear una alarma compuesta que incluya las dos alarmas de métrica para publicar una notificación en el tema de SNS.
- [ ] Configurar el monitoreo detallado para las instancias de EC2. Crear una alarma de métrica para el espacio en disco y una alarma de métrica para la métrica `DiskReadOps`. Crear una alarma compuesta que incluya las dos alarmas de métrica para publicar una notificación en el tema de SNS.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa Amazon CloudFront para servir contenido estático de su aplicación web a sus usuarios. La distribución de CloudFront usa un sitio web local (on-premises) existente como origen personalizado. La empresa requiere el uso de TLS entre CloudFront y el servidor de origen. Esta configuración ha funcionado como se esperaba durante varios meses. Sin embargo, los usuarios ahora están experimentando errores `HTTP 502 (Bad Gateway)` al ver páginas web que incluyen contenido de la distribución de CloudFront. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?

- [x] Examinar la fecha de vencimiento del certificado en el sitio de origen. Validar que el certificado no haya expirado. Reemplazar el certificado si es necesario.
- [ ] Examinar el nombre de host en el certificado en el sitio de origen. Validar que el nombre de host coincida con uno de los nombres de host en la distribución de CloudFront. Reemplazar el certificado si es necesario.
- [ ] Examinar las reglas de firewall asociadas con el servidor de origen. Validar que el puerto `443` esté abierto para tráfico entrante desde internet. Crear una regla de entrada si es necesario.
- [ ] Examinar las reglas de `ACL` de red asociadas con la distribución de CloudFront. Validar que el puerto `443` esté abierto para tráfico de salida hacia el servidor de origen. Crear una regla de salida si es necesario.

**[⬆ Volver arriba](#table-of-contents)**

### Una distribución de Amazon CloudFront tiene un único bucket de Amazon S3 como su origen. Un ingeniero de CloudOps debe asegurarse de que los usuarios solo puedan acceder al bucket de S3 a través de solicitudes provenientes del endpoint de CloudFront. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar S3 Block Public Access en el bucket de S3. Actualizar la política del bucket de S3 para permitir la acción `GetObject` únicamente desde la distribución de CloudFront.
- [ ] Configurar Origin Shield en la distribución de CloudFront. Actualizar el origen de CloudFront para incluir un encabezado personalizado `Origin_Shield`.
- [x] Crear una Origin Access Identity (OAI). Asignar la OAI a la distribución de CloudFront. Actualizar la política del bucket de S3 para restringir el acceso a la OAI.
- [ ] Crear una Origin Access Identity (OAI). Asignar la OAI al bucket de S3. Actualizar el origen de CloudFront para incluir un encabezado personalizado `Origin` con el valor de la OAI.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está diseñando una solución para una instancia de base de datos de Amazon RDS para PostgreSQL. Las credenciales de la base de datos deben almacenarse y rotarse mensualmente. Las aplicaciones que se conectan a la instancia de base de datos envían tráfico intensivo en escritura con conexiones de cliente variables que a veces aumentan significativamente en un corto período de tiempo. ¿Qué solución debe elegir un ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Configurar AWS Key Management Service (AWS KMS) para rotar automáticamente las claves de la instancia de base de datos. Usar RDS Proxy para manejar los aumentos en las conexiones a la base de datos.
- [ ] Configurar AWS Key Management Service (AWS KMS) para rotar automáticamente las claves de la instancia de base de datos. Usar réplicas de lectura de RDS para manejar los aumentos en las conexiones a la base de datos.
- [x] Configurar AWS Secrets Manager para rotar automáticamente las credenciales de la instancia de base de datos. Usar RDS Proxy para manejar los aumentos en las conexiones a la base de datos.
- [ ] Configurar AWS Secrets Manager para rotar automáticamente las credenciales de la instancia de base de datos. Usar réplicas de lectura de RDS para manejar los aumentos en las conexiones a la base de datos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere reducir costos para trabajos que se pueden completar en cualquier momento. Los trabajos actualmente se ejecutan usando múltiples instancias de Amazon EC2 On-Demand y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier motivo, debe reiniciarse desde el principio. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?

- [ ] Comprar Instancias Reservadas para los trabajos.
- [ ] Enviar una solicitud de Instancia Spot única (one-time) para los trabajos.
- [x] Enviar una solicitud de Instancias Spot con una duración definida para los trabajos.
- [ ] Usar una combinación de Instancias On-Demand e Instancias Spot para los trabajos.

**[⬆ Volver arriba](#table-of-contents)**

### Un entorno consta de 100 instancias de Amazon EC2 Windows. El agente de Amazon CloudWatch está desplegado y ejecutándose en todas las instancias de EC2 con un archivo de configuración base para capturar archivos de registro. Existe un nuevo requisito para capturar los archivos de registro `DHCP` que existen en 50 de las instancias. ¿Cuál es la forma MÁS eficiente operativamente para cumplir con este nuevo requisito?

- [x] Crear un archivo de configuración adicional del agente de CloudWatch para capturar los registros `DHCP`. Usar AWS Systems Manager Run Command para reiniciar el agente de CloudWatch en cada instancia de EC2 con la opción `append-config` para aplicar el archivo de configuración adicional.
- [ ] Iniciar sesión en cada instancia de EC2 con derechos de administrador. Crear un script de PowerShell para enviar los archivos de registro base necesarios y los archivos de registro `DHCP` a CloudWatch.
- [ ] Ejecutar el asistente del archivo de configuración del agente de CloudWatch en cada instancia de EC2. Verificar que los archivos de registro base estén incluidos y agregar los archivos de registro `DHCP` durante el proceso de creación del asistente.
- [ ] Ejecutar el asistente del archivo de configuración del agente de CloudWatch en cada instancia de EC2 y seleccionar el nivel de detalle avanzado. Esto capturará los archivos de registro del sistema operativo.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa necesita monitorear la utilización de disco de volúmenes de Amazon Elastic Block Store (Amazon EBS). Los volúmenes EBS están adjuntos a instancias de Amazon EC2 Linux. Un ingeniero de CloudOps debe configurar una alarma de Amazon CloudWatch que emita una alerta cuando la utilización de disco aumente a más del `80%`. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija tres.)

- [x] Crear un rol de IAM que incluya la política administrada de AWS `CloudWatchAgentServerPolicy`. Adjuntar el rol a las instancias.
- [ ] Crear un rol de IAM que incluya la política administrada de AWS `CloudWatchApplicationInsightsReadOnlyAccess`. Adjuntar el rol a las instancias.
- [x] Instalar e iniciar el agente de CloudWatch usando AWS Systems Manager o la línea de comandos.
- [ ] Instalar e iniciar el agente de CloudWatch usando un rol de IAM. Adjuntar la política administrada de AWS `CloudWatchAgentServerPolicy` al rol.
- [x] Configurar una alarma de CloudWatch para que entre en estado `ALARM` cuando la métrica de CloudWatch `disk_used_percent` sea mayor que `80%`.
- [ ] Configurar una alarma de CloudWatch para que entre en estado `ALARM` cuando la métrica de CloudWatch `disk_used` sea mayor que `80%` o cuando la métrica de CloudWatch `disk_free` sea menor que `20%`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa mantiene un gran conjunto de datos sensibles en un bucket de Amazon S3. El equipo de seguridad de la empresa le pide a un ingeniero de CloudOps que ayude a verificar que todos los objetos actuales en el bucket de S3 estén cifrados. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear un script que se ejecute contra el bucket de S3 y muestre el estado de cada objeto.
- [x] Crear una configuración de S3 Inventory en el bucket de S3. Incluir los campos de estado apropiados.
- [ ] Proporcionar al equipo de seguridad un usuario de IAM con acceso de lectura al bucket de S3.
- [ ] Usar la AWS CLI para mostrar una lista de todos los objetos en el bucket de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps administra una aplicación web que se ejecuta en instancias de Amazon EC2 detrás de un ELB Application Load Balancer (ALB). Las instancias se ejecutan en un grupo de EC2 Auto Scaling. El ingeniero quiere establecer una alarma para cuando todas las instancias de destino asociadas con el `ALB` estén no saludables. ¿Qué condición se debe usar con la alarma?

- [x] `AWS/ApplicationELB HealthyHostCount <= 0`.
- [ ] `AWS/ApplicationELB UnhealthyHostCount >= 1`.
- [ ] `AWS/EC2 StatusCheckFailed <= 0`.
- [ ] `AWS/EC2 StatusCheckFailed >= 1`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere monitorear los grupos de seguridad de sus instancias de Amazon EC2 para asegurarse de que `SSH` no esté abierto al público. Si el puerto está abierto, la empresa necesita cerrarlo lo antes posible. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Agregar una alarma de Amazon CloudWatch para detectar los grupos de seguridad que permiten `SSH`.
- [x] Agregar una regla de AWS Config para detectar los grupos de seguridad que permiten `SSH`.
- [ ] Agregar una plantilla de evaluación a Amazon Inspector para detectar los grupos de seguridad que permiten `SSH`.
- [x] Llamar a un runbook de AWS Systems Manager Automation para cerrar el puerto.
- [ ] Llamar a AWS Systems Manager Run Command para cerrar el puerto.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que se ejecuta en instancias de Amazon EC2 en una `VPC`. La aplicación necesita acceso para descargar actualizaciones de software desde internet. La `VPC` tiene subredes públicas y subredes privadas. La política de seguridad de la empresa requiere que todas las instancias de EC2 se desplieguen en subredes privadas. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Agregar una puerta de enlace de internet a la `VPC`. En la tabla de enrutamiento de las subredes privadas, agregar una ruta a la puerta de enlace de internet.
- [ ] Agregar una puerta de enlace `NAT` a una subred privada. En la tabla de enrutamiento de las subredes privadas, agregar una ruta a la puerta de enlace `NAT`.
- [x] Agregar una puerta de enlace `NAT` a una subred pública. En la tabla de enrutamiento de las subredes privadas, agregar una ruta a la puerta de enlace `NAT`.
- [ ] Agregar dos puertas de enlace de internet a la `VPC`. En las tablas de enrutamiento de las subredes privadas y subredes públicas, agregar una ruta a cada puerta de enlace de internet.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha configurado una nueva instancia de Amazon EC2 como servidor web en una subred pública. La instancia usa el puerto `80` de `HTTP` y el puerto `443` de `HTTPS`. El ingeniero de CloudOps ha confirmado la conectividad a internet descargando actualizaciones del sistema operativo y software desde repositorios públicos. Sin embargo, el ingeniero de CloudOps no puede acceder a la instancia desde un navegador web en internet. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para solucionar este problema? (Elija tres.)

- [x] Asegurarse de que las reglas de entrada del grupo de seguridad de la instancia permitan tráfico en los puertos `80` y `443`.
- [ ] Asegurarse de que las reglas de salida del grupo de seguridad de la instancia permitan tráfico en los puertos `80` y `443`.
- [ ] Asegurarse de que los puertos efímeros `1024-65535` estén permitidos en las reglas de entrada de la `ACL` de red asociada con la subred de la instancia.
- [x] Asegurarse de que los puertos efímeros `1024-65535` estén permitidos en las reglas de salida de la `ACL` de red asociada con la subred de la instancia.
- [x] Asegurarse de que las reglas de filtrado de cualquier firewall que se ejecute en la instancia permitan tráfico entrante en los puertos `80` y `443`.
- [ ] Asegurarse de que AWS WAF esté activado para la instancia y esté bloqueando el tráfico web.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa realizó recientemente una auditoría de seguridad de todas sus aplicaciones internas desarrolladas internamente. Ciertas aplicaciones críticas para el negocio que manejan datos sensibles fueron marcadas porque usan clústeres de Amazon ES que están abiertos para lectura/escritura a un grupo de usuarios más amplio del previsto. ¿Quién es responsable de corregir el problema?

- [ ] AWS Premium Support.
- [ ] El equipo de Amazon ES.
- [ ] El equipo de AWS IAM.
- [x] El ingeniero de CloudOps.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha desplegado una aplicación en AWS. La aplicación se ejecuta en una flota de instancias de Amazon EC2 Linux que están en un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para usar plantillas de lanzamiento (launch templates). Las plantillas de lanzamiento lanzan instancias de EC2 respaldadas por Amazon Elastic Block Store (Amazon EBS) que usan volúmenes EBS `General Purpose SSD (gp3)` para almacenamiento primario. Un ingeniero de CloudOps necesita implementar una solución para asegurar que todas las instancias de EC2 puedan compartir los mismos archivos subyacentes. La solución también debe asegurar que los datos sean consistentes. ¿Qué solución cumple con estos requisitos?

- [x] Crear un sistema de archivos de Amazon Elastic File System (Amazon EFS). Crear una nueva versión de la plantilla de lanzamiento que incluya datos de usuario (user data) que monten el sistema de archivos EFS. Actualizar el grupo de Auto Scaling para usar la nueva versión de la plantilla de lanzamiento a fin de ciclar instancias de EC2 más nuevas y terminar las instancias de EC2 más antiguas.
- [ ] Habilitar Multi-Attach en los volúmenes EBS. Crear una nueva versión de la plantilla de lanzamiento que incluya datos de usuario que monten el volumen EBS. Actualizar el grupo de Auto Scaling para usar la nueva versión de la plantilla a fin de ciclar instancias de EC2 más nuevas y terminar las instancias de EC2 más antiguas.
- [ ] Crear un cron job que sincronice los datos entre los volúmenes EBS para todas las instancias de EC2 en el grupo de Auto Scaling. Crear un lifecycle hook durante el lanzamiento de instancias para configurar el cron job en todas las instancias de EC2. Rotar las instancias de EC2 más antiguas.
- [ ] Crear una nueva versión de la plantilla de lanzamiento que cree un sistema de archivos de Amazon Elastic File System (Amazon EFS). Actualizar el grupo de Auto Scaling para usar la nueva versión de la plantilla a fin de ciclar instancias de EC2 más nuevas y terminar las instancias de EC2 más antiguas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja una aplicación en instancias de Amazon EC2. Las instancias están en un grupo de Amazon EC2 Auto Scaling que usa una plantilla de lanzamiento. La cantidad de tráfico de la aplicación cambia a lo largo del día. Los eventos de escalado ocurren con frecuencia. Un ingeniero de CloudOps necesita ayudar a los desarrolladores a solucionar problemas de la aplicación. Cuando un evento de escalado elimina una instancia, EC2 Auto Scaling termina la instancia antes de que los desarrolladores puedan iniciar sesión en la instancia para diagnosticar problemas. ¿Qué solución evitará la terminación de la instancia para que los desarrolladores puedan iniciar sesión en ella?

- [ ] Asegurarse de que la configuración Delete on termination esté desactivada en la sección `UserData` de la plantilla de lanzamiento.
- [x] Actualizar el grupo de Auto Scaling habilitando la protección contra reducción de escala (scale-in protection) de instancias para las instancias recién lanzadas.
- [ ] Usar Amazon Inspector para configurar un paquete de reglas que proteja a las instancias de la terminación.
- [ ] Usar Amazon GuardDuty para configurar reglas que protejan a las instancias de la terminación.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación que se ejecuta en instancias de Amazon EC2 en un grupo de Auto Scaling en múltiples Zonas de disponibilidad se desplegó usando una plantilla de AWS CloudFormation. El equipo de SysOps ha parcheado la versión de la Amazon Machine Image (AMI) y debe actualizar todas las instancias de EC2 para usar la nueva AMI. ¿Cómo puede el ingeniero de CloudOps usar CloudFormation para aplicar la nueva AMI mientras mantiene un nivel mínimo de instancias activas para garantizar la continuidad del servicio?

- [ ] Ejecutar el comando `update-stack` de aws cloudformation con la opción `rollback-configuration`.
- [ ] Actualizar la plantilla de CloudFormation con el nuevo ID de AMI, luego reiniciar las instancias de EC2.
- [ ] Desplegar un segundo stack de CloudFormation y usar Amazon Route 53 para redirigir el tráfico al nuevo stack.
- [x] Establecer una política `AutoScalingRollingUpdate` en la plantilla de CloudFormation para actualizar el stack.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja una aplicación interna en instancias de Amazon EC2 On-Demand detrás de un Application Load Balancer (ALB). Las instancias están en un grupo de Amazon EC2 Auto Scaling. Los empleados usan la aplicación para proporcionar precios de productos a clientes potenciales. El grupo de Auto Scaling está configurado con una política de escalado dinámico y rastrea el uso promedio de CPU de las instancias. Los empleados han notado que a veces la aplicación se vuelve lenta o no responde. Un ingeniero de CloudOps descubre que algunas instancias están experimentando una alta carga de CPU. El grupo de Auto Scaling no puede escalar hacia afuera porque la empresa está alcanzando la cuota de servicio de instancias de EC2. El ingeniero de CloudOps necesita implementar una solución que proporcione una notificación cuando la empresa alcance el `70%` o más de la cuota de servicio de instancias de EC2. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear una función de AWS Lambda que liste las instancias de EC2, cuente las instancias de EC2, y compare el número total con el valor de cuota aplicado usando la API de Service Quotas. Configurar la función Lambda para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) si la utilización de la cuota es igual o mayor al `70%`. Crear una regla de Amazon EventBridge para invocar la función Lambda.
- [ ] Crear una función de AWS Lambda que liste las instancias de EC2, cuente las instancias de EC2, y compare el número total con el valor de cuota aplicado usando la API de Amazon CloudWatch Metrics. Configurar la función Lambda para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) si la utilización de la cuota es igual o mayor al `70%`. Crear una regla de Amazon EventBridge para invocar la función Lambda.
- [x] Usar la consola de Service Quotas para crear una alarma de Amazon CloudWatch para las instancias de EC2. Configurar la alarma con una utilización de cuota igual o mayor al `70%`. Configurar la alarma para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) cuando la alarma entre en estado `ALARM`.
- [ ] Crear una alarma de Amazon CloudWatch. Configurar la alarma con un umbral del `70%` para la métrica `CPUUtilization` de las instancias de EC2. Configurar la alarma para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) cuando la alarma entre en estado `ALARM`.

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo de desarrolladores usa varios buckets de Amazon S3 como repositorios centralizados. Usuarios de todo el mundo suben grandes conjuntos de archivos a estos repositorios. Las aplicaciones del equipo de desarrollo procesan estos archivos posteriormente. Un ingeniero de CloudOps configura un nuevo bucket de S3, `DOC-EXAMPLE-BUCKET`, para soportar una nueva carga de trabajo. El nuevo bucket de S3 también recibe cargas regulares de grandes conjuntos de archivos de usuarios de todo el mundo. Cuando el nuevo bucket de S3 entra en producción, el rendimiento de carga desde ciertas áreas geográficas es menor que el rendimiento de carga que proporcionan los buckets de S3 existentes. ¿Qué debe hacer el ingeniero de CloudOps para remediar este problema?

- [ ] Aprovisionar un clúster de Amazon ElastiCache for Redis para el nuevo bucket de S3. Proporcionar a los desarrolladores el endpoint de configuración del clúster para usar en sus llamadas de API.
- [ ] Agregar el nuevo bucket de S3 a una nueva distribución de Amazon CloudFront. Proporcionar a los desarrolladores el nombre de dominio de la nueva distribución para usar en sus llamadas de API.
- [x] Habilitar S3 Transfer Acceleration para el nuevo bucket de S3. Verificar que los desarrolladores estén usando el nombre de endpoint `DOC-EXAMPLE-BUCKET.s3-accelerate.amazonaws.com` en sus llamadas de API.
- [ ] Usar la carga multiparte (multipart upload) de S3 para el nuevo bucket de S3. Verificar que los desarrolladores estén usando nombres de endpoint de S3 específicos de la región, como `DOC-EXAMPLE-BUCKETS3`, `[Region] amazonaws.com`, en sus llamadas de API.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps quiere usar AWS Systems Manager Patch Manager para automatizar el proceso de aplicar parches a instancias de Amazon EC2 Windows. El ingeniero de CloudOps quiere asegurarse de que los parches se aprueben automáticamente 2 días después de la fecha de lanzamiento para las instancias de desarrollo. Los parches también deben aprobarse automáticamente 5 días después de la fecha de lanzamiento para las instancias de producción. El mantenimiento debe ocurrir solo durante una ventana de 2 horas para todas las instancias. ¿Qué solución cumple con estos requisitos?

- [ ] Usar etiquetas para identificar las instancias de desarrollo y producción. En Patch Manager, crear dos grupos de parches y una línea base de parches. Agregar un retraso de aprobación automática a cada grupo de parches. Crear una única ventana de mantenimiento.
- [x] Usar etiquetas para identificar las instancias de desarrollo y producción. En Patch Manager, crear dos grupos de parches y dos líneas base de parches. Especificar un retraso de aprobación automática en cada una de las líneas base de parches. Crear una única ventana de mantenimiento.
- [ ] Usar etiquetas para identificar las instancias de desarrollo y producción. En Patch Manager, crear dos grupos de parches y una línea base de parches. Crear dos ventanas de mantenimiento separadas, cada una con un retraso de aprobación automática.
- [ ] Usar etiquetas para identificar las instancias de desarrollo. En Patch Manager, crear un grupo de parches y una línea base de parches. Especificar retrasos de aprobación automática en la línea base de parches. Agregar las instancias de desarrollo al nuevo grupo de parches. Usar líneas base de parches predefinidas de Patch Manager para todas las instancias restantes. Crear una única ventana de mantenimiento.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene usuarios que despliegan instancias de Amazon EC2 con más capacidad de rendimiento de disco de la requerida. Un ingeniero de CloudOps necesita revisar todos los volúmenes de Amazon Elastic Block Store (Amazon EBS) asociados con las instancias y crear recomendaciones de optimización de costos basadas en IOPS y rendimiento (throughput). ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Usar los gráficos de monitoreo en la consola de EC2 para ver las métricas de los volúmenes EBS. Revisar el espacio consumido contra el espacio aprovisionado en cada volumen. Identificar cualquier volumen que tenga baja utilización.
- [ ] Detener las instancias de EC2 desde la consola de EC2. Cambiar el tipo de instancia de EC2 a uno optimizado para Amazon EBS. Iniciar las instancias de EC2.
- [x] Habilitar AWS Compute Optimizer. Permitir tiempo suficiente para que se recopilen las métricas. Revisar los hallazgos de Compute Optimizer para los volúmenes EBS.
- [ ] Instalar la herramienta `fio` en las instancias de EC2 y crear un archivo `.cfg` para aproximar las cargas de trabajo requeridas. Usar los resultados del benchmark para evaluar si los volúmenes EBS aprovisionados son del tipo más apropiado.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita aprovisionar una nueva flota de instancias Spot de Amazon EC2 en un grupo de Amazon EC2 Auto Scaling. El grupo de Auto Scaling usará una amplia variedad de tipos de instancia. La flota configurada debe provenir de los pools que tengan la mayor disponibilidad para el número de instancias que se lancen. ¿Qué solución cumple con estos requisitos?

- [ ] Lanzar las instancias Spot hasta la capacidad máxima del grupo de Auto Scaling.
- [ ] Lanzar las instancias Spot usando la estrategia diversificada (diversified).
- [x] Lanzar las instancias Spot usando la estrategia de optimización de capacidad (capacity optimized).
- [ ] Usar el Spot Instance advisor para ayudar a determinar la mejor estrategia de asignación Spot.

**[⬆ Volver arriba](#table-of-contents)**

### Los usuarios reportan cierres de sesión forzados constantes en una aplicación web con estado (stateful). Los cierres de sesión ocurren antes de la expiración de un temporizador de cierre de sesión de la aplicación de 15 minutos. La aplicación web está alojada en instancias de Amazon EC2 que están en un grupo de Auto Scaling. Las instancias se ejecutan detrás de un Application Load Balancer (ALB) que tiene un único grupo de destino (target group). El `ALB` está configurado como el origen en una distribución de Amazon CloudFront. La afinidad de sesión (sticky sessions) ya está habilitada en el grupo de destino del `ALB` y usa cookies basadas en duración. La aplicación web genera su propia cookie de aplicación. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para resolver el problema de cierre de sesión? (Elija dos.)

- [ ] Cambiar al algoritmo de solicitudes pendientes mínimas (least outstanding requests) en el grupo de destino del `ALB`.
- [x] Configurar el reenvío de cookies (cookie forwarding) en la configuración de comportamiento de caché de la distribución de CloudFront.
- [ ] Configurar la cookie basada en duración para que se llame AWSALB.
- [ ] Configurar el `ALB` para usar el encabezado de cookie de expiración.
- [x] Cambiar el `ALB` para usar cookies basadas en la aplicación.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación web pública que experimenta aumentos rápidos de tráfico después de que aparecen anuncios en la televisión local. La aplicación se ejecuta en instancias de Amazon EC2 que están en un grupo de Auto Scaling. El grupo de Auto Scaling no logra mantener el ritmo del tráfico después de que se transmite un anuncio. La empresa a menudo necesita escalar hasta 100 instancias de EC2 durante los aumentos de tráfico. Los tiempos de inicio de las instancias son largos debido a un proceso de arranque que crea cachés de datos específicos de la máquina, únicos para cada instancia. No se sabe el momento exacto en que aparecerán los anuncios en televisión. Un ingeniero de CloudOps debe implementar una solución para que la aplicación pueda funcionar correctamente durante los aumentos de tráfico. ¿Qué solución cumple con estos requisitos?

- [x] Crear un warm pool. Mantener suficientes instancias en estado `Stopped` para satisfacer la demanda aumentada.
- [ ] Iniciar 100 instancias. Permitir que el proceso de arranque termine de ejecutarse. Almacenar estos datos en el volumen de instance store antes de detener las instancias.
- [ ] Aumentar el valor del tiempo de calentamiento (warmup time) de instancia en la política de escalado.
- [ ] Usar escalado predictivo para el grupo de Auto Scaling.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja un servidor de archivos basado en Windows en una flota de instancias de Amazon EC2 en múltiples Zonas de disponibilidad. La configuración actual no permite que los servidores de aplicaciones accedan a los archivos simultáneamente desde la flota de EC2. ¿Qué solución permitirá este acceso de la manera MÁS eficiente operativamente?

- [ ] Crear un sistema de archivos de Amazon Elastic File System (Amazon EFS) Multi-AZ. Copiar los archivos al sistema de archivos EFS. Conectar el sistema de archivos EFS a puntos de montaje en los servidores de aplicaciones.
- [x] Crear un sistema de archivos de Amazon FSx for Windows File Server Multi-AZ. Copiar los archivos al sistema de archivos Amazon FSx. Ajustar las conexiones de los servidores de aplicaciones para usar el recurso compartido (share) que expone el sistema de archivos Amazon FSx.
- [ ] Crear un volumen de Amazon Elastic Block Store (Amazon EBS) con EBS Multi-Attach habilitado. Crear un grupo de Auto Scaling para el servidor de archivos Windows. Usar un script en los datos de usuario del servidor de archivos para adjuntar la etiqueta SharedFileAccess al volumen EBS durante el lanzamiento.
- [ ] Crear dos sistemas de archivos de Amazon FSx for Windows File Server. Configurar la replicación de Distributed File System (DFS) entre los sistemas de archivos. Copiar los archivos a los sistemas de archivos Amazon FSx. Ajustar las conexiones de los servidores de aplicaciones para usar los recursos compartidos que exponen los sistemas de archivos Amazon FSx.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa desplegó recientemente una aplicación en producción. El entorno de producción actualmente se ejecuta en una única instancia de Amazon EC2 que aloja la aplicación web y una base de datos MariaDB. La política de la empresa establece que todos los entornos de producción de TI deben ser de alta disponibilidad. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [x] Migrar la base de datos desde la instancia de EC2 a una instancia de base de datos de Amazon RDS para MariaDB Multi-AZ. Ejecutar la aplicación en instancias de EC2 que estén en un grupo de Auto Scaling que se extienda a través de múltiples Zonas de disponibilidad. Colocar las instancias de EC2 detrás de un balanceador de carga.
- [ ] Migrar la base de datos desde la instancia de EC2 a una instancia de base de datos de Amazon RDS para MariaDB Multi-AZ. Usar AWS Application Migration Service para convertir la aplicación en una función de AWS Lambda. Especificar la opción Multi-AZ para la función Lambda.
- [ ] Copiar la base de datos a una instancia de EC2 diferente en una Zona de disponibilidad diferente. Usar AWS Backup para crear Amazon Machine Images (AMI) de la instancia de EC2 de la aplicación y la instancia de EC2 de la base de datos. Crear una función de AWS Lambda que realice verificaciones de salud cada minuto. En caso de falla, configurar la función Lambda para lanzar una nueva instancia de EC2 a partir de las AMI que creó AWS Backup.
- [ ] Migrar la base de datos a una instancia de EC2 diferente. Colocar la instancia de EC2 de la aplicación en un grupo de Auto Scaling que se extienda a través de múltiples Zonas de disponibilidad. Crear una Amazon Machine Image (AMI) a partir de la instancia de EC2 de la base de datos. Usar la AMI para lanzar una segunda instancia de EC2 de base de datos en una Zona de disponibilidad diferente. Poner la segunda instancia de EC2 de base de datos en estado detenido (stopped). Usar la segunda instancia de EC2 de base de datos como espera (standby).

**[⬆ Volver arriba](#table-of-contents)**


### El trabajo de reportes de una empresa que solía ejecutarse en 15 minutos ahora tarda una hora en completarse. Una aplicación genera los reportes. La aplicación se ejecuta en instancias de Amazon EC2 y extrae datos de una instancia de base de datos de Amazon RDS para MySQL. Un ingeniero de CloudOps revisa el panel de Amazon CloudWatch para la instancia de RDS y nota que las métricas de Read IOPS son altas, incluso cuando los reportes no se están ejecutando. El ingeniero de CloudOps necesita mejorar el rendimiento y la disponibilidad de la instancia de RDS. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar un clúster de Amazon ElastiCache delante de la instancia de RDS. Actualizar el trabajo de reportes para consultar el clúster de ElastiCache.
- [x] Desplegar una réplica de lectura (read replica) de RDS. Actualizar el trabajo de reportes para consultar el endpoint de lectura (reader endpoint).
- [ ] Crear una distribución de Amazon CloudFront. Configurar la instancia de RDS como el origen. Actualizar el trabajo de reportes para consultar la distribución de CloudFront.
- [ ] Aumentar el tamaño de la instancia de RDS.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que usa un bucket de Amazon S3 para almacenamiento de objetos. Un desarrollador necesita configurar el cifrado en tránsito para el bucket de S3. Todos los objetos de S3 que contienen datos personales deben cifrarse en reposo con claves de AWS Key Management Service (AWS KMS), las cuales se pueden rotar bajo demanda. ¿Qué combinación de pasos cumple con estos requisitos? (Elija dos.)

- [ ] Escribir una política de bucket de S3 para permitir solo conexiones cifradas sobre `HTTPS` usando un límite de permisos (permissions boundary).
- [ ] Configurar una política de bucket de S3 para habilitar el cifrado del lado del cliente para los objetos que contienen datos personales usando una clave administrada por el cliente de AWS KMS.
- [x] Configurar la aplicación para cifrar los objetos usando una clave administrada por el cliente de AWS KMS antes de subir los objetos que contienen datos personales a Amazon S3.
- [x] Escribir una política de bucket de S3 para permitir solo conexiones cifradas sobre `HTTPS` usando la condición `aws:SecureTransport`.
- [ ] Configurar la configuración de S3 Block Public Access para el bucket de S3 para permitir solo conexiones cifradas sobre `HTTPS`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps descubrió que un servidor de aplicación de Amazon EC2 recién desplegado no puede conectarse a una instancia de base de datos de Amazon RDS existente. Después de habilitar `VPC` Flow Logs y confirmar que el flow log está activo en la consola, el grupo de registro no se puede encontrar en Amazon CloudWatch. ¿Cuáles son las razones MÁS probables de esta situación? (Elija dos.)

- [ ] El ingeniero debe configurar los `VPC` Flow Logs para que se envíen a AWS CloudTrail.
- [x] El ingeniero ha esperado menos de diez minutos para que se cree el grupo de registro en CloudWatch.
- [ ] Los `VPC` Flow Logs de la cuenta han sido deshabilitados mediante una Política de Control de Servicio.
- [x] No se ha enviado tráfico relevante desde que se crearon los `VPC` Flow Logs.
- [ ] La cuenta tiene Amazon GuardDuty habilitado.

**[⬆ Volver arriba](#table-of-contents)**

### El ingeniero de CloudOps de una empresa está solucionando problemas de comunicación entre los componentes de una aplicación. La empresa configuró los flow logs de `VPC` para que se publiquen en Amazon CloudWatch Logs. Sin embargo, no hay registros en CloudWatch Logs. ¿Qué podría estar bloqueando que los flow logs de `VPC` se publiquen en CloudWatch Logs?

- [x] A la política de IAM adjunta al rol de IAM para el flow log le falta el permiso `CreateLogGroup` de logs.
- [ ] A la política de IAM adjunta al rol de IAM para el flow log le falta el permiso `CreateExportTask` de logs.
- [ ] La `VPC` está configurada para direcciones IPv6.
- [ ] La `VPC` está emparejada (peered) con otra `VPC` en la cuenta de AWS.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps configura los flow logs de `VPC` para que se publiquen en Amazon CloudWatch Logs. El ingeniero de CloudOps revisa los registros en CloudWatch Logs y nota menos tráfico del esperado. Después de que el ingeniero de CloudOps compara los flow logs de `VPC` con registros capturados localmente (on-premises), el ingeniero de CloudOps cree que los flow logs de `VPC` están incompletos. ¿Cuál de las siguientes es una posible razón para la diferencia en el tráfico?

- [ ] Se ha aplicado limitación (throttling) a CloudWatch Logs.
- [ ] El rol de IAM de CloudWatch no tiene una relación de confianza con el servicio de flow logs de `VPC`.
- [ ] El flow log de `VPC` todavía está en proceso de creación.
- [x] Los flow logs de `VPC` no pueden capturar tráfico desde servidores locales (on-premises) hacia una `VPC`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está revisando los `VPC` Flow Logs para solucionar problemas de conectividad en una `VPC`. Al revisar los registros, el ingeniero de CloudOps nota que el tráfico rechazado no aparece listado. ¿Qué debe hacer el ingeniero de CloudOps para asegurarse de que todo el tráfico se registre?

- [x] Crear un nuevo flow log que tenga una configuración de filtro para capturar todo el tráfico.
- [ ] Crear un nuevo flow log. Configurar el formato de registro en un formato personalizado. Seleccionar los campos apropiados para incluir en el registro.
- [ ] Editar el flow log existente. Cambiar la configuración de filtro para capturar todo el tráfico.
- [ ] Editar el flow log existente. Configurar el formato de registro en un formato personalizado. Seleccionar los campos apropiados para incluir en el registro.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja una aplicación web en una instancia de Amazon EC2 en una `VPC` de producción. Las conexiones de clientes a la aplicación están fallando. Un ingeniero de CloudOps inspecciona los flow logs de `VPC` y encuentra la siguiente entrada. ¿Cuál es una posible causa de estas conexiones fallidas?

![Question 282](images/question282.png)

- [ ] Una regla de denegación del grupo de seguridad está bloqueando el tráfico en el puerto `443`.
- [ ] La instancia de EC2 está apagada.
- [x] La `ACL` de red está bloqueando el tráfico `HTTPS`.
- [ ] La `VPC` no tiene una puerta de enlace de internet adjunta.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha creado una puerta de enlace `NAT` en una subred pública en una `VPC`. La `VPC` también contiene una subred privada que incluye instancias de Amazon EC2. Las instancias de EC2 usan la puerta de enlace `NAT` para acceder a internet y descargar parches y actualizaciones. La empresa ha configurado un flow log de `VPC` para la interfaz de red elástica de la puerta de enlace `NAT`. La empresa está publicando la salida en Amazon CloudWatch Logs. Un ingeniero de CloudOps debe identificar los cinco destinos de internet principales con los que se comunican las instancias de EC2 en la subred privada para las descargas. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito de la manera MÁS eficiente operativamente?

- [ ] Usar eventos de AWS CloudTrail Insights para identificar los cinco destinos de internet principales.
- [ ] Usar los registros estándar de Amazon CloudFront (access logs) para identificar los cinco destinos de internet principales.
- [x] Usar CloudWatch Logs Insights para identificar los cinco destinos de internet principales.
- [ ] Cambiar el flow log para publicar registros en Amazon S3. Usar Amazon Athena para consultar los archivos de registro en Amazon S3.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación web de una sola página en AWS. La aplicación usa Amazon CloudFront para entregar contenido estático desde un origen de bucket de Amazon S3. La aplicación también usa un clúster de Amazon Elastic Kubernetes Service (Amazon EKS) para atender llamadas de API. Los usuarios a veces reportan que el sitio web no está operativo, incluso cuando el monitoreo muestra que la página de inicio es alcanzable y que el clúster de EKS está saludable. Un ingeniero de CloudOps debe implementar monitoreo adicional que pueda detectar cuándo el sitio web no está operativo antes de que los usuarios reporten el problema. ¿Qué solución cumple con estos requisitos?

- [x] Crear un canary de monitor de latido (heartbeat monitor) de Amazon CloudWatch Synthetics que apunte al nombre de dominio completamente calificado (FQDN) del sitio web.
- [ ] Crear un canary de API de Amazon CloudWatch Synthetics que monitoree la disponibilidad de los endpoints de API del clúster de EKS.
- [ ] Crear un monitor de aplicación de Amazon CloudWatch RUM que apunte al nombre de dominio completamente calificado (FQDN) del sitio web. Configurar el monitor de aplicación para recopilar telemetría de rendimiento y errores de JavaScript.
- [ ] Crear un monitor de aplicación de Amazon CloudWatch RUM que use los endpoints de API del clúster de EKS.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está haciendo la transición desde aplicaciones alojadas en instancias de Amazon EC2. La empresa quiere implementar una arquitectura sin servidor (serverless) que use Amazon S3, Amazon API Gateway, AWS Lambda y Amazon CloudFront. Como parte de esta transición, la empresa tiene direcciones IP elásticas que no están asociadas con ninguna instancia de EC2 después de que estas se terminan. Un ingeniero de CloudOps necesita automatizar el proceso de liberar todas las direcciones IP elásticas no asociadas que permanecen después de que las instancias de EC2 se terminan. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?

- [x] Activar la regla administrada de AWS Config `eip-attached` para que se ejecute automáticamente cuando ocurran cambios de recursos en la cuenta de AWS. Configurar la remediación automática para la regla. Especificar el runbook de AWS Systems Manager Automation `AWS-ReleaseElasticIP` para la remediación. Especificar un rol apropiado que tenga permisos para la remediación.
- [ ] Crear una función Lambda personalizada que llame a la operación de API `ReleaseAddress` de EC2 y especifique el `AllocationId` de la dirección IP elástica. Invocar la función Lambda usando una regla de Amazon EventBridge. Especificar servicios de AWS como el origen del evento, All Events como el tipo de evento, y AWS Trusted Advisor como el destino.
- [ ] Crear una regla de Amazon EventBridge. Especificar servicios de AWS como el origen del evento, `Instance State-change Notification` como el tipo de evento, y Amazon EC2 como el servicio. Invocar una función Lambda que extraiga la dirección IP elástica de la notificación. Usar AWS CloudFormation para liberar la dirección especificando el `AllocationId` como parámetro de entrada.
- [ ] Crear una función Lambda personalizada que llame a la operación de API `ReleaseAddress` de EC2 y especifique el `AllocationId` de la dirección IP elástica. Invocar la función Lambda usando una regla de Amazon EventBridge. Especificar servicios de AWS como el origen del evento, `Instance State-change Notification` como el tipo de evento, y Amazon EC2 como el servicio.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ejecutando una aplicación en un grupo de instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias de EC2 se ejecutan en tres Zonas de disponibilidad. La empresa necesita proporcionar a los clientes un máximo de dos direcciones IP estáticas para sus aplicaciones. ¿Cómo debe un ingeniero de CloudOps cumplir con este requisito?

- [x] Agregar AWS Global Accelerator delante del Application Load Balancer.
- [ ] Agregar un Network Load Balancer interno detrás del Application Load Balancer.
- [ ] Configurar el Application Load Balancer en solo dos Zonas de disponibilidad.
- [ ] Crear dos direcciones IP elásticas y asignarlas al Application Load Balancer.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa almacena contenido multimedia en un bucket de Amazon S3 y usa Amazon CloudFront para distribuir el contenido a sus usuarios. Debido a los términos de licencia, la empresa no está autorizada a distribuir el contenido en algunos países. Un ingeniero de CloudOps debe restringir el acceso a ciertos países. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Configurar la política del bucket de S3 para denegar la operación `GetObject` según la condición `s3:LocationConstraint`.
- [ ] Crear una Origin Access Identity (OAI) secundaria. Configurar la política del bucket de S3 para prevenir el acceso desde países no autorizados.
- [x] Habilitar la función de restricción geográfica (geo restriction) en la distribución de CloudFront para prevenir el acceso desde países no autorizados.
- [ ] Actualizar la aplicación para generar URLs firmadas de CloudFront solo para direcciones IP en países autorizados.

**[⬆ Volver arriba](#table-of-contents)**

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

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha exigido el uso de autenticación multifactor (MFA) para todos los usuarios de IAM, y requiere que los usuarios hagan todas las llamadas de API usando la CLI. Sin embargo, no se les pide a los usuarios que ingresen tokens de MFA, y pueden ejecutar comandos de la CLI sin MFA. En un intento por hacer cumplir MFA, la empresa adjuntó una política de IAM a todos los usuarios que deniega las llamadas de API que no se hayan autenticado con MFA. ¿Qué paso adicional se debe tomar para asegurar que las llamadas de API se autentiquen usando MFA?

- [ ] Habilitar MFA en roles de IAM, y requerir que los usuarios de IAM usen credenciales de rol para firmar las llamadas de API.
- [ ] Pedir a los usuarios de IAM que inicien sesión en la consola de administración de AWS con MFA antes de hacer llamadas de API usando la CLI.
- [ ] Restringir a los usuarios de IAM al uso de la consola, ya que MFA no es compatible para uso de la CLI.
- [x] Requerir que los usuarios usen credenciales temporales del comando `get-session-token` para firmar las llamadas de API.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita diseñar un plan de recuperación ante desastres (DR) para una aplicación en AWS. La aplicación se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Las instancias están en un grupo de Auto Scaling. La aplicación usa una base de datos Amazon Aurora PostgreSQL. El Objetivo de Tiempo de Recuperación (RTO) y el Objetivo de Punto de Recuperación (RPO) son de 15 minutos cada uno. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS rentable? (Elija dos.)

- [ ] Configurar los respaldos de Aurora para que se exporten a la región de DR.
- [x] Configurar el clúster de Aurora para replicar datos a la región de DR usando la opción de base de datos global (global database) de Aurora.
- [ ] Configurar la región de DR con un `ALB` y un grupo de Auto Scaling. Usar la misma configuración que en la región primaria.
- [x] Configurar la región de DR con un `ALB` y un grupo de Auto Scaling. Establecer la capacidad mínima, máxima y deseada del grupo de Auto Scaling en `1`.
- [ ] Lanzar manualmente un nuevo `ALB` y un nuevo grupo de Auto Scaling usando AWS CloudFormation durante una actividad de conmutación por error (failover).

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación intensiva en memoria que se ejecuta en una flota de instancias de Amazon EC2 detrás de un Elastic Load Balancer (ELB). Las instancias se ejecutan en un grupo de Auto Scaling. Un ingeniero de CloudOps debe asegurarse de que la aplicación pueda escalar según el número de usuarios que se conectan a la aplicación. ¿Qué solución cumple con estos requisitos?

- [x] Crear una política de escalado que escale la aplicación según la métrica de Amazon CloudWatch `ActiveConnectionCount` que genera el ELB.
- [ ] Crear una política de escalado que escale la aplicación según la métrica de Amazon CloudWatch `mem_used` que genera el ELB.
- [ ] Crear una política de escalado programado para aumentar el número de instancias de EC2 en el grupo de Auto Scaling para soportar conexiones adicionales.
- [ ] Crear e implementar un script en el ELB para exponer el número de usuarios conectados como una métrica personalizada de Amazon CloudWatch. Crear una política de escalado que use la métrica.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa que usa AWS Organizations requiere que ningún bucket de Amazon S3 en sus cuentas de producción sea eliminado jamás. ¿Cuál es el enfoque MÁS SIMPLE que puede tomar el ingeniero de CloudOps para asegurar que los buckets de S3 en esas cuentas nunca puedan eliminarse?

- [ ] Configurar `MFA Delete` en todos los buckets de S3 para evitar que se eliminen los buckets.
- [x] Usar Políticas de Control de Servicio para denegar la acción `s3:DeleteBucket` en todos los buckets de las cuentas de producción.
- [ ] Crear un grupo de IAM que tenga una política de IAM para denegar la acción `s3:DeleteBucket` en todos los buckets de las cuentas de producción.
- [ ] Usar AWS Shield para denegar la acción `s3:DeleteBucket` en la cuenta de AWS en lugar de en todos los buckets de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que se ejecuta en una instancia de EC2 en una Zona de disponibilidad. Se le ha encomendado a un ingeniero de CloudOps hacer que la aplicación sea de alta disponibilidad. El ingeniero creó una configuración de lanzamiento (launch configuration) a partir de la instancia de EC2 en ejecución. El ingeniero también configuró correctamente un balanceador de carga. ¿Qué paso debe completar el ingeniero a continuación para hacer que la aplicación sea de alta disponibilidad?

- [ ] Crear un grupo de Auto Scaling usando la configuración de lanzamiento en al menos `2` Zonas de disponibilidad con un tamaño mínimo de `1`, capacidad deseada de `1`, y un tamaño máximo de `1`.
- [x] Crear un grupo de Auto Scaling usando la configuración de lanzamiento en al menos `3` Zonas de disponibilidad con un tamaño mínimo de `2`, capacidad deseada de `2`, y un tamaño máximo de `2`.
- [ ] Crear un grupo de Auto Scaling usando la configuración de lanzamiento en al menos `2` regiones con un tamaño mínimo de `1`, capacidad deseada de `1`, y un tamaño máximo de `1`.
- [ ] Crear un grupo de Auto Scaling usando la configuración de lanzamiento en al menos `3` regiones con un tamaño mínimo de `2`, capacidad deseada de `2`, y un tamaño máximo de `2`.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación se ejecuta en múltiples instancias de EC2. Como parte de una iniciativa para mejorar la seguridad general de la infraestructura, las instancias de EC2 se movieron a una subred privada. Sin embargo, desde que se movieron, las instancias de EC2 no han podido actualizarse automáticamente, y un ingeniero de CloudOps no ha podido conectarse a ellas remotamente por `SSH`. ¿Qué dos acciones podría tomar el ingeniero para resolver estos problemas de forma segura? (Elija dos.)

- [x] Configurar un bastion host en una subred pública, y configurar los grupos de seguridad y tablas de enrutamiento en consecuencia.
- [ ] Configurar un bastion host en la subred privada, y configurar los grupos de seguridad en consecuencia.
- [ ] Configurar un balanceador de carga en una subred pública, y configurar las tablas de enrutamiento en consecuencia.
- [x] Configurar una puerta de enlace `NAT` en una subred pública, y cambiar las tablas de enrutamiento de la subred privada en consecuencia.
- [ ] Configurar una puerta de enlace `NAT` en una subred privada, y asegurarse de que las tablas de enrutamiento estén configuradas en consecuencia.

**[⬆ Volver arriba](#table-of-contents)**

### El uso de servicios de AWS Cloud de una empresa está creciendo rápidamente, por lo que se le ha pedido a un ingeniero de CloudOps que genere detalles del gasto diario para compartir con la gerencia. ¿Qué método debe elegir el ingeniero para producir estos datos?

- [ ] Compartir la factura mensual de AWS con la gerencia.
- [ ] Usar los registros de AWS CloudTrail para acceder a los costos diarios en formato JSON.
- [x] Configurar un Cost and Usage Report diario y descargar la salida desde Amazon S3.
- [ ] Monitorear los costos de AWS con Amazon CloudWatch y crear alarmas y notificaciones de facturación.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa de comercio electrónico ha construido una aplicación web que usa un clúster de base de datos Amazon Aurora. El clúster de base de datos incluye tipos de instancia optimizados para memoria con un nodo de escritura (writer) y un nodo de lectura (reader). El volumen de tráfico cambia a lo largo del día. Durante aumentos repentinos de tráfico, las métricas de Amazon CloudWatch para el clúster de base de datos indican un alto consumo de RAM y un aumento en la latencia de las consultas select. Un ingeniero de CloudOps debe implementar un cambio de configuración para mejorar el rendimiento del clúster de base de datos. El cambio debe minimizar el tiempo de inactividad y no debe resultar en pérdida de datos. ¿Qué cambio cumple con estos requisitos?

- [x] Agregar una réplica de Aurora al clúster de base de datos.
- [ ] Modificar el clúster de base de datos para convertirlo en un clúster de base de datos multi-master.
- [ ] Tomar una instantánea del clúster de base de datos. A partir de esa instantánea, crear un nuevo clúster de base de datos que tenga instancias optimizadas para memoria más grandes.
- [ ] Aumentar la capacidad de almacenamiento en disco del clúster de base de datos al doble de la capacidad de disco existente.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación de comercio web almacena sus datos en un clúster de base de datos Amazon Aurora con una réplica de Aurora. La aplicación muestra la información del carrito de compras leyendo datos desde el endpoint de lectura (reader endpoint). Al monitorear la base de datos Aurora, el ingeniero de CloudOps observa que la métrica `AuroraReplicaLagMaximum` para una sola réplica es alta. ¿Qué comportamiento es MÁS probable que la aplicación esté exhibiendo a los usuarios?

- [ ] Los usuarios no pueden agregar ningún artículo al carrito de compras.
- [x] Los usuarios notan intermitentemente que el carrito no se actualiza correctamente.
- [ ] Los usuarios no pueden eliminar ningún artículo del carrito de compras.
- [ ] Los usuarios no pueden usar la aplicación porque está mostrando una página de error.

**[⬆ Volver arriba](#table-of-contents)**

### Los usuarios están experimentando periódicamente tiempos de respuesta lentos de una base de datos relacional. La base de datos se ejecuta en una instancia ráfaga (burstable) de Amazon EC2 con un volumen de Amazon Elastic Block Store (Amazon EBS) `General Purpose SSD (gp2)` de `350 GB`. Un ingeniero de CloudOps monitorea la instancia de EC2 en Amazon CloudWatch y observa que la métrica `VolumeReadOps` cae a menos del `10%` de su valor máximo durante los períodos de respuesta lenta. ¿Qué debe hacer el ingeniero de CloudOps para asegurar un rendimiento consistentemente alto?

- [ ] Convertir el volumen `gp2` a un volumen EBS `General Purpose SSD (gp3)`.
- [ ] Convertir el volumen `gp2` a un volumen EBS `Cold HDD (sc1)`.
- [ ] Convertir la instancia de EC2 a un tipo de instancia optimizado para memoria.
- [x] Activar el modo ilimitado (unlimited mode) en la instancia de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### AnyCompany ha adquirido Example Corp y está intentando consolidar los sistemas empresariales de ambas compañías. El departamento de TI de AnyCompany necesita integrarse con el sistema de tickets de TI de Example Corp. Un ingeniero de CloudOps debe implementar una solución que use alarmas de Amazon CloudWatch para instancias de Amazon EC2 en la cuenta de AnyCompany para crear nuevos tickets en el sistema de tickets de Example Corp. El sistema de tickets proporciona un endpoint `HTTPS` para la creación de nuevos tickets. El sistema de tickets acepta mensajes en el siguiente formato JSON. ¿Qué enfoque para crear tickets a partir de las alarmas de CloudWatch cumple con estos requisitos con el MENOR tiempo de desarrollo?

![Question 299](images/question299.png)

- [ ] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique EventBridge API destinations como destino. Configurar EventBridge API destinations para enviar eventos al endpoint `HTTPS`. En la regla de EventBridge, crear un input transformer para convertir el origen a una salida compatible con el sistema de tickets.
- [ ] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique un flujo de datos de Amazon Kinesis como destino. Crear una función de AWS Lambda para recibir eventos del flujo de datos de Kinesis. Configurar la función Lambda para iniciar un trabajo de AWS Glue que transforme los datos y reenvíe la salida al endpoint `HTTPS`.
- [x] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique Amazon Simple Notification Service (Amazon SNS) como destino. Configurar Amazon SNS para transformar los eventos y enviarlos al endpoint `HTTPS`.
- [ ] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique una máquina de estados de AWS Step Functions como destino. Crear una función de AWS Lambda y un trabajo de AWS Glue en Step Functions para transformar los eventos y enviarlos al endpoint `HTTPS`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta sus aplicaciones en una gran cantidad de instancias de Amazon EC2. Un ingeniero de CloudOps debe implementar una solución para notificar al equipo de operaciones cada vez que cambie el estado de una instancia de EC2. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear un script que capture los cambios de estado de las instancias y publique una notificación en un tema de Amazon Simple Notification Service (Amazon SNS). Usar AWS Systems Manager Run Command para ejecutar el script en todas las instancias de EC2.
- [x] Crear una regla de evento de Amazon EventBridge que capture los cambios de estado de las instancias de EC2. Establecer un tema de Amazon Simple Notification Service (Amazon SNS) como destino.
- [ ] Crear una regla de evento de Amazon EventBridge que capture los cambios de estado de las instancias de EC2. Establecer como destino una función de AWS Lambda que publique una notificación en un tema de Amazon Simple Notification Service (Amazon SNS).
- [ ] Crear una regla personalizada de AWS Config que evalúe los cambios de estado de las instancias con remediación automática. Usar la regla para invocar una función de AWS Lambda que publique una notificación en un tema de Amazon Simple Notification Service (Amazon SNS).

**[⬆ Volver arriba](#table-of-contents)**


### Una empresa está ejecutando instancias de Amazon EC2 On-Demand en un grupo de Auto Scaling. Las instancias procesan mensajes de una cola de Amazon Simple Queue Service (Amazon SQS). El grupo de Auto Scaling está configurado para escalar según el número de mensajes en la cola. Los mensajes pueden tardar hasta 12 horas en procesarse completamente. Un ingeniero de CloudOps debe asegurarse de que las instancias no se interrumpan durante el procesamiento de mensajes. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Habilitar la protección contra reducción de escala (scale-in protection) de instancias para la instancia específica en el grupo de Auto Scaling al inicio del procesamiento del mensaje llamando a la API de Amazon EC2 Auto Scaling desde el script de procesamiento. Deshabilitar la protección contra reducción de escala de instancias después de que el procesamiento del mensaje se complete llamando a la API de Amazon EC2 Auto Scaling desde el script de procesamiento.
- [ ] Establecer la política de terminación del grupo de Auto Scaling en `OldestInstance`.
- [ ] Establecer la política de terminación del grupo de Auto Scaling en `OldestLaunchConfiguration`.
- [ ] Suspender los procesos de escalado `Launch and Terminate` para la instancia específica en el grupo de Auto Scaling al inicio del procesamiento del mensaje llamando a la API de Amazon EC2 Auto Scaling desde el script de procesamiento. Reanudar los procesos de escalado después de que el procesamiento del mensaje se complete llamando a la API de Amazon EC2 Auto Scaling desde el script de procesamiento.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que recopila notificaciones de miles de sistemas de alarma. Las notificaciones incluyen notificaciones de alarma y notificaciones de información. Las notificaciones de información incluyen los procesos de armado y desarmado del sistema, y el estado de los sensores. Todas las notificaciones se guardan como mensajes en una cola de Amazon Simple Queue Service (Amazon SQS). Las instancias de Amazon EC2 que están en un grupo de Auto Scaling procesan los mensajes. Un ingeniero de CloudOps necesita implementar una solución que priorice las notificaciones de alarma sobre las notificaciones de información. ¿Qué solución cumple con estos requisitos?

- [ ] Ajustar el grupo de Auto Scaling para escalar más rápido cuando haya un alto número de mensajes en la cola.
- [ ] Usar la función fanout de Amazon Simple Notification Service (Amazon SNS) con Amazon SQS para enviar las notificaciones en paralelo a todas las instancias de EC2.
- [ ] Agregar un stream de Amazon DynamoDB para acelerar el procesamiento de mensajes.
- [x] Crear una cola para notificaciones de alarma y una cola para notificaciones de información. Actualizar la aplicación para recopilar mensajes primero de la cola de notificaciones de alarma.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps es responsable de más de `50` instancias de Amazon EC2 desplegadas en una única cuenta de AWS de producción. Las instancias de EC2 ejecutan varios sistemas operativos diferentes. Los estándares de la empresa requieren que el parchado se complete al menos una vez al mes. El ingeniero de CloudOps quiere usar AWS Systems Manager para reducir el número de horas que la empresa dedica al parchado del sistema operativo cada mes. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija tres.)

- [x] Agrupar instancias de EC2 similares en grupos de recursos usando AWS Resource Groups.
- [ ] Crear una programación en Systems Manager Patch Manager. Especificar el grupo de recursos apropiado como el destino.
- [x] Especificar runbooks de Systems Manager Automation para parchar los sistemas operativos. Registrar los runbooks como tareas en la ventana de mantenimiento. Especificar el grupo de recursos apropiado como el destino.
- [ ] Crear un runbook de Systems Manager Automation para monitorear y controlar el estado de los parches requeridos. Aplicar el runbook a Systems Manager Patch Manager.
- [x] Crear una única ventana de mantenimiento de Systems Manager para cada grupo de recursos.
- [ ] Configurar Systems Manager Fleet Manager para aplicar un runbook de Systems Manager Automation al grupo de recursos apropiado.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa necesita hacer cumplir los requisitos de etiquetado para tablas de Amazon DynamoDB en sus cuentas de AWS. Un ingeniero de CloudOps debe implementar una solución para identificar y remediar todas las tablas de DynamoDB que no tengan las etiquetas apropiadas. ¿Qué solución cumple con estos requisitos con el MENOR esfuerzo operativo?

- [ ] Crear una función de AWS Lambda personalizada para evaluar y remediar todas las tablas de DynamoDB. Crear una regla programada de Amazon EventBridge para invocar la función Lambda.
- [ ] Crear una función de AWS Lambda personalizada para evaluar y remediar todas las tablas de DynamoDB. Crear una regla personalizada de AWS Config para invocar la función Lambda.
- [x] Usar la regla administrada de AWS Config `required-tags` para evaluar todas las tablas de DynamoDB en busca de las etiquetas apropiadas. Configurar una acción de remediación automática que use un runbook personalizado de AWS Systems Manager Automation.
- [ ] Crear una regla administrada de Amazon EventBridge para evaluar todas las tablas de DynamoDB en busca de las etiquetas apropiadas. Configurar la regla de EventBridge para ejecutar un runbook personalizado de AWS Systems Manager Automation para la remediación.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que usa tablas de Amazon DynamoDB. Las tablas están distribuidas entre cuentas de AWS y regiones de AWS. La empresa usa AWS CloudFormation para desplegar recursos de AWS. Un nuevo equipo en la empresa está eliminando recursos de AWS que no se usan. El equipo elimina accidentalmente varias tablas de DynamoDB de producción al ejecutar una función de AWS Lambda que hace una llamada de API `DeleteTable` de DynamoDB. Las eliminaciones de tablas causan una interrupción de la aplicación. Un ingeniero de CloudOps debe implementar una solución que minimice la posibilidad de eliminaciones accidentales de tablas. La solución también debe minimizar la pérdida de datos resultante de eliminaciones accidentales. ¿Qué combinación de pasos cumple con estos requisitos? (Elija dos.)

- [ ] Habilitar la protección contra terminación para los stacks de CloudFormation que despliegan las tablas de DynamoDB.
- [x] Habilitar la protección contra eliminación (deletion protection) para las tablas de DynamoDB.
- [x] Habilitar la recuperación a un punto en el tiempo (point-in-time recovery) para las tablas de DynamoDB. Restaurar las tablas si se eliminan accidentalmente.
- [ ] Programar respaldos diarios de las tablas de DynamoDB. Restaurar las tablas si se eliminan accidentalmente.
- [ ] Exportar las tablas de DynamoDB a Amazon S3 todos los días. Usar Import from Amazon S3 para restaurar datos de las tablas que se eliminen accidentalmente.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere rastrear sus costos de AWS en todas las cuentas miembro que forman parte de una organización en AWS Organizations. Los administradores de las cuentas miembro quieren recibir una notificación cuando los costos estimados superen un monto predeterminado cada mes. Los administradores no pueden configurar una alarma de facturación. Los permisos de IAM para todos los usuarios son correctos. ¿Cuál podría ser la causa de este problema?

- [x] La cuenta de administración/pagadora no tiene activadas las alertas de facturación.
- [ ] La empresa no ha configurado AWS Resource Access Manager (AWS RAM) para compartir información de facturación entre las cuentas miembro y la cuenta de administración/pagadora.
- [ ] Amazon GuardDuty está activado para todas las cuentas.
- [ ] La empresa no ha configurado una regla de AWS Config para monitorear la facturación.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está solucionando problemas de una `VPC` con subredes públicas y privadas que usan `ACL` de red personalizadas. Las instancias en la subred privada no pueden acceder a internet. Hay una puerta de enlace de internet adjunta a la subred pública. La subred privada tiene una ruta hacia una puerta de enlace `NAT` que también está adjunta a la subred pública. Las instancias de Amazon EC2 están asociadas con el grupo de seguridad predeterminado de la `VPC`. ¿Qué está causando el problema en este escenario?

- [x] Hay una `ACL` de red en la subred privada configurada para denegar todo el tráfico de salida.
- [ ] No hay ninguna puerta de enlace `NAT` desplegada en la subred privada de la `VPC`.
- [ ] El grupo de seguridad predeterminado de la `VPC` bloquea todo el tráfico entrante hacia las instancias de EC2.
- [ ] El grupo de seguridad predeterminado de la `VPC` bloquea todo el tráfico saliente desde las instancias de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una organización está ejecutando múltiples aplicaciones para sus clientes. Cada aplicación se despliega ejecutando una plantilla base de AWS CloudFormation que configura una nueva `VPC`. Todas las aplicaciones se ejecutan en la misma cuenta de AWS y región de AWS. Un ingeniero de CloudOps ha notado que al intentar desplegar el mismo stack de AWS CloudFormation, este falla al desplegarse. ¿Cuál es probablemente el problema?

- [ ] La Amazon Machine Image usada no está disponible en esa región.
- [ ] La plantilla de AWS CloudFormation necesita actualizarse a la última versión.
- [ ] Los parámetros de configuración de la `VPC` han cambiado y deben actualizarse en la plantilla.
- [x] La cuenta ha alcanzado el límite predeterminado de `VPC` permitidas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa de servicios financieros está ejecutando software de computación distribuida para administrar una flota de 20 servidores para sus cálculos. Hay 2 nodos de control y 18 nodos trabajadores (worker) que ejecutan los cálculos. Los nodos de control pueden iniciar automáticamente los nodos trabajadores cuando sea necesario. Actualmente, todos los nodos se ejecutan on-demand, y los nodos trabajadores se usan aproximadamente 4 horas cada día. ¿Qué combinación de acciones será MÁS rentable? (Elija dos.)

- [ ] Usar Dedicated Hosts para los nodos de control.
- [x] Usar Instancias Reservadas para los nodos de control.
- [ ] Usar Instancias Reservadas para los nodos trabajadores.
- [ ] Usar Instancias Spot para los nodos de control e Instancias On-Demand si no hay disponibilidad Spot.
- [x] Usar Instancias Spot para los nodos trabajadores e Instancias On-Demand si no hay disponibilidad Spot.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación web que experimenta problemas de rendimiento varias veces cada noche. Un análisis de causa raíz revela picos en el uso de CPU que duran 5 minutos en una instancia de Amazon EC2 Linux. Se le encarga a un ingeniero de CloudOps encontrar el ID de proceso (PID) del servicio o proceso que está consumiendo más CPU. ¿Cómo puede el ingeniero lograr esto con el MENOR esfuerzo?

- [ ] Configurar una función de AWS Lambda en Python `3.7` para que se ejecute cada minuto y capture el PID y envíe una notificación.
- [x] Configurar el plugin `procstat` para recopilar y enviar métricas de CPU de los procesos en ejecución.
- [ ] Iniciar sesión en la instancia de EC2 Linux usando una clave `.pem` cada noche y luego ejecutar el comando top.
- [ ] Usar la métrica predeterminada de uso de CPU de Amazon CloudWatch para capturar el PID en el panel de CloudWatch.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa AWS Organizations para alojar varias aplicaciones en múltiples cuentas de AWS. Varios equipos son responsables de construir y mantener la infraestructura de las aplicaciones en las cuentas de AWS. Un ingeniero de CloudOps debe implementar una solución para asegurar que las cuentas de usuario y los permisos se administren centralizadamente. La solución debe integrarse con el entorno de Active Directory local (on-premises) existente de la empresa. El ingeniero de CloudOps ya ha habilitado AWS IAM Identity Center (AWS Single Sign-On) y ha configurado una conexión de AWS Direct Connect. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear un dominio Simple AD, y establecer una relación de confianza de bosque (forest trust) con el dominio de Active Directory local. Establecer el dominio Simple AD como el origen de identidad para IAM Identity Center. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.
- [ ] Crear un controlador de dominio de Active Directory en una instancia de Amazon EC2 unida al dominio de Active Directory local. Establecer el controlador de dominio de Active Directory como el origen de identidad para IAM Identity Center. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.
- [x] Crear un AD Connector asociado con el dominio de Active Directory local. Establecer el AD Connector como el origen de identidad para IAM Identity Center. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.
- [ ] Usar el directorio SSO integrado como el origen de identidad para IAM Identity Center. Copiar los usuarios y grupos desde el dominio de Active Directory local. Crear los conjuntos de permisos basados en roles requeridos. Asignar cada grupo de usuarios a las cuentas de AWS que el grupo administrará.

**[⬆ Volver arriba](#table-of-contents)**

### Se le ha pedido a un ingeniero de CloudOps que configure etiquetas de asignación de costos definidas por el usuario para una nueva cuenta de AWS. La empresa usa AWS Organizations para la administración de cuentas. ¿Qué debe hacer el ingeniero para habilitar las etiquetas de asignación de costos definidas por el usuario?

- [ ] Iniciar sesión en la consola de AWS Billing and Cost Management de la nueva cuenta, y usar el administrador de Cost Allocation Tags para crear las nuevas etiquetas de asignación de costos definidas por el usuario.
- [x] Iniciar sesión en la consola de AWS Billing and Cost Management de la cuenta pagadora, y usar el administrador de Cost Allocation Tags para crear las nuevas etiquetas de asignación de costos definidas por el usuario.
- [ ] Iniciar sesión en la consola de administración de AWS de la nueva cuenta, usar el Tag Editor para crear las nuevas etiquetas definidas por el usuario, luego usar el administrador de Cost Allocation Tags en la nueva cuenta para marcar las etiquetas como etiquetas de asignación de costos.
- [ ] Iniciar sesión en la consola de administración de AWS de la nueva cuenta, usar el Tag Editor para crear las nuevas etiquetas definidas por el usuario, luego usar el administrador de Cost Allocation Tags en la cuenta pagadora para marcar las etiquetas como etiquetas de asignación de costos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita configurar un bucket de Amazon S3 para alojar una aplicación web. El ingeniero de CloudOps ha creado el bucket de S3 y ha copiado los archivos estáticos de la aplicación web al bucket de S3. La empresa tiene una política de que ningún bucket de S3 debe ser público. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Crear una distribución de Amazon CloudFront. Configurar el bucket de S3 como origen con una Origin Access Identity (OAI). Otorgar a la OAI el permiso `s3:GetObject` en la política del bucket de S3.
- [ ] Configurar el alojamiento de sitio web estático en el bucket de S3. Usar Amazon Route 53 para crear un `CNAME` de `DNS` que apunte al endpoint del sitio web de S3.
- [ ] Crear un Application Load Balancer (ALB). Cambiar el protocolo a `HTTPS` en la configuración del listener del `ALB`. Reenviar el tráfico al bucket de S3.
- [ ] Crear un accelerator en AWS Global Accelerator. Configurar una configuración de listener para el puerto `443`. Establecer el tipo de endpoint para reenviar el tráfico al bucket de S3.

**[⬆ Volver arriba](#table-of-contents)**

### Un volumen de Amazon EBS adjunto a una instancia de EC2 fue modificado recientemente. Parte de la modificación incluyó aumentar la capacidad de almacenamiento. El ingeniero de CloudOps nota que la capacidad de almacenamiento aumentada no se refleja en el sistema de archivos. ¿Qué paso debe completar el ingeniero para usar la capacidad de almacenamiento aumentada?

- [ ] Reiniciar la instancia de EC2.
- [x] Extender el sistema de archivos del volumen.
- [ ] Desconectar el volumen EBS, redimensionarlo, y volver a conectarlo.
- [ ] Tomar una instantánea de EBS y restaurarla en el volumen más grande.

**[⬆ Volver arriba](#table-of-contents)**

### Recientemente, varios archivos críticos se eliminaron por error de un bucket compartido de Amazon S3. Un ingeniero de CloudOps necesita prevenir que ocurran eliminaciones accidentales en el futuro habilitando `MFA Delete`. Una vez habilitado, ¿qué actividades del bucket requerirán autenticación MFA? (Elija dos.)

- [x] Eliminar permanentemente una versión de objeto del bucket.
- [ ] Deshabilitar el cifrado predeterminado de objetos para el bucket.
- [ ] Listar todas las versiones de objetos eliminados en el bucket.
- [x] Suspender el versionado en el bucket.
- [ ] Habilitar `MFA Add` en el bucket.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está probando una aplicación alojada en cinco instancias de Amazon EC2. Las instancias se ejecutan en un grupo de Auto Scaling detrás de un Application Load Balancer (`ALB`). El alto uso de CPU durante las pruebas de carga está causando que el grupo de Auto Scaling escale hacia afuera. El ingeniero de CloudOps debe solucionar el problema para encontrar la causa raíz del alto uso de CPU antes de que el grupo de Auto Scaling escale hacia afuera. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Habilitar la protección contra reducción de escala (scale-in protection) de instancias.
- [ ] Colocar la instancia en estado Standby.
- [ ] Eliminar el listener del `ALB`.
- [x] Suspender los tipos de proceso `Launch and Terminate`.

**[⬆ Volver arriba](#table-of-contents)**

### Se le ha encomendado a un ingeniero de CloudOps desplegar la infraestructura de una empresa como código. El ingeniero quiere escribir una única plantilla que pueda reutilizarse para múltiples entornos de una manera segura y repetible. ¿Cuál es la forma recomendada de usar AWS CloudFormation para cumplir con este requisito?

- [x] Usar parámetros para aprovisionar los recursos.
- [ ] Usar stacks anidados (nested stacks) para aprovisionar los recursos.
- [ ] Usar datos de usuario (user data) de Amazon EC2 para aprovisionar los recursos.
- [ ] Usar políticas de stack para aprovisionar los recursos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps es responsable de una gran flota de instancias de EC2 y debe saber si alguna instancia se verá afectada por el próximo mantenimiento de hardware. ¿Qué opción proporcionaría esta información con el MENOR esfuerzo administrativo?

- [ ] Monitorear AWS CloudTrail en busca de llamadas a la API `StopInstances` relacionadas con el mantenimiento próximo.
- [x] Revisar el Personal Health Dashboard en busca de cualquier mantenimiento programado.
- [ ] Desde la consola de administración de AWS, listar cualquier instancia con verificaciones de estado del sistema fallidas.
- [ ] Desplegar una solución de monitoreo de terceros para proporcionar monitoreo en tiempo real de instancias de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está creando recursos a partir de una plantilla de AWS CloudFormation que define un grupo de Auto Scaling de instancias de Amazon EC2. La plantilla de lanzamiento del grupo de Auto Scaling aprovisiona cada instancia de EC2 usando un script de datos de usuario. La creación del recurso de grupo de Auto Scaling está fallando debido a un error. La condición de espera (wait condition) no está recibiendo el número requerido de señales. ¿Cómo debe el ingeniero de CloudOps resolver este error?

- [x] Ejecutar `cfn-signal` al finalizar el script de datos de usuario.
- [ ] Modificar el grupo de seguridad de las instancias de EC2 para permitir tráfico saliente en el puerto `443`.
- [ ] Reducir el valor de `DesiredCapacity` del grupo de Auto Scaling en la plantilla de CloudFormation.
- [ ] Establecer la propiedad `AssociatePublicIpAddress` en `True` en la plantilla de lanzamiento del grupo de Auto Scaling.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja una aplicación web en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias están en un grupo de Amazon EC2 Auto Scaling. Se accede a la aplicación con una URL pública. Un ingeniero de CloudOps necesita implementar una solución de monitoreo que verifique la disponibilidad de la aplicación y siga las mismas rutas y acciones que un cliente. El ingeniero de CloudOps debe recibir una notificación si menos del `95%` de las ejecuciones de monitoreo no encuentran errores. ¿Qué solución cumple con estos requisitos?

- [x] Crear un canary de Amazon CloudWatch Synthetics con un script que siga las rutas del cliente. Programar el canary para que se ejecute en una programación recurrente. Crear una alarma de CloudWatch que publique un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando la métrica `SuccessPercent` sea menor al `95%`.
- [ ] Crear verificaciones de salud (health checks) de Amazon Route 53 que monitoreen la disponibilidad del endpoint. Crear alarmas de Amazon CloudWatch que publiquen un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando la métrica `HealthCheckPercentageHealthy` sea menor al `95%`.
- [ ] Crear una única función de AWS Lambda para verificar si los endpoints están disponibles para cada ruta de cliente. Programar la función Lambda usando Amazon EventBridge (Amazon CloudWatch Events). Configurar la función Lambda para publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando un endpoint devuelva un error.
- [ ] Crear una función de AWS Lambda para cada ruta de cliente para verificar si ese endpoint específico está disponible. Programar las funciones Lambda usando Amazon EventBridge (Amazon CloudWatch Events). Configurar cada función Lambda para publicar una métrica personalizada en Amazon CloudWatch para el estado del endpoint. Crear alarmas de CloudWatch basadas en cada métrica personalizada para publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando una alarma esté en estado `ALARM`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps que trabaja en una instancia de Amazon EC2 ha configurado incorrectamente el reloj por una hora. La instancia de EC2 está enviando datos a Amazon CloudWatch a través del agente de CloudWatch. Las marcas de tiempo en los registros están 45 minutos en el futuro. ¿Cuál será el resultado de esta configuración?

- [ ] Amazon CloudWatch no capturará los datos porque están en el futuro.
- [x] Amazon CloudWatch aceptará los datos de métrica personalizada y los registrará.
- [ ] El agente de Amazon CloudWatch verificará el servidor de Network Time Protocol (NTP) antes de enviar los datos, y el agente corregirá la hora.
- [ ] El agente de Amazon CloudWatch verificará el servidor de Network Time Protocol (NTP), y el agente no enviará los datos porque están más de 30 minutos en el futuro.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha configurado un agente de CloudWatch para enviar métricas personalizadas a Amazon CloudWatch y ahora está ensamblando un panel de CloudWatch para mostrar estas métricas. ¿Qué pasos debe tomar el ingeniero para completar esta tarea?

- [ ] Seleccionar el AWS Namespace, filtrar por nombre de métrica, luego agregar al panel.
- [ ] Agregar un widget de texto, seleccionar la métrica apropiada del namespace personalizado, luego agregar al panel.
- [x] Seleccionar el widget y las métricas apropiadas del namespace personalizado, luego agregar al panel.
- [ ] Abrir la consola de CloudWatch, desde CloudWatch Events, agregar todas las métricas personalizadas.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita crear una réplica de la infraestructura de AWS existente de una empresa en una nueva cuenta de AWS. Actualmente, se usa un portafolio de AWS Service Catalog para crear y administrar recursos. ¿Cuál es la forma MÁS eficiente de lograr esto?

- [ ] Crear una plantilla de AWS CloudFormation para usar el portafolio de AWS Service Catalog en la nueva cuenta de AWS.
- [ ] Crear manualmente un portafolio de AWS Service Catalog en la nueva cuenta de AWS que duplique el portafolio original.
- [ ] Ejecutar una función de AWS Lambda para crear un nuevo portafolio de AWS Service Catalog basado en la salida de la operación de API `DescribePortfolio`.
- [x] Compartir el portafolio de AWS Service Catalog con las otras cuentas de AWS e importar el portafolio a las otras cuentas de AWS.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación desplegada en dos regiones de AWS en una configuración activa-pasiva. La aplicación se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB) en cada región. Las instancias están en un grupo de Amazon EC2 Auto Scaling en cada región. La aplicación usa una zona alojada de Amazon Route 53 para `DNS`. Un ingeniero de CloudOps necesita configurar la conmutación por error (failover) automática a la región secundaria. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Configurar registros alias de Route 53 que apunten a cada `ALB`. Elegir una política de enrutamiento de failover. Establecer `Evaluate Target Health` en `Yes`.
- [ ] Configurar registros `CNAME` que apunten a cada ALB. Elegir una política de enrutamiento de failover. Establecer `Evaluate Target Health` en `Yes`.
- [ ] Configurar verificaciones de salud de Elastic Load Balancing (ELB) para el grupo de Auto Scaling. Agregar un grupo de destino al `ALB` en la región primaria. Incluir las instancias de EC2 en la región secundaria como destinos.
- [ ] Configurar verificaciones de salud de EC2 para el grupo de Auto Scaling. Agregar un grupo de destino al `ALB` en la región primaria. Incluir las instancias de EC2 en la región secundaria como destinos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa planea lanzar un sitio web estático en su dominio `example.com` y subdominio `www.example.com` usando Amazon S3. ¿Cómo debe el ingeniero de CloudOps cumplir con este requisito?

- [ ] Crear un bucket de S3 llamado `example.com` para tanto el dominio como el subdominio.
- [ ] Crear un bucket de S3 con un comodín llamado `*.example.com` para tanto el dominio como el subdominio.
- [x] Crear dos buckets de S3 llamados `example.com` y `www.example.com`. Configurar el bucket del subdominio para redirigir las solicitudes al bucket del dominio.
- [ ] Crear dos buckets de S3 llamados `http://example.com` y `http://*.example.com`. Configurar el bucket comodín (`*`) para redirigir las solicitudes al bucket del dominio.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps está manteniendo una aplicación que se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Los usuarios reportan errores al intentar iniciar la aplicación. El ingeniero nota un aumento en la métrica de Amazon CloudWatch `HTTPCode_ELB_5xx_Count` para el balanceador de carga. ¿Cuál es una posible causa de este aumento?

- [ ] El `ALB` está asociado con subredes privadas dentro de la `VPC`.
- [ ] El `ALB` recibió una solicitud de un cliente, pero el cliente cerró la conexión.
- [ ] El grupo de seguridad del `ALB` no está configurado para permitir tráfico entrante de los usuarios.
- [x] El grupo de destino del `ALB` no contiene instancias de EC2 saludables.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene varias cuentas miembro que forman parte de una organización en AWS Organizations. La empresa descubrió recientemente que los administradores han estado usando credenciales de usuario raíz de la cuenta. La empresa debe evitar que los ingenieros usen credenciales de usuario raíz para realizar cualquier acción en instancias de Amazon EC2. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Crear una política de IAM basada en identidad en cada cuenta miembro para denegar acciones en instancias de EC2 por parte del usuario raíz.
- [x] En la cuenta de administración de la organización, crear una Política de Control de Servicio (SCP) para denegar acciones en instancias de EC2 por parte del usuario raíz en todas las cuentas miembro.
- [ ] Usar AWS Config para prevenir cualquier acción en instancias de EC2 por parte del usuario raíz.
- [ ] Usar Amazon Inspector en cada cuenta miembro para escanear inicios de sesión de usuario raíz y prevenir cualquier acción en instancias de EC2 por parte del usuario raíz.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa crea una nueva cuenta miembro usando AWS Organizations. Un ingeniero de CloudOps necesita agregar AWS Business Support a la nueva cuenta. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con este requisito? (Elija dos.)

- [x] Iniciar sesión en la nueva cuenta usando credenciales de IAM. Cambiar el plan de soporte.
- [ ] Iniciar sesión en la nueva cuenta usando credenciales de usuario raíz. Cambiar el plan de soporte.
- [ ] Usar la API de AWS Support para cambiar el plan de soporte.
- [ ] Restablecer la contraseña del usuario raíz de la cuenta.
- [x] Crear un usuario de IAM que tenga privilegios de administrador en la nueva cuenta.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa aloja su sitio web en la región `us-east-1`. La empresa se está preparando para desplegar su sitio web en la región `eu-central-1`. Los visitantes del sitio web ubicados en Europa deben acceder al sitio web alojado en `eu-central-1`. Todos los demás visitantes acceden al sitio web alojado en `us-east-1`. La empresa usa Amazon Route 53 para administrar los registros `DNS` del sitio web. ¿Qué política de enrutamiento debe aplicar un ingeniero de CloudOps al conjunto de registros de Route 53 para cumplir con estos requisitos?

- [x] Política de enrutamiento por geolocalización (Geolocation).
- [ ] Política de enrutamiento por geoproximidad (Geoproximity).
- [ ] Política de enrutamiento por latencia (Latency).
- [ ] Política de enrutamiento de respuesta múltiple (Multivalue answer).

**[⬆ Volver arriba](#table-of-contents)**

### El ingeniero de CloudOps de una empresa administra una flota de cientos de instancias de Amazon EC2 que ejecutan cargas de trabajo basadas en Windows y cargas de trabajo basadas en Linux. Cada instancia de EC2 tiene una etiqueta que identifica su sistema operativo. Todas las instancias de EC2 ejecutan AWS Systems Manager Session Manager. Se reporta una vulnerabilidad de día cero, y no hay parches disponibles. El equipo de seguridad de la empresa proporciona código para todos los sistemas operativos relevantes para reducir el riesgo de la vulnerabilidad. El ingeniero de CloudOps necesita implementar el código en las instancias de EC2 y debe proporcionar un informe que muestre que el código se ejecutó exitosamente en todas las instancias. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos lo más rápido posible?

- [x] Usar Systems Manager Run Command. Elegir el documento `AWS-RunShellScript` o el documento `AWS-RunPowerShellScript`. Configurar Run Command con el código del equipo de seguridad. Especificar la etiqueta del sistema operativo en el parámetro Targets. Ejecutar el comando. Proporcionar el historial de comandos como evidencia al equipo de seguridad.
- [ ] Crear una función de AWS Lambda que se conecte a las instancias de EC2 a través de Session Manager. Configurar la función Lambda para identificar el sistema operativo, ejecutar el código del equipo de seguridad, y devolver los resultados a una instancia de base de datos de Amazon RDS. Consultar la instancia de base de datos para obtener los resultados. Proporcionar los resultados como evidencia al equipo de seguridad.
- [ ] Iniciar sesión en cada instancia de EC2. Ejecutar el código del equipo de seguridad en cada instancia de EC2. Copiar y pegar los resultados de cada ejecución en una única hoja de cálculo. Proporcionar la hoja de cálculo como evidencia al equipo de seguridad.
- [ ] Actualizar las plantillas de lanzamiento de las instancias de EC2 para incluir el código del equipo de seguridad en los datos de usuario. Volver a lanzar las instancias de EC2 usando las plantillas de lanzamiento actualizadas. Recuperar los registros de instancia de EC2 de cada instancia. Proporcionar los registros de instancia de EC2 como evidencia al equipo de seguridad.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps es responsable de la seguridad de la cuenta de AWS de una empresa. La empresa tiene una política según la cual un usuario solo puede detener o terminar instancias de Amazon EC2 cuando el usuario está autenticado usando un dispositivo de autenticación multifactor (MFA). ¿Qué política debe aplicar el ingeniero de CloudOps para cumplir con este requisito?

- [x] Opción A.
![Question 331 option A](images/question331_A.png)
- [ ] Opción B.
![Question 331 option B](images/question331_B.png)
- [ ] Opción C.
![Question 331 option C](images/question331_C.png)
- [ ] Opción D.
![Question 331 option D](images/question331_D.png)

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está configurando una conexión de emparejamiento (peering) de `VPC` entre su `VPC` y la `VPC` de un cliente. La `VPC` de la empresa tiene un bloque `CIDR` IPv4 de `172.16.0.0/16`, y la del cliente tiene un bloque `CIDR` IPv4 de `10.0.0.0/16`. El ingeniero de CloudOps quiere poder hacer ping a la dirección IP privada de la base de datos del cliente desde una de las instancias de Amazon EC2 de la empresa. ¿Qué acción se debe tomar para cumplir con los requisitos?

- [ ] Asegurarse de que ambas cuentas estén vinculadas y sean parte de la facturación consolidada para crear una red de intercambio de archivos, y luego habilitar el emparejamiento de `VPC`.
- [x] Asegurarse de que ambos propietarios de `VPC` agreguen manualmente una ruta a las tablas de enrutamiento de la `VPC` que apunte al rango de direcciones IP de la otra `VPC`.
- [ ] Indicar al cliente que configure una `VPC` con el mismo bloque `CIDR` IPv4 que la `VPC` de origen: `172.16.0.0/16`.
- [ ] Indicar al cliente que cree una puerta de enlace privada virtual para vincular las dos `VPC`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación web a la que los usuarios acceden usando el nombre de dominio `www.example.com`. La empresa administra el nombre de dominio usando Amazon Route 53. La empresa creó una distribución de Amazon CloudFront delante de la aplicación y le gustaría que `www.example.com` acceda a la aplicación a través de CloudFront. ¿Cuál es la forma MÁS rentable de lograr esto?

- [ ] Crear un registro `CNAME` en Amazon Route 53 que apunte a la URL de la distribución de CloudFront.
- [x] Crear un registro `ALIAS` en Amazon Route 53 que apunte a la URL de la distribución de CloudFront.
- [ ] Crear un registro `A` en Amazon Route 53 que apunte a la dirección IP pública de la aplicación web.
- [ ] Crear un registro `PTR` en Amazon Route 53 que apunte a la dirección IP pública de la aplicación web.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita desplegar una aplicación en múltiples regiones de AWS. El ingeniero de CloudOps debe implementar una solución que dirija a los usuarios a la región con la menor latencia. En caso de falla, la solución debe dirigir automáticamente las solicitudes a una región con una instancia saludable de la aplicación. La empresa necesita una solución con el menor tiempo de conmutación por error (failover). ¿Qué solución cumple con estos requisitos?

- [ ] Crear registros `A` de Amazon Route 53 que tengan el mismo nombre para cada endpoint. Usar una política de enrutamiento por latencia. Asociar una verificación de salud con cada registro.
- [ ] Crear registros `A` de Amazon Route 53 que tengan el mismo nombre para cada endpoint. Usar una política de enrutamiento de failover. Asociar una verificación de salud con cada registro.
- [x] Crear un standard accelerator de AWS Global Accelerator. Crear un grupo de endpoints para cada región. Agregar un listener al accelerator. Asociar el grupo de endpoints con el listener.
- [ ] Crear registros `A` de Amazon Route 53 que tengan el mismo nombre para cada endpoint. Usar una política de enrutamiento por geolocalización. Asociar una verificación de salud con cada registro.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está usando alarmas de Amazon CloudWatch para monitorear cargas de trabajo de Amazon Elastic Kubernetes Service (Amazon EKS). Las alarmas se inician a través de una definición de umbral y no están ayudando a que el clúster de EKS opere de manera más eficiente. Un ingeniero de CloudOps debe implementar una solución que identifique anomalías y genere recomendaciones sobre cómo abordarlas. ¿Qué solución cumple con estos requisitos?

- [ ] Usar la detección de anomalías de CloudWatch para identificar anomalías y proporcionar recomendaciones.
- [x] Usar CloudWatch Container Insights con Amazon DevOps Guru para identificar anomalías y proporcionar recomendaciones.
- [ ] Usar CloudWatch Container Insights para identificar anomalías y proporcionar recomendaciones.
- [ ] Usar la detección de anomalías de CloudWatch con CloudWatch Container Insights para identificar anomalías y proporcionar recomendaciones.

**[⬆ Volver arriba](#table-of-contents)**

### La aplicación de una empresa actualmente usa un rol de IAM que permite acceso total a todos los servicios de AWS. Un ingeniero de CloudOps debe asegurarse de que las políticas de IAM de la empresa permitan solo los permisos que la aplicación requiere. ¿Cómo puede el ingeniero de CloudOps crear una política que cumpla con este requisito?

- [ ] Activar AWS CloudTrail. Generar una política usando AWS Security Hub.
- [ ] Activar Amazon EventBridge (Amazon CloudWatch Events). Generar una política usando AWS Identity and Access Management Access Analyzer.
- [ ] Usar la AWS CLI para ejecutar el comando `get-generated-policy` en AWS Identity and Access Management Access Analyzer.
- [x] Activar AWS CloudTrail. Generar una política usando AWS Identity and Access Management Access Analyzer.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa almacena datos sensibles en un bucket de Amazon S3. La empresa debe registrar todos los intentos de acceso al bucket de S3. El equipo de riesgos de la empresa debe recibir notificación inmediata sobre cualquier evento de eliminación. ¿Qué solución cumple con estos requisitos?

- [x] Habilitar el registro de acceso del servidor (S3 server access logging) de S3 para los registros de auditoría. Configurar una notificación de Amazon Simple Notification Service (Amazon SNS) para el bucket de S3. Seleccionar `DeleteObject` como el tipo de evento para el sistema de alertas.
- [ ] Habilitar el registro de acceso del servidor de S3 para los registros de auditoría. Lanzar una instancia de Amazon EC2 para el sistema de alertas. Ejecutar un cron job en la instancia de EC2 para descargar los registros de acceso cada día y buscar un evento `DeleteObject`.
- [ ] Usar Amazon CloudWatch Logs para los registros de auditoría. Usar alarmas de Amazon CloudWatch con una notificación de Amazon Simple Notification Service (Amazon SNS) para el sistema de alertas.
- [ ] Usar Amazon CloudWatch Logs para los registros de auditoría. Lanzar una instancia de Amazon EC2 para el sistema de alertas. Ejecutar un cron job en la instancia de EC2 cada día para comparar la lista de elementos con la lista del día anterior. Configurar el cron job para enviar una notificación si falta un elemento.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa almacena sus datos internos dentro de un bucket de Amazon S3. Todos los datos existentes dentro del bucket de S3 están protegidos usando cifrado del lado del servidor con claves de cifrado administradas por Amazon S3 (SSE-S3). El versionado de S3 está habilitado. Un ingeniero de CloudOps debe replicar los datos internos a otro bucket de S3 en una cuenta de AWS diferente para recuperación ante desastres. Todos los datos existentes se copian del bucket de S3 de origen al bucket de S3 de destino. ¿Qué solución de replicación es MÁS eficiente operativamente?

- [x] Agregar una regla de replicación al bucket de origen y especificar el bucket de destino. Crear una política de bucket para el bucket de destino que permita al propietario del bucket de origen replicar objetos.
- [ ] Programar un trabajo de AWS Batch con Amazon EventBridge para copiar nuevos objetos del bucket de origen al bucket de destino. Crear un rol de IAM de Batch Operations en la cuenta de destino.
- [ ] Configurar una notificación de eventos de Amazon S3 para el bucket de origen que invoque una función de AWS Lambda para copiar nuevos objetos al bucket de destino. Asegurarse de que la función Lambda tenga permisos de acceso entre cuentas.
- [ ] Ejecutar un script programado en una instancia de Amazon EC2 para copiar nuevos objetos del bucket de origen al bucket de destino. Asignar permisos de acceso entre cuentas al rol de la instancia de EC2.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa desplegó recientemente MySQL en una instancia de Amazon EC2 con un volumen de arranque predeterminado. La empresa tiene la intención de restaurar una base de datos de 1.75 TB. Un ingeniero de CloudOps necesita aprovisionar el volumen correcto de Amazon Elastic Block Store (Amazon EBS). La base de datos requerirá un rendimiento de lectura de hasta 10,000 IOPS y no se espera que crezca en tamaño. ¿Qué solución proporcionará el rendimiento requerido al MENOR costo?

- [ ] Desplegar un volumen `Cold HDD (sc1)` de 2 TB.
- [ ] Desplegar un volumen `Throughput Optimized HDD (st1)` de 2 TB.
- [x] Desplegar un volumen `General Purpose SSD (gp3)` de 2 TB. Establecer los IOPS en 10,000.
- [ ] Desplegar un volumen `Provisioned IOPS SSD (io2)` de 2 TB. Establecer los IOPS en 10,000.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa administra su entorno multi-cuenta usando AWS Organizations. La empresa necesita automatizar la creación de respaldos incrementales diarios de cualquier volumen de Amazon Elastic Block Store (Amazon EBS) que esté marcado con una etiqueta Lifecycle: Production en una de sus cuentas de AWS primarias. La empresa quiere evitar que los usuarios usen permisos `*` de Amazon EC2 para eliminar cualquiera de estas instantáneas de producción. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear una instantánea diaria de todos los volúmenes EBS usando Amazon Data Lifecycle Manager. Especificar Lifecycle como la clave de etiqueta. Especificar Production como el valor de etiqueta.
- [x] Asociar una Política de Control de Servicio (SCP) con la cuenta para denegar a los usuarios la capacidad de eliminar instantáneas de EBS. Crear una regla de Amazon EventBridge con una programación cron de 24 horas. Configurar EBS Create Snapshot como el destino. Dirigir a todos los volúmenes EBS con las etiquetas especificadas.
- [ ] Crear una instantánea diaria de todos los volúmenes EBS usando AWS Backup. Especificar Lifecycle como la clave de etiqueta. Especificar Production como el valor de etiqueta.
- [ ] Crear una Amazon Machine Image (AMI) diaria de cada instancia de EC2 de producción dentro de la cuenta de AWS usando Amazon Data Lifecycle Manager.

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación web acepta pedidos de usuarios en línea y coloca los pedidos en una cola de Amazon SQS. Las instancias de Amazon EC2 en un grupo de EC2 Auto Scaling leen los mensajes de la cola, procesan los pedidos, y envían por correo electrónico las confirmaciones de pedido a los usuarios. El grupo de Auto Scaling escala hacia arriba y hacia abajo según la profundidad de la cola. Al comienzo de cada día hábil, los usuarios reportan que los correos de confirmación se retrasan. ¿Qué acción resolverá este problema?

- [x] Crear una acción de escalado programado para escalar hacia arriba en anticipación al tráfico.
- [ ] Cambiar el grupo de Auto Scaling para escalar hacia arriba y hacia abajo según el uso de CPU.
- [ ] Cambiar la configuración de lanzamiento para lanzar tipos de instancia de EC2 más grandes.
- [ ] Modificar la política de escalado para desplegar más instancias de EC2 al escalar hacia arriba.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ha desarrollado un servicio que se despliega en una flota de instancias de Amazon EC2 basadas en Linux que están en un grupo de Auto Scaling. El servicio falla ocasionalmente de manera inesperada debido a un error en el código de la aplicación. El equipo de ingeniería de la empresa determina que resolver la causa subyacente de la falla del servicio podría tomar varias semanas. Un ingeniero de CloudOps necesita crear una solución para automatizar la recuperación si el servicio falla en cualquiera de las instancias de EC2. ¿Qué soluciones cumplen con este requisito? (Elija dos.)

- [ ] Instalar el agente de Amazon CloudWatch en las instancias de EC2. Configurar el agente de CloudWatch para monitorear el servicio. Establecer la acción de CloudWatch para reiniciar si falla la verificación de salud del servicio.
- [ ] Etiquetar las instancias de EC2. Crear una función de AWS Lambda que use AWS Systems Manager Session Manager para iniciar sesión en las instancias de EC2 etiquetadas y reiniciar el servicio. Programar la función Lambda para que se ejecute cada 5 minutos.
- [x] Etiquetar las instancias de EC2. Usar AWS Systems Manager State Manager para crear una asociación que use el documento `AWS-RunShellScript`. Configurar el comando de asociación con un script que verifique si el servicio se está ejecutando y que lo inicie si no lo está. Para los destinos, especificar la etiqueta de la instancia de EC2. Programar la asociación para que se ejecute cada 5 minutos.
- [x] Actualizar los datos de usuario de EC2 especificados en la plantilla de lanzamiento del grupo de Auto Scaling para incluir un script que se ejecute en una programación cron cada 5 minutos. Configurar el script para verificar si el servicio se está ejecutando y para iniciarlo si no lo está. Volver a desplegar todas las instancias de EC2 en el grupo de Auto Scaling con la plantilla de lanzamiento actualizada.
- [ ] Actualizar los datos de usuario de EC2 especificados en la plantilla de lanzamiento del grupo de Auto Scaling para asegurar que el servicio se ejecute durante el inicio. Volver a desplegar todas las instancias de EC2 en el grupo de Auto Scaling con la plantilla de lanzamiento actualizada.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está escribiendo una función de AWS Lambda en la Cuenta A de AWS para colocar objetos en un bucket de Amazon S3 en la Cuenta B de AWS. La función Lambda puede escribir exitosamente nuevos objetos en el bucket de S3, pero los usuarios de IAM en la Cuenta B no pueden eliminar objetos escritos en el bucket por la Cuenta A. ¿Qué paso corregirá este problema?

- [ ] Agregar el permiso `s3:DeleteObject` al rol de ejecución de IAM de la función de AWS Lambda en la Cuenta A.
- [ ] Cambiar la política del bucket de S3 en la Cuenta B para permitir el permiso `s3:DeleteObject` para la Cuenta A.
- [ ] Deshabilitar el cifrado del lado del servidor para los objetos escritos en el bucket de S3 por la función Lambda.
- [x] Modificar la función Lambda para llamar a la operación de API `s3:PutObjectAcl` y especificar bucket owner, full control.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita automatizar la invocación de una función de AWS Lambda. La función Lambda debe ejecutarse al final de cada día para generar un informe sobre datos almacenados en un bucket de Amazon S3. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que tenga un patrón de evento para Amazon S3 y la función Lambda como destino.
- [x] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que tenga una programación y la función Lambda como destino.
- [ ] Crear una notificación de eventos de S3 para invocar la función Lambda cada vez que los objetos cambien en el bucket de S3.
- [ ] Desplegar una instancia de Amazon EC2 con un cron job para invocar la función Lambda.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps tiene un sitio web de Amazon S3 y quiere restringir el acceso a una única distribución de Amazon CloudFront. Los visitantes del sitio web no deben poder eludir CloudFront ni ver el sitio web de S3 directamente desde el bucket. ¿Qué servicio o función de AWS cumple con estos requisitos?

- [ ] `ACL` del bucket de S3.
- [ ] AWS Firewall Manager.
- [ ] Zona alojada privada de Amazon Route 53.
- [x] Origin Access Identity (OAI).

**[⬆ Volver arriba](#table-of-contents)**

### Una aplicación que se ejecuta en Amazon EC2 permite a los usuarios lanzar trabajos por lotes (batch jobs) para análisis de datos. Los trabajos se ejecutan de forma asíncrona, y se notifica al usuario cuando se completan. Aunque pueden ejecutarse múltiples trabajos simultáneamente, la solicitud de un usuario no necesita cumplirse hasta dentro de 24 horas. Para ejecutar un trabajo, la aplicación lanza una instancia de EC2 adicional que realiza todos los cálculos analíticos. Un trabajo tarda entre 75 y 110 minutos en completarse y no se puede interrumpir. ¿Cuál es la forma MÁS rentable de ejecutar esta carga de trabajo?

- [ ] Ejecutar la aplicación en instancias de EC2 On-Demand. Ejecutar los trabajos en Instancias Spot con una duración especificada.
- [ ] Ejecutar la aplicación en instancias de EC2 Reservadas. Ejecutar los trabajos en AWS Lambda.
- [ ] Ejecutar la aplicación en instancias de EC2 On-Demand. Ejecutar los trabajos en instancias de EC2 On-Demand.
- [x] Ejecutar la aplicación en instancias de EC2 Reservadas. Ejecutar los trabajos en Instancias Spot con una duración especificada.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa de comercio electrónico quiere reducir costos en sus trabajos nocturnos que agregan las ventas del día actual y almacenan los resultados en Amazon S3. Los trabajos actualmente se ejecutan usando múltiples instancias on-demand y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier razón, debe reiniciarse desde el principio. ¿Qué método es el MÁS rentable según estos requisitos?

- [ ] Usar una combinación de Instancias On-Demand y Spot para la ejecución de trabajos.
- [x] Enviar una solicitud de Spot block para usar en la ejecución de trabajos.
- [ ] Comprar Instancias Reservadas para usar en la ejecución de trabajos.
- [ ] Enviar una solicitud de Instancia Spot única (one-time) para la ejecución de trabajos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa quiere reducir costos en trabajos que se pueden completar en cualquier momento. Los trabajos actualmente se ejecutan usando múltiples instancias On-Demand, y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier razón, se puede reiniciar desde el principio. ¿Qué método es el MÁS rentable según estos requisitos?

- [ ] Comprar Instancias Reservadas para usar en la ejecución de trabajos.
- [ ] Enviar una solicitud de Instancia Spot única (one-time) para la ejecución de trabajos.
- [x] Enviar una solicitud de Spot block para usar en la ejecución de trabajos.
- [ ] Usar una combinación de Instancias On-Demand y Spot para la ejecución de trabajos.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita recopilar el contenido de archivos de registro de una aplicación personalizada que está desplegada en cientos de instancias de Amazon EC2 que ejecutan Ubuntu. Los archivos de registro deben almacenarse en Amazon CloudWatch Logs. ¿Cómo debe el ingeniero de CloudOps recopilar los archivos de registro de la aplicación con el MENOR esfuerzo operativo?

- [ ] Configurar el servicio `syslogd` en cada instancia de EC2 para recopilar y enviar los archivos de registro de la aplicación a CloudWatch Logs.
- [ ] Instalar el agente de CloudWatch usando el administrador de paquetes de Amazon Linux en cada instancia de EC2. Configurar cada agente para recopilar los archivos de registro de la aplicación.
- [ ] Instalar el agente de CloudWatch en cada instancia de EC2 usando AWS Systems Manager. Crear una configuración de agente en cada instancia usando el asistente de configuración de CloudWatch. Configurar cada agente para recopilar los archivos de registro de la aplicación.
- [x] Almacenar una configuración del agente de CloudWatch en AWS Systems Manager Parameter Store. Instalar el agente de CloudWatch en cada instancia de EC2 usando Systems Manager. Configurar cada agente para recopilar los archivos de registro de la aplicación.

**[⬆ Volver arriba](#table-of-contents)**

### La política de seguridad de una empresa establece que no está permitido conectarse a instancias de Amazon EC2 mediante `SSH` y `RDP`. Si se requiere acceso, el personal autorizado puede conectarse a las instancias usando AWS Systems Manager Session Manager. Los usuarios reportan que no pueden conectarse a una instancia específica de Amazon EC2 que ejecuta Ubuntu y tiene preinstalado AWS Systems Manager Agent (SSM Agent). Estos usuarios pueden usar Session Manager para conectarse a otras instancias en la misma subred, y están en un grupo de IAM que tiene permiso de Session Manager para todas las instancias. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?

- [ ] Agregar una regla de entrada para el puerto `22` en el grupo de seguridad asociado con la instancia Ubuntu.
- [x] Asignar la política administrada `AmazonSSMManagedInstanceCore` al perfil de instancia de EC2 para la instancia Ubuntu.
- [ ] Configurar el SSM Agent para iniciar sesión con un nombre de usuario `ubuntu`.
- [ ] Generar un nuevo par de claves, configurar Session Manager para usar este nuevo par de claves, y proporcionar la clave privada a los usuarios.

**[⬆ Volver arriba](#table-of-contents)**


### Un ingeniero de CloudOps está creando un sitio web simple, orientado al público, que se ejecuta en Amazon EC2. El ingeniero de CloudOps creó la instancia de EC2 en una subred pública existente y asignó una dirección IP elástica a la instancia. Luego, el ingeniero de CloudOps creó y aplicó un nuevo grupo de seguridad a la instancia para permitir tráfico `HTTP` entrante desde `0.0.0.0/0`. Finalmente, el ingeniero de CloudOps creó una nueva `ACL` de red y la aplicó a la subred para permitir tráfico `HTTP` entrante desde `0.0.0.0/0`. Sin embargo, no se puede acceder al sitio web desde internet. ¿Cuál es la causa de este problema?

- [x] El ingeniero de CloudOps no creó una regla de salida que permita el tráfico de retorno de puertos efímeros en la nueva `ACL` de red.
- [ ] El ingeniero de CloudOps no creó una regla de salida en el grupo de seguridad que permita tráfico `HTTP` desde el puerto `80`.
- [ ] La dirección IP elástica asignada a la instancia de EC2 ha cambiado.
- [ ] Hay una `ACL` de red adicional asociada con la subred que incluye una regla que deniega el tráfico `HTTP` entrante desde el puerto `80`.

**[⬆ Volver arriba](#table-of-contents)**

### La infraestructura de la aplicación de una empresa se desplegó usando AWS CloudFormation y consiste en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias se ejecutan en un grupo de EC2 Auto Scaling en múltiples Zonas de disponibilidad. Al lanzar una nueva versión de la aplicación, el despliegue de actualización debe evitar cambios de `DNS` y permitir reversión (rollback). ¿Qué solución debe usar un ingeniero de CloudOps para cumplir con los requisitos de despliegue de este nuevo lanzamiento?

- [ ] Configurar el grupo de Auto Scaling para usar lifecycle hooks. Desplegar nuevas instancias con la nueva versión de la aplicación. Completar la acción del lifecycle hook una vez que estén saludables.
- [ ] Crear una nueva Amazon Machine Image (AMI) que contenga el código actualizado. Crear una configuración de lanzamiento con la AMI. Actualizar el grupo de Auto Scaling para usar la nueva configuración de lanzamiento.
- [ ] Desplegar un segundo stack de CloudFormation. Esperar a que la aplicación esté disponible. Cambiar al nuevo Application Load Balancer.
- [x] Modificar la plantilla de CloudFormation para usar una política `AutoScalingReplacingUpdate`. Actualizar el stack. Realizar una segunda actualización con el nuevo lanzamiento.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa usa un bucket de Amazon S3 para almacenar archivos de datos. El bucket de S3 contiene cientos de objetos. La empresa necesita reemplazar una etiqueta en todos los objetos del bucket de S3 por otra etiqueta. ¿Cuál es la forma MÁS eficiente operativamente de cumplir con este requisito?

- [x] Usar S3 Batch Operations. Especificar la operación para reemplazar todas las etiquetas de objeto.
- [ ] Usar la AWS CLI para obtener las etiquetas de cada objeto. Guardar las etiquetas en una lista. Usar S3 Batch Operations. Especificar la operación para eliminar todas las etiquetas de objeto. Usar la AWS CLI y la lista para volver a etiquetar los objetos.
- [ ] Usar la AWS CLI para obtener las etiquetas de cada objeto. Guardar las etiquetas en una lista. Usar la AWS CLI y la lista para eliminar las etiquetas de objeto. Usar la AWS CLI y la lista para volver a etiquetar los objetos.
- [ ] Usar la AWS CLI para copiar los objetos a otro bucket de S3. Agregar la nueva etiqueta a los objetos copiados. Eliminar los objetos originales.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene un clúster de instancias Spot de Amazon EC2 Linux que leen muchos archivos de, y escriben muchos archivos en, volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos. Las instancias de EC2 se inician y se detienen con frecuencia. Como parte del proceso cuando se inicia una instancia de EC2, se restaura un volumen EBS a partir de una instantánea. Los volúmenes EBS que se restauran a partir de instantáneas están experimentando un rendimiento inicial más bajo de lo esperado. La carga de trabajo de la empresa necesita casi todos los IOPS aprovisionados en los volúmenes EBS adjuntos. Las instancias de EC2 no pueden soportar la carga de trabajo cuando el rendimiento de los volúmenes EBS es demasiado bajo. Un ingeniero de CloudOps debe implementar una solución para asegurar que los volúmenes EBS proporcionen el rendimiento esperado cuando se restauren a partir de instantáneas. ¿Qué solución cumple con estos requisitos?

- [x] Configurar la restauración rápida de instantáneas (fast snapshot restore, FSR) en las instantáneas que se usan.
- [ ] Restaurar cada instantánea en un volumen EBS sin cifrar. Cifrar el volumen EBS cuando el rendimiento se estabilice.
- [ ] Formatear los volúmenes EBS como sistemas de archivos XFS antes de restaurar las instantáneas.
- [ ] Aumentar el búfer de lectura anticipada (read-ahead) de Linux a 1 MiB.

**[⬆ Volver arriba](#table-of-contents)**

### Los usuarios del sitio web reportan que las páginas de una aplicación se cargan lentamente al comienzo de la jornada laboral. La aplicación se ejecuta en instancias de Amazon EC2, y los datos se almacenan en una base de datos de Amazon RDS. El ingeniero de CloudOps sospecha que el problema está relacionado con el alto uso de CPU en un componente de esta aplicación. ¿Cómo puede el ingeniero descubrir qué componente está causando el cuello de botella de rendimiento?

- [ ] Usar AWS CloudTrail para revisar el historial de uso de recursos de cada componente.
- [x] Usar métricas de Amazon CloudWatch para examinar el uso de recursos de cada componente.
- [ ] Usar Amazon Inspector para ver los detalles de uso de recursos de cada componente.
- [ ] Usar Amazon CloudWatch Events para examinar los eventos de alto uso de cada componente.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene un bucket de Amazon S3 que contiene datos sensibles. Los datos deben cifrarse en tránsito y en reposo. La empresa cifra los datos en el bucket de S3 usando una clave de AWS Key Management Service (AWS KMS). Un desarrollador necesita otorgar a varias otras cuentas de AWS el permiso para usar la operación `GetObject` de S3 para recuperar los datos del bucket de S3. ¿Cómo puede el desarrollador exigir que todas las solicitudes para recuperar los datos proporcionen cifrado en tránsito?

- [x] Definir una política basada en recursos en el bucket de S3 para denegar el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.
- [ ] Definir una política basada en recursos en el bucket de S3 para permitir el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.
- [ ] Definir una política basada en roles en los roles de las otras cuentas para denegar el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.
- [ ] Definir una política basada en recursos en la clave KMS para denegar el acceso cuando una solicitud cumpla la condición `aws:SecureTransport`: `false`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está manteniendo una aplicación web usando una distribución web de Amazon CloudFront, un Application Load Balancer (ALB), Amazon RDS, y Amazon EC2 en una `VPC`. Todos los servicios tienen el registro habilitado. El ingeniero necesita investigar códigos de estado `HTTP` de Capa 7 de la aplicación web. ¿Qué fuentes de registro contienen los códigos de estado? (Elija dos.)

- [ ] `VPC` Flow Logs.
- [ ] Registros de AWS CloudTrail.
- [x] Registros de acceso del `ALB`.
- [x] Registros de acceso de CloudFront.
- [ ] Registros de RDS.

**[⬆ Volver arriba](#table-of-contents)**

### Después de un cambio de red, los servidores de aplicación no pueden conectarse a la base de datos correspondiente de Amazon RDS MySQL. ¿Qué debe analizar el ingeniero de CloudOps?

- [x] `VPC` Flow Logs.
- [ ] Registros de Elastic Load Balancing.
- [ ] Registros de Amazon CloudFront.
- [ ] Registros de error de Amazon RDS MySQL.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps configuró los flow logs de `VPC` usando el formato predeterminado. El ingeniero de CloudOps especificó Amazon CloudWatch Logs como destino. Esta solución ha funcionado exitosamente durante varios meses. Sin embargo, debido a requisitos adicionales de solución de problemas, el ingeniero de CloudOps necesita incluir el campo `tcp-flags` en los flow logs. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [x] Crear un nuevo flow log. Incluir el campo `tcp-flags` en el formato de registro personalizado. Eliminar el flow log original.
- [ ] En el grupo de registro de CloudWatch Logs, modificar el filtro para incluir el campo `tcp-flags` y el campo type.
- [ ] En CloudWatch Metrics, modificar la configuración de métrica para incluir el campo `tcp-flags`.
- [ ] Modificar el flow log existente. Incluir el campo `tcp-flags` y el campo type en el formato de registro personalizado. Guardar la configuración.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación en cientos de instancias de Amazon EC2 en tres Zonas de disponibilidad. La aplicación llama a una API de terceros a través de internet público. Un ingeniero de CloudOps debe proporcionar al tercero una lista de direcciones IP estáticas para que el tercero pueda permitir el tráfico desde la aplicación. ¿Qué solución cumple con estos requisitos?

- [x] Agregar una puerta de enlace `NAT` en la subred pública de cada Zona de disponibilidad. Hacer que la puerta de enlace `NAT` sea la ruta predeterminada de todas las subredes privadas en esas Zonas de disponibilidad.
- [ ] Asignar una dirección IP elástica en cada Zona de disponibilidad. Asociar la dirección IP elástica con todas las instancias en la Zona de disponibilidad.
- [ ] Colocar las instancias detrás de un Network Load Balancer (NLB). Enviar el tráfico a internet a través de la dirección IP privada del NLB.
- [ ] Actualizar la tabla de enrutamiento principal para enviar el tráfico a internet a través de una dirección IP elástica asignada a cada instancia.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está administrando una aplicación que se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias se ejecutan en un grupo de Auto Scaling en múltiples Zonas de disponibilidad. La aplicación almacena datos en una instancia de base de datos de Amazon RDS MySQL. El ingeniero debe asegurarse de que la aplicación permanezca disponible si la base de datos deja de responder. ¿Cómo se pueden cumplir estos requisitos?

- [ ] Crear réplicas de lectura para la base de datos RDS y usarlas en caso de una falla de base de datos.
- [ ] Crear una nueva instancia de RDS a partir de la instantánea de la instancia de RDS original si ocurre una falla.
- [ ] Mantener una base de datos RDS separada en ejecución y cambiar el endpoint en la aplicación web si ocurre una falla.
- [x] Modificar la instancia de RDS para que sea un despliegue Multi-AZ.

**[⬆ Volver arriba](#table-of-contents)**

### Los equipos de desarrollo mantienen varias cargas de trabajo en AWS. La gerencia de la empresa está preocupada por el aumento de costos y quiere que el ingeniero de CloudOps configure alertas para que los equipos sean notificados cuando el gasto se acerque a límites preestablecidos. ¿Qué servicio de AWS satisfará estos requisitos?

- [x] AWS Budgets.
- [ ] AWS Cost Explorer.
- [ ] AWS Trusted Advisor.
- [ ] AWS Cost and Usage Report.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está administrando una red `VPC` que consiste en subredes públicas y privadas. Las instancias en las subredes privadas acceden a internet a través de una puerta de enlace `NAT`. Una factura reciente de AWS muestra que los cargos de la puerta de enlace `NAT` se han duplicado. El ingeniero quiere identificar qué instancias están generando la mayor cantidad de tráfico de red. ¿Cómo se debe lograr esto?

- [x] Habilitar flow logs en la interfaz de red elástica de la puerta de enlace `NAT` y usar Amazon CloudWatch Insights para filtrar los datos según las direcciones IP de origen.
- [ ] Ejecutar un informe de AWS Cost and Usage y agrupar los hallazgos por ID de instancia.
- [ ] Usar la función de duplicación de tráfico (`VPC` traffic mirroring) para enviar tráfico a Amazon QuickSight.
- [ ] Usar las métricas de Amazon CloudWatch generadas por la puerta de enlace `NAT` para cada instancia individual.

**[⬆ Volver arriba](#table-of-contents)**

### Un equipo de aplicaciones le ha pedido a un ingeniero de CloudOps que aprovisione un entorno adicional para una aplicación en cuatro regiones adicionales. La aplicación se ejecuta en más de 100 instancias en `us-east-1`, usando AMI completamente preparadas (fully baked). Se ha creado una plantilla de AWS CloudFormation para desplegar recursos en `us-east-1`. ¿Qué debe hacer el ingeniero de CloudOps para aprovisionar la aplicación rápidamente?

- [x] Copiar la AMI a cada región usando `aws ec2 copy-image`. Actualizar el mapeo de CloudFormation para incluir mapeos para las AMI copiadas.
- [ ] Crear una instantánea de la instancia en ejecución y copiar la instantánea a las otras regiones. Crear una AMI a partir de las instantáneas. Actualizar la plantilla de CloudFormation para cada región para usar la nueva AMI.
- [ ] Ejecutar la plantilla de CloudFormation existente en cada región adicional basándose en el éxito de la plantilla usada actualmente en `us-east-1`.
- [ ] Actualizar la plantilla de CloudFormation para incluir las regiones adicionales en el grupo de Auto Scaling. Actualizar el stack existente en `us-east-1`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está intentando administrar sus costos en AWS Cloud. Un ingeniero de CloudOps necesita que etiquetas específicas definidas por la empresa y asignadas a recursos aparezcan en el informe de facturación. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Activar las etiquetas como etiquetas de asignación de costos generadas por AWS.
- [x] Activar las etiquetas como etiquetas de asignación de costos definidas por el usuario.
- [ ] Crear una nueva categoría de costos. Seleccionar la dimensión de facturación de cuenta.
- [ ] Crear un nuevo AWS Cost and Usage Report. Incluir los ID de recursos.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene un departamento de Ventas y un departamento de Marketing. La empresa usa una cuenta de AWS. Existe la necesidad de determinar qué cargos se generan en la plataforma de AWS por cada departamento. También existe la necesidad de recibir notificaciones cuando se aproxime o se supere un nivel de costo especificado. ¿Qué dos acciones debe tomar un ingeniero de CloudOps para lograr ambos requisitos con el MENOR esfuerzo administrativo? (Elija dos.)

- [ ] Usar AWS Trusted Advisor para obtener un informe que contenga los elementos verificados en el pilar de Optimización de Costos.
- [ ] Descargar el informe de facturación detallado, cargarlo en una base de datos, y hacer coincidir las líneas de partida con una lista de recursos conocidos por departamento.
- [x] Crear un script usando la AWS CLI para aplicar automáticamente etiquetas a los recursos existentes de cada departamento. Programar el script para que se ejecute semanalmente.
- [ ] Usar AWS Organizations para crear una Unidad Organizacional de departamento y permitir que solo el personal autorizado en cada departamento cree recursos.
- [x] Crear un presupuesto (Budget) desde la consola de Billing and Cost Management. Especificar el tipo de presupuesto como Cost, asignar etiquetas para cada departamento, definir notificaciones, y especificar cualquier otra opción según sea necesario.

**[⬆ Volver arriba](#table-of-contents)**

### El director financiero (CFO) de una organización ha notado un aumento en los costos de almacenamiento de Amazon S3 durante los últimos meses. Un ingeniero de CloudOps sospecha que estos costos están relacionados con el almacenamiento de versiones antiguas de objetos de S3 de uno de sus buckets de S3. ¿Qué puede hacer el ingeniero para confirmar esta sospecha?

- [x] Habilitar S3 Inventory y luego consultar el inventario para identificar el almacenamiento total de versiones de objeto anteriores.
- [ ] Usar etiquetas de asignación de costos a nivel de objeto para identificar el almacenamiento total de versiones de objeto anteriores.
- [ ] Habilitar la función de análisis de Amazon S3 para el bucket para identificar el almacenamiento total de versiones de objeto anteriores.
- [ ] Usar métricas de almacenamiento de Amazon CloudWatch para el bucket de S3 para identificar el almacenamiento total de versiones de objeto anteriores.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ejecutando una nueva promoción que resultará en un aumento masivo de tráfico para una sola aplicación. El ingeniero de CloudOps debe preparar la aplicación y asegurarse de que los clientes tengan una gran experiencia. La aplicación es intensiva en memoria y se ejecuta detrás de un AWS Application Load Balancer (ALB). El `ALB` ha sido precalentado (pre-warmed), y la aplicación está en un grupo de Auto Scaling. ¿Qué métrica integrada se debe usar para controlar la política de escalado del grupo de Auto Scaling?

- [ ] `RejectedConnectionCount`.
- [x] `RequestCountPerTarget`.
- [ ] `CPUUtilization`.
- [ ] `MemoryUtilization`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa planea expandirse a una región adicional de AWS con fines de recuperación ante desastres. La empresa usa AWS CloudFormation, y su infraestructura está bien definida como código. La empresa quisiera reutilizar la mayor cantidad posible de su código existente al desplegar recursos en regiones adicionales. Un ingeniero de CloudOps está revisando cómo se seleccionan las Amazon Machine Images (AMI) en AWS CloudFormation, pero tiene problemas para hacer que el mismo stack funcione en la nueva región. ¿Qué acción facilitaría la administración de múltiples regiones?

- [ ] Nombrar cada AMI en la nueva región exactamente igual que la AMI equivalente en la primera región.
- [ ] Duplicar el stack para que se puedan codificar nombres de AMI únicos en el stack apropiado.
- [ ] Crear un alias para cada AMI de modo que se pueda hacer referencia a una AMI por un nombre común entre regiones.
- [x] Crear una sección `Mappings` en el stack, y definir las asociaciones de región a AMI.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está administrando una cuenta de AWS donde los desarrolladores están autorizados a lanzar instancias de Amazon EC2 para probar código nuevo. Para limitar los costos, el ingeniero debe asegurarse de que las instancias de EC2 en la cuenta se terminen 24 horas después del lanzamiento. ¿Cómo debe el ingeniero cumplir con estos requisitos?

- [ ] Crear una alarma de Amazon CloudWatch basada en la métrica `CPUUtilization`. Cuando la métrica sea `0%` durante 24 horas, activar una acción para terminar la instancia de EC2 cuando se active la alarma.
- [x] Crear una función de AWS Lambda para verificar todas las instancias de EC2 y terminar las instancias que se ejecuten por más de 24 horas. Activar la función con un evento de Amazon CloudWatch Events cada 15 minutos.
- [ ] Agregar una acción a AWS Trusted Advisor para apagar instancias de EC2 según la verificación Low Utilization Amazon EC2 Instances, terminando las instancias identificadas por Trusted Advisor como en ejecución por más de 24 horas.
- [ ] Instalar el agente unificado de Amazon CloudWatch en cada instancia de EC2. Configurar el agente para terminar las instancias después de que se hayan ejecutado durante 24 horas.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está almacenando informes mensuales en Amazon S3. El requisito de seguridad de la empresa establece que el tráfico desde la `VPC` del cliente hacia Amazon S3 no puede atravesar internet. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Usar AWS Direct Connect y una interfaz virtual pública para conectarse a Amazon S3.
- [ ] Usar una puerta de enlace `NAT` administrada para conectarse a Amazon S3.
- [x] Desplegar un endpoint de `VPC` para conectarse a Amazon S3.
- [ ] Desplegar una puerta de enlace de internet para conectarse a Amazon S3.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa ejecuta una aplicación en instancias de Amazon EC2. Las instancias de EC2 están en un grupo de Auto Scaling y se ejecutan detrás de un Application Load Balancer (ALB). La aplicación experimenta errores cuando el total de solicitudes supera las 100 solicitudes por segundo. Un ingeniero de CloudOps debe recopilar información sobre el total de solicitudes durante un período de 2 semanas para determinar cuándo las solicitudes superaron este umbral. ¿Qué debe hacer el ingeniero de CloudOps para recopilar estos datos?

- [x] Usar la métrica `RequestCount` del `ALB`. Configurar un rango de tiempo de 2 semanas y un período de 1 minuto. Examinar el gráfico para determinar los horarios y volúmenes de tráfico pico.
- [ ] Usar la matemática de métricas de Amazon CloudWatch para generar una suma de los conteos de solicitudes de todas las instancias de EC2 durante un período de 2 semanas. Ordenar por un intervalo de 1 minuto.
- [ ] Crear métricas personalizadas de Amazon CloudWatch en las plantillas de configuración de lanzamiento de EC2 para crear métricas de solicitud agregadas en todas las instancias de EC2.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events). Configurar un patrón de coincidencia de eventos de EC2 que cree una métrica basada en solicitudes de EC2. Mostrar los datos en un gráfico.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita crear un informe que muestre cuántos bytes se envían y reciben de cada miembro del grupo de destino para un Application Load Balancer (ALB). ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [x] Habilitar el registro de acceso para el `ALB`. Guardar los registros en un bucket de Amazon S3.
- [ ] Instalar el agente de Amazon CloudWatch en las instancias del grupo de destino.
- [x] Usar Amazon Athena para consultar los registros del `ALB`. Consultar la tabla. Usar los campos `received_bytes` y `sent_bytes` para calcular el total de bytes agrupados por el campo de puerto de destino.
- [ ] Usar Amazon Athena para consultar los registros del `ALB`. Consultar la tabla. Usar los campos `received_bytes` y `sent_bytes` para calcular el total de bytes agrupados por el campo de puerto de cliente.
- [ ] Crear un panel de Amazon CloudWatch que muestre la estadística Sum de la métrica ProcessedBytes para el `ALB`.

**[⬆ Volver arriba](#table-of-contents)**

### El ingeniero de CloudOps de una empresa administra una flota de instancias de Amazon EC2 Windows que se ejecutan en una única cuenta de AWS. Las instancias tienen una etiqueta que incluye una clave `OS` y un valor `Windows`. La empresa usa AWS Systems Manager para parchar las instancias. La empresa ha instalado el agente de Amazon CloudWatch en las instancias, pero la configuración es inconsistente. El ingeniero de CloudOps necesita reconfigurar cada instancia para usar la misma configuración predefinida de CloudWatch. ¿Qué combinación de pasos cumple con estos requisitos? (Elija dos.)

- [ ] Almacenar el archivo de configuración del agente de CloudWatch en un bucket de Amazon S3.
- [ ] Almacenar el contenido del archivo de configuración del agente de CloudWatch en Systems Manager OpsCenter.
- [x] Almacenar el contenido del archivo de configuración del agente de CloudWatch en Systems Manager Parameter Store.
- [x] Crear una asociación de Systems Manager State Manager para ejecutar el documento de Systems Manager Run Command `AmazonCloudWatch-ManageAgent`. Seleccionar Systems Manager como fuente de configuración opcional. Dirigir a las instancias según los valores de etiqueta.
- [ ] Crear una asociación de Systems Manager State Manager para ejecutar el documento de Systems Manager Run Command `AmazonCloudWatch-ManageAgent`. Configurar el documento para usar la ubicación del bucket de S3 como fuente de configuración. Dirigir a las instancias según el valor de etiqueta.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que se ejecuta detrás de un Application Load Balancer (ALB) en la región `us-west-2`. Un conjunto de registros de Amazon Route 53 contiene un registro alias para `app.anycompany.com` que hace referencia al `ALB` en `us-west-2` y usa una política de enrutamiento simple. La aplicación está experimentando un aumento de usuarios de otras ubicaciones del mundo. Estos usuarios están experimentando alta latencia. La mayoría de los nuevos usuarios están cerca de la región `ap-southeast-2`. La empresa despliega una copia de la aplicación en `ap-southeast-2`. Un ingeniero de CloudOps debe implementar una solución que enrute automáticamente las solicitudes al endpoint de menor latencia para los usuarios sin cambiar la URL. ¿Qué solución cumple con estos requisitos?

- [ ] Agregar un nuevo valor al registro alias existente para `app.anycompany.com` con el nombre `DNS` del nuevo `ALB` en `ap-southeast-2`.
- [ ] Cambiar el registro alias existente para usar una política de enrutamiento por geolocalización. Crear dos registros de geolocalización, uno que haga referencia a cada ALB. Seleccionar la ubicación más cercana a cada región.
- [x] Cambiar el registro alias existente para usar una política de enrutamiento por latencia. Crear dos registros de latencia, uno que haga referencia a cada `ALB`.
- [ ] Cambiar el registro alias existente para usar una política de enrutamiento de valores múltiples (multivalue). Agregar el nombre `DNS` de cada `ALB` al registro.

**[⬆ Volver arriba](#table-of-contents)**


### Una empresa tiene dos cuentas de AWS: desarrollo y producción. Todas las aplicaciones envían registros a un bucket de Amazon S3 específico para cada cuenta, y los desarrolladores están solicitando acceso a los buckets de S3 de la cuenta de producción para ver los registros. ¿Cuál es la forma MÁS eficiente de proporcionar a los desarrolladores el acceso?

- [ ] Crear una función de AWS Lambda con un rol de IAM adjunto que tenga acceso a los buckets de S3 de ambas cuentas. Extraer los registros del bucket de S3 de producción al bucket de S3 de desarrollo.
- [ ] Crear usuarios de IAM para cada desarrollador en la cuenta de producción, y agregar a los desarrolladores a un grupo de IAM que proporcione acceso de solo lectura al bucket de registros de S3.
- [ ] Crear un bastion host de Amazon EC2 con un rol de IAM adjunto que tenga acceso al bucket de registros de S3 de producción, y luego aprovisionar acceso para los desarrolladores en el host.
- [x] Crear una política basada en recursos para el bucket de S3 en la cuenta de producción que otorgue acceso a la cuenta de desarrollo, y luego delegar el acceso en la cuenta de desarrollo.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una política que establece que todos los registros de instancias de Amazon EC2 deben publicarse en Amazon CloudWatch Logs. Un ingeniero de CloudOps está solucionando problemas de una instancia de EC2 que ejecuta Amazon Linux 2. La instancia de EC2 no está publicando registros en CloudWatch Logs. El agente de Amazon CloudWatch se está ejecutando en la instancia de EC2, y el archivo de configuración del agente es correcto. ¿Qué debe hacer el ingeniero de CloudOps para resolver el problema?

- [ ] Configurar la AWS CLI en la instancia de EC2. Crear un cron job que llame a la operación de API `PutLogEvents` para enviar los archivos de registro a CloudWatch cada 5 minutos.
- [ ] Inspeccionar el período de retención del grupo de registro de CloudWatch Logs. Asegurarse de que el período de retención esté establecido en un valor mayor a 1 día.
- [ ] Configurar un flujo de datos de Amazon Kinesis que se ejecute en la misma región de AWS que la instancia de EC2. Configurar el agente de CloudWatch en la instancia de EC2 para enviar eventos de CloudWatch al flujo de datos.
- [x] Asegurarse de que el rol de IAM adjunto a la instancia de EC2 tenga permisos en CloudWatch Logs para las acciones `CreateLogGroup`, `CreateLogStream`, `PutLogEvents`, y `DescribeLogStreams`.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa está ejecutando un sitio popular de redes sociales en instancias de EC2. La aplicación almacena datos en una instancia de base de datos de Amazon RDS para MySQL y ha implementado caché de lectura usando un clúster de ElastiCache for Redis (modo clúster habilitado) para mejorar los tiempos de lectura. Un evento social ocurrirá durante el fin de semana, y el ingeniero de CloudOps espera que el tráfico del sitio web se triplique. ¿Qué puede hacer un ingeniero de CloudOps para asegurar tiempos de lectura mejorados para los usuarios durante el evento social?

- [ ] Usar Amazon RDS Multi-AZ.
- [x] Agregar shards al clúster de Redis existente.
- [ ] Descargar los datos estáticos a Amazon S3.
- [ ] Lanzar un segundo clúster de Redis Multi-AZ.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps está rediseñando la arquitectura de una aplicación. El ingeniero de CloudOps ha movido la base de datos de una subred pública, donde la base de datos usaba un endpoint público, a una subred privada para restringir el acceso desde la red pública. Después de este cambio, una función de AWS Lambda que requiere acceso de lectura a la base de datos no puede conectarse a la base de datos. El ingeniero de CloudOps debe resolver este problema sin comprometer la seguridad. ¿Qué solución cumple con estos requisitos?

- [x] Crear un endpoint de interfaz de AWS PrivateLink para la función Lambda. Conectarse a la base de datos usando su endpoint privado.
- [ ] Conectar la función Lambda a la `VPC` de la base de datos. Conectarse a la base de datos usando su endpoint privado.
- [ ] Adjuntar un rol de IAM a la función Lambda con permisos de lectura a la base de datos.
- [ ] Mover la base de datos a una subred pública. Usar grupos de seguridad para acceso seguro.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps ha implementado un diseño de red `VPC` con los siguientes requisitos: Dos Zonas de disponibilidad (`AZ`). Dos subredes privadas. Dos subredes públicas. Una puerta de enlace de internet. Una puerta de enlace `NAT`. ¿Qué podría causar que las aplicaciones en la `VPC` fallen durante una interrupción de `AZ`?

- [ ] Una única puerta de enlace privada virtual, porque solo puede asociarse con una única `AZ`.
- [ ] Una única puerta de enlace de internet, porque no es redundante entre ambas `AZ`.
- [x] Una única puerta de enlace `NAT`, porque no es redundante entre ambas `AZ`.
- [ ] La tabla de enrutamiento principal predeterminada de la `VPC`, porque solo puede asociarse con una única `AZ`.

**[⬆ Volver arriba](#table-of-contents)**

### Una organización almacena datos sensibles de clientes en buckets de S3 protegidos por políticas de bucket. Recientemente, ha habido reportes de que entidades no autorizadas dentro de la empresa han estado intentando acceder a los datos en esos buckets de S3. El director de seguridad de la información (CISO) quisiera saber qué buckets están siendo objetivo y determinar quién es responsable de intentar acceder a esa información. ¿Qué pasos debe tomar un ingeniero de CloudOps para cumplir con el requisito del CISO? (Elija dos.)

- [ ] Habilitar Amazon S3 Analytics en todos los buckets de S3 afectados para obtener un informe de qué buckets están siendo accedidos sin autorización.
- [x] Habilitar el registro de acceso del servidor (S3 Server Access Logging) de Amazon S3 en todos los buckets de S3 afectados y hacer que los registros se almacenen en un bucket dedicado para registros.
- [ ] Usar Amazon Athena para consultar el informe de S3 Analytics en busca de errores `HTTP` `403`, y determinar el usuario o rol de IAM que hace las solicitudes.
- [x] Usar Amazon Athena para consultar los registros de acceso del servidor de S3 en busca de errores `HTTP` `403`, y determinar el usuario o rol de IAM que hace las solicitudes.
- [ ] Usar Amazon Athena para consultar los registros de acceso del servidor de S3 en busca de errores `HTTP` `503`, y determinar el usuario o rol de IAM que hace las solicitudes.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa se está preparando para una campaña de marketing que aumentará el tráfico hacia una nueva aplicación web. La aplicación usa Amazon API Gateway y AWS Lambda para la lógica de la aplicación. La aplicación almacena datos relevantes de usuario en un clúster de base de datos Amazon Aurora MySQL que tiene una réplica de Aurora. Las consultas de base de datos de la aplicación son `5%` de escritura y `95%` de lectura. ¿Qué debe hacer un ingeniero de CloudOps para escalar la base de datos cuando aumente el tráfico?

- [x] Configurar Aurora Auto Scaling para agregar o quitar réplicas de Aurora en el clúster según el uso promedio de CPU de las réplicas de Aurora.
- [ ] Configurar Aurora Auto Scaling para aumentar o disminuir el tamaño de las réplicas de Aurora según el uso promedio de CPU de las réplicas de Aurora.
- [ ] Configurar AWS Auto Scaling para monitorear el clúster de Aurora. Configurar AWS Auto Scaling para agregar o quitar réplicas de Aurora en el clúster según el uso promedio de CPU de la instancia primaria.
- [ ] Configurar AWS Auto Scaling para monitorear el clúster de Aurora. Configurar AWS Auto Scaling para agregar o quitar réplicas de Aurora en el clúster según el uso promedio de CPU de la réplica de Aurora existente.

**[⬆ Volver arriba](#table-of-contents)**

### Una instancia de Amazon EC2 en una subred privada necesita copiar datos a un bucket de Amazon S3. Por razones de seguridad, la conexión desde la instancia de EC2 a Amazon S3 no debe atravesar internet. ¿Qué acción debe tomar el ingeniero de CloudOps para lograr esto?

- [ ] Crear una instancia `NAT` y enrutar el tráfico destinado a Amazon S3 a través de ella.
- [ ] Crear una conexión `VPN` entre la instancia de EC2 y Amazon S3.
- [x] Crear un endpoint de `VPC` de S3 en la `VPC` donde reside la instancia de EC2.
- [ ] Usar AWS Direct Connect para maximizar el rendimiento y mantener el tráfico privado.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación web pública existente para `www.example.com`. El Application Load Balancer (ALB) está configurado con un único listener `HTTP` en el puerto `80`. Un ingeniero de CloudOps debe asegurarse de que todas las solicitudes web a `www.example.com` estén cifradas entre el cliente y el `ALB`. El ingeniero de CloudOps ya ha solicitado y validado un certificado público para `www.example.com` en AWS Certificate Manager (ACM). Los usuarios existentes de la aplicación no deben tener que cambiar el endpoint al que se conectan. ¿Qué conjunto adicional de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear un listener adicional del `ALB` para `HTTPS` en el puerto `443`. Establecer la acción predeterminada para reenviar todo el tráfico al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado.
- [ ] Crear un listener adicional del `ALB` para `HTTPS` en el puerto `443`. Establecer la acción predeterminada para reenviar todo el tráfico al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado. Eliminar el listener `HTTP` original en el puerto `80`.
- [ ] Modificar la regla predeterminada del `ALB` para el listener `HTTP` del puerto `80`. Crear una regla en el listener para reenviar todo el tráfico del host www.example.com al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado.
- [x] Modificar la regla predeterminada del `ALB` para el listener `HTTP` del puerto `80` para redirigir a `HTTPS` en el puerto `443`. Crear un listener adicional de `HTTPS` en el puerto `443`. Establecer la acción predeterminada para reenviar todo el tráfico al grupo de destino. Especificar el certificado de ACM creado para `www.example.com` como el certificado SSL predeterminado.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps necesita configurar la zona alojada de Amazon Route 53 para `example.com` y `www.example.com` para que apunten a un Application Load Balancer (ALB). ¿Qué combinación de acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Configurar un registro `A` para `example.com` que apunte a la dirección IP del `ALB`.
- [ ] Configurar un registro `A` para `www.example.com` que apunte a la dirección IP del `ALB`.
- [x] Configurar un registro alias para `example.com` que apunte al `CNAME` del `ALB`.
- [x] Configurar un registro alias para `www.example.com` que apunte al registro `example.com` de Route 53.
- [ ] Configurar un registro `CNAME` para `example.com` que apunte al `CNAME` del `ALB`.

**[⬆ Volver arriba](#table-of-contents)**

### Un ingeniero de CloudOps creó una función de AWS Lambda dentro de una `VPC` sin acceso a internet. La función Lambda extrae mensajes de una cola de Amazon SQS y los almacena en una instancia de Amazon RDS en la misma `VPC`. Después de ejecutar la función Lambda, los datos no aparecen en la instancia de RDS. ¿Cuáles de las siguientes son posibles causas de esto? (Elija dos.)

- [ ] No se ha creado un endpoint de `VPC` para Amazon RDS.
- [x] No se ha creado un endpoint de `VPC` para Amazon SQS.
- [x] El grupo de seguridad de RDS no permite conexiones desde la función Lambda.
- [ ] La subred asociada con la función Lambda no tiene una puerta de enlace de internet adjunta.
- [ ] La subred asociada con la función Lambda tiene una puerta de enlace `NAT`.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. ¿Cuál de las siguientes afirmaciones NO es verdadera en este escenario?

- [x] La `VPC` creará una instancia de enrutamiento y la adjuntará a una subred pública.
- [ ] La `VPC` creará dos subredes.
- [ ] La `VPC` creará una puerta de enlace de internet y la adjuntará a la `VPC`.
- [ ] La `VPC` lanzará una instancia NAT con una IP elástica.

**[⬆ Volver arriba](#table-of-contents)**

### Una empresa tiene una aplicación que usa una función programada de AWS Lambda para recuperar conjuntos de datos de fuentes externas a través de internet. La función no está asociada con una `VPC`. La empresa está modificando la aplicación para almacenar la información que la función Lambda recupera en una instancia de base de datos de Amazon RDS en una subred privada. La `VPC` tiene dos subredes públicas y dos subredes privadas. Un ingeniero de CloudOps debe desplegar una solución que permita a la función Lambda acceder a la nueva base de datos y continuar accediendo a internet. ¿Qué solución cumple con estos requisitos?

- [ ] Crear una nueva función Lambda con acceso `VPC` y una dirección IP elástica. Adjuntar la función a subredes públicas en dos Zonas de disponibilidad. Asociar un grupo de seguridad con la dirección IP elástica. Configurar las reglas de salida del grupo de seguridad para permitir que Lambda acceda a los recursos requeridos.
- [ ] Crear una nueva función Lambda con acceso `VPC` y dos direcciones IP públicas. Adjuntar la función a subredes públicas en las mismas Zonas de disponibilidad que usa la base de datos. Asociar un grupo de seguridad con la función. Configurar las reglas de entrada del grupo de seguridad para permitir que Lambda acceda a los recursos requeridos.
- [x] Reconfigurar la función Lambda para acceso `VPC`. Agregar puertas de enlace `NAT` a las subredes públicas en la `VPC`. Agregar entradas de tabla de enrutamiento en las subredes privadas para enrutar a través de las puertas de enlace `NAT` hacia internet. Adjuntar la función a las subredes privadas que soportan la base de datos. Asociar un grupo de seguridad con la función. Configurar las reglas de salida del grupo de seguridad para permitir que Lambda acceda a internet.
- [ ] Reconfigurar la función Lambda para acceso `VPC`. Adjuntar la función a las subredes privadas. Agregar entradas de tabla de enrutamiento en las subredes privadas para enrutar a través de la puerta de enlace de internet hacia internet. Asociar un grupo de seguridad con las subredes. Configurar las reglas de entrada del grupo de seguridad para permitir que Lambda acceda a los recursos requeridos a través de la puerta de enlace de internet.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred privada usa `CIDR` `20.0.0.0/24`. El ID de la instancia `NAT` es `i-a12345`. ¿Cuál de las siguientes entradas se requiere en la tabla de enrutamiento principal adjunta a la subred privada para permitir que las instancias se conecten a internet?

- [x] Destino: `0.0.0.0/0` y Destino: `i-a12345`.
- [ ] Destino: `20.0.0.0/0` y Destino: `80`.
- [ ] Destino: `20.0.0.0/0` y Destino: `i-a12345`.
- [ ] Destino: `20.0.0.0/24` y Destino: `i-a12345`.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. ¿Cuál de las siguientes afirmaciones es verdadera en este escenario?

- [ ] La `VPC` de AWS creará automáticamente una instancia `NAT` de tamaño micro.
- [x] La `VPC` vincula la tabla de enrutamiento principal con una subred privada y una tabla de enrutamiento personalizada con una subred pública.
- [ ] El usuario debe crear manualmente una instancia `NAT`.
- [ ] La `VPC` vincula la tabla de enrutamiento principal con una subred pública y una tabla de enrutamiento personalizada con una subred privada.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred privada usa `CIDR` `20.0.0.0/24`. ¿Cuál de las siguientes entradas se requiere en la tabla de enrutamiento principal para permitir que las instancias en la `VPC` se comuniquen entre sí?

- [ ] Destino: `20.0.0.0/24` y Destino: `VPC`.
- [x] Destino: `20.0.0.0/16` y Destino: `Local`.
- [ ] Destino: `20.0.0.0/0` y Destino: `ALL`.
- [ ] Destino: `20.0.0.0/24` y Destino: `Local`.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. El usuario no ha lanzado ninguna instancia manualmente y está intentando eliminar la `VPC`. ¿Qué sucederá en este escenario?

- [ ] No permitirá eliminar la `VPC` ya que tiene subredes con tablas de enrutamiento.
- [ ] No permitirá eliminar la `VPC` ya que tiene una instancia de enrutamiento en ejecución.
- [ ] Terminará la `VPC` junto con todas las instancias lanzadas por el asistente.
- [x] No permitirá eliminar la `VPC` ya que tiene una instancia `NAT` en ejecución.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred pública usa `CIDR` `20.0.1.0/24`. El usuario planea alojar un servidor web en la subred pública (puerto `80`) y un servidor de base de datos en la subred privada (puerto `3306`). El usuario está configurando un grupo de seguridad para la subred pública (`WebSecGrp`) y la subred privada (`DBSecGrp`). ¿Cuál de las siguientes entradas se requiere en el grupo de seguridad del servidor web (`WebSecGrp`)?

- [ ] Configurar `Destination` como el ID del grupo de seguridad de la base de datos (`DbSecGrp`) para el puerto `3306` de salida.
- [ ] `80` para `Destination` `0.0.0.0/0` de salida.
- [ ] Configurar el puerto `3306` para origen `20.0.0.0/24` de entrada.
- [x] Configurar el puerto `80` de entrada para origen `20.0.0.0/16`.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado una subred pública `CIDR` `20.0.0.0/24` y subredes solo `VPN` `CIDR` `20.0.1.0/24` junto con la puerta de enlace `VPN` `vgw-12345` para conectarse al centro de datos del usuario. ¿Cuál de las siguientes opciones es una entrada válida para la tabla de enrutamiento principal en este escenario?

- [ ] Destino: `20.0.0.0/24` y Destino: `vgw-12345`.
- [ ] Destino: `20.0.0.0/16` y Destino: `ALL`.
- [ ] Destino: `20.0.1.0/16` y Destino: `vgw-12345`.
- [x] Destino: `0.0.0.0/0` y Destino: `vgw-12345`.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con subredes públicas y privadas usando el asistente de `VPC`. La `VPC` tiene `CIDR` `20.0.0.0/16`. La subred pública usa `CIDR` `20.0.1.0/24`. El usuario planea alojar un servidor web en la subred pública (puerto `80`) y un servidor de base de datos en la subred privada (puerto `3306`). El usuario está configurando un grupo de seguridad para la subred pública (`WebSecGrp`) y la subred privada (`DBSecGrp`). ¿Cuál de las siguientes entradas se requiere en el grupo de seguridad de la base de datos de la subred privada (`DBSecGrp`)?

- [x] Permitir entrada en el puerto `3306` para origen el grupo de seguridad del servidor web (`WebSecGrp`).
- [ ] Permitir entrada en el puerto `3306` desde origen `20.0.0.0/16`.
- [ ] Permitir salida en el puerto `3306` para destino el grupo de seguridad del servidor web (`WebSecGrp`).
- [ ] Permitir salida en el puerto `80` para destino la IP de la instancia `NAT`.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente de `VPC`. El usuario ha creado un `CIDR` público `20.0.0.0/24` y una subred solo `VPN` `CIDR` `20.0.1.0/24` junto con el acceso `VPN` de hardware para conectarse al centro de datos del usuario. ¿Cuál de los siguientes componentes NO está presente cuando la `VPC` se configura con el asistente?

- [ ] Tabla de enrutamiento principal adjunta con una subred solo `VPN`.
- [x] Una instancia `NAT` configurada para permitir que las instancias de la subred `VPN` se conecten a internet.
- [ ] Tabla de enrutamiento personalizada adjunta con una subred pública.
- [ ] Una puerta de enlace de internet para una subred pública.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado subredes públicas y solo `VPN` junto con acceso `VPN` de hardware para conectarse al centro de datos del usuario. El usuario aún no ha lanzado ninguna instancia ni ha modificado o eliminado ninguna configuración. Quiere eliminar esta `VPC` desde la consola. ¿La consola permitirá al usuario eliminar la `VPC`?

- [ ] Sí, la consola eliminará todas las configuraciones y también eliminará la puerta de enlace privada virtual.
- [x] No, la consola le pedirá al usuario que desconecte manualmente la puerta de enlace privada virtual primero y luego permitirá eliminar la `VPC`.
- [ ] Sí, la consola eliminará todas las configuraciones y desconectará la puerta de enlace privada virtual.
- [ ] No, ya que la instancia `NAT` está en ejecución.

**[⬆ Volver arriba](#table-of-contents)**

### Un usuario ha creado una `VPC` con `CIDR` `20.0.0.0/16` usando el asistente. El usuario ha creado una subred pública `CIDR` `20.0.0.0/24` y subredes solo `VPN` `CIDR` `20.0.1.0/24` junto con la puerta de enlace `VPN` `vgw-12345` para conectarse al centro de datos del usuario. El centro de datos del usuario tiene `CIDR` `172.28.0.0/12`. El usuario también ha configurado una instancia `NAT` `i-123456` para permitir tráfico a internet desde la subred `VPN`. ¿Cuál de las siguientes opciones NO es una entrada válida para la tabla de enrutamiento principal en este escenario?

- [x] Destino: `20.0.1.0/24` y Destino: `i-12345`.
- [ ] Destino: `0.0.0.0/0` y Destino: `i-12345`.
- [ ] Destino: `172.28.0.0/12` y Destino: `vgw-12345`.
- [ ] Destino: `20.0.0.0/16` y Destino: `local`.

**[⬆ Volver arriba](#table-of-contents)**
