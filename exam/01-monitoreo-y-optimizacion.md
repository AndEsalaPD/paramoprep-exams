# Dominio 1: Monitoreo, registro, análisis, remediación y optimización del rendimiento (22 %)

Preguntas de práctica AWS Certified CloudOps Engineer – Associate (SOA-C03) — 106 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [Un ingeniero de CloudOps ha habilitado AWS CloudTrail en una cuenta de AWS. Si CloudTrail se deshabilita, debe volver a habilitarse de inmediato. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos SIN escribir código personalizado?](#un-ingeniero-de-cloudops-ha-habilitado-aws-cloudtrail-en-una-cuenta-de-aws-si-cloudtrail-se-deshabilita-debe-volver-a-habilitarse-de-inmediato-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-sin-escribir-código-personalizado) |
| 2 | [Una empresa utiliza un sistema de archivos de Amazon Elastic File System (Amazon EFS) para compartir archivos entre muchas instancias de Amazon EC2 con Linux. Un ingeniero de CloudOps observa que la métrica `PercentIOLimit` del sistema de archivos se mantiene consistentemente en `100%` durante 15 minutos o más. El ingeniero de CloudOps también observa que la aplicación que lee y escribe en ese sistema de archivos tiene un rendimiento deficiente. La aplicación requiere alto throughput y muchas IOPS al acceder al sistema de archivos. ¿Qué debe hacer el ingeniero de CloudOps para remediar la métrica `PercentIOLimit` consistentemente alta?](#una-empresa-utiliza-un-sistema-de-archivos-de-amazon-elastic-file-system-amazon-efs-para-compartir-archivos-entre-muchas-instancias-de-amazon-ec2-con-linux-un-ingeniero-de-cloudops-observa-que-la-métrica-percentiolimit-del-sistema-de-archivos-se-mantiene-consistentemente-en-100-durante-15-minutos-o-más-el-ingeniero-de-cloudops-también-observa-que-la-aplicación-que-lee-y-escribe-en-ese-sistema-de-archivos-tiene-un-rendimiento-deficiente-la-aplicación-requiere-alto-throughput-y-muchas-iops-al-acceder-al-sistema-de-archivos-qué-debe-hacer-el-ingeniero-de-cloudops-para-remediar-la-métrica-percentiolimit-consistentemente-alta) |
| 3 | [Una empresa migró una aplicación intensiva en operaciones de E/S a una instancia de Amazon EC2 de propósito general. La instancia de EC2 tiene adjunto un único volumen de Amazon Elastic Block Store (Amazon EBS) de tipo General Purpose SSD. Los usuarios de la aplicación reportan que ciertas acciones que requieren lectura y escritura intensivas en disco tardan mucho más de lo normal o fallan por completo. Al revisar las métricas de rendimiento del volumen de EBS, un ingeniero de CloudOps observa que la métrica `VolumeQueueLength` se mantiene consistentemente alta durante los mismos períodos en los que los usuarios reportan problemas. El ingeniero de CloudOps necesita resolver este problema para restaurar el rendimiento completo de la aplicación. ¿Qué acción cumple con estos requisitos?](#una-empresa-migró-una-aplicación-intensiva-en-operaciones-de-es-a-una-instancia-de-amazon-ec2-de-propósito-general-la-instancia-de-ec2-tiene-adjunto-un-único-volumen-de-amazon-elastic-block-store-amazon-ebs-de-tipo-general-purpose-ssd-los-usuarios-de-la-aplicación-reportan-que-ciertas-acciones-que-requieren-lectura-y-escritura-intensivas-en-disco-tardan-mucho-más-de-lo-normal-o-fallan-por-completo-al-revisar-las-métricas-de-rendimiento-del-volumen-de-ebs-un-ingeniero-de-cloudops-observa-que-la-métrica-volumequeuelength-se-mantiene-consistentemente-alta-durante-los-mismos-períodos-en-los-que-los-usuarios-reportan-problemas-el-ingeniero-de-cloudops-necesita-resolver-este-problema-para-restaurar-el-rendimiento-completo-de-la-aplicación-qué-acción-cumple-con-estos-requisitos) |
| 4 | [Una empresa tiene una política que exige que todas las instancias de Amazon EC2 tengan un conjunto específico de etiquetas (tags). Si una instancia de EC2 no tiene las etiquetas requeridas, la instancia no conforme debe terminarse. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-tiene-una-política-que-exige-que-todas-las-instancias-de-amazon-ec2-tengan-un-conjunto-específico-de-etiquetas-tags-si-una-instancia-de-ec2-no-tiene-las-etiquetas-requeridas-la-instancia-no-conforme-debe-terminarse-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 5 | [Una empresa tiene múltiples instancias de Amazon EC2 que ejecutan una aplicación intensiva en recursos en un entorno de desarrollo. Un ingeniero de CloudOps está implementando una solución para detener estas instancias de EC2 cuando no están en uso. ¿Qué solución cumple con este requisito?](#una-empresa-tiene-múltiples-instancias-de-amazon-ec2-que-ejecutan-una-aplicación-intensiva-en-recursos-en-un-entorno-de-desarrollo-un-ingeniero-de-cloudops-está-implementando-una-solución-para-detener-estas-instancias-de-ec2-cuando-no-están-en-uso-qué-solución-cumple-con-este-requisito) |
| 6 | [Un ingeniero de CloudOps es responsable de una aplicación heredada (legacy) intensiva en CPU. La aplicación solo puede escalarse verticalmente. Actualmente, la aplicación está desplegada en una única instancia de Amazon EC2 `t2.large`. El sistema muestra un uso de CPU del `90%` y una latencia de rendimiento significativa después de unos minutos. ¿Qué cambio se debe hacer para aliviar el problema de rendimiento?](#un-ingeniero-de-cloudops-es-responsable-de-una-aplicación-heredada-legacy-intensiva-en-cpu-la-aplicación-solo-puede-escalarse-verticalmente-actualmente-la-aplicación-está-desplegada-en-una-única-instancia-de-amazon-ec2-t2large-el-sistema-muestra-un-uso-de-cpu-del-90-y-una-latencia-de-rendimiento-significativa-después-de-unos-minutos-qué-cambio-se-debe-hacer-para-aliviar-el-problema-de-rendimiento) |
| 7 | [Una empresa tiene una aplicación crítica sin servidor (serverless) que utiliza múltiples funciones de AWS Lambda. Cada función Lambda genera `1 GB` de datos de registro diariamente en su propio grupo de registros (log group) de Amazon CloudWatch Logs. El equipo de seguridad de la empresa solicita un conteo de errores de la aplicación, agrupados por tipo, en todos los grupos de registros. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-tiene-una-aplicación-crítica-sin-servidor-serverless-que-utiliza-múltiples-funciones-de-aws-lambda-cada-función-lambda-genera-1-gb-de-datos-de-registro-diariamente-en-su-propio-grupo-de-registros-log-group-de-amazon-cloudwatch-logs-el-equipo-de-seguridad-de-la-empresa-solicita-un-conteo-de-errores-de-la-aplicación-agrupados-por-tipo-en-todos-los-grupos-de-registros-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 8 | [Un ingeniero de CloudOps ha lanzado una instancia de Amazon EC2 de propósito general de tamaño grande para procesar regularmente archivos de datos de gran tamaño. La instancia tiene adjunto un volumen de Amazon Elastic Block Store (Amazon EBS) de 1 TB de tipo `General Purpose SSD (gp2)`. La instancia también está optimizada para EBS. Para ahorrar costos, el ingeniero de CloudOps detiene la instancia cada noche y la reinicia cada mañana. Cuando el procesamiento de datos está activo, las métricas de Amazon CloudWatch de la instancia muestran consistentemente 3.000 `VolumeReadOps`. El ingeniero de CloudOps debe mejorar el rendimiento de E/S garantizando la integridad de los datos. ¿Qué acción cumple con estos requisitos?](#un-ingeniero-de-cloudops-ha-lanzado-una-instancia-de-amazon-ec2-de-propósito-general-de-tamaño-grande-para-procesar-regularmente-archivos-de-datos-de-gran-tamaño-la-instancia-tiene-adjunto-un-volumen-de-amazon-elastic-block-store-amazon-ebs-de-1-tb-de-tipo-general-purpose-ssd-gp2-la-instancia-también-está-optimizada-para-ebs-para-ahorrar-costos-el-ingeniero-de-cloudops-detiene-la-instancia-cada-noche-y-la-reinicia-cada-mañana-cuando-el-procesamiento-de-datos-está-activo-las-métricas-de-amazon-cloudwatch-de-la-instancia-muestran-consistentemente-3000-volumereadops-el-ingeniero-de-cloudops-debe-mejorar-el-rendimiento-de-es-garantizando-la-integridad-de-los-datos-qué-acción-cumple-con-estos-requisitos) |
| 9 | [Una empresa ejecuta cargas de trabajo en 90 instancias de Amazon EC2 en la región `eu-west-1` dentro de una cuenta de AWS. En 2 meses, la empresa migrará las cargas de trabajo de `eu-west-1` a la región `eu-west-3`. La empresa necesita reducir el costo de las instancias de EC2. La empresa está dispuesta a asumir un compromiso de 1 año que comenzará la próxima semana. La empresa debe elegir una opción de compra de instancias de EC2 que proporcione descuentos para las 90 instancias de EC2 sin importar la región durante el período de 1 año. ¿Qué solución cumple con estos requisitos?](#una-empresa-ejecuta-cargas-de-trabajo-en-90-instancias-de-amazon-ec2-en-la-región-eu-west-1-dentro-de-una-cuenta-de-aws-en-2-meses-la-empresa-migrará-las-cargas-de-trabajo-de-eu-west-1-a-la-región-eu-west-3-la-empresa-necesita-reducir-el-costo-de-las-instancias-de-ec2-la-empresa-está-dispuesta-a-asumir-un-compromiso-de-1-año-que-comenzará-la-próxima-semana-la-empresa-debe-elegir-una-opción-de-compra-de-instancias-de-ec2-que-proporcione-descuentos-para-las-90-instancias-de-ec2-sin-importar-la-región-durante-el-período-de-1-año-qué-solución-cumple-con-estos-requisitos) |
| 10 | [Un ingeniero de CloudOps necesita crear alertas basadas en las métricas de lectura y escritura de volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos a una instancia de Amazon EC2. El ingeniero de CloudOps crea y habilita alarmas de Amazon CloudWatch para la métrica `DiskReadBytes` y la métrica `DiskWriteBytes`. Una herramienta de monitoreo personalizada instalada en la instancia de EC2, con la misma configuración de alarma, indica que las métricas del volumen han superado el umbral. Sin embargo, las alarmas de CloudWatch no entraron en estado `ALARM`. ¿Qué acción garantizará que las alarmas de CloudWatch funcionen correctamente?](#un-ingeniero-de-cloudops-necesita-crear-alertas-basadas-en-las-métricas-de-lectura-y-escritura-de-volúmenes-de-amazon-elastic-block-store-amazon-ebs-adjuntos-a-una-instancia-de-amazon-ec2-el-ingeniero-de-cloudops-crea-y-habilita-alarmas-de-amazon-cloudwatch-para-la-métrica-diskreadbytes-y-la-métrica-diskwritebytes-una-herramienta-de-monitoreo-personalizada-instalada-en-la-instancia-de-ec2-con-la-misma-configuración-de-alarma-indica-que-las-métricas-del-volumen-han-superado-el-umbral-sin-embargo-las-alarmas-de-cloudwatch-no-entraron-en-estado-alarm-qué-acción-garantizará-que-las-alarmas-de-cloudwatch-funcionen-correctamente) |
| 11 | [Una empresa necesita ver una lista de grupos de seguridad que están abiertos a internet en el puerto `3389`. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-necesita-ver-una-lista-de-grupos-de-seguridad-que-están-abiertos-a-internet-en-el-puerto-3389-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 12 | [Una aplicación se ejecuta en múltiples instancias de Amazon EC2 dentro de un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para usar la versión más reciente de una plantilla de lanzamiento (launch template). Un ingeniero de CloudOps debe diseñar una solución que administre de forma centralizada los registros de la aplicación y los conserve durante no más de 90 días. ¿Qué solución cumple con estos requisitos?](#una-aplicación-se-ejecuta-en-múltiples-instancias-de-amazon-ec2-dentro-de-un-grupo-de-auto-scaling-el-grupo-de-auto-scaling-está-configurado-para-usar-la-versión-más-reciente-de-una-plantilla-de-lanzamiento-launch-template-un-ingeniero-de-cloudops-debe-diseñar-una-solución-que-administre-de-forma-centralizada-los-registros-de-la-aplicación-y-los-conserve-durante-no-más-de-90-días-qué-solución-cumple-con-estos-requisitos) |
| 13 | [Una empresa está realizando una venta relámpago (flash sale) en su sitio web. El sitio web está alojado en instancias de Amazon EC2 de rendimiento con ráfagas (burstable) dentro de un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para lanzar instancias cuando el uso de CPU supera el `70%`. Un par de horas después de iniciada la venta, los usuarios reportan tiempos de carga lentos y mensajes de error por conexiones rechazadas. Un ingeniero de CloudOps revisa las métricas de Amazon CloudWatch y observa que el uso de CPU está en `20%` en toda la flota de instancias. El ingeniero de CloudOps debe restaurar la funcionalidad del sitio web sin hacer cambios en la infraestructura de red. ¿Qué solución cumple con estos requisitos?](#una-empresa-está-realizando-una-venta-relámpago-flash-sale-en-su-sitio-web-el-sitio-web-está-alojado-en-instancias-de-amazon-ec2-de-rendimiento-con-ráfagas-burstable-dentro-de-un-grupo-de-auto-scaling-el-grupo-de-auto-scaling-está-configurado-para-lanzar-instancias-cuando-el-uso-de-cpu-supera-el-70-un-par-de-horas-después-de-iniciada-la-venta-los-usuarios-reportan-tiempos-de-carga-lentos-y-mensajes-de-error-por-conexiones-rechazadas-un-ingeniero-de-cloudops-revisa-las-métricas-de-amazon-cloudwatch-y-observa-que-el-uso-de-cpu-está-en-20-en-toda-la-flota-de-instancias-el-ingeniero-de-cloudops-debe-restaurar-la-funcionalidad-del-sitio-web-sin-hacer-cambios-en-la-infraestructura-de-red-qué-solución-cumple-con-estos-requisitos) |
| 14 | [Una empresa ha lanzado un sitio web de redes sociales que permite a los usuarios subir imágenes directamente a un bucket centralizado de Amazon S3. El sitio web es popular en zonas geográficamente distantes de la región de AWS donde se encuentra el bucket de S3. Los usuarios reportan que las cargas son lentas. Un ingeniero de CloudOps debe mejorar la velocidad de carga. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?](#una-empresa-ha-lanzado-un-sitio-web-de-redes-sociales-que-permite-a-los-usuarios-subir-imágenes-directamente-a-un-bucket-centralizado-de-amazon-s3-el-sitio-web-es-popular-en-zonas-geográficamente-distantes-de-la-región-de-aws-donde-se-encuentra-el-bucket-de-s3-los-usuarios-reportan-que-las-cargas-son-lentas-un-ingeniero-de-cloudops-debe-mejorar-la-velocidad-de-carga-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 15 | [Una empresa tiene una aplicación móvil que usa Amazon S3 para almacenar imágenes. Las imágenes son populares durante una semana, y luego el número de solicitudes de acceso disminuye con el tiempo. Las imágenes deben tener alta disponibilidad y ser accesibles de inmediato cuando se soliciten. Un ingeniero de CloudOps debe reducir los costos de almacenamiento en S3 para la empresa. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?](#una-empresa-tiene-una-aplicación-móvil-que-usa-amazon-s3-para-almacenar-imágenes-las-imágenes-son-populares-durante-una-semana-y-luego-el-número-de-solicitudes-de-acceso-disminuye-con-el-tiempo-las-imágenes-deben-tener-alta-disponibilidad-y-ser-accesibles-de-inmediato-cuando-se-soliciten-un-ingeniero-de-cloudops-debe-reducir-los-costos-de-almacenamiento-en-s3-para-la-empresa-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-rentable) |
| 16 | [Una empresa usa AWS Organizations para administrar múltiples cuentas de AWS con facturación consolidada habilitada. Los propietarios de las cuentas miembro de la organización quieren los beneficios de las Instancias Reservadas (RI) pero no quieren compartir las RI con otras cuentas. ¿Qué solución cumple con estos requisitos?](#una-empresa-usa-aws-organizations-para-administrar-múltiples-cuentas-de-aws-con-facturación-consolidada-habilitada-los-propietarios-de-las-cuentas-miembro-de-la-organización-quieren-los-beneficios-de-las-instancias-reservadas-ri-pero-no-quieren-compartir-las-ri-con-otras-cuentas-qué-solución-cumple-con-estos-requisitos) |
| 17 | [Una aplicación de videojuegos está desplegada en cuatro instancias de Amazon EC2 dentro de una `VPC` predeterminada. El ingeniero de CloudOps ha notado latencia consistentemente alta en las respuestas mientras se transfieren datos entre las cuatro instancias. El ingeniero no tiene manera de modificar el código de la aplicación. La forma MÁS efectiva de reducir la latencia es volver a lanzar las instancias de EC2 en:](#una-aplicación-de-videojuegos-está-desplegada-en-cuatro-instancias-de-amazon-ec2-dentro-de-una-vpc-predeterminada-el-ingeniero-de-cloudops-ha-notado-latencia-consistentemente-alta-en-las-respuestas-mientras-se-transfieren-datos-entre-las-cuatro-instancias-el-ingeniero-no-tiene-manera-de-modificar-el-código-de-la-aplicación-la-forma-más-efectiva-de-reducir-la-latencia-es-volver-a-lanzar-las-instancias-de-ec2-en) |
| 18 | [El departamento financiero de una empresa necesita ver los detalles de costos de cada proyecto en una cuenta de AWS. Un ingeniero de CloudOps debe realizar la configuración inicial requerida para ver el costo de cada proyecto en Cost Explorer. ¿Qué solución cumple con este requisito?](#el-departamento-financiero-de-una-empresa-necesita-ver-los-detalles-de-costos-de-cada-proyecto-en-una-cuenta-de-aws-un-ingeniero-de-cloudops-debe-realizar-la-configuración-inicial-requerida-para-ver-el-costo-de-cada-proyecto-en-cost-explorer-qué-solución-cumple-con-este-requisito) |
| 19 | [Un ingeniero de CloudOps debe configurar una capa resiliente de instancias de Amazon EC2 para una aplicación de computación de alto rendimiento (HPC). La aplicación HPC requiere latencia mínima entre nodos. ¿Qué acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)](#un-ingeniero-de-cloudops-debe-configurar-una-capa-resiliente-de-instancias-de-amazon-ec2-para-una-aplicación-de-computación-de-alto-rendimiento-hpc-la-aplicación-hpc-requiere-latencia-mínima-entre-nodos-qué-acciones-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-elija-dos) |
| 20 | [Un ingeniero de CloudOps administra los buckets de Amazon S3 de una empresa. El ingeniero de CloudOps ha identificado `5 GB` de cargas multiparte incompletas en un bucket de S3 de la cuenta de AWS de la empresa. El ingeniero de CloudOps necesita reducir la cantidad de objetos de cargas multiparte incompletas en el bucket de S3. ¿Qué solución cumple con este requisito?](#un-ingeniero-de-cloudops-administra-los-buckets-de-amazon-s3-de-una-empresa-el-ingeniero-de-cloudops-ha-identificado-5-gb-de-cargas-multiparte-incompletas-en-un-bucket-de-s3-de-la-cuenta-de-aws-de-la-empresa-el-ingeniero-de-cloudops-necesita-reducir-la-cantidad-de-objetos-de-cargas-multiparte-incompletas-en-el-bucket-de-s3-qué-solución-cumple-con-este-requisito) |
| 21 | [Una empresa usa Amazon Elastic File System (Amazon EFS) para compartir un sistema de archivos entre varias instancias de Amazon EC2. A medida que aumenta el uso, los usuarios reportan que la recuperación de archivos desde el sistema de archivos EFS es más lenta de lo normal. ¿Qué acción debe tomar un ingeniero de CloudOps para mejorar el rendimiento del sistema de archivos?](#una-empresa-usa-amazon-elastic-file-system-amazon-efs-para-compartir-un-sistema-de-archivos-entre-varias-instancias-de-amazon-ec2-a-medida-que-aumenta-el-uso-los-usuarios-reportan-que-la-recuperación-de-archivos-desde-el-sistema-de-archivos-efs-es-más-lenta-de-lo-normal-qué-acción-debe-tomar-un-ingeniero-de-cloudops-para-mejorar-el-rendimiento-del-sistema-de-archivos) |
| 22 | [Una empresa tiene una aplicación que los clientes usan para buscar registros en un sitio web. Los datos de la aplicación se almacenan en un clúster de Amazon Aurora DB. El uso de la aplicación varía según la temporada y el día de la semana. La popularidad del sitio web está aumentando, y el sitio web experimenta un rendimiento más lento debido al aumento de carga en el clúster de base de datos durante los períodos de actividad pico. Los registros de la aplicación muestran que los problemas de rendimiento ocurren cuando los usuarios buscan información. Rara vez se realiza la misma búsqueda varias veces. Un ingeniero de CloudOps debe mejorar el rendimiento de la plataforma usando una solución que maximice la eficiencia de los recursos. ¿Qué solución cumple con estos requisitos?](#una-empresa-tiene-una-aplicación-que-los-clientes-usan-para-buscar-registros-en-un-sitio-web-los-datos-de-la-aplicación-se-almacenan-en-un-clúster-de-amazon-aurora-db-el-uso-de-la-aplicación-varía-según-la-temporada-y-el-día-de-la-semana-la-popularidad-del-sitio-web-está-aumentando-y-el-sitio-web-experimenta-un-rendimiento-más-lento-debido-al-aumento-de-carga-en-el-clúster-de-base-de-datos-durante-los-períodos-de-actividad-pico-los-registros-de-la-aplicación-muestran-que-los-problemas-de-rendimiento-ocurren-cuando-los-usuarios-buscan-información-rara-vez-se-realiza-la-misma-búsqueda-varias-veces-un-ingeniero-de-cloudops-debe-mejorar-el-rendimiento-de-la-plataforma-usando-una-solución-que-maximice-la-eficiencia-de-los-recursos-qué-solución-cumple-con-estos-requisitos) |
| 23 | [El equipo de seguridad está preocupado porque el número de políticas de AWS Identity and Access Management (IAM) que se usan en el entorno está aumentando. El equipo le encargó a un ingeniero de CloudOps que reportara el número actual de políticas de IAM en uso y el total de políticas de IAM disponibles. ¿Qué servicio de AWS debe usar el ingeniero para verificar cómo se compara el uso actual de políticas de IAM con los límites de servicio actuales?](#el-equipo-de-seguridad-está-preocupado-porque-el-número-de-políticas-de-aws-identity-and-access-management-iam-que-se-usan-en-el-entorno-está-aumentando-el-equipo-le-encargó-a-un-ingeniero-de-cloudops-que-reportara-el-número-actual-de-políticas-de-iam-en-uso-y-el-total-de-políticas-de-iam-disponibles-qué-servicio-de-aws-debe-usar-el-ingeniero-para-verificar-cómo-se-compara-el-uso-actual-de-políticas-de-iam-con-los-límites-de-servicio-actuales) |
| 24 | [Un ingeniero de CloudOps notó que se está creando una gran cantidad de direcciones IP elásticas en la cuenta de AWS de la empresa, pero no se están asociando con instancias de Amazon EC2, y están generando cargos por direcciones IP elásticas en la factura mensual. ¿Cómo puede el ingeniero identificar quién está creando las direcciones IP elásticas?](#un-ingeniero-de-cloudops-notó-que-se-está-creando-una-gran-cantidad-de-direcciones-ip-elásticas-en-la-cuenta-de-aws-de-la-empresa-pero-no-se-están-asociando-con-instancias-de-amazon-ec2-y-están-generando-cargos-por-direcciones-ip-elásticas-en-la-factura-mensual-cómo-puede-el-ingeniero-identificar-quién-está-creando-las-direcciones-ip-elásticas) |
| 25 | [El departamento de TI de una empresa notó un aumento en el gasto de su cuenta de AWS para desarrolladores. Hay más de 50 desarrolladores usando la cuenta, y el equipo de finanzas quiere determinar los costos de servicio incurridos por cada desarrollador. ¿Qué debe hacer un ingeniero de CloudOps para recopilar esta información? (Seleccione DOS.)](#el-departamento-de-ti-de-una-empresa-notó-un-aumento-en-el-gasto-de-su-cuenta-de-aws-para-desarrolladores-hay-más-de-50-desarrolladores-usando-la-cuenta-y-el-equipo-de-finanzas-quiere-determinar-los-costos-de-servicio-incurridos-por-cada-desarrollador-qué-debe-hacer-un-ingeniero-de-cloudops-para-recopilar-esta-información-seleccione-dos) |
| 26 | [Una empresa ejecuta una aplicación en una flota de instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Las instancias de EC2 son lanzadas por un grupo de Auto Scaling y se registran automáticamente en un grupo de destino. Un ingeniero de CloudOps debe configurar una notificación para alertar a los propietarios de la aplicación cuando los destinos fallen las verificaciones de estado. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?](#una-empresa-ejecuta-una-aplicación-en-una-flota-de-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-alb-las-instancias-de-ec2-son-lanzadas-por-un-grupo-de-auto-scaling-y-se-registran-automáticamente-en-un-grupo-de-destino-un-ingeniero-de-cloudops-debe-configurar-una-notificación-para-alertar-a-los-propietarios-de-la-aplicación-cuando-los-destinos-fallen-las-verificaciones-de-estado-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 27 | [Una empresa ejecuta su infraestructura en instancias de Amazon EC2 que corren en un grupo de Auto Scaling. Recientemente, la empresa promovió código defectuoso a toda la flota de EC2. Este código defectuoso hizo que el grupo de Auto Scaling escalara las instancias antes de que se pudieran recuperar los registros de la aplicación. ¿Qué debe hacer un ingeniero de CloudOps para conservar los registros de la aplicación después de que las instancias sean terminadas?](#una-empresa-ejecuta-su-infraestructura-en-instancias-de-amazon-ec2-que-corren-en-un-grupo-de-auto-scaling-recientemente-la-empresa-promovió-código-defectuoso-a-toda-la-flota-de-ec2-este-código-defectuoso-hizo-que-el-grupo-de-auto-scaling-escalara-las-instancias-antes-de-que-se-pudieran-recuperar-los-registros-de-la-aplicación-qué-debe-hacer-un-ingeniero-de-cloudops-para-conservar-los-registros-de-la-aplicación-después-de-que-las-instancias-sean-terminadas) |
| 28 | [Un ingeniero de CloudOps debe crear una solución que notifique inmediatamente a los desarrolladores de software si una función de AWS Lambda presenta un error. ¿Qué solución cumple con este requisito?](#un-ingeniero-de-cloudops-debe-crear-una-solución-que-notifique-inmediatamente-a-los-desarrolladores-de-software-si-una-función-de-aws-lambda-presenta-un-error-qué-solución-cumple-con-este-requisito) |
| 29 | [Un ingeniero de CloudOps debe crear una solución que apague automáticamente cualquier instancia de Amazon EC2 que tenga menos del `10%` de uso promedio de CPU durante 60 minutos o más. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?](#un-ingeniero-de-cloudops-debe-crear-una-solución-que-apague-automáticamente-cualquier-instancia-de-amazon-ec2-que-tenga-menos-del-10-de-uso-promedio-de-cpu-durante-60-minutos-o-más-qué-solución-cumple-con-este-requisito-de-la-manera-más-eficiente-operativamente) |
| 30 | [Se notifica a un ingeniero de CloudOps que una instancia de Amazon EC2 dejó de responder. La consola de administración de AWS indica que las verificaciones de sistema están fallando. ¿Qué debe hacer primero el ingeniero para resolver este problema?](#se-notifica-a-un-ingeniero-de-cloudops-que-una-instancia-de-amazon-ec2-dejó-de-responder-la-consola-de-administración-de-aws-indica-que-las-verificaciones-de-sistema-están-fallando-qué-debe-hacer-primero-el-ingeniero-para-resolver-este-problema) |
| 31 | [Una empresa tiene una aplicación web existente que se ejecuta en dos instancias de Amazon EC2 detrás de un Application Load Balancer (ALB) a través de dos Zonas de disponibilidad. La aplicación usa una instancia de Amazon RDS Multi-AZ. Los conjuntos de registros de Amazon Route 53 enrutan las solicitudes de contenido dinámico al balanceador de carga y las solicitudes de contenido estático a un bucket de Amazon S3. Los visitantes del sitio reportan tiempos de carga extremadamente largos. ¿Qué acciones se deben tomar para mejorar el rendimiento del sitio web? (Seleccione DOS)](#una-empresa-tiene-una-aplicación-web-existente-que-se-ejecuta-en-dos-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-alb-a-través-de-dos-zonas-de-disponibilidad-la-aplicación-usa-una-instancia-de-amazon-rds-multi-az-los-conjuntos-de-registros-de-amazon-route-53-enrutan-las-solicitudes-de-contenido-dinámico-al-balanceador-de-carga-y-las-solicitudes-de-contenido-estático-a-un-bucket-de-amazon-s3-los-visitantes-del-sitio-reportan-tiempos-de-carga-extremadamente-largos-qué-acciones-se-deben-tomar-para-mejorar-el-rendimiento-del-sitio-web-seleccione-dos) |
| 32 | [Se sabe que un proceso errático usa todo un procesador y se ejecuta al `100%`. Un ingeniero de CloudOps quiere automatizar el reinicio de la instancia una vez que el problema ocurra durante más de 2 minutos. ¿Cómo se puede lograr esto?](#se-sabe-que-un-proceso-errático-usa-todo-un-procesador-y-se-ejecuta-al-100-un-ingeniero-de-cloudops-quiere-automatizar-el-reinicio-de-la-instancia-una-vez-que-el-problema-ocurra-durante-más-de-2-minutos-cómo-se-puede-lograr-esto) |
| 33 | [Un ingeniero de CloudOps observa un evento de escalado (scale-up) para un grupo de Amazon EC2 Auto Scaling. Amazon CloudWatch muestra un pico en la métrica `RequestCount` del Application Load Balancer asociado. Al ingeniero le gustaría conocer las direcciones IP de origen de las solicitudes. ¿Dónde puede el ingeniero encontrar esta información?](#un-ingeniero-de-cloudops-observa-un-evento-de-escalado-scale-up-para-un-grupo-de-amazon-ec2-auto-scaling-amazon-cloudwatch-muestra-un-pico-en-la-métrica-requestcount-del-application-load-balancer-asociado-al-ingeniero-le-gustaría-conocer-las-direcciones-ip-de-origen-de-las-solicitudes-dónde-puede-el-ingeniero-encontrar-esta-información) |
| 34 | [Una empresa está ejecutando una aplicación sin servidor (serverless) en AWS Lambda. La aplicación almacena datos en una instancia de base de datos de Amazon RDS for MySQL. El uso ha aumentado constantemente, y recientemente han ocurrido numerosos errores de `too many connections` cuando la función Lambda intenta conectarse a la base de datos. La empresa ya ha configurado la base de datos para usar el valor máximo posible de `max_connections`. ¿Qué debe hacer un ingeniero de CloudOps para resolver estos errores?](#una-empresa-está-ejecutando-una-aplicación-sin-servidor-serverless-en-aws-lambda-la-aplicación-almacena-datos-en-una-instancia-de-base-de-datos-de-amazon-rds-for-mysql-el-uso-ha-aumentado-constantemente-y-recientemente-han-ocurrido-numerosos-errores-de-too-many-connections-cuando-la-función-lambda-intenta-conectarse-a-la-base-de-datos-la-empresa-ya-ha-configurado-la-base-de-datos-para-usar-el-valor-máximo-posible-de-max_connections-qué-debe-hacer-un-ingeniero-de-cloudops-para-resolver-estos-errores) |
| 35 | [Un ingeniero de CloudOps recibe una notificación de que una aplicación que se ejecuta en instancias de Amazon EC2 no ha podido autenticarse en una base de datos de Amazon RDS. Para solucionar el problema, el ingeniero de CloudOps necesita investigar la rotación de contraseñas de AWS Secrets Manager. ¿Qué registro de Amazon CloudWatch proporcionará información sobre la rotación de contraseñas?](#un-ingeniero-de-cloudops-recibe-una-notificación-de-que-una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-no-ha-podido-autenticarse-en-una-base-de-datos-de-amazon-rds-para-solucionar-el-problema-el-ingeniero-de-cloudops-necesita-investigar-la-rotación-de-contraseñas-de-aws-secrets-manager-qué-registro-de-amazon-cloudwatch-proporcionará-información-sobre-la-rotación-de-contraseñas) |
| 36 | [Una función de AWS Lambda falla intermitentemente varias veces al día. Un ingeniero de CloudOps debe averiguar con qué frecuencia ha ocurrido este error en los últimos 7 días. ¿Qué acción cumple con este requisito de la manera MÁS eficiente operativamente?](#una-función-de-aws-lambda-falla-intermitentemente-varias-veces-al-día-un-ingeniero-de-cloudops-debe-averiguar-con-qué-frecuencia-ha-ocurrido-este-error-en-los-últimos-7-días-qué-acción-cumple-con-este-requisito-de-la-manera-más-eficiente-operativamente) |
| 37 | [Un ingeniero de CloudOps debe configurar notificaciones para cuando la facturación combinada supere un cierto umbral para todas las cuentas de AWS dentro de una empresa. El ingeniero ha configurado AWS Organizations y habilitado la facturación consolidada. ¿Qué pasos adicionales debe realizar el ingeniero para configurar las alertas de facturación?](#un-ingeniero-de-cloudops-debe-configurar-notificaciones-para-cuando-la-facturación-combinada-supere-un-cierto-umbral-para-todas-las-cuentas-de-aws-dentro-de-una-empresa-el-ingeniero-ha-configurado-aws-organizations-y-habilitado-la-facturación-consolidada-qué-pasos-adicionales-debe-realizar-el-ingeniero-para-configurar-las-alertas-de-facturación) |
| 38 | [Una empresa tiene una carga de trabajo Windows de alto rendimiento. La carga de trabajo requiere un volumen de almacenamiento que proporcione un rendimiento constante de 10,000 IOPS. La empresa no quiere pagar por capacidad adicional innecesaria para lograr este rendimiento. ¿Qué solución cumple con estos requisitos con el MENOR costo?](#una-empresa-tiene-una-carga-de-trabajo-windows-de-alto-rendimiento-la-carga-de-trabajo-requiere-un-volumen-de-almacenamiento-que-proporcione-un-rendimiento-constante-de-10000-iops-la-empresa-no-quiere-pagar-por-capacidad-adicional-innecesaria-para-lograr-este-rendimiento-qué-solución-cumple-con-estos-requisitos-con-el-menor-costo) |
| 39 | [Una empresa tiene científicos que cargan objetos de datos grandes a un bucket de Amazon S3. Los científicos cargan los objetos como cargas multiparte. Las cargas multiparte a menudo fallan debido a una mala conectividad del cliente final. La empresa quiere optimizar los costos de almacenamiento asociados con los datos. Un ingeniero de CloudOps debe implementar una solución que presente métricas para cargas incompletas. La solución también debe eliminar automáticamente cualquier carga incompleta después de 7 días. ¿Qué solución cumple con estos requisitos?](#una-empresa-tiene-científicos-que-cargan-objetos-de-datos-grandes-a-un-bucket-de-amazon-s3-los-científicos-cargan-los-objetos-como-cargas-multiparte-las-cargas-multiparte-a-menudo-fallan-debido-a-una-mala-conectividad-del-cliente-final-la-empresa-quiere-optimizar-los-costos-de-almacenamiento-asociados-con-los-datos-un-ingeniero-de-cloudops-debe-implementar-una-solución-que-presente-métricas-para-cargas-incompletas-la-solución-también-debe-eliminar-automáticamente-cualquier-carga-incompleta-después-de-7-días-qué-solución-cumple-con-estos-requisitos) |
| 40 | [Una empresa está ejecutando un software de computación distribuida para administrar una flota de 20 instancias de Amazon EC2 para cálculos. La flota incluye 2 nodos de control y 18 nodos de tareas para ejecutar los cálculos. Los nodos de control pueden iniciar automáticamente los nodos de tareas. Actualmente, todos los nodos se ejecutan bajo demanda (on-demand). Los nodos de control deben estar disponibles las 24 horas del día, los 7 días de la semana. Los nodos de tareas se ejecutan durante 4 horas cada día. Un ingeniero de CloudOps necesita optimizar el costo de esta solución. ¿Qué combinación de acciones cumple con estos requisitos? (Elija dos.)](#una-empresa-está-ejecutando-un-software-de-computación-distribuida-para-administrar-una-flota-de-20-instancias-de-amazon-ec2-para-cálculos-la-flota-incluye-2-nodos-de-control-y-18-nodos-de-tareas-para-ejecutar-los-cálculos-los-nodos-de-control-pueden-iniciar-automáticamente-los-nodos-de-tareas-actualmente-todos-los-nodos-se-ejecutan-bajo-demanda-on-demand-los-nodos-de-control-deben-estar-disponibles-las-24-horas-del-día-los-7-días-de-la-semana-los-nodos-de-tareas-se-ejecutan-durante-4-horas-cada-día-un-ingeniero-de-cloudops-necesita-optimizar-el-costo-de-esta-solución-qué-combinación-de-acciones-cumple-con-estos-requisitos-elija-dos) |
| 41 | [Se supone que una empresa recibe un archivo de datos cada hora en un bucket de Amazon S3. Una notificación de evento de S3 invoca una función de AWS Lambda cada vez que llega un archivo. La función procesa los datos para que los use una aplicación. El equipo de la aplicación nota que, a veces, el archivo no llega. El equipo de la aplicación quiere recibir una notificación siempre que el archivo no llegue. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#se-supone-que-una-empresa-recibe-un-archivo-de-datos-cada-hora-en-un-bucket-de-amazon-s3-una-notificación-de-evento-de-s3-invoca-una-función-de-aws-lambda-cada-vez-que-llega-un-archivo-la-función-procesa-los-datos-para-que-los-use-una-aplicación-el-equipo-de-la-aplicación-nota-que-a-veces-el-archivo-no-llega-el-equipo-de-la-aplicación-quiere-recibir-una-notificación-siempre-que-el-archivo-no-llegue-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 42 | [Una empresa tiene una aplicación web que experimenta problemas de rendimiento varias veces cada noche. Un análisis de causa raíz revela aumentos repentinos en el uso de CPU que duran 5 minutos en una instancia de Amazon EC2 Linux. Un ingeniero de CloudOps debe encontrar el ID de proceso (PID) del servicio o proceso que está consumiendo más CPU. ¿Qué debe hacer el ingeniero de CloudOps para recopilar la información de uso del proceso con el MENOR esfuerzo posible?](#una-empresa-tiene-una-aplicación-web-que-experimenta-problemas-de-rendimiento-varias-veces-cada-noche-un-análisis-de-causa-raíz-revela-aumentos-repentinos-en-el-uso-de-cpu-que-duran-5-minutos-en-una-instancia-de-amazon-ec2-linux-un-ingeniero-de-cloudops-debe-encontrar-el-id-de-proceso-pid-del-servicio-o-proceso-que-está-consumiendo-más-cpu-qué-debe-hacer-el-ingeniero-de-cloudops-para-recopilar-la-información-de-uso-del-proceso-con-el-menor-esfuerzo-posible) |
| 43 | [Un equipo administra una cuenta de AWS que es miembro de una organización en AWS Organizations. La organización tiene habilitadas las funciones de facturación consolidada. La cuenta aloja varias aplicaciones. Un ingeniero de CloudOps ha aplicado etiquetas (tags) a los recursos dentro de la cuenta para reflejar el entorno. El equipo necesita un informe del desglose de cargos por entorno. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#un-equipo-administra-una-cuenta-de-aws-que-es-miembro-de-una-organización-en-aws-organizations-la-organización-tiene-habilitadas-las-funciones-de-facturación-consolidada-la-cuenta-aloja-varias-aplicaciones-un-ingeniero-de-cloudops-ha-aplicado-etiquetas-tags-a-los-recursos-dentro-de-la-cuenta-para-reflejar-el-entorno-el-equipo-necesita-un-informe-del-desglose-de-cargos-por-entorno-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 44 | [Se sabe que un proceso errático usa un procesador completo y se ejecuta al `100%`. Un ingeniero de CloudOps quiere automatizar el reinicio de una instancia de Amazon EC2 cuando el problema ocurre por más de 2 minutos. ¿Cómo se puede lograr esto?](#se-sabe-que-un-proceso-errático-usa-un-procesador-completo-y-se-ejecuta-al-100-un-ingeniero-de-cloudops-quiere-automatizar-el-reinicio-de-una-instancia-de-amazon-ec2-cuando-el-problema-ocurre-por-más-de-2-minutos-cómo-se-puede-lograr-esto) |
| 45 | [Una empresa está implementando seguridad y cumplimiento normativo usando AWS Trusted Advisor. El equipo de SysOps de la empresa está validando la lista de verificaciones de Trusted Advisor a las que puede acceder. ¿Qué factor afectará la cantidad de verificaciones de Trusted Advisor disponibles?](#una-empresa-está-implementando-seguridad-y-cumplimiento-normativo-usando-aws-trusted-advisor-el-equipo-de-sysops-de-la-empresa-está-validando-la-lista-de-verificaciones-de-trusted-advisor-a-las-que-puede-acceder-qué-factor-afectará-la-cantidad-de-verificaciones-de-trusted-advisor-disponibles) |
| 46 | [Un ingeniero de CloudOps está investigando problemas en una instancia de base de datos de Amazon RDS para MariaDB. El ingeniero de CloudOps quiere mostrar la carga de la base de datos categorizada por eventos de espera detallados. ¿Cómo puede el ingeniero de CloudOps lograr este objetivo?](#un-ingeniero-de-cloudops-está-investigando-problemas-en-una-instancia-de-base-de-datos-de-amazon-rds-para-mariadb-el-ingeniero-de-cloudops-quiere-mostrar-la-carga-de-la-base-de-datos-categorizada-por-eventos-de-espera-detallados-cómo-puede-el-ingeniero-de-cloudops-lograr-este-objetivo) |
| 47 | [Un usuario que trabaja en la consola de Amazon EC2 aumentó el tamaño de un volumen de Amazon Elastic Block Store (Amazon EBS) adjunto a una instancia de Amazon EC2 Windows. El cambio no se refleja en el sistema de archivos. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?](#un-usuario-que-trabaja-en-la-consola-de-amazon-ec2-aumentó-el-tamaño-de-un-volumen-de-amazon-elastic-block-store-amazon-ebs-adjunto-a-una-instancia-de-amazon-ec2-windows-el-cambio-no-se-refleja-en-el-sistema-de-archivos-qué-debe-hacer-un-ingeniero-de-cloudops-para-resolver-este-problema) |
| 48 | [Una empresa ha migrado su aplicación a AWS. La empresa alojará la aplicación en instancias de Amazon EC2 de múltiples familias de instancias. Durante las pruebas iniciales, un ingeniero de CloudOps identifica problemas de rendimiento en instancias de EC2 seleccionadas. La empresa tiene una política estricta de asignación de presupuesto, por lo que el ingeniero de CloudOps debe usar los tipos de recursos correctos con las características de rendimiento que coincidan con la carga de trabajo. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-ha-migrado-su-aplicación-a-aws-la-empresa-alojará-la-aplicación-en-instancias-de-amazon-ec2-de-múltiples-familias-de-instancias-durante-las-pruebas-iniciales-un-ingeniero-de-cloudops-identifica-problemas-de-rendimiento-en-instancias-de-ec2-seleccionadas-la-empresa-tiene-una-política-estricta-de-asignación-de-presupuesto-por-lo-que-el-ingeniero-de-cloudops-debe-usar-los-tipos-de-recursos-correctos-con-las-características-de-rendimiento-que-coincidan-con-la-carga-de-trabajo-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 49 | [Un ingeniero de CloudOps es responsable de una gran flota de instancias de Amazon EC2 y debe saber si alguna instancia se verá afectada por el próximo mantenimiento de hardware. ¿Qué opción proporcionaría esta información con el MENOR esfuerzo administrativo?](#un-ingeniero-de-cloudops-es-responsable-de-una-gran-flota-de-instancias-de-amazon-ec2-y-debe-saber-si-alguna-instancia-se-verá-afectada-por-el-próximo-mantenimiento-de-hardware-qué-opción-proporcionaría-esta-información-con-el-menor-esfuerzo-administrativo) |
| 50 | [Una aplicación de análisis de datos se está ejecutando en una instancia de Amazon EC2. Un ingeniero de CloudOps debe agregar dimensiones personalizadas a las métricas recopiladas por el agente de Amazon CloudWatch. ¿Cómo puede el ingeniero de CloudOps cumplir con este requisito?](#una-aplicación-de-análisis-de-datos-se-está-ejecutando-en-una-instancia-de-amazon-ec2-un-ingeniero-de-cloudops-debe-agregar-dimensiones-personalizadas-a-las-métricas-recopiladas-por-el-agente-de-amazon-cloudwatch-cómo-puede-el-ingeniero-de-cloudops-cumplir-con-este-requisito) |
| 51 | [Una empresa recibe una alerta de una alarma de Amazon CloudWatch. La alarma indica que una aplicación web que se ejecuta en instancias de Amazon EC2 no está respondiendo a las solicitudes. Las instancias de EC2 tienen un sistema operativo Red Hat Enterprise Linux y están en un grupo de Auto Scaling. El grupo de Auto Scaling tiene una capacidad mínima de 2 y una capacidad máxima de 5. Una investigación revela que la aplicación web está experimentando errores por falta de memoria (out-of-memory). La empresa agrega memoria a la aplicación web y quiere monitorear el uso de memoria del sistema operativo. Actualmente no existe una métrica de memoria de CloudWatch para las instancias de EC2 en el grupo de Auto Scaling. ¿Qué debe hacer un ingeniero de CloudOps para proporcionar una métrica de memoria de CloudWatch para las instancias de EC2?](#una-empresa-recibe-una-alerta-de-una-alarma-de-amazon-cloudwatch-la-alarma-indica-que-una-aplicación-web-que-se-ejecuta-en-instancias-de-amazon-ec2-no-está-respondiendo-a-las-solicitudes-las-instancias-de-ec2-tienen-un-sistema-operativo-red-hat-enterprise-linux-y-están-en-un-grupo-de-auto-scaling-el-grupo-de-auto-scaling-tiene-una-capacidad-mínima-de-2-y-una-capacidad-máxima-de-5-una-investigación-revela-que-la-aplicación-web-está-experimentando-errores-por-falta-de-memoria-out-of-memory-la-empresa-agrega-memoria-a-la-aplicación-web-y-quiere-monitorear-el-uso-de-memoria-del-sistema-operativo-actualmente-no-existe-una-métrica-de-memoria-de-cloudwatch-para-las-instancias-de-ec2-en-el-grupo-de-auto-scaling-qué-debe-hacer-un-ingeniero-de-cloudops-para-proporcionar-una-métrica-de-memoria-de-cloudwatch-para-las-instancias-de-ec2) |
| 52 | [Un ingeniero de CloudOps debe administrar la seguridad de una cuenta de AWS. Recientemente, la clave de acceso de un usuario de IAM se subió por error a un repositorio de código público. El ingeniero de CloudOps debe identificar todo lo que fue cambiado usando esta clave de acceso. ¿Cómo debe el ingeniero de CloudOps cumplir con estos requisitos?](#un-ingeniero-de-cloudops-debe-administrar-la-seguridad-de-una-cuenta-de-aws-recientemente-la-clave-de-acceso-de-un-usuario-de-iam-se-subió-por-error-a-un-repositorio-de-código-público-el-ingeniero-de-cloudops-debe-identificar-todo-lo-que-fue-cambiado-usando-esta-clave-de-acceso-cómo-debe-el-ingeniero-de-cloudops-cumplir-con-estos-requisitos) |
| 53 | [Si el navegador de la consola de administración de AWS no muestra que ha iniciado sesión en una cuenta de AWS, cierre el navegador y vuelva a abrir la consola usando el acceso directo de la consola de administración de AWS desde el escritorio de la VM. Si la funcionalidad de copiar y pegar no funciona en su entorno, consulte el archivo de instrucciones en el escritorio de la VM y use `Ctrl+C`, `Ctrl+V` o `Command-C`, `Command-V`. Configure Amazon EventBridge para cumplir con los siguientes requisitos. 1. Use la región `us-east-2` para todos los recursos. 2. A menos que se especifique lo contrario a continuación, use la configuración predeterminada. 3. Use su propia nomenclatura de recursos a menos que se especifique un nombre de recurso a continuación. 4. Asegúrese de que todos los eventos de Amazon EC2 en el bus de eventos predeterminado sean reproducibles (replayable) durante los últimos 90 días. 5. Cree una regla llamada `RunFunction` para enviar el mensaje exacto `{"name":"example"}` cada 15 minutos a una función de AWS Lambda existente llamada LogEventFunction. 6. Cree una regla llamada `SpotWarning` para enviar una notificación a un nuevo tema estándar de Amazon SNS llamado `TopicEvents` cada vez que se interrumpa una instancia Spot de Amazon EC2. NO cree ninguna suscripción al tema. La notificación debe coincidir con la siguiente estructura: `Input path: {instance: detail.instance-id} Input template: The EC2 Spot Instance <instance> has been interrupted.` Importante: Haga clic en el botón Next para completar este laboratorio y continuar al siguiente. Una vez que haga clic en el botón Next, NO podrá volver a este laboratorio.](#si-el-navegador-de-la-consola-de-administración-de-aws-no-muestra-que-ha-iniciado-sesión-en-una-cuenta-de-aws-cierre-el-navegador-y-vuelva-a-abrir-la-consola-usando-el-acceso-directo-de-la-consola-de-administración-de-aws-desde-el-escritorio-de-la-vm-si-la-funcionalidad-de-copiar-y-pegar-no-funciona-en-su-entorno-consulte-el-archivo-de-instrucciones-en-el-escritorio-de-la-vm-y-use-ctrlc-ctrlv-o-command-c-command-v-configure-amazon-eventbridge-para-cumplir-con-los-siguientes-requisitos-1-use-la-región-us-east-2-para-todos-los-recursos-2-a-menos-que-se-especifique-lo-contrario-a-continuación-use-la-configuración-predeterminada-3-use-su-propia-nomenclatura-de-recursos-a-menos-que-se-especifique-un-nombre-de-recurso-a-continuación-4-asegúrese-de-que-todos-los-eventos-de-amazon-ec2-en-el-bus-de-eventos-predeterminado-sean-reproducibles-replayable-durante-los-últimos-90-días-5-cree-una-regla-llamada-runfunction-para-enviar-el-mensaje-exacto-nameexample-cada-15-minutos-a-una-función-de-aws-lambda-existente-llamada-logeventfunction-6-cree-una-regla-llamada-spotwarning-para-enviar-una-notificación-a-un-nuevo-tema-estándar-de-amazon-sns-llamado-topicevents-cada-vez-que-se-interrumpa-una-instancia-spot-de-amazon-ec2-no-cree-ninguna-suscripción-al-tema-la-notificación-debe-coincidir-con-la-siguiente-estructura-input-path-instance-detailinstance-id-input-template-the-ec2-spot-instance-instance-has-been-interrupted-importante-haga-clic-en-el-botón-next-para-completar-este-laboratorio-y-continuar-al-siguiente-una-vez-que-haga-clic-en-el-botón-next-no-podrá-volver-a-este-laboratorio) |
| 54 | [Una empresa tiene una carga de trabajo con estado (stateful) de larga duración en una única instancia de Amazon EC2 On-Demand de propósito general xlarge. Las métricas muestran que el servicio siempre está usando `80%` de su memoria disponible y `40%` de su CPU disponible. Un ingeniero de CloudOps debe reducir el costo del servicio sin afectar negativamente el rendimiento. ¿Qué cambio en el tipo de instancia cumplirá con estos requisitos?](#una-empresa-tiene-una-carga-de-trabajo-con-estado-stateful-de-larga-duración-en-una-única-instancia-de-amazon-ec2-on-demand-de-propósito-general-xlarge-las-métricas-muestran-que-el-servicio-siempre-está-usando-80-de-su-memoria-disponible-y-40-de-su-cpu-disponible-un-ingeniero-de-cloudops-debe-reducir-el-costo-del-servicio-sin-afectar-negativamente-el-rendimiento-qué-cambio-en-el-tipo-de-instancia-cumplirá-con-estos-requisitos) |
| 55 | [Cuando la infraestructura de la nube de AWS experimenta un evento que puede afectar a una organización, ¿qué servicio de AWS se puede usar para ver cuáles recursos de la organización están afectados?](#cuando-la-infraestructura-de-la-nube-de-aws-experimenta-un-evento-que-puede-afectar-a-una-organización-qué-servicio-de-aws-se-puede-usar-para-ver-cuáles-recursos-de-la-organización-están-afectados) |
| 56 | [Una empresa ejecuta una aplicación en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias de EC2 están en un grupo de Auto Scaling. La aplicación a veces se vuelve lenta y no responde. Las métricas de Amazon CloudWatch muestran que algunas instancias de EC2 están experimentando alta carga de CPU. Un ingeniero de CloudOps necesita crear un panel (dashboard) de CloudWatch que pueda mostrar automáticamente las métricas de CPU de todas las instancias de EC2. Las métricas deben incluir las nuevas instancias que se lancen como parte del grupo de Auto Scaling. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?](#una-empresa-ejecuta-una-aplicación-en-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-las-instancias-de-ec2-están-en-un-grupo-de-auto-scaling-la-aplicación-a-veces-se-vuelve-lenta-y-no-responde-las-métricas-de-amazon-cloudwatch-muestran-que-algunas-instancias-de-ec2-están-experimentando-alta-carga-de-cpu-un-ingeniero-de-cloudops-necesita-crear-un-panel-dashboard-de-cloudwatch-que-pueda-mostrar-automáticamente-las-métricas-de-cpu-de-todas-las-instancias-de-ec2-las-métricas-deben-incluir-las-nuevas-instancias-que-se-lancen-como-parte-del-grupo-de-auto-scaling-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-de-la-manera-más-eficiente-operativamente) |
| 57 | [Una empresa ejecuta cientos de instancias de Amazon EC2 en una única región de AWS. Cada instancia de EC2 tiene dos volúmenes adjuntos de Amazon Elastic Block Store (Amazon EBS) de 1 GiB `General Purpose SSD (gp2)`. Una carga de trabajo crítica está usando toda la capacidad de IOPS disponible en los volúmenes EBS. Según la política de la empresa, esta no puede cambiar los tipos de instancia ni los tipos de volumen EBS sin completar extensas pruebas de aceptación para validar que las aplicaciones de la empresa funcionarán correctamente. Un ingeniero de CloudOps necesita aumentar el rendimiento de E/S de los volúmenes EBS lo más rápido posible. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?](#una-empresa-ejecuta-cientos-de-instancias-de-amazon-ec2-en-una-única-región-de-aws-cada-instancia-de-ec2-tiene-dos-volúmenes-adjuntos-de-amazon-elastic-block-store-amazon-ebs-de-1-gib-general-purpose-ssd-gp2-una-carga-de-trabajo-crítica-está-usando-toda-la-capacidad-de-iops-disponible-en-los-volúmenes-ebs-según-la-política-de-la-empresa-esta-no-puede-cambiar-los-tipos-de-instancia-ni-los-tipos-de-volumen-ebs-sin-completar-extensas-pruebas-de-aceptación-para-validar-que-las-aplicaciones-de-la-empresa-funcionarán-correctamente-un-ingeniero-de-cloudops-necesita-aumentar-el-rendimiento-de-es-de-los-volúmenes-ebs-lo-más-rápido-posible-qué-acción-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 58 | [Una empresa planea alojar sus aplicaciones web con estado (stateful) en AWS. Un ingeniero de CloudOps está usando un grupo de Auto Scaling de instancias de Amazon EC2. Las aplicaciones web se ejecutarán las 24 horas del día, los 7 días de la semana, durante todo el año. La empresa debe poder cambiar el tipo de instancia dentro de la misma familia de instancias más adelante en el año según los patrones de tráfico y uso. ¿Qué opción de compra de instancias EC2 cumplirá con estos requisitos de la manera MÁS rentable?](#una-empresa-planea-alojar-sus-aplicaciones-web-con-estado-stateful-en-aws-un-ingeniero-de-cloudops-está-usando-un-grupo-de-auto-scaling-de-instancias-de-amazon-ec2-las-aplicaciones-web-se-ejecutarán-las-24-horas-del-día-los-7-días-de-la-semana-durante-todo-el-año-la-empresa-debe-poder-cambiar-el-tipo-de-instancia-dentro-de-la-misma-familia-de-instancias-más-adelante-en-el-año-según-los-patrones-de-tráfico-y-uso-qué-opción-de-compra-de-instancias-ec2-cumplirá-con-estos-requisitos-de-la-manera-más-rentable) |
| 59 | [Una empresa necesita subir gigabytes de archivos todos los días. La empresa necesita lograr mayor rendimiento y velocidades de carga hacia Amazon S3. ¿Qué acción debe tomar un ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-necesita-subir-gigabytes-de-archivos-todos-los-días-la-empresa-necesita-lograr-mayor-rendimiento-y-velocidades-de-carga-hacia-amazon-s3-qué-acción-debe-tomar-un-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 60 | [Un equipo de aplicación está trabajando con un ingeniero de CloudOps para definir alarmas de Amazon CloudWatch para una aplicación. El equipo de aplicación no conoce el uso esperado ni el crecimiento esperado de la aplicación. ¿Qué solución debe recomendar el ingeniero de CloudOps?](#un-equipo-de-aplicación-está-trabajando-con-un-ingeniero-de-cloudops-para-definir-alarmas-de-amazon-cloudwatch-para-una-aplicación-el-equipo-de-aplicación-no-conoce-el-uso-esperado-ni-el-crecimiento-esperado-de-la-aplicación-qué-solución-debe-recomendar-el-ingeniero-de-cloudops) |
| 61 | [Una empresa de comercio electrónico usa un clúster de Amazon ElastiCache for Memcached para el almacenamiento en caché en memoria de consultas de productos populares en el sitio de compras. Al revisar los datos recientes de métricas de Amazon CloudWatch para el clúster de ElastiCache, el ingeniero de CloudOps nota una gran cantidad de desalojos (evictions). ¿Cuál de las siguientes acciones reducirá estos desalojos? (Elija dos.)](#una-empresa-de-comercio-electrónico-usa-un-clúster-de-amazon-elasticache-for-memcached-para-el-almacenamiento-en-caché-en-memoria-de-consultas-de-productos-populares-en-el-sitio-de-compras-al-revisar-los-datos-recientes-de-métricas-de-amazon-cloudwatch-para-el-clúster-de-elasticache-el-ingeniero-de-cloudops-nota-una-gran-cantidad-de-desalojos-evictions-cuál-de-las-siguientes-acciones-reducirá-estos-desalojos-elija-dos) |
| 62 | [Una empresa necesita garantizar un cumplimiento estricto de un presupuesto para 25 aplicaciones desplegadas en AWS. Equipos separados son responsables de los costos de almacenamiento, cómputo y base de datos. Un ingeniero de CloudOps debe implementar una solución automatizada para alertar a cada equipo cuando su gasto proyectado exceda un monto trimestral establecido por el departamento de finanzas. La solución no puede incurrir en costos adicionales de cómputo, almacenamiento o base de datos. ¿Qué solución cumple con estos requisitos?](#una-empresa-necesita-garantizar-un-cumplimiento-estricto-de-un-presupuesto-para-25-aplicaciones-desplegadas-en-aws-equipos-separados-son-responsables-de-los-costos-de-almacenamiento-cómputo-y-base-de-datos-un-ingeniero-de-cloudops-debe-implementar-una-solución-automatizada-para-alertar-a-cada-equipo-cuando-su-gasto-proyectado-exceda-un-monto-trimestral-establecido-por-el-departamento-de-finanzas-la-solución-no-puede-incurrir-en-costos-adicionales-de-cómputo-almacenamiento-o-base-de-datos-qué-solución-cumple-con-estos-requisitos) |
| 63 | [Se requiere que un ingeniero de CloudOps monitoree el espacio libre en volúmenes de Amazon EBS adjuntos a instancias de Amazon EC2 basadas en Microsoft Windows dentro de la cuenta de una empresa. El ingeniero debe recibir alertas sobre posibles problemas. ¿Qué debe hacer el ingeniero para recibir alertas por correo electrónico antes de que el poco espacio de almacenamiento afecte el rendimiento de la instancia de EC2?](#se-requiere-que-un-ingeniero-de-cloudops-monitoree-el-espacio-libre-en-volúmenes-de-amazon-ebs-adjuntos-a-instancias-de-amazon-ec2-basadas-en-microsoft-windows-dentro-de-la-cuenta-de-una-empresa-el-ingeniero-debe-recibir-alertas-sobre-posibles-problemas-qué-debe-hacer-el-ingeniero-para-recibir-alertas-por-correo-electrónico-antes-de-que-el-poco-espacio-de-almacenamiento-afecte-el-rendimiento-de-la-instancia-de-ec2) |
| 64 | [Un ingeniero de CloudOps quiere monitorear el espacio libre en disco disponible en un conjunto de instancias de Amazon EC2 que tienen volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos. El ingeniero de CloudOps quiere recibir una notificación cuando el espacio de disco usado de los volúmenes EBS supere un valor umbral, pero solo cuando la métrica `DiskReadOps` también supere un valor umbral. El ingeniero de CloudOps ha configurado un tema de Amazon Simple Notification Service (Amazon SNS). ¿Cómo puede el ingeniero de CloudOps recibir la notificación solo cuando ambas métricas superen sus valores umbral?](#un-ingeniero-de-cloudops-quiere-monitorear-el-espacio-libre-en-disco-disponible-en-un-conjunto-de-instancias-de-amazon-ec2-que-tienen-volúmenes-de-amazon-elastic-block-store-amazon-ebs-adjuntos-el-ingeniero-de-cloudops-quiere-recibir-una-notificación-cuando-el-espacio-de-disco-usado-de-los-volúmenes-ebs-supere-un-valor-umbral-pero-solo-cuando-la-métrica-diskreadops-también-supere-un-valor-umbral-el-ingeniero-de-cloudops-ha-configurado-un-tema-de-amazon-simple-notification-service-amazon-sns-cómo-puede-el-ingeniero-de-cloudops-recibir-la-notificación-solo-cuando-ambas-métricas-superen-sus-valores-umbral) |
| 65 | [Una empresa quiere reducir costos para trabajos que se pueden completar en cualquier momento. Los trabajos actualmente se ejecutan usando múltiples instancias de Amazon EC2 On-Demand y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier motivo, debe reiniciarse desde el principio. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?](#una-empresa-quiere-reducir-costos-para-trabajos-que-se-pueden-completar-en-cualquier-momento-los-trabajos-actualmente-se-ejecutan-usando-múltiples-instancias-de-amazon-ec2-on-demand-y-tardan-un-poco-menos-de-2-horas-en-completarse-si-un-trabajo-falla-por-cualquier-motivo-debe-reiniciarse-desde-el-principio-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-rentable) |
| 66 | [Un entorno consta de 100 instancias de Amazon EC2 Windows. El agente de Amazon CloudWatch está desplegado y ejecutándose en todas las instancias de EC2 con un archivo de configuración base para capturar archivos de registro. Existe un nuevo requisito para capturar los archivos de registro `DHCP` que existen en 50 de las instancias. ¿Cuál es la forma MÁS eficiente operativamente para cumplir con este nuevo requisito?](#un-entorno-consta-de-100-instancias-de-amazon-ec2-windows-el-agente-de-amazon-cloudwatch-está-desplegado-y-ejecutándose-en-todas-las-instancias-de-ec2-con-un-archivo-de-configuración-base-para-capturar-archivos-de-registro-existe-un-nuevo-requisito-para-capturar-los-archivos-de-registro-dhcp-que-existen-en-50-de-las-instancias-cuál-es-la-forma-más-eficiente-operativamente-para-cumplir-con-este-nuevo-requisito) |
| 67 | [Una empresa necesita monitorear la utilización de disco de volúmenes de Amazon Elastic Block Store (Amazon EBS). Los volúmenes EBS están adjuntos a instancias de Amazon EC2 Linux. Un ingeniero de CloudOps debe configurar una alarma de Amazon CloudWatch que emita una alerta cuando la utilización de disco aumente a más del `80%`. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija tres.)](#una-empresa-necesita-monitorear-la-utilización-de-disco-de-volúmenes-de-amazon-elastic-block-store-amazon-ebs-los-volúmenes-ebs-están-adjuntos-a-instancias-de-amazon-ec2-linux-un-ingeniero-de-cloudops-debe-configurar-una-alarma-de-amazon-cloudwatch-que-emita-una-alerta-cuando-la-utilización-de-disco-aumente-a-más-del-80-qué-combinación-de-pasos-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-elija-tres) |
| 68 | [Un ingeniero de CloudOps administra una aplicación web que se ejecuta en instancias de Amazon EC2 detrás de un ELB Application Load Balancer (ALB). Las instancias se ejecutan en un grupo de EC2 Auto Scaling. El ingeniero quiere establecer una alarma para cuando todas las instancias de destino asociadas con el `ALB` estén no saludables. ¿Qué condición se debe usar con la alarma?](#un-ingeniero-de-cloudops-administra-una-aplicación-web-que-se-ejecuta-en-instancias-de-amazon-ec2-detrás-de-un-elb-application-load-balancer-alb-las-instancias-se-ejecutan-en-un-grupo-de-ec2-auto-scaling-el-ingeniero-quiere-establecer-una-alarma-para-cuando-todas-las-instancias-de-destino-asociadas-con-el-alb-estén-no-saludables-qué-condición-se-debe-usar-con-la-alarma) |
| 69 | [Una empresa quiere monitorear los grupos de seguridad de sus instancias de Amazon EC2 para asegurarse de que `SSH` no esté abierto al público. Si el puerto está abierto, la empresa necesita cerrarlo lo antes posible. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)](#una-empresa-quiere-monitorear-los-grupos-de-seguridad-de-sus-instancias-de-amazon-ec2-para-asegurarse-de-que-ssh-no-esté-abierto-al-público-si-el-puerto-está-abierto-la-empresa-necesita-cerrarlo-lo-antes-posible-qué-combinación-de-acciones-debe-tomar-un-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-elija-dos) |
| 70 | [Una empresa aloja una aplicación interna en instancias de Amazon EC2 On-Demand detrás de un Application Load Balancer (ALB). Las instancias están en un grupo de Amazon EC2 Auto Scaling. Los empleados usan la aplicación para proporcionar precios de productos a clientes potenciales. El grupo de Auto Scaling está configurado con una política de escalado dinámico y rastrea el uso promedio de CPU de las instancias. Los empleados han notado que a veces la aplicación se vuelve lenta o no responde. Un ingeniero de CloudOps descubre que algunas instancias están experimentando una alta carga de CPU. El grupo de Auto Scaling no puede escalar hacia afuera porque la empresa está alcanzando la cuota de servicio de instancias de EC2. El ingeniero de CloudOps necesita implementar una solución que proporcione una notificación cuando la empresa alcance el `70%` o más de la cuota de servicio de instancias de EC2. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?](#una-empresa-aloja-una-aplicación-interna-en-instancias-de-amazon-ec2-on-demand-detrás-de-un-application-load-balancer-alb-las-instancias-están-en-un-grupo-de-amazon-ec2-auto-scaling-los-empleados-usan-la-aplicación-para-proporcionar-precios-de-productos-a-clientes-potenciales-el-grupo-de-auto-scaling-está-configurado-con-una-política-de-escalado-dinámico-y-rastrea-el-uso-promedio-de-cpu-de-las-instancias-los-empleados-han-notado-que-a-veces-la-aplicación-se-vuelve-lenta-o-no-responde-un-ingeniero-de-cloudops-descubre-que-algunas-instancias-están-experimentando-una-alta-carga-de-cpu-el-grupo-de-auto-scaling-no-puede-escalar-hacia-afuera-porque-la-empresa-está-alcanzando-la-cuota-de-servicio-de-instancias-de-ec2-el-ingeniero-de-cloudops-necesita-implementar-una-solución-que-proporcione-una-notificación-cuando-la-empresa-alcance-el-70-o-más-de-la-cuota-de-servicio-de-instancias-de-ec2-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-eficiente-operativamente) |
| 71 | [Un equipo de desarrolladores usa varios buckets de Amazon S3 como repositorios centralizados. Usuarios de todo el mundo suben grandes conjuntos de archivos a estos repositorios. Las aplicaciones del equipo de desarrollo procesan estos archivos posteriormente. Un ingeniero de CloudOps configura un nuevo bucket de S3, `DOC-EXAMPLE-BUCKET`, para soportar una nueva carga de trabajo. El nuevo bucket de S3 también recibe cargas regulares de grandes conjuntos de archivos de usuarios de todo el mundo. Cuando el nuevo bucket de S3 entra en producción, el rendimiento de carga desde ciertas áreas geográficas es menor que el rendimiento de carga que proporcionan los buckets de S3 existentes. ¿Qué debe hacer el ingeniero de CloudOps para remediar este problema?](#un-equipo-de-desarrolladores-usa-varios-buckets-de-amazon-s3-como-repositorios-centralizados-usuarios-de-todo-el-mundo-suben-grandes-conjuntos-de-archivos-a-estos-repositorios-las-aplicaciones-del-equipo-de-desarrollo-procesan-estos-archivos-posteriormente-un-ingeniero-de-cloudops-configura-un-nuevo-bucket-de-s3-doc-example-bucket-para-soportar-una-nueva-carga-de-trabajo-el-nuevo-bucket-de-s3-también-recibe-cargas-regulares-de-grandes-conjuntos-de-archivos-de-usuarios-de-todo-el-mundo-cuando-el-nuevo-bucket-de-s3-entra-en-producción-el-rendimiento-de-carga-desde-ciertas-áreas-geográficas-es-menor-que-el-rendimiento-de-carga-que-proporcionan-los-buckets-de-s3-existentes-qué-debe-hacer-el-ingeniero-de-cloudops-para-remediar-este-problema) |
| 72 | [Una empresa tiene usuarios que despliegan instancias de Amazon EC2 con más capacidad de rendimiento de disco de la requerida. Un ingeniero de CloudOps necesita revisar todos los volúmenes de Amazon Elastic Block Store (Amazon EBS) asociados con las instancias y crear recomendaciones de optimización de costos basadas en IOPS y rendimiento (throughput). ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?](#una-empresa-tiene-usuarios-que-despliegan-instancias-de-amazon-ec2-con-más-capacidad-de-rendimiento-de-disco-de-la-requerida-un-ingeniero-de-cloudops-necesita-revisar-todos-los-volúmenes-de-amazon-elastic-block-store-amazon-ebs-asociados-con-las-instancias-y-crear-recomendaciones-de-optimización-de-costos-basadas-en-iops-y-rendimiento-throughput-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-de-la-manera-más-eficiente-operativamente) |
| 73 | [Una empresa ha creado una puerta de enlace `NAT` en una subred pública en una `VPC`. La `VPC` también contiene una subred privada que incluye instancias de Amazon EC2. Las instancias de EC2 usan la puerta de enlace `NAT` para acceder a internet y descargar parches y actualizaciones. La empresa ha configurado un flow log de `VPC` para la interfaz de red elástica de la puerta de enlace `NAT`. La empresa está publicando la salida en Amazon CloudWatch Logs. Un ingeniero de CloudOps debe identificar los cinco destinos de internet principales con los que se comunican las instancias de EC2 en la subred privada para las descargas. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito de la manera MÁS eficiente operativamente?](#una-empresa-ha-creado-una-puerta-de-enlace-nat-en-una-subred-pública-en-una-vpc-la-vpc-también-contiene-una-subred-privada-que-incluye-instancias-de-amazon-ec2-las-instancias-de-ec2-usan-la-puerta-de-enlace-nat-para-acceder-a-internet-y-descargar-parches-y-actualizaciones-la-empresa-ha-configurado-un-flow-log-de-vpc-para-la-interfaz-de-red-elástica-de-la-puerta-de-enlace-nat-la-empresa-está-publicando-la-salida-en-amazon-cloudwatch-logs-un-ingeniero-de-cloudops-debe-identificar-los-cinco-destinos-de-internet-principales-con-los-que-se-comunican-las-instancias-de-ec2-en-la-subred-privada-para-las-descargas-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito-de-la-manera-más-eficiente-operativamente) |
| 74 | [Una empresa ejecuta una aplicación web de una sola página en AWS. La aplicación usa Amazon CloudFront para entregar contenido estático desde un origen de bucket de Amazon S3. La aplicación también usa un clúster de Amazon Elastic Kubernetes Service (Amazon EKS) para atender llamadas de API. Los usuarios a veces reportan que el sitio web no está operativo, incluso cuando el monitoreo muestra que la página de inicio es alcanzable y que el clúster de EKS está saludable. Un ingeniero de CloudOps debe implementar monitoreo adicional que pueda detectar cuándo el sitio web no está operativo antes de que los usuarios reporten el problema. ¿Qué solución cumple con estos requisitos?](#una-empresa-ejecuta-una-aplicación-web-de-una-sola-página-en-aws-la-aplicación-usa-amazon-cloudfront-para-entregar-contenido-estático-desde-un-origen-de-bucket-de-amazon-s3-la-aplicación-también-usa-un-clúster-de-amazon-elastic-kubernetes-service-amazon-eks-para-atender-llamadas-de-api-los-usuarios-a-veces-reportan-que-el-sitio-web-no-está-operativo-incluso-cuando-el-monitoreo-muestra-que-la-página-de-inicio-es-alcanzable-y-que-el-clúster-de-eks-está-saludable-un-ingeniero-de-cloudops-debe-implementar-monitoreo-adicional-que-pueda-detectar-cuándo-el-sitio-web-no-está-operativo-antes-de-que-los-usuarios-reporten-el-problema-qué-solución-cumple-con-estos-requisitos) |
| 75 | [Una empresa está haciendo la transición desde aplicaciones alojadas en instancias de Amazon EC2. La empresa quiere implementar una arquitectura sin servidor (serverless) que use Amazon S3, Amazon API Gateway, AWS Lambda y Amazon CloudFront. Como parte de esta transición, la empresa tiene direcciones IP elásticas que no están asociadas con ninguna instancia de EC2 después de que estas se terminan. Un ingeniero de CloudOps necesita automatizar el proceso de liberar todas las direcciones IP elásticas no asociadas que permanecen después de que las instancias de EC2 se terminan. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?](#una-empresa-está-haciendo-la-transición-desde-aplicaciones-alojadas-en-instancias-de-amazon-ec2-la-empresa-quiere-implementar-una-arquitectura-sin-servidor-serverless-que-use-amazon-s3-amazon-api-gateway-aws-lambda-y-amazon-cloudfront-como-parte-de-esta-transición-la-empresa-tiene-direcciones-ip-elásticas-que-no-están-asociadas-con-ninguna-instancia-de-ec2-después-de-que-estas-se-terminan-un-ingeniero-de-cloudops-necesita-automatizar-el-proceso-de-liberar-todas-las-direcciones-ip-elásticas-no-asociadas-que-permanecen-después-de-que-las-instancias-de-ec2-se-terminan-qué-solución-cumple-con-este-requisito-de-la-manera-más-eficiente-operativamente) |
| 76 | [El uso de servicios de AWS Cloud de una empresa está creciendo rápidamente, por lo que se le ha pedido a un ingeniero de CloudOps que genere detalles del gasto diario para compartir con la gerencia. ¿Qué método debe elegir el ingeniero para producir estos datos?](#el-uso-de-servicios-de-aws-cloud-de-una-empresa-está-creciendo-rápidamente-por-lo-que-se-le-ha-pedido-a-un-ingeniero-de-cloudops-que-genere-detalles-del-gasto-diario-para-compartir-con-la-gerencia-qué-método-debe-elegir-el-ingeniero-para-producir-estos-datos) |
| 77 | [Los usuarios están experimentando periódicamente tiempos de respuesta lentos de una base de datos relacional. La base de datos se ejecuta en una instancia ráfaga (burstable) de Amazon EC2 con un volumen de Amazon Elastic Block Store (Amazon EBS) `General Purpose SSD (gp2)` de `350 GB`. Un ingeniero de CloudOps monitorea la instancia de EC2 en Amazon CloudWatch y observa que la métrica `VolumeReadOps` cae a menos del `10%` de su valor máximo durante los períodos de respuesta lenta. ¿Qué debe hacer el ingeniero de CloudOps para asegurar un rendimiento consistentemente alto?](#los-usuarios-están-experimentando-periódicamente-tiempos-de-respuesta-lentos-de-una-base-de-datos-relacional-la-base-de-datos-se-ejecuta-en-una-instancia-ráfaga-burstable-de-amazon-ec2-con-un-volumen-de-amazon-elastic-block-store-amazon-ebs-general-purpose-ssd-gp2-de-350-gb-un-ingeniero-de-cloudops-monitorea-la-instancia-de-ec2-en-amazon-cloudwatch-y-observa-que-la-métrica-volumereadops-cae-a-menos-del-10-de-su-valor-máximo-durante-los-períodos-de-respuesta-lenta-qué-debe-hacer-el-ingeniero-de-cloudops-para-asegurar-un-rendimiento-consistentemente-alto) |
| 78 | [AnyCompany ha adquirido Example Corp y está intentando consolidar los sistemas empresariales de ambas compañías. El departamento de TI de AnyCompany necesita integrarse con el sistema de tickets de TI de Example Corp. Un ingeniero de CloudOps debe implementar una solución que use alarmas de Amazon CloudWatch para instancias de Amazon EC2 en la cuenta de AnyCompany para crear nuevos tickets en el sistema de tickets de Example Corp. El sistema de tickets proporciona un endpoint `HTTPS` para la creación de nuevos tickets. El sistema de tickets acepta mensajes en el siguiente formato JSON. ¿Qué enfoque para crear tickets a partir de las alarmas de CloudWatch cumple con estos requisitos con el MENOR tiempo de desarrollo?](#anycompany-ha-adquirido-example-corp-y-está-intentando-consolidar-los-sistemas-empresariales-de-ambas-compañías-el-departamento-de-ti-de-anycompany-necesita-integrarse-con-el-sistema-de-tickets-de-ti-de-example-corp-un-ingeniero-de-cloudops-debe-implementar-una-solución-que-use-alarmas-de-amazon-cloudwatch-para-instancias-de-amazon-ec2-en-la-cuenta-de-anycompany-para-crear-nuevos-tickets-en-el-sistema-de-tickets-de-example-corp-el-sistema-de-tickets-proporciona-un-endpoint-https-para-la-creación-de-nuevos-tickets-el-sistema-de-tickets-acepta-mensajes-en-el-siguiente-formato-json-qué-enfoque-para-crear-tickets-a-partir-de-las-alarmas-de-cloudwatch-cumple-con-estos-requisitos-con-el-menor-tiempo-de-desarrollo) |
| 79 | [Una empresa ejecuta sus aplicaciones en una gran cantidad de instancias de Amazon EC2. Un ingeniero de CloudOps debe implementar una solución para notificar al equipo de operaciones cada vez que cambie el estado de una instancia de EC2. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-ejecuta-sus-aplicaciones-en-una-gran-cantidad-de-instancias-de-amazon-ec2-un-ingeniero-de-cloudops-debe-implementar-una-solución-para-notificar-al-equipo-de-operaciones-cada-vez-que-cambie-el-estado-de-una-instancia-de-ec2-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 80 | [Una empresa necesita hacer cumplir los requisitos de etiquetado para tablas de Amazon DynamoDB en sus cuentas de AWS. Un ingeniero de CloudOps debe implementar una solución para identificar y remediar todas las tablas de DynamoDB que no tengan las etiquetas apropiadas. ¿Qué solución cumple con estos requisitos con el MENOR esfuerzo operativo?](#una-empresa-necesita-hacer-cumplir-los-requisitos-de-etiquetado-para-tablas-de-amazon-dynamodb-en-sus-cuentas-de-aws-un-ingeniero-de-cloudops-debe-implementar-una-solución-para-identificar-y-remediar-todas-las-tablas-de-dynamodb-que-no-tengan-las-etiquetas-apropiadas-qué-solución-cumple-con-estos-requisitos-con-el-menor-esfuerzo-operativo) |
| 81 | [Una empresa quiere rastrear sus costos de AWS en todas las cuentas miembro que forman parte de una organización en AWS Organizations. Los administradores de las cuentas miembro quieren recibir una notificación cuando los costos estimados superen un monto predeterminado cada mes. Los administradores no pueden configurar una alarma de facturación. Los permisos de IAM para todos los usuarios son correctos. ¿Cuál podría ser la causa de este problema?](#una-empresa-quiere-rastrear-sus-costos-de-aws-en-todas-las-cuentas-miembro-que-forman-parte-de-una-organización-en-aws-organizations-los-administradores-de-las-cuentas-miembro-quieren-recibir-una-notificación-cuando-los-costos-estimados-superen-un-monto-predeterminado-cada-mes-los-administradores-no-pueden-configurar-una-alarma-de-facturación-los-permisos-de-iam-para-todos-los-usuarios-son-correctos-cuál-podría-ser-la-causa-de-este-problema) |
| 82 | [Una empresa de servicios financieros está ejecutando software de computación distribuida para administrar una flota de 20 servidores para sus cálculos. Hay 2 nodos de control y 18 nodos trabajadores (worker) que ejecutan los cálculos. Los nodos de control pueden iniciar automáticamente los nodos trabajadores cuando sea necesario. Actualmente, todos los nodos se ejecutan on-demand, y los nodos trabajadores se usan aproximadamente 4 horas cada día. ¿Qué combinación de acciones será MÁS rentable? (Elija dos.)](#una-empresa-de-servicios-financieros-está-ejecutando-software-de-computación-distribuida-para-administrar-una-flota-de-20-servidores-para-sus-cálculos-hay-2-nodos-de-control-y-18-nodos-trabajadores-worker-que-ejecutan-los-cálculos-los-nodos-de-control-pueden-iniciar-automáticamente-los-nodos-trabajadores-cuando-sea-necesario-actualmente-todos-los-nodos-se-ejecutan-on-demand-y-los-nodos-trabajadores-se-usan-aproximadamente-4-horas-cada-día-qué-combinación-de-acciones-será-más-rentable-elija-dos) |
| 83 | [Una empresa tiene una aplicación web que experimenta problemas de rendimiento varias veces cada noche. Un análisis de causa raíz revela picos en el uso de CPU que duran 5 minutos en una instancia de Amazon EC2 Linux. Se le encarga a un ingeniero de CloudOps encontrar el ID de proceso (PID) del servicio o proceso que está consumiendo más CPU. ¿Cómo puede el ingeniero lograr esto con el MENOR esfuerzo?](#una-empresa-tiene-una-aplicación-web-que-experimenta-problemas-de-rendimiento-varias-veces-cada-noche-un-análisis-de-causa-raíz-revela-picos-en-el-uso-de-cpu-que-duran-5-minutos-en-una-instancia-de-amazon-ec2-linux-se-le-encarga-a-un-ingeniero-de-cloudops-encontrar-el-id-de-proceso-pid-del-servicio-o-proceso-que-está-consumiendo-más-cpu-cómo-puede-el-ingeniero-lograr-esto-con-el-menor-esfuerzo) |
| 84 | [Se le ha pedido a un ingeniero de CloudOps que configure etiquetas de asignación de costos definidas por el usuario para una nueva cuenta de AWS. La empresa usa AWS Organizations para la administración de cuentas. ¿Qué debe hacer el ingeniero para habilitar las etiquetas de asignación de costos definidas por el usuario?](#se-le-ha-pedido-a-un-ingeniero-de-cloudops-que-configure-etiquetas-de-asignación-de-costos-definidas-por-el-usuario-para-una-nueva-cuenta-de-aws-la-empresa-usa-aws-organizations-para-la-administración-de-cuentas-qué-debe-hacer-el-ingeniero-para-habilitar-las-etiquetas-de-asignación-de-costos-definidas-por-el-usuario) |
| 85 | [Un volumen de Amazon EBS adjunto a una instancia de EC2 fue modificado recientemente. Parte de la modificación incluyó aumentar la capacidad de almacenamiento. El ingeniero de CloudOps nota que la capacidad de almacenamiento aumentada no se refleja en el sistema de archivos. ¿Qué paso debe completar el ingeniero para usar la capacidad de almacenamiento aumentada?](#un-volumen-de-amazon-ebs-adjunto-a-una-instancia-de-ec2-fue-modificado-recientemente-parte-de-la-modificación-incluyó-aumentar-la-capacidad-de-almacenamiento-el-ingeniero-de-cloudops-nota-que-la-capacidad-de-almacenamiento-aumentada-no-se-refleja-en-el-sistema-de-archivos-qué-paso-debe-completar-el-ingeniero-para-usar-la-capacidad-de-almacenamiento-aumentada) |
| 86 | [Un ingeniero de CloudOps es responsable de una gran flota de instancias de EC2 y debe saber si alguna instancia se verá afectada por el próximo mantenimiento de hardware. ¿Qué opción proporcionaría esta información con el MENOR esfuerzo administrativo?](#un-ingeniero-de-cloudops-es-responsable-de-una-gran-flota-de-instancias-de-ec2-y-debe-saber-si-alguna-instancia-se-verá-afectada-por-el-próximo-mantenimiento-de-hardware-qué-opción-proporcionaría-esta-información-con-el-menor-esfuerzo-administrativo) |
| 87 | [Una empresa aloja una aplicación web en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias están en un grupo de Amazon EC2 Auto Scaling. Se accede a la aplicación con una URL pública. Un ingeniero de CloudOps necesita implementar una solución de monitoreo que verifique la disponibilidad de la aplicación y siga las mismas rutas y acciones que un cliente. El ingeniero de CloudOps debe recibir una notificación si menos del `95%` de las ejecuciones de monitoreo no encuentran errores. ¿Qué solución cumple con estos requisitos?](#una-empresa-aloja-una-aplicación-web-en-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-las-instancias-están-en-un-grupo-de-amazon-ec2-auto-scaling-se-accede-a-la-aplicación-con-una-url-pública-un-ingeniero-de-cloudops-necesita-implementar-una-solución-de-monitoreo-que-verifique-la-disponibilidad-de-la-aplicación-y-siga-las-mismas-rutas-y-acciones-que-un-cliente-el-ingeniero-de-cloudops-debe-recibir-una-notificación-si-menos-del-95-de-las-ejecuciones-de-monitoreo-no-encuentran-errores-qué-solución-cumple-con-estos-requisitos) |
| 88 | [Un ingeniero de CloudOps que trabaja en una instancia de Amazon EC2 ha configurado incorrectamente el reloj por una hora. La instancia de EC2 está enviando datos a Amazon CloudWatch a través del agente de CloudWatch. Las marcas de tiempo en los registros están 45 minutos en el futuro. ¿Cuál será el resultado de esta configuración?](#un-ingeniero-de-cloudops-que-trabaja-en-una-instancia-de-amazon-ec2-ha-configurado-incorrectamente-el-reloj-por-una-hora-la-instancia-de-ec2-está-enviando-datos-a-amazon-cloudwatch-a-través-del-agente-de-cloudwatch-las-marcas-de-tiempo-en-los-registros-están-45-minutos-en-el-futuro-cuál-será-el-resultado-de-esta-configuración) |
| 89 | [Un ingeniero de CloudOps ha configurado un agente de CloudWatch para enviar métricas personalizadas a Amazon CloudWatch y ahora está ensamblando un panel de CloudWatch para mostrar estas métricas. ¿Qué pasos debe tomar el ingeniero para completar esta tarea?](#un-ingeniero-de-cloudops-ha-configurado-un-agente-de-cloudwatch-para-enviar-métricas-personalizadas-a-amazon-cloudwatch-y-ahora-está-ensamblando-un-panel-de-cloudwatch-para-mostrar-estas-métricas-qué-pasos-debe-tomar-el-ingeniero-para-completar-esta-tarea) |
| 90 | [Un ingeniero de CloudOps está manteniendo una aplicación que se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Los usuarios reportan errores al intentar iniciar la aplicación. El ingeniero nota un aumento en la métrica de Amazon CloudWatch `HTTPCode_ELB_5xx_Count` para el balanceador de carga. ¿Cuál es una posible causa de este aumento?](#un-ingeniero-de-cloudops-está-manteniendo-una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-alb-los-usuarios-reportan-errores-al-intentar-iniciar-la-aplicación-el-ingeniero-nota-un-aumento-en-la-métrica-de-amazon-cloudwatch-httpcode_elb_5xx_count-para-el-balanceador-de-carga-cuál-es-una-posible-causa-de-este-aumento) |
| 91 | [Una empresa está usando alarmas de Amazon CloudWatch para monitorear cargas de trabajo de Amazon Elastic Kubernetes Service (Amazon EKS). Las alarmas se inician a través de una definición de umbral y no están ayudando a que el clúster de EKS opere de manera más eficiente. Un ingeniero de CloudOps debe implementar una solución que identifique anomalías y genere recomendaciones sobre cómo abordarlas. ¿Qué solución cumple con estos requisitos?](#una-empresa-está-usando-alarmas-de-amazon-cloudwatch-para-monitorear-cargas-de-trabajo-de-amazon-elastic-kubernetes-service-amazon-eks-las-alarmas-se-inician-a-través-de-una-definición-de-umbral-y-no-están-ayudando-a-que-el-clúster-de-eks-opere-de-manera-más-eficiente-un-ingeniero-de-cloudops-debe-implementar-una-solución-que-identifique-anomalías-y-genere-recomendaciones-sobre-cómo-abordarlas-qué-solución-cumple-con-estos-requisitos) |
| 92 | [Una empresa desplegó recientemente MySQL en una instancia de Amazon EC2 con un volumen de arranque predeterminado. La empresa tiene la intención de restaurar una base de datos de 1.75 TB. Un ingeniero de CloudOps necesita aprovisionar el volumen correcto de Amazon Elastic Block Store (Amazon EBS). La base de datos requerirá un rendimiento de lectura de hasta 10,000 IOPS y no se espera que crezca en tamaño. ¿Qué solución proporcionará el rendimiento requerido al MENOR costo?](#una-empresa-desplegó-recientemente-mysql-en-una-instancia-de-amazon-ec2-con-un-volumen-de-arranque-predeterminado-la-empresa-tiene-la-intención-de-restaurar-una-base-de-datos-de-175-tb-un-ingeniero-de-cloudops-necesita-aprovisionar-el-volumen-correcto-de-amazon-elastic-block-store-amazon-ebs-la-base-de-datos-requerirá-un-rendimiento-de-lectura-de-hasta-10000-iops-y-no-se-espera-que-crezca-en-tamaño-qué-solución-proporcionará-el-rendimiento-requerido-al-menor-costo) |
| 93 | [Una aplicación que se ejecuta en Amazon EC2 permite a los usuarios lanzar trabajos por lotes (batch jobs) para análisis de datos. Los trabajos se ejecutan de forma asíncrona, y se notifica al usuario cuando se completan. Aunque pueden ejecutarse múltiples trabajos simultáneamente, la solicitud de un usuario no necesita cumplirse hasta dentro de 24 horas. Para ejecutar un trabajo, la aplicación lanza una instancia de EC2 adicional que realiza todos los cálculos analíticos. Un trabajo tarda entre 75 y 110 minutos en completarse y no se puede interrumpir. ¿Cuál es la forma MÁS rentable de ejecutar esta carga de trabajo?](#una-aplicación-que-se-ejecuta-en-amazon-ec2-permite-a-los-usuarios-lanzar-trabajos-por-lotes-batch-jobs-para-análisis-de-datos-los-trabajos-se-ejecutan-de-forma-asíncrona-y-se-notifica-al-usuario-cuando-se-completan-aunque-pueden-ejecutarse-múltiples-trabajos-simultáneamente-la-solicitud-de-un-usuario-no-necesita-cumplirse-hasta-dentro-de-24-horas-para-ejecutar-un-trabajo-la-aplicación-lanza-una-instancia-de-ec2-adicional-que-realiza-todos-los-cálculos-analíticos-un-trabajo-tarda-entre-75-y-110-minutos-en-completarse-y-no-se-puede-interrumpir-cuál-es-la-forma-más-rentable-de-ejecutar-esta-carga-de-trabajo) |
| 94 | [Una empresa de comercio electrónico quiere reducir costos en sus trabajos nocturnos que agregan las ventas del día actual y almacenan los resultados en Amazon S3. Los trabajos actualmente se ejecutan usando múltiples instancias on-demand y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier razón, debe reiniciarse desde el principio. ¿Qué método es el MÁS rentable según estos requisitos?](#una-empresa-de-comercio-electrónico-quiere-reducir-costos-en-sus-trabajos-nocturnos-que-agregan-las-ventas-del-día-actual-y-almacenan-los-resultados-en-amazon-s3-los-trabajos-actualmente-se-ejecutan-usando-múltiples-instancias-on-demand-y-tardan-un-poco-menos-de-2-horas-en-completarse-si-un-trabajo-falla-por-cualquier-razón-debe-reiniciarse-desde-el-principio-qué-método-es-el-más-rentable-según-estos-requisitos) |
| 95 | [Una empresa quiere reducir costos en trabajos que se pueden completar en cualquier momento. Los trabajos actualmente se ejecutan usando múltiples instancias On-Demand, y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier razón, se puede reiniciar desde el principio. ¿Qué método es el MÁS rentable según estos requisitos?](#una-empresa-quiere-reducir-costos-en-trabajos-que-se-pueden-completar-en-cualquier-momento-los-trabajos-actualmente-se-ejecutan-usando-múltiples-instancias-on-demand-y-tardan-un-poco-menos-de-2-horas-en-completarse-si-un-trabajo-falla-por-cualquier-razón-se-puede-reiniciar-desde-el-principio-qué-método-es-el-más-rentable-según-estos-requisitos) |
| 96 | [Un ingeniero de CloudOps necesita recopilar el contenido de archivos de registro de una aplicación personalizada que está desplegada en cientos de instancias de Amazon EC2 que ejecutan Ubuntu. Los archivos de registro deben almacenarse en Amazon CloudWatch Logs. ¿Cómo debe el ingeniero de CloudOps recopilar los archivos de registro de la aplicación con el MENOR esfuerzo operativo?](#un-ingeniero-de-cloudops-necesita-recopilar-el-contenido-de-archivos-de-registro-de-una-aplicación-personalizada-que-está-desplegada-en-cientos-de-instancias-de-amazon-ec2-que-ejecutan-ubuntu-los-archivos-de-registro-deben-almacenarse-en-amazon-cloudwatch-logs-cómo-debe-el-ingeniero-de-cloudops-recopilar-los-archivos-de-registro-de-la-aplicación-con-el-menor-esfuerzo-operativo) |
| 97 | [Una empresa tiene un clúster de instancias Spot de Amazon EC2 Linux que leen muchos archivos de, y escriben muchos archivos en, volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos. Las instancias de EC2 se inician y se detienen con frecuencia. Como parte del proceso cuando se inicia una instancia de EC2, se restaura un volumen EBS a partir de una instantánea. Los volúmenes EBS que se restauran a partir de instantáneas están experimentando un rendimiento inicial más bajo de lo esperado. La carga de trabajo de la empresa necesita casi todos los IOPS aprovisionados en los volúmenes EBS adjuntos. Las instancias de EC2 no pueden soportar la carga de trabajo cuando el rendimiento de los volúmenes EBS es demasiado bajo. Un ingeniero de CloudOps debe implementar una solución para asegurar que los volúmenes EBS proporcionen el rendimiento esperado cuando se restauren a partir de instantáneas. ¿Qué solución cumple con estos requisitos?](#una-empresa-tiene-un-clúster-de-instancias-spot-de-amazon-ec2-linux-que-leen-muchos-archivos-de-y-escriben-muchos-archivos-en-volúmenes-de-amazon-elastic-block-store-amazon-ebs-adjuntos-las-instancias-de-ec2-se-inician-y-se-detienen-con-frecuencia-como-parte-del-proceso-cuando-se-inicia-una-instancia-de-ec2-se-restaura-un-volumen-ebs-a-partir-de-una-instantánea-los-volúmenes-ebs-que-se-restauran-a-partir-de-instantáneas-están-experimentando-un-rendimiento-inicial-más-bajo-de-lo-esperado-la-carga-de-trabajo-de-la-empresa-necesita-casi-todos-los-iops-aprovisionados-en-los-volúmenes-ebs-adjuntos-las-instancias-de-ec2-no-pueden-soportar-la-carga-de-trabajo-cuando-el-rendimiento-de-los-volúmenes-ebs-es-demasiado-bajo-un-ingeniero-de-cloudops-debe-implementar-una-solución-para-asegurar-que-los-volúmenes-ebs-proporcionen-el-rendimiento-esperado-cuando-se-restauren-a-partir-de-instantáneas-qué-solución-cumple-con-estos-requisitos) |
| 98 | [Los usuarios del sitio web reportan que las páginas de una aplicación se cargan lentamente al comienzo de la jornada laboral. La aplicación se ejecuta en instancias de Amazon EC2, y los datos se almacenan en una base de datos de Amazon RDS. El ingeniero de CloudOps sospecha que el problema está relacionado con el alto uso de CPU en un componente de esta aplicación. ¿Cómo puede el ingeniero descubrir qué componente está causando el cuello de botella de rendimiento?](#los-usuarios-del-sitio-web-reportan-que-las-páginas-de-una-aplicación-se-cargan-lentamente-al-comienzo-de-la-jornada-laboral-la-aplicación-se-ejecuta-en-instancias-de-amazon-ec2-y-los-datos-se-almacenan-en-una-base-de-datos-de-amazon-rds-el-ingeniero-de-cloudops-sospecha-que-el-problema-está-relacionado-con-el-alto-uso-de-cpu-en-un-componente-de-esta-aplicación-cómo-puede-el-ingeniero-descubrir-qué-componente-está-causando-el-cuello-de-botella-de-rendimiento) |
| 99 | [Un ingeniero de CloudOps está manteniendo una aplicación web usando una distribución web de Amazon CloudFront, un Application Load Balancer (ALB), Amazon RDS, y Amazon EC2 en una `VPC`. Todos los servicios tienen el registro habilitado. El ingeniero necesita investigar códigos de estado `HTTP` de Capa 7 de la aplicación web. ¿Qué fuentes de registro contienen los códigos de estado? (Elija dos.)](#un-ingeniero-de-cloudops-está-manteniendo-una-aplicación-web-usando-una-distribución-web-de-amazon-cloudfront-un-application-load-balancer-alb-amazon-rds-y-amazon-ec2-en-una-vpc-todos-los-servicios-tienen-el-registro-habilitado-el-ingeniero-necesita-investigar-códigos-de-estado-http-de-capa-7-de-la-aplicación-web-qué-fuentes-de-registro-contienen-los-códigos-de-estado-elija-dos) |
| 100 | [Los equipos de desarrollo mantienen varias cargas de trabajo en AWS. La gerencia de la empresa está preocupada por el aumento de costos y quiere que el ingeniero de CloudOps configure alertas para que los equipos sean notificados cuando el gasto se acerque a límites preestablecidos. ¿Qué servicio de AWS satisfará estos requisitos?](#los-equipos-de-desarrollo-mantienen-varias-cargas-de-trabajo-en-aws-la-gerencia-de-la-empresa-está-preocupada-por-el-aumento-de-costos-y-quiere-que-el-ingeniero-de-cloudops-configure-alertas-para-que-los-equipos-sean-notificados-cuando-el-gasto-se-acerque-a-límites-preestablecidos-qué-servicio-de-aws-satisfará-estos-requisitos) |
| 101 | [Una empresa está intentando administrar sus costos en AWS Cloud. Un ingeniero de CloudOps necesita que etiquetas específicas definidas por la empresa y asignadas a recursos aparezcan en el informe de facturación. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-está-intentando-administrar-sus-costos-en-aws-cloud-un-ingeniero-de-cloudops-necesita-que-etiquetas-específicas-definidas-por-la-empresa-y-asignadas-a-recursos-aparezcan-en-el-informe-de-facturación-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 102 | [Una empresa tiene un departamento de Ventas y un departamento de Marketing. La empresa usa una cuenta de AWS. Existe la necesidad de determinar qué cargos se generan en la plataforma de AWS por cada departamento. También existe la necesidad de recibir notificaciones cuando se aproxime o se supere un nivel de costo especificado. ¿Qué dos acciones debe tomar un ingeniero de CloudOps para lograr ambos requisitos con el MENOR esfuerzo administrativo? (Elija dos.)](#una-empresa-tiene-un-departamento-de-ventas-y-un-departamento-de-marketing-la-empresa-usa-una-cuenta-de-aws-existe-la-necesidad-de-determinar-qué-cargos-se-generan-en-la-plataforma-de-aws-por-cada-departamento-también-existe-la-necesidad-de-recibir-notificaciones-cuando-se-aproxime-o-se-supere-un-nivel-de-costo-especificado-qué-dos-acciones-debe-tomar-un-ingeniero-de-cloudops-para-lograr-ambos-requisitos-con-el-menor-esfuerzo-administrativo-elija-dos) |
| 103 | [El director financiero (CFO) de una organización ha notado un aumento en los costos de almacenamiento de Amazon S3 durante los últimos meses. Un ingeniero de CloudOps sospecha que estos costos están relacionados con el almacenamiento de versiones antiguas de objetos de S3 de uno de sus buckets de S3. ¿Qué puede hacer el ingeniero para confirmar esta sospecha?](#el-director-financiero-cfo-de-una-organización-ha-notado-un-aumento-en-los-costos-de-almacenamiento-de-amazon-s3-durante-los-últimos-meses-un-ingeniero-de-cloudops-sospecha-que-estos-costos-están-relacionados-con-el-almacenamiento-de-versiones-antiguas-de-objetos-de-s3-de-uno-de-sus-buckets-de-s3-qué-puede-hacer-el-ingeniero-para-confirmar-esta-sospecha) |
| 104 | [Una empresa ejecuta una aplicación en instancias de Amazon EC2. Las instancias de EC2 están en un grupo de Auto Scaling y se ejecutan detrás de un Application Load Balancer (ALB). La aplicación experimenta errores cuando el total de solicitudes supera las 100 solicitudes por segundo. Un ingeniero de CloudOps debe recopilar información sobre el total de solicitudes durante un período de 2 semanas para determinar cuándo las solicitudes superaron este umbral. ¿Qué debe hacer el ingeniero de CloudOps para recopilar estos datos?](#una-empresa-ejecuta-una-aplicación-en-instancias-de-amazon-ec2-las-instancias-de-ec2-están-en-un-grupo-de-auto-scaling-y-se-ejecutan-detrás-de-un-application-load-balancer-alb-la-aplicación-experimenta-errores-cuando-el-total-de-solicitudes-supera-las-100-solicitudes-por-segundo-un-ingeniero-de-cloudops-debe-recopilar-información-sobre-el-total-de-solicitudes-durante-un-período-de-2-semanas-para-determinar-cuándo-las-solicitudes-superaron-este-umbral-qué-debe-hacer-el-ingeniero-de-cloudops-para-recopilar-estos-datos) |
| 105 | [Un ingeniero de CloudOps necesita crear un informe que muestre cuántos bytes se envían y reciben de cada miembro del grupo de destino para un Application Load Balancer (ALB). ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)](#un-ingeniero-de-cloudops-necesita-crear-un-informe-que-muestre-cuántos-bytes-se-envían-y-reciben-de-cada-miembro-del-grupo-de-destino-para-un-application-load-balancer-alb-qué-combinación-de-pasos-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-elija-dos) |
| 106 | [Una empresa tiene una política que establece que todos los registros de instancias de Amazon EC2 deben publicarse en Amazon CloudWatch Logs. Un ingeniero de CloudOps está solucionando problemas de una instancia de EC2 que ejecuta Amazon Linux 2. La instancia de EC2 no está publicando registros en CloudWatch Logs. El agente de Amazon CloudWatch se está ejecutando en la instancia de EC2, y el archivo de configuración del agente es correcto. ¿Qué debe hacer el ingeniero de CloudOps para resolver el problema?](#una-empresa-tiene-una-política-que-establece-que-todos-los-registros-de-instancias-de-amazon-ec2-deben-publicarse-en-amazon-cloudwatch-logs-un-ingeniero-de-cloudops-está-solucionando-problemas-de-una-instancia-de-ec2-que-ejecuta-amazon-linux-2-la-instancia-de-ec2-no-está-publicando-registros-en-cloudwatch-logs-el-agente-de-amazon-cloudwatch-se-está-ejecutando-en-la-instancia-de-ec2-y-el-archivo-de-configuración-del-agente-es-correcto-qué-debe-hacer-el-ingeniero-de-cloudops-para-resolver-el-problema) |

### Un ingeniero de CloudOps ha habilitado AWS CloudTrail en una cuenta de AWS. Si CloudTrail se deshabilita, debe volver a habilitarse de inmediato. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos SIN escribir código personalizado?

- [ ] Agregar la cuenta de AWS a AWS Organizations. Habilitar CloudTrail en la cuenta de administración (management account).
- [x] Crear una regla de AWS Config que se invoque cuando cambie la configuración de CloudTrail.
Aplicar la acción de remediación automática `AWS-ConfigureCloudTrailLogging`.
- [ ] Crear una regla de AWS Config que se invoque cuando cambie la configuración de CloudTrail.
Configurar la regla para que invoque una función de AWS Lambda que habilite CloudTrail.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) programada cada hora para ejecutar un documento de Automation de AWS Systems Manager que habilite CloudTrail.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa utiliza un sistema de archivos de Amazon Elastic File System (Amazon EFS) para compartir archivos entre muchas instancias de Amazon EC2 con Linux. Un ingeniero de CloudOps observa que la métrica `PercentIOLimit` del sistema de archivos se mantiene consistentemente en `100%` durante 15 minutos o más. El ingeniero de CloudOps también observa que la aplicación que lee y escribe en ese sistema de archivos tiene un rendimiento deficiente. La aplicación requiere alto throughput y muchas IOPS al acceder al sistema de archivos. ¿Qué debe hacer el ingeniero de CloudOps para remediar la métrica `PercentIOLimit` consistentemente alta?

- [ ] Crear un nuevo sistema de archivos EFS que use el modo de rendimiento Max I/O. Usar AWS DataSync para migrar los datos al nuevo sistema de archivos EFS.
- [ ] Crear una política de ciclo de vida en EFS para transicionar los archivos futuros a la clase de almacenamiento de Acceso Infrecuente (IA) y mejorar el rendimiento. Usar AWS DataSync para migrar los datos existentes al almacenamiento IA.
- [ ] Modificar el sistema de archivos EFS existente y activar el modo de rendimiento Max I/O.
- [x] Modificar el sistema de archivos EFS existente y activar el modo `Provisioned Throughput` (rendimiento aprovisionado).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa migró una aplicación intensiva en operaciones de E/S a una instancia de Amazon EC2 de propósito general. La instancia de EC2 tiene adjunto un único volumen de Amazon Elastic Block Store (Amazon EBS) de tipo General Purpose SSD. Los usuarios de la aplicación reportan que ciertas acciones que requieren lectura y escritura intensivas en disco tardan mucho más de lo normal o fallan por completo. Al revisar las métricas de rendimiento del volumen de EBS, un ingeniero de CloudOps observa que la métrica `VolumeQueueLength` se mantiene consistentemente alta durante los mismos períodos en los que los usuarios reportan problemas. El ingeniero de CloudOps necesita resolver este problema para restaurar el rendimiento completo de la aplicación. ¿Qué acción cumple con estos requisitos?

- [ ] Modificar el tipo de instancia a uno optimizado para almacenamiento.
- [ ] Modificar las propiedades del volumen desmarcando la opción Auto-Enable Volume I/O.
- [x] Modificar las propiedades del volumen para aumentar las IOPS.
- [ ] Modificar la instancia para habilitar redes mejoradas (enhanced networking).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una política que exige que todas las instancias de Amazon EC2 tengan un conjunto específico de etiquetas (tags). Si una instancia de EC2 no tiene las etiquetas requeridas, la instancia no conforme debe terminarse. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que envíe todos los cambios de estado de las instancias de EC2 a una función de AWS Lambda para determinar si cada instancia es conforme. Terminar cualquier instancia no conforme.
- [ ] Crear una política de IAM que haga cumplir todos los requisitos de etiquetado de instancias de EC2. Si una instancia no tiene las etiquetas requeridas, la política terminará la instancia no conforme.
- [ ] Crear una función de AWS Lambda para determinar si cada instancia de EC2 es conforme y terminar una instancia si no lo es. Programar la función Lambda para que se invoque cada 5 minutos.
- [x] Crear una regla de AWS Config para verificar si están presentes las etiquetas requeridas. Si una instancia de EC2 no es conforme, invocar un documento de Automation de AWS Systems Manager para terminar la instancia.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene múltiples instancias de Amazon EC2 que ejecutan una aplicación intensiva en recursos en un entorno de desarrollo. Un ingeniero de CloudOps está implementando una solución para detener estas instancias de EC2 cuando no están en uso. ¿Qué solución cumple con este requisito?

- [ ] Evaluar los registros de AWS CloudTrail para verificar que no haya actividad de la API de EC2. Invocar una función de AWS Lambda para detener las instancias de EC2.
- [x] Crear una alarma de Amazon CloudWatch para detener las instancias de EC2 cuando el uso promedio de CPU sea inferior al `5%` durante un período de 30 minutos.
- [ ] Crear una métrica de Amazon CloudWatch para detener las instancias de EC2 cuando la métrica `VolumeReadBytes` sea inferior a `500` durante un período de 30 minutos.
- [ ] Usar AWS Config para invocar una función de AWS Lambda que detenga las instancias de EC2 según los cambios de configuración de recursos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps es responsable de una aplicación heredada (legacy) intensiva en CPU. La aplicación solo puede escalarse verticalmente. Actualmente, la aplicación está desplegada en una única instancia de Amazon EC2 `t2.large`. El sistema muestra un uso de CPU del `90%` y una latencia de rendimiento significativa después de unos minutos. ¿Qué cambio se debe hacer para aliviar el problema de rendimiento?

- [ ] Cambiar el volumen de Amazon EBS a Provisioned IOPS.
- [x] Actualizar a una instancia optimizada para cómputo (compute-optimized).
- [ ] Agregar instancias `t2.large` adicionales a la aplicación.
- [ ] Comprar Instancias Reservadas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación crítica sin servidor (serverless) que utiliza múltiples funciones de AWS Lambda. Cada función Lambda genera `1 GB` de datos de registro diariamente en su propio grupo de registros (log group) de Amazon CloudWatch Logs. El equipo de seguridad de la empresa solicita un conteo de errores de la aplicación, agrupados por tipo, en todos los grupos de registros. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [x] Realizar una consulta de CloudWatch Logs Insights que use el comando `stats` y la función `count`.
- [ ] Realizar una búsqueda en CloudWatch Logs que use la palabra clave `groupby` y la función `count`.
- [ ] Realizar una consulta de Amazon Athena que use las palabras clave `SELECT` y `GROUP BY`.
- [ ] Realizar una consulta de Amazon RDS que use las palabras clave `SELECT` y `GROUP BY`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps ha lanzado una instancia de Amazon EC2 de propósito general de tamaño grande para procesar regularmente archivos de datos de gran tamaño. La instancia tiene adjunto un volumen de Amazon Elastic Block Store (Amazon EBS) de 1 TB de tipo `General Purpose SSD (gp2)`. La instancia también está optimizada para EBS. Para ahorrar costos, el ingeniero de CloudOps detiene la instancia cada noche y la reinicia cada mañana. Cuando el procesamiento de datos está activo, las métricas de Amazon CloudWatch de la instancia muestran consistentemente 3.000 `VolumeReadOps`. El ingeniero de CloudOps debe mejorar el rendimiento de E/S garantizando la integridad de los datos. ¿Qué acción cumple con estos requisitos?

- [ ] Cambiar el tipo de instancia a una de propósito general grande y con ráfagas (burstable).
- [ ] Cambiar el tipo de instancia a una de propósito general extra grande.
- [ ] Aumentar el volumen de EBS a un volumen `General Purpose SSD (gp2)` de 2 TB.
- [x] Mover los datos que residen en el volumen de EBS al almacenamiento de instancia (instance store).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta cargas de trabajo en 90 instancias de Amazon EC2 en la región `eu-west-1` dentro de una cuenta de AWS. En 2 meses, la empresa migrará las cargas de trabajo de `eu-west-1` a la región `eu-west-3`. La empresa necesita reducir el costo de las instancias de EC2. La empresa está dispuesta a asumir un compromiso de 1 año que comenzará la próxima semana. La empresa debe elegir una opción de compra de instancias de EC2 que proporcione descuentos para las 90 instancias de EC2 sin importar la región durante el período de 1 año. ¿Qué solución cumple con estos requisitos?

- [ ] Comprar Instancias Reservadas Estándar de EC2.
- [ ] Comprar un Savings Plan de instancias de EC2.
- [ ] Comprar Instancias Reservadas Convertibles de EC2.
- [x] Comprar un Compute Savings Plan.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita crear alertas basadas en las métricas de lectura y escritura de volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos a una instancia de Amazon EC2. El ingeniero de CloudOps crea y habilita alarmas de Amazon CloudWatch para la métrica `DiskReadBytes` y la métrica `DiskWriteBytes`. Una herramienta de monitoreo personalizada instalada en la instancia de EC2, con la misma configuración de alarma, indica que las métricas del volumen han superado el umbral. Sin embargo, las alarmas de CloudWatch no entraron en estado `ALARM`. ¿Qué acción garantizará que las alarmas de CloudWatch funcionen correctamente?

- [ ] Instalar y configurar el agente de CloudWatch en la instancia de EC2 para capturar las métricas deseadas.
- [ ] Instalar y configurar el AWS Systems Manager Agent en la instancia de EC2 para capturar las métricas deseadas.
- [x] Reconfigurar las alarmas de CloudWatch para usar la métrica `VolumeReadBytes` y la métrica `VolumeWriteBytes` de los volúmenes de EBS.
- [ ] Reconfigurar las alarmas de CloudWatch para usar la métrica `VolumeReadBytes` y la métrica `VolumeWriteBytes` de la instancia de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa necesita ver una lista de grupos de seguridad que están abiertos a internet en el puerto `3389`. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Configurar Amazon GuardDuty para escanear los grupos de seguridad y reportar acceso sin restricciones en el puerto `3389`.
- [ ] Configurar una Política de Control de Servicio (SCP) para identificar los grupos de seguridad que permiten acceso sin restricciones en el puerto `3389`.
- [ ] Usar AWS Identity and Access Management Access Analyzer para encontrar instancias que tengan acceso sin restricciones en el puerto `3389`.
- [x] Usar AWS Trusted Advisor para encontrar grupos de seguridad que permitan acceso sin restricciones en el puerto `3389`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una aplicación se ejecuta en múltiples instancias de Amazon EC2 dentro de un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para usar la versión más reciente de una plantilla de lanzamiento (launch template). Un ingeniero de CloudOps debe diseñar una solución que administre de forma centralizada los registros de la aplicación y los conserve durante no más de 90 días. ¿Qué solución cumple con estos requisitos?

- [ ] Lanzar una Amazon Machine Image (AMI) preconfigurada con el agente de Amazon CloudWatch Logs para enviar registros a un bucket de Amazon S3. Aplicar una política de ciclo de vida de S3 de 90 días en el bucket de S3 para que los registros de la aplicación expiren.
- [ ] Lanzar una Amazon Machine Image (AMI) preconfigurada con el agente de Amazon CloudWatch Logs para enviar registros a un grupo de registros (log group). Crear una regla programada de Amazon EventBridge (Amazon CloudWatch Events) para realizar una actualización de instancias (instance refresh) cada 90 días.
- [x] Actualizar los datos de usuario (user data) de la plantilla de lanzamiento para instalar y configurar el agente de Amazon CloudWatch Logs, de modo que envíe los registros a un grupo de registros. Configurar el período de retención del grupo de registros en 90 días.
- [ ] Actualizar los datos de usuario de la plantilla de lanzamiento para instalar y configurar el agente de Amazon CloudWatch Logs, de modo que envíe los registros a un grupo de registros. Establecer la configuración de rotación de registros de las instancias de EC2 en 90 días.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está realizando una venta relámpago (flash sale) en su sitio web. El sitio web está alojado en instancias de Amazon EC2 de rendimiento con ráfagas (burstable) dentro de un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para lanzar instancias cuando el uso de CPU supera el `70%`. Un par de horas después de iniciada la venta, los usuarios reportan tiempos de carga lentos y mensajes de error por conexiones rechazadas. Un ingeniero de CloudOps revisa las métricas de Amazon CloudWatch y observa que el uso de CPU está en `20%` en toda la flota de instancias. El ingeniero de CloudOps debe restaurar la funcionalidad del sitio web sin hacer cambios en la infraestructura de red. ¿Qué solución cumple con estos requisitos?

- [x] Activar el modo ilimitado (unlimited mode) para las instancias del grupo de Auto Scaling.
- [ ] Implementar una distribución de Amazon CloudFront para descargar el tráfico del grupo de Auto Scaling.
- [ ] Mover el sitio web a otra región de AWS que esté más cerca de los usuarios.
- [ ] Reducir el tamaño deseado del grupo de Auto Scaling para aumentar artificialmente el promedio de uso de CPU.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha lanzado un sitio web de redes sociales que permite a los usuarios subir imágenes directamente a un bucket centralizado de Amazon S3. El sitio web es popular en zonas geográficamente distantes de la región de AWS donde se encuentra el bucket de S3. Los usuarios reportan que las cargas son lentas. Un ingeniero de CloudOps debe mejorar la velocidad de carga. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] Crear puntos de acceso de S3 en regiones más cercanas a los usuarios.
- [ ] Crear un acelerador en AWS Global Accelerator para el bucket de S3.
- [x] Habilitar S3 Transfer Acceleration en el bucket de S3.
- [ ] Habilitar el intercambio de recursos de origen cruzado (CORS) en el bucket de S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación móvil que usa Amazon S3 para almacenar imágenes. Las imágenes son populares durante una semana, y luego el número de solicitudes de acceso disminuye con el tiempo. Las imágenes deben tener alta disponibilidad y ser accesibles de inmediato cuando se soliciten. Un ingeniero de CloudOps debe reducir los costos de almacenamiento en S3 para la empresa. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?

- [ ] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 Glacier después de 7 días.
- [ ] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 One Zone-Infrequent Access (S3 One Zone-IA) después de 7 días.
- [ ] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 Standard después de 7 días.
- [x] Crear una política de ciclo de vida de S3 para transicionar las imágenes a S3 Standard-Infrequent Access (S3 Standard-IA) después de 7 días.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa AWS Organizations para administrar múltiples cuentas de AWS con facturación consolidada habilitada. Los propietarios de las cuentas miembro de la organización quieren los beneficios de las Instancias Reservadas (RI) pero no quieren compartir las RI con otras cuentas. ¿Qué solución cumple con estos requisitos?

- [x] Comprar RI en cuentas miembro individuales. Deshabilitar el uso compartido del descuento de RI en la cuenta de administración.
- [ ] Comprar RI en cuentas miembro individuales. Deshabilitar el uso compartido del descuento de RI en las cuentas miembro.
- [ ] Comprar RI en la cuenta de administración. Deshabilitar el uso compartido del descuento de RI en la cuenta de administración.
- [ ] Comprar RI en la cuenta de administración. Deshabilitar el uso compartido del descuento de RI en las cuentas miembro.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una aplicación de videojuegos está desplegada en cuatro instancias de Amazon EC2 dentro de una `VPC` predeterminada. El ingeniero de CloudOps ha notado latencia consistentemente alta en las respuestas mientras se transfieren datos entre las cuatro instancias. El ingeniero no tiene manera de modificar el código de la aplicación. La forma MÁS efectiva de reducir la latencia es volver a lanzar las instancias de EC2 en:

- [ ] Una `VPC` dedicada.
- [ ] Una sola subred dentro de la `VPC`.
- [x] Un grupo de ubicación (placement group).
- [ ] Una sola Zona de disponibilidad.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El departamento financiero de una empresa necesita ver los detalles de costos de cada proyecto en una cuenta de AWS. Un ingeniero de CloudOps debe realizar la configuración inicial requerida para ver el costo de cada proyecto en Cost Explorer. ¿Qué solución cumple con este requisito?

- [x] Activar las etiquetas de asignación de costos (cost allocation tags). Agregar una etiqueta de proyecto a los recursos correspondientes.
- [ ] Configurar la facturación consolidada. Crear Informes de Costos y Uso de AWS (AWS Cost and Usage Reports).
- [ ] Usar AWS Budgets. Crear informes de AWS Budgets.
- [ ] Usar categorías de costos para definir grupos personalizados basados en dimensiones de costo y uso de AWS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe configurar una capa resiliente de instancias de Amazon EC2 para una aplicación de computación de alto rendimiento (HPC). La aplicación HPC requiere latencia mínima entre nodos. ¿Qué acciones debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Crear un sistema de archivos de Amazon Elastic File System (Amazon EFS). Montar el sistema de archivos en las instancias de EC2 usando datos de usuario (user data).
- [ ] Crear un Network Load Balancer Multi-AZ frente a las instancias de EC2.
- [x] Colocar las instancias de EC2 en un grupo de Auto Scaling dentro de una única subred.
- [x] Lanzar las instancias de EC2 en un grupo de ubicación (placement group) de tipo clúster.
- [ ] Lanzar las instancias de EC2 en un grupo de ubicación de tipo partición.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps administra los buckets de Amazon S3 de una empresa. El ingeniero de CloudOps ha identificado `5 GB` de cargas multiparte incompletas en un bucket de S3 de la cuenta de AWS de la empresa. El ingeniero de CloudOps necesita reducir la cantidad de objetos de cargas multiparte incompletas en el bucket de S3. ¿Qué solución cumple con este requisito?

- [x] Crear una regla de ciclo de vida de S3 en el bucket de S3 para eliminar marcadores expirados o cargas multiparte incompletas.
- [ ] Exigir a los usuarios que realizan cargas de archivos a Amazon S3 que usen el S3 TransferUtility.
- [ ] Habilitar el versionado de S3 en el bucket de S3 que contiene las cargas multiparte incompletas.
- [ ] Crear un S3 Object Lambda Access Point para eliminar las cargas multiparte incompletas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa Amazon Elastic File System (Amazon EFS) para compartir un sistema de archivos entre varias instancias de Amazon EC2. A medida que aumenta el uso, los usuarios reportan que la recuperación de archivos desde el sistema de archivos EFS es más lenta de lo normal. ¿Qué acción debe tomar un ingeniero de CloudOps para mejorar el rendimiento del sistema de archivos?

- [x] Configurar el sistema de archivos para usar `Provisioned Throughput` (rendimiento aprovisionado).
- [ ] Habilitar el cifrado en tránsito en el sistema de archivos.
- [ ] Identificar archivos no utilizados en el sistema de archivos y eliminarlos.
- [ ] Redimensionar el volumen de Amazon Elastic Block Store (Amazon EBS) de cada una de las instancias de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación que los clientes usan para buscar registros en un sitio web. Los datos de la aplicación se almacenan en un clúster de Amazon Aurora DB. El uso de la aplicación varía según la temporada y el día de la semana. La popularidad del sitio web está aumentando, y el sitio web experimenta un rendimiento más lento debido al aumento de carga en el clúster de base de datos durante los períodos de actividad pico. Los registros de la aplicación muestran que los problemas de rendimiento ocurren cuando los usuarios buscan información. Rara vez se realiza la misma búsqueda varias veces. Un ingeniero de CloudOps debe mejorar el rendimiento de la plataforma usando una solución que maximice la eficiencia de los recursos. ¿Qué solución cumple con estos requisitos?

- [ ] Desplegar un clúster de Amazon ElastiCache for Redis frente al clúster de base de datos. Modificar la aplicación para que verifique la caché antes de emitir nuevas consultas a la base de datos. Agregar los resultados de cualquier consulta a la caché.
- [x] Desplegar una réplica de Aurora para el clúster de base de datos. Modificar la aplicación para que use el endpoint de lector (reader endpoint) para las operaciones de búsqueda. Usar Aurora Auto Scaling para escalar el número de réplicas según la carga.
- [ ] Usar Provisioned IOPS en los volúmenes de almacenamiento que respaldan el clúster de base de datos para mejorar el rendimiento lo suficiente como para soportar la carga pico de la aplicación.
- [ ] Aumentar el tamaño de la instancia del clúster de base de datos a un tamaño suficiente para soportar la carga pico de la aplicación. Usar Aurora Auto Scaling para escalar el tamaño de la instancia según la carga.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El equipo de seguridad está preocupado porque el número de políticas de AWS Identity and Access Management (IAM) que se usan en el entorno está aumentando. El equipo le encargó a un ingeniero de CloudOps que reportara el número actual de políticas de IAM en uso y el total de políticas de IAM disponibles. ¿Qué servicio de AWS debe usar el ingeniero para verificar cómo se compara el uso actual de políticas de IAM con los límites de servicio actuales?

- [x] AWS Trusted Advisor.
- [ ] Amazon Inspector.
- [ ] AWS Config.
- [ ] AWS Organizations.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps notó que se está creando una gran cantidad de direcciones IP elásticas en la cuenta de AWS de la empresa, pero no se están asociando con instancias de Amazon EC2, y están generando cargos por direcciones IP elásticas en la factura mensual. ¿Cómo puede el ingeniero identificar quién está creando las direcciones IP elásticas?

- [ ] Adjuntar una etiqueta de asignación de costos (`cost-allocation`) a cada dirección IP elástica solicitada, con el nombre de usuario de IAM del desarrollador que la crea.
- [x] Consultar los registros de AWS CloudTrail usando Amazon Athena para buscar eventos de direcciones IP elásticas.
- [ ] Crear una alarma de CloudWatch sobre la métrica `EIPCreated` y enviar una notificación de Amazon SNS cuando se active la alarma.
- [ ] Usar Amazon Inspector para obtener un informe de todas las direcciones IP elásticas creadas en los últimos 30 días.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El departamento de TI de una empresa notó un aumento en el gasto de su cuenta de AWS para desarrolladores. Hay más de 50 desarrolladores usando la cuenta, y el equipo de finanzas quiere determinar los costos de servicio incurridos por cada desarrollador. ¿Qué debe hacer un ingeniero de CloudOps para recopilar esta información? (Seleccione DOS.)

- [x] Activar la etiqueta `createdBy` en la cuenta.
- [ ] Analizar el uso con dashboards de Amazon CloudWatch.
- [x] Analizar el uso con Cost Explorer.
- [ ] Configurar AWS Trusted Advisor para rastrear el uso de recursos.
- [ ] Crear una alarma de facturación en AWS Budgets.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación en una flota de instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Las instancias de EC2 son lanzadas por un grupo de Auto Scaling y se registran automáticamente en un grupo de destino. Un ingeniero de CloudOps debe configurar una notificación para alertar a los propietarios de la aplicación cuando los destinos fallen las verificaciones de estado. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Crear una alarma de Amazon CloudWatch sobre la métrica `UnHealthyHostCount`. Configurar una acción para enviar una notificación de Amazon Simple Notification Service (Amazon SNS) cuando la métrica sea mayor que 0.
- [ ] Configurar una acción de ciclo de vida personalizada (lifecycle hook) de Amazon EC2 Auto Scaling para enviar una notificación de Amazon SNS cuando una instancia esté en estado Pending:Wait.
- [ ] Actualizar el grupo de Auto Scaling. Configurar una notificación de actividad para enviar una notificación de Amazon SNS para el tipo de evento Unhealthy.
- [ ] Actualizar la verificación de estado del `ALB` para enviar una notificación de Amazon SNS cuando una instancia esté no saludable.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta su infraestructura en instancias de Amazon EC2 que corren en un grupo de Auto Scaling. Recientemente, la empresa promovió código defectuoso a toda la flota de EC2. Este código defectuoso hizo que el grupo de Auto Scaling escalara las instancias antes de que se pudieran recuperar los registros de la aplicación. ¿Qué debe hacer un ingeniero de CloudOps para conservar los registros de la aplicación después de que las instancias sean terminadas?

- [ ] Configurar un lifecycle hook de Auto Scaling para crear una instantánea del almacenamiento efímero al terminar las instancias.
- [x] Crear una nueva Amazon Machine Image (AMI) que tenga instalado y configurado el agente de Amazon CloudWatch para enviar registros a Amazon CloudWatch Logs. Actualizar la plantilla de lanzamiento para usar la nueva AMI.
- [ ] Crear una nueva Amazon Machine Image (AMI) que tenga un script personalizado configurado para enviar registros a AWS CloudTrail. Actualizar la plantilla de lanzamiento para usar la nueva AMI.
- [ ] Instalar el agente de Amazon CloudWatch en la Amazon Machine Image (AMI) definida en la plantilla de lanzamiento. Configurar el agente de CloudWatch para respaldar los registros en almacenamiento efímero.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe crear una solución que notifique inmediatamente a los desarrolladores de software si una función de AWS Lambda presenta un error. ¿Qué solución cumple con este requisito?

- [x] Crear un tema (topic) de Amazon Simple Notification Service (Amazon SNS) con una suscripción de correo electrónico para cada desarrollador. Crear una alarma de Amazon CloudWatch usando la métrica `Errors` y el nombre de la función Lambda como dimensión. Configurar la alarma para enviar una notificación al tema de SNS cuando el estado de la alarma llegue a `ALARM`.
- [ ] Crear un tema de Amazon SNS con una suscripción móvil para cada desarrollador. Crear una alarma de Amazon EventBridge (Amazon CloudWatch Events) usando `LambdaError` como patrón de evento y el nombre del tema de SNS como recurso. Configurar la alarma para enviar una notificación al tema de SNS cuando el estado de la alarma llegue a `ALARM`.
- [ ] Verificar la dirección de correo electrónico de cada desarrollador en Amazon Simple Email Service (Amazon SES). Crear una regla de Amazon CloudWatch usando la métrica `LambdaError` y las direcciones de correo electrónico de los desarrolladores como dimensiones. Configurar la regla para enviar un correo electrónico a través de Amazon SES cuando el estado de la regla llegue a `ALARM`.
- [ ] Verificar el teléfono móvil de cada desarrollador en Amazon Simple Email Service (Amazon SES). Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) usando `Errors` como patrón de evento y el nombre de la función Lambda como recurso. Configurar la regla para enviar una notificación push a través de Amazon SES cuando el estado de la regla llegue a `ALARM`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe crear una solución que apague automáticamente cualquier instancia de Amazon EC2 que tenga menos del `10%` de uso promedio de CPU durante 60 minutos o más. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?

- [ ] Implementar un cron job en cada instancia de EC2 que se ejecute cada 60 minutos y calcule el uso actual de CPU. Iniciar el apagado de la instancia si el uso de CPU es menor al `10%`.
- [x] Implementar una alarma de Amazon CloudWatch para cada instancia de EC2 que monitoree el uso promedio de CPU. Establecer el período en 1 hora y el umbral en `10%`. Configurar una acción de EC2 en la alarma para detener la instancia.
- [ ] Instalar el agente unificado de Amazon CloudWatch en cada instancia de EC2 y habilitar el conjunto de métricas predefinidas de nivel Básico. Registrar el uso de CPU cada 60 minutos e iniciar el apagado de la instancia si el uso de CPU es menor al `10%`.
- [ ] Usar AWS Systems Manager Run Command para obtener el uso de CPU de cada instancia de EC2 cada 60 minutos. Iniciar el apagado de la instancia si el uso de CPU es menor al `10%`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Se notifica a un ingeniero de CloudOps que una instancia de Amazon EC2 dejó de responder. La consola de administración de AWS indica que las verificaciones de sistema están fallando. ¿Qué debe hacer primero el ingeniero para resolver este problema?

- [ ] Reiniciar (reboot) la instancia de EC2 para que se pueda lanzar en un nuevo host.
- [x] Detener e iniciar (stop/start) la instancia de EC2 para que se pueda lanzar en un nuevo host.
- [ ] Terminar la instancia de EC2 y volver a lanzarla.
- [ ] Ver el registro de AWS CloudTrail para investigar qué cambió en la instancia de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación web existente que se ejecuta en dos instancias de Amazon EC2 detrás de un Application Load Balancer (ALB) a través de dos Zonas de disponibilidad. La aplicación usa una instancia de Amazon RDS Multi-AZ. Los conjuntos de registros de Amazon Route 53 enrutan las solicitudes de contenido dinámico al balanceador de carga y las solicitudes de contenido estático a un bucket de Amazon S3. Los visitantes del sitio reportan tiempos de carga extremadamente largos. ¿Qué acciones se deben tomar para mejorar el rendimiento del sitio web? (Seleccione DOS)

- [x] Agregar caché de Amazon CloudFront para el contenido estático.
- [ ] Cambiar el listener del balanceador de carga de `HTTPS` a `TCP`.
- [ ] Habilitar el enrutamiento basado en latencia de Amazon Route 53.
- [x] Implementar Amazon EC2 Auto Scaling para los servidores web.
- [ ] Mover el contenido estático de Amazon S3 a los servidores web.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Se sabe que un proceso errático usa todo un procesador y se ejecuta al `100%`. Un ingeniero de CloudOps quiere automatizar el reinicio de la instancia una vez que el problema ocurra durante más de 2 minutos. ¿Cómo se puede lograr esto?

- [ ] Crear una alarma de Amazon CloudWatch para la instancia de Amazon EC2 con monitoreo básico. Habilitar una acción para reiniciar la instancia.
- [x] Crear una alarma de CloudWatch para la instancia de EC2 con monitoreo detallado. Habilitar una acción para reiniciar la instancia.
- [ ] Crear una función de AWS Lambda para reiniciar la instancia de EC2, activada de forma programada cada 2 minutos.
- [ ] Crear una función Lambda para reiniciar la instancia de EC2, activada por verificaciones de estado de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps observa un evento de escalado (scale-up) para un grupo de Amazon EC2 Auto Scaling. Amazon CloudWatch muestra un pico en la métrica `RequestCount` del Application Load Balancer asociado. Al ingeniero le gustaría conocer las direcciones IP de origen de las solicitudes. ¿Dónde puede el ingeniero encontrar esta información?

- [ ] Registros de Auto Scaling.
- [ ] Registros de AWS CloudTrail.
- [ ] Registros de la instancia de EC2.
- [x] Registros de acceso del Elastic Load Balancer.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está ejecutando una aplicación sin servidor (serverless) en AWS Lambda. La aplicación almacena datos en una instancia de base de datos de Amazon RDS for MySQL. El uso ha aumentado constantemente, y recientemente han ocurrido numerosos errores de `too many connections` cuando la función Lambda intenta conectarse a la base de datos. La empresa ya ha configurado la base de datos para usar el valor máximo posible de `max_connections`. ¿Qué debe hacer un ingeniero de CloudOps para resolver estos errores?

- [ ] Crear una réplica de lectura de la base de datos. Usar Amazon Route 53 para crear un registro `DNS` ponderado que contenga ambas bases de datos.
- [x] Usar Amazon RDS Proxy para crear un proxy. Actualizar la cadena de conexión en la función Lambda.
- [ ] Aumentar el valor del parámetro `max_connect_errors` en el grupo de parámetros que usa la base de datos.
- [ ] Actualizar la concurrencia reservada (reserved concurrency) de la función Lambda a un valor más alto.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps recibe una notificación de que una aplicación que se ejecuta en instancias de Amazon EC2 no ha podido autenticarse en una base de datos de Amazon RDS. Para solucionar el problema, el ingeniero de CloudOps necesita investigar la rotación de contraseñas de AWS Secrets Manager. ¿Qué registro de Amazon CloudWatch proporcionará información sobre la rotación de contraseñas?

- [ ] Registros de AWS CloudTrail.
- [ ] Registros de la aplicación de la instancia de EC2.
- [x] Registros de la función de AWS Lambda.
- [ ] Registros de la base de datos RDS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una función de AWS Lambda falla intermitentemente varias veces al día. Un ingeniero de CloudOps debe averiguar con qué frecuencia ha ocurrido este error en los últimos 7 días. ¿Qué acción cumple con este requisito de la manera MÁS eficiente operativamente?

- [ ] Usar Amazon Athena para consultar los registros de Amazon CloudWatch asociados con la función Lambda.
- [ ] Usar Amazon Athena para consultar los registros de AWS CloudTrail asociados con la función Lambda.
- [x] Usar Amazon CloudWatch Logs Insights para consultar los registros asociados de la función Lambda.
- [ ] Usar Amazon Elasticsearch Service (Amazon ES) para transmitir los registros de Amazon CloudWatch de la función Lambda.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe configurar notificaciones para cuando la facturación combinada supere un cierto umbral para todas las cuentas de AWS dentro de una empresa. El ingeniero ha configurado AWS Organizations y habilitado la facturación consolidada. ¿Qué pasos adicionales debe realizar el ingeniero para configurar las alertas de facturación?

- [ ] En la cuenta de pagador: habilitar las alertas de facturación en la consola de Billing and Cost Management; publicar un mensaje de Amazon SNS cuando se active la alerta de facturación.
- [ ] En cada cuenta: habilitar las alertas de facturación en la consola de Billing and Cost Management; configurar una alarma de facturación en Amazon CloudWatch; publicar un mensaje de SNS cuando se active la alarma.
- [ ] En la cuenta de pagador: habilitar las alertas de facturación en la consola de Billing and Cost Management; configurar una alarma de facturación en la consola de Billing and Cost Management para publicar un mensaje de SNS cuando se active la alarma.
- [x] En la cuenta de pagador: habilitar las alertas de facturación en la consola de Billing and Cost Management; configurar una alarma de facturación en Amazon CloudWatch; publicar un mensaje de SNS cuando se active la alarma.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una carga de trabajo Windows de alto rendimiento. La carga de trabajo requiere un volumen de almacenamiento que proporcione un rendimiento constante de 10,000 IOPS. La empresa no quiere pagar por capacidad adicional innecesaria para lograr este rendimiento. ¿Qué solución cumple con estos requisitos con el MENOR costo?

- [ ] Usar un volumen de Amazon Elastic Block Store (Amazon EBS) `Provisioned IOPS SSD (io1)` configurado con 10,000 IOPS aprovisionadas.
- [x] Usar un volumen de Amazon Elastic Block Store (Amazon EBS) `General Purpose SSD (gp3)` configurado con 10,000 IOPS aprovisionadas.
- [ ] Usar un sistema de archivos de Amazon Elastic File System (Amazon EFS) en modo Max I/O.
- [ ] Usar un sistema de archivos de Amazon FSx for Windows File Server configurado con 10,000 IOPS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene científicos que cargan objetos de datos grandes a un bucket de Amazon S3. Los científicos cargan los objetos como cargas multiparte. Las cargas multiparte a menudo fallan debido a una mala conectividad del cliente final. La empresa quiere optimizar los costos de almacenamiento asociados con los datos. Un ingeniero de CloudOps debe implementar una solución que presente métricas para cargas incompletas. La solución también debe eliminar automáticamente cualquier carga incompleta después de 7 días. ¿Qué solución cumple con estos requisitos?

- [x] Revisar la métrica Incomplete Multipart Upload Bytes en el dashboard de S3 Storage Lens. Crear una política de ciclo de vida de S3 para eliminar automáticamente cualquier carga multiparte incompleta después de 7 días.
- [ ] Implementar S3 Intelligent-Tiering para mover los datos a clases de almacenamiento de menor costo después de 7 días. Crear una política de S3 Storage Lens para eliminar automáticamente cualquier carga multiparte incompleta después de 7 días.
- [ ] Acceder a la consola de S3. Revisar la pestaña de Métricas para verificar el almacenamiento que consumen las cargas multiparte incompletas. Crear una función de AWS Lambda para eliminar cualquier carga multiparte incompleta después de 7 días.
- [ ] Usar la herramienta de análisis de clase de almacenamiento de S3 analytics para identificar y medir las cargas multiparte incompletas. Configurar una política de bucket de S3 para hacer cumplir restricciones sobre las cargas multiparte y eliminar las incompletas después de 7 días.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está ejecutando un software de computación distribuida para administrar una flota de 20 instancias de Amazon EC2 para cálculos. La flota incluye 2 nodos de control y 18 nodos de tareas para ejecutar los cálculos. Los nodos de control pueden iniciar automáticamente los nodos de tareas. Actualmente, todos los nodos se ejecutan bajo demanda (on-demand). Los nodos de control deben estar disponibles las 24 horas del día, los 7 días de la semana. Los nodos de tareas se ejecutan durante 4 horas cada día. Un ingeniero de CloudOps necesita optimizar el costo de esta solución. ¿Qué combinación de acciones cumple con estos requisitos? (Elija dos.)

- [x] Comprar Savings Plans de instancias de EC2 para los nodos de control.
- [ ] Usar Hosts Dedicados para los nodos de control.
- [ ] Usar Instancias Reservadas para los nodos de tareas.
- [ ] Usar instancias Spot para los nodos de control. Usar instancias On-Demand si no hay disponibilidad Spot.
- [x] Usar instancias Spot para los nodos de tareas. Usar instancias On-Demand si no hay disponibilidad Spot.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Se supone que una empresa recibe un archivo de datos cada hora en un bucket de Amazon S3. Una notificación de evento de S3 invoca una función de AWS Lambda cada vez que llega un archivo. La función procesa los datos para que los use una aplicación. El equipo de la aplicación nota que, a veces, el archivo no llega. El equipo de la aplicación quiere recibir una notificación siempre que el archivo no llegue. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Agregar una regla de ciclo de vida de S3 en el bucket de S3 con un alcance limitado a objetos creados en la última hora. Configurar otra notificación de evento de S3 para que se invoque mediante la transición de ciclo de vida cuando el número de objetos transicionados sea cero. Publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) para notificar al equipo de la aplicación.
- [ ] Configurar otra notificación de evento de S3 para invocar una función Lambda que publique un mensaje en una cola de Amazon Simple Queue Service (Amazon SQS). Crear una alarma de Amazon CloudWatch para publicar un mensaje en un tema de Amazon SNS y notificar al equipo de la aplicación cuando la métrica ApproximateAgeOfOldestMessage de la cola sea mayor a 1 hora.
- [x] Crear una alarma de Amazon CloudWatch para publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) que alerte al equipo de la aplicación cuando la métrica Invocations de la función Lambda sea cero durante una hora. Configurar la alarma para tratar los datos faltantes como incumplimiento (breaching).
- [ ] Crear una nueva función Lambda para obtener la marca de tiempo del archivo más reciente en el bucket de S3. Si la marca de tiempo tiene más de 1 hora de antigüedad, publicar un mensaje en un tema de Amazon SNS para notificar al equipo de la aplicación. Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para invocar la nueva función cada hora.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación web que experimenta problemas de rendimiento varias veces cada noche. Un análisis de causa raíz revela aumentos repentinos en el uso de CPU que duran 5 minutos en una instancia de Amazon EC2 Linux. Un ingeniero de CloudOps debe encontrar el ID de proceso (PID) del servicio o proceso que está consumiendo más CPU. ¿Qué debe hacer el ingeniero de CloudOps para recopilar la información de uso del proceso con el MENOR esfuerzo posible?

- [x] Configurar el plugin `procstat` del agente de Amazon CloudWatch para capturar métricas de procesos de CPU.
- [ ] Configurar una función de AWS Lambda que se ejecute cada minuto para capturar el PID y enviar una notificación.
- [ ] Iniciar sesión en la instancia de EC2 usando una clave `.pem` cada noche. Luego ejecutar el comando top.
- [ ] Usar la métrica predeterminada de uso de CPU de Amazon CloudWatch para capturar el PID en CloudWatch.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un equipo administra una cuenta de AWS que es miembro de una organización en AWS Organizations. La organización tiene habilitadas las funciones de facturación consolidada. La cuenta aloja varias aplicaciones. Un ingeniero de CloudOps ha aplicado etiquetas (tags) a los recursos dentro de la cuenta para reflejar el entorno. El equipo necesita un informe del desglose de cargos por entorno. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Filtrar, mapear y categorizar grupos de recursos en Tag Editor.
- [ ] Asegurarse de que las Políticas de Control de Servicio (SCP) de la organización permitan el acceso a las etiquetas de asignación de costos.
- [ ] Asegurarse de que las credenciales de IAM utilizadas para acceder a Cost Explorer tengan permisos para agrupar costos por etiquetas.
- [x] Activar las claves de etiquetas para la asignación de costos en la cuenta de administración de la organización.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Se sabe que un proceso errático usa un procesador completo y se ejecuta al `100%`. Un ingeniero de CloudOps quiere automatizar el reinicio de una instancia de Amazon EC2 cuando el problema ocurre por más de 2 minutos. ¿Cómo se puede lograr esto?

- [ ] Crear una alarma de Amazon CloudWatch para la instancia de EC2 con monitoreo básico. Agregar una acción para reiniciar la instancia.
- [x] Crear una alarma de Amazon CloudWatch para la instancia de EC2 con monitoreo detallado. Agregar una acción para reiniciar la instancia.
- [ ] Crear una función de AWS Lambda para reiniciar la instancia de EC2, invocada de forma programada cada 2 minutos.
- [ ] Crear una función de AWS Lambda para reiniciar la instancia de EC2, invocada por verificaciones de salud (health checks) de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está implementando seguridad y cumplimiento normativo usando AWS Trusted Advisor. El equipo de SysOps de la empresa está validando la lista de verificaciones de Trusted Advisor a las que puede acceder. ¿Qué factor afectará la cantidad de verificaciones de Trusted Advisor disponibles?

- [ ] Si al menos una instancia de Amazon EC2 está en estado de ejecución.
- [x] El plan de soporte de AWS.
- [ ] Una Política de Control de Servicio (SCP) de AWS Organizations.
- [ ] Si el usuario raíz de la cuenta de AWS tiene habilitada la autenticación multifactor (MFA).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está investigando problemas en una instancia de base de datos de Amazon RDS para MariaDB. El ingeniero de CloudOps quiere mostrar la carga de la base de datos categorizada por eventos de espera detallados. ¿Cómo puede el ingeniero de CloudOps lograr este objetivo?

- [ ] Crear un panel (dashboard) de Amazon CloudWatch.
- [x] Habilitar `Performance Insights` de Amazon RDS.
- [ ] Habilitar y configurar `Enhanced Monitoring`.
- [ ] Revisar los registros de la base de datos en Amazon CloudWatch Logs.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un usuario que trabaja en la consola de Amazon EC2 aumentó el tamaño de un volumen de Amazon Elastic Block Store (Amazon EBS) adjunto a una instancia de Amazon EC2 Windows. El cambio no se refleja en el sistema de archivos. ¿Qué debe hacer un ingeniero de CloudOps para resolver este problema?

- [x] Extender el sistema de archivos con herramientas a nivel de sistema operativo para usar la nueva capacidad de almacenamiento.
- [ ] Volver a adjuntar el volumen EBS a la instancia de EC2.
- [ ] Reiniciar la instancia de EC2 que está adjunta al volumen EBS.
- [ ] Tomar una instantánea del volumen EBS. Reemplazar el volumen original por un volumen creado a partir de la instantánea.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha migrado su aplicación a AWS. La empresa alojará la aplicación en instancias de Amazon EC2 de múltiples familias de instancias. Durante las pruebas iniciales, un ingeniero de CloudOps identifica problemas de rendimiento en instancias de EC2 seleccionadas. La empresa tiene una política estricta de asignación de presupuesto, por lo que el ingeniero de CloudOps debe usar los tipos de recursos correctos con las características de rendimiento que coincidan con la carga de trabajo. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Comprar Instancias Reservadas (RI) regionales para ahorros de costos inmediatos. Revisar y actuar sobre las recomendaciones de rightsizing de EC2 en Cost Explorer. Intercambiar las RI por la familia de instancias óptima después del rightsizing.
- [ ] Comprar Instancias Reservadas (RI) zonales para las instancias existentes. Monitorear la utilización de RI en la consola de AWS Billing and Cost Management. Hacer ajustes en los tamaños de instancia para optimizar la utilización.
- [x] Revisar y actuar sobre las recomendaciones de AWS Compute Optimizer. Comprar Compute Savings Plans para reducir el costo requerido para ejecutar los recursos de cómputo.
- [ ] Revisar las métricas de utilización de recursos en el AWS Cost and Usage Report. Ajustar el tamaño (rightsize) de las instancias de EC2. Crear Reservas de Capacidad On-Demand para los recursos ajustados.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps es responsable de una gran flota de instancias de Amazon EC2 y debe saber si alguna instancia se verá afectada por el próximo mantenimiento de hardware. ¿Qué opción proporcionaría esta información con el MENOR esfuerzo administrativo?

- [ ] Desplegar una solución de monitoreo de terceros para proporcionar monitoreo en tiempo real de instancias EC2.
- [ ] Listar las instancias con verificaciones de estado del sistema fallidas usando la consola de administración de AWS.
- [ ] Monitorear AWS CloudTrail en busca de llamadas a la API `StopInstances`.
- [x] Revisar el AWS Personal Health Dashboard.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una aplicación de análisis de datos se está ejecutando en una instancia de Amazon EC2. Un ingeniero de CloudOps debe agregar dimensiones personalizadas a las métricas recopiladas por el agente de Amazon CloudWatch. ¿Cómo puede el ingeniero de CloudOps cumplir con este requisito?

- [ ] Crear un script de shell personalizado para extraer las dimensiones y recopilar las métricas usando el agente de Amazon CloudWatch.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para evaluar las dimensiones personalizadas requeridas y enviar las métricas a Amazon Simple Notification Service (Amazon SNS).
- [ ] Crear una función de AWS Lambda para recopilar las métricas de AWS CloudTrail y enviar las métricas a un grupo de Amazon CloudWatch Logs.
- [x] Crear un campo `append_dimensions` en el archivo de configuración del agente de Amazon CloudWatch para recopilar las métricas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa recibe una alerta de una alarma de Amazon CloudWatch. La alarma indica que una aplicación web que se ejecuta en instancias de Amazon EC2 no está respondiendo a las solicitudes. Las instancias de EC2 tienen un sistema operativo Red Hat Enterprise Linux y están en un grupo de Auto Scaling. El grupo de Auto Scaling tiene una capacidad mínima de 2 y una capacidad máxima de 5. Una investigación revela que la aplicación web está experimentando errores por falta de memoria (out-of-memory). La empresa agrega memoria a la aplicación web y quiere monitorear el uso de memoria del sistema operativo. Actualmente no existe una métrica de memoria de CloudWatch para las instancias de EC2 en el grupo de Auto Scaling. ¿Qué debe hacer un ingeniero de CloudOps para proporcionar una métrica de memoria de CloudWatch para las instancias de EC2?

- [x] Usar una Amazon Machine Image (AMI) que incluya el agente de CloudWatch.
- [ ] Activar el monitoreo detallado de CloudWatch.
- [ ] Activar Instance Metadata Service Version 2 (IMDSv2).
- [ ] Usar una Amazon Machine Image (AMI) basada en Amazon Linux.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe administrar la seguridad de una cuenta de AWS. Recientemente, la clave de acceso de un usuario de IAM se subió por error a un repositorio de código público. El ingeniero de CloudOps debe identificar todo lo que fue cambiado usando esta clave de acceso. ¿Cómo debe el ingeniero de CloudOps cumplir con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) para enviar todos los eventos de IAM a una función de AWS Lambda para su análisis.
- [ ] Consultar los registros de Amazon EC2 usando Amazon CloudWatch Logs Insights para todos los eventos iniciados con la clave de acceso comprometida dentro del período de tiempo sospechoso.
- [x] Buscar en el historial de eventos de AWS CloudTrail todos los eventos iniciados con la clave de acceso comprometida dentro del período de tiempo sospechoso.
- [ ] Buscar en los `VPC` Flow Logs todos los eventos iniciados con la clave de acceso comprometida dentro del período de tiempo sospechoso.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Si el navegador de la consola de administración de AWS no muestra que ha iniciado sesión en una cuenta de AWS, cierre el navegador y vuelva a abrir la consola usando el acceso directo de la consola de administración de AWS desde el escritorio de la VM. Si la funcionalidad de copiar y pegar no funciona en su entorno, consulte el archivo de instrucciones en el escritorio de la VM y use `Ctrl+C`, `Ctrl+V` o `Command-C`, `Command-V`. Configure Amazon EventBridge para cumplir con los siguientes requisitos. 1. Use la región `us-east-2` para todos los recursos. 2. A menos que se especifique lo contrario a continuación, use la configuración predeterminada. 3. Use su propia nomenclatura de recursos a menos que se especifique un nombre de recurso a continuación. 4. Asegúrese de que todos los eventos de Amazon EC2 en el bus de eventos predeterminado sean reproducibles (replayable) durante los últimos 90 días. 5. Cree una regla llamada `RunFunction` para enviar el mensaje exacto `{"name":"example"}` cada 15 minutos a una función de AWS Lambda existente llamada LogEventFunction. 6. Cree una regla llamada `SpotWarning` para enviar una notificación a un nuevo tema estándar de Amazon SNS llamado `TopicEvents` cada vez que se interrumpa una instancia Spot de Amazon EC2. NO cree ninguna suscripción al tema. La notificación debe coincidir con la siguiente estructura: `Input path: {instance: detail.instance-id} Input template: The EC2 Spot Instance <instance> has been interrupted.` Importante: Haga clic en el botón Next para completar este laboratorio y continuar al siguiente. Una vez que haga clic en el botón Next, NO podrá volver a este laboratorio.

![Question 210](images/question210.png)

- [x] 1. Haga clic en `Event pattern form` en `Event patterns`. 2. Seleccione `AWS service`. 3. En `Step 1: Create rule`, seleccione `Event Pattern` bajo `Event Source`. 4. Asegúrese de que esté seleccionado `Build event pattern to match events by service`. 5. Asegúrese de que `Service Name` tenga seleccionado `EC2`. 6. Asegúrese de que `Event Type` tenga seleccionado `EC2 Spot Instance Interruption Warning`. 7. Seleccione `SNS topic` bajo `Targets`. 8. Asegúrese de que `TopicEvents` tenga seleccionado `Topic`. 9. Haga clic en `Input Transformer` y asegúrese de tener `{"instance":"$.detail-instance-id"}`. 10. Escriba una descripción y haga clic en `Configure details`. 11. En `Step 2: Configure rule details`, cree 2 reglas: `RunFunction` y `SpotWarning`. 12. Asegúrese de que el `State` de las reglas esté configurado como `Enabled` en ese paso. 13. Valide en CloudWatch Events o EventBridge.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una carga de trabajo con estado (stateful) de larga duración en una única instancia de Amazon EC2 On-Demand de propósito general xlarge. Las métricas muestran que el servicio siempre está usando `80%` de su memoria disponible y `40%` de su CPU disponible. Un ingeniero de CloudOps debe reducir el costo del servicio sin afectar negativamente el rendimiento. ¿Qué cambio en el tipo de instancia cumplirá con estos requisitos?

- [ ] Cambiar a una instancia On-Demand large optimizada para cómputo.
- [x] Cambiar a una instancia On-Demand large optimizada para memoria.
- [ ] Cambiar a una instancia Spot xlarge de propósito general.
- [ ] Cambiar a dos instancias On-Demand large de propósito general.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Cuando la infraestructura de la nube de AWS experimenta un evento que puede afectar a una organización, ¿qué servicio de AWS se puede usar para ver cuáles recursos de la organización están afectados?

- [ ] AWS Service Health Dashboard.
- [ ] AWS Trusted Advisor.
- [x] AWS Personal Health Dashboard.
- [ ] AWS Systems Manager.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias de EC2 están en un grupo de Auto Scaling. La aplicación a veces se vuelve lenta y no responde. Las métricas de Amazon CloudWatch muestran que algunas instancias de EC2 están experimentando alta carga de CPU. Un ingeniero de CloudOps necesita crear un panel (dashboard) de CloudWatch que pueda mostrar automáticamente las métricas de CPU de todas las instancias de EC2. Las métricas deben incluir las nuevas instancias que se lancen como parte del grupo de Auto Scaling. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear un panel de CloudWatch. Usar notificaciones de actividad del grupo de Auto Scaling para invocar una función personalizada de AWS Lambda. Usar la función Lambda para actualizar el panel de CloudWatch y monitorear la métrica `CPUUtilization` de los nuevos ID de instancia.
- [ ] Crear un panel de CloudWatch. Ejecutar un script personalizado en cada instancia de EC2 para transmitir el uso de CPU al panel.
- [x] Usar CloudWatch metrics explorer para filtrar por la etiqueta `aws:autoscaling:groupName` y crear una visualización para la métrica `CPUUtilization`. Agregar la visualización a un panel de CloudWatch.
- [ ] Usar CloudWatch metrics explorer para filtrar por estado de instancia y crear una visualización para la métrica `CPUUtilization`. Agregar la visualización a un panel de CloudWatch.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta cientos de instancias de Amazon EC2 en una única región de AWS. Cada instancia de EC2 tiene dos volúmenes adjuntos de Amazon Elastic Block Store (Amazon EBS) de 1 GiB `General Purpose SSD (gp2)`. Una carga de trabajo crítica está usando toda la capacidad de IOPS disponible en los volúmenes EBS. Según la política de la empresa, esta no puede cambiar los tipos de instancia ni los tipos de volumen EBS sin completar extensas pruebas de aceptación para validar que las aplicaciones de la empresa funcionarán correctamente. Un ingeniero de CloudOps necesita aumentar el rendimiento de E/S de los volúmenes EBS lo más rápido posible. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con estos requisitos?

- [x] Aumentar el tamaño de los volúmenes EBS de 1 GiB.
- [ ] Agregar dos interfaces de red elásticas adicionales en cada instancia de EC2.
- [ ] Activar Transfer Acceleration en los volúmenes EBS de la región.
- [ ] Agregar todas las instancias de EC2 a un grupo de ubicación (placement group) de tipo cluster.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa planea alojar sus aplicaciones web con estado (stateful) en AWS. Un ingeniero de CloudOps está usando un grupo de Auto Scaling de instancias de Amazon EC2. Las aplicaciones web se ejecutarán las 24 horas del día, los 7 días de la semana, durante todo el año. La empresa debe poder cambiar el tipo de instancia dentro de la misma familia de instancias más adelante en el año según los patrones de tráfico y uso. ¿Qué opción de compra de instancias EC2 cumplirá con estos requisitos de la manera MÁS rentable?

- [x] Instancias Reservadas Convertibles.
- [ ] Instancias On-Demand.
- [ ] Instancias Spot.
- [ ] Instancias Reservadas Estándar.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa necesita subir gigabytes de archivos todos los días. La empresa necesita lograr mayor rendimiento y velocidades de carga hacia Amazon S3. ¿Qué acción debe tomar un ingeniero de CloudOps para cumplir con este requisito?

- [ ] Crear una distribución de Amazon CloudFront con el método `HTTP` GET permitido y el bucket de S3 como origen.
- [ ] Crear un clúster de Amazon ElastiCache y habilitar el almacenamiento en caché para el bucket de S3.
- [ ] Configurar AWS Global Accelerator con el bucket de S3.
- [x] Habilitar S3 Transfer Acceleration y usar el endpoint de aceleración al subir archivos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un equipo de aplicación está trabajando con un ingeniero de CloudOps para definir alarmas de Amazon CloudWatch para una aplicación. El equipo de aplicación no conoce el uso esperado ni el crecimiento esperado de la aplicación. ¿Qué solución debe recomendar el ingeniero de CloudOps?

- [x] Crear alarmas de CloudWatch basadas en detección de anomalías (anomaly detection).
- [ ] Crear alarmas de CloudWatch usando un conjunto de alarmas compuestas.
- [ ] Crear alarmas de CloudWatch usando umbrales estáticos.
- [ ] Crear alarmas de CloudWatch que traten los datos faltantes como incumplimiento (breaching).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa de comercio electrónico usa un clúster de Amazon ElastiCache for Memcached para el almacenamiento en caché en memoria de consultas de productos populares en el sitio de compras. Al revisar los datos recientes de métricas de Amazon CloudWatch para el clúster de ElastiCache, el ingeniero de CloudOps nota una gran cantidad de desalojos (evictions). ¿Cuál de las siguientes acciones reducirá estos desalojos? (Elija dos.)

- [x] Agregar un nodo adicional al clúster de ElastiCache.
- [ ] Aumentar el tiempo de vida (TTL) de ElastiCache.
- [x] Aumentar el tamaño de los nodos individuales dentro del clúster de ElastiCache.
- [ ] Colocar un Elastic Load Balancer delante del clúster de ElastiCache.
- [ ] Usar Amazon Simple Queue Service (Amazon SQS) para desacoplar el clúster de ElastiCache.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa necesita garantizar un cumplimiento estricto de un presupuesto para 25 aplicaciones desplegadas en AWS. Equipos separados son responsables de los costos de almacenamiento, cómputo y base de datos. Un ingeniero de CloudOps debe implementar una solución automatizada para alertar a cada equipo cuando su gasto proyectado exceda un monto trimestral establecido por el departamento de finanzas. La solución no puede incurrir en costos adicionales de cómputo, almacenamiento o base de datos. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar AWS Cost and Usage Reports para enviar un informe diario a un bucket de Amazon S3. Crear una función de AWS Lambda que evalúe el gasto por servicio y notifique a cada equipo usando notificaciones de Amazon Simple Notification Service (Amazon SNS). Invocar la función Lambda cuando se coloque un informe en el bucket de S3.
- [ ] Configurar AWS Cost and Usage Reports para enviar un informe diario a un bucket de Amazon S3. Crear una regla en Amazon EventBridge (Amazon CloudWatch Events) para evaluar el gasto por servicio y notificar a cada equipo usando Amazon Simple Queue Service (Amazon SQS) cuando se supere el umbral de costo.
- [ ] Usar AWS Budgets para crear un presupuesto de costos y seleccionar cada uno de los servicios en uso. Especificar el monto del presupuesto definido por el departamento de finanzas junto con el umbral de costo proyectado. Ingresar los destinatarios de correo electrónico apropiados para el presupuesto.
- [x] Usar AWS Budgets para crear un presupuesto de costos para cada equipo, filtrando por los servicios que poseen. Especificar el monto del presupuesto definido por el departamento de finanzas junto con un umbral de costo proyectado. Ingresar los destinatarios de correo electrónico apropiados para cada presupuesto.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Se requiere que un ingeniero de CloudOps monitoree el espacio libre en volúmenes de Amazon EBS adjuntos a instancias de Amazon EC2 basadas en Microsoft Windows dentro de la cuenta de una empresa. El ingeniero debe recibir alertas sobre posibles problemas. ¿Qué debe hacer el ingeniero para recibir alertas por correo electrónico antes de que el poco espacio de almacenamiento afecte el rendimiento de la instancia de EC2?

- [ ] Usar métricas integradas de Amazon CloudWatch, y configurar alarmas de CloudWatch y un tema de Amazon SNS para notificaciones por correo electrónico.
- [ ] Usar registros de AWS CloudTrail y configurar el trail para enviar notificaciones a un tema de Amazon SNS.
- [x] Usar el agente de Amazon CloudWatch para enviar métricas de espacio en disco, luego configurar alarmas de CloudWatch usando un tema de Amazon SNS.
- [ ] Usar AWS Trusted Advisor y habilitar alertas de notificación por correo electrónico para el espacio en disco de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps quiere monitorear el espacio libre en disco disponible en un conjunto de instancias de Amazon EC2 que tienen volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos. El ingeniero de CloudOps quiere recibir una notificación cuando el espacio de disco usado de los volúmenes EBS supere un valor umbral, pero solo cuando la métrica `DiskReadOps` también supere un valor umbral. El ingeniero de CloudOps ha configurado un tema de Amazon Simple Notification Service (Amazon SNS). ¿Cómo puede el ingeniero de CloudOps recibir la notificación solo cuando ambas métricas superen sus valores umbral?

- [x] Instalar el agente de Amazon CloudWatch en las instancias de EC2. Crear una alarma de métrica para el espacio en disco y una alarma de métrica para la métrica `DiskReadOps`. Crear una alarma compuesta que incluya las dos alarmas de métrica para publicar una notificación en el tema de SNS.
- [ ] Instalar el agente de Amazon CloudWatch en las instancias de EC2. Crear una alarma de métrica para el espacio en disco y una alarma de métrica para la métrica `DiskReadOps`. Configurar cada alarma para publicar una notificación en el tema de SNS.
- [ ] Crear una alarma de métrica para la métrica `EBSByteBalance%` y una alarma de métrica para la métrica `DiskReadOps`. Crear una alarma compuesta que incluya las dos alarmas de métrica para publicar una notificación en el tema de SNS.
- [ ] Configurar el monitoreo detallado para las instancias de EC2. Crear una alarma de métrica para el espacio en disco y una alarma de métrica para la métrica `DiskReadOps`. Crear una alarma compuesta que incluya las dos alarmas de métrica para publicar una notificación en el tema de SNS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa quiere reducir costos para trabajos que se pueden completar en cualquier momento. Los trabajos actualmente se ejecutan usando múltiples instancias de Amazon EC2 On-Demand y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier motivo, debe reiniciarse desde el principio. ¿Qué solución cumple con estos requisitos de la manera MÁS rentable?

- [ ] Comprar Instancias Reservadas para los trabajos.
- [ ] Enviar una solicitud de Instancia Spot única (one-time) para los trabajos.
- [x] Enviar una solicitud de Instancias Spot con una duración definida para los trabajos.
- [ ] Usar una combinación de Instancias On-Demand e Instancias Spot para los trabajos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un entorno consta de 100 instancias de Amazon EC2 Windows. El agente de Amazon CloudWatch está desplegado y ejecutándose en todas las instancias de EC2 con un archivo de configuración base para capturar archivos de registro. Existe un nuevo requisito para capturar los archivos de registro `DHCP` que existen en 50 de las instancias. ¿Cuál es la forma MÁS eficiente operativamente para cumplir con este nuevo requisito?

- [x] Crear un archivo de configuración adicional del agente de CloudWatch para capturar los registros `DHCP`. Usar AWS Systems Manager Run Command para reiniciar el agente de CloudWatch en cada instancia de EC2 con la opción `append-config` para aplicar el archivo de configuración adicional.
- [ ] Iniciar sesión en cada instancia de EC2 con derechos de administrador. Crear un script de PowerShell para enviar los archivos de registro base necesarios y los archivos de registro `DHCP` a CloudWatch.
- [ ] Ejecutar el asistente del archivo de configuración del agente de CloudWatch en cada instancia de EC2. Verificar que los archivos de registro base estén incluidos y agregar los archivos de registro `DHCP` durante el proceso de creación del asistente.
- [ ] Ejecutar el asistente del archivo de configuración del agente de CloudWatch en cada instancia de EC2 y seleccionar el nivel de detalle avanzado. Esto capturará los archivos de registro del sistema operativo.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa necesita monitorear la utilización de disco de volúmenes de Amazon Elastic Block Store (Amazon EBS). Los volúmenes EBS están adjuntos a instancias de Amazon EC2 Linux. Un ingeniero de CloudOps debe configurar una alarma de Amazon CloudWatch que emita una alerta cuando la utilización de disco aumente a más del `80%`. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija tres.)

- [x] Crear un rol de IAM que incluya la política administrada de AWS `CloudWatchAgentServerPolicy`. Adjuntar el rol a las instancias.
- [ ] Crear un rol de IAM que incluya la política administrada de AWS `CloudWatchApplicationInsightsReadOnlyAccess`. Adjuntar el rol a las instancias.
- [x] Instalar e iniciar el agente de CloudWatch usando AWS Systems Manager o la línea de comandos.
- [ ] Instalar e iniciar el agente de CloudWatch usando un rol de IAM. Adjuntar la política administrada de AWS `CloudWatchAgentServerPolicy` al rol.
- [x] Configurar una alarma de CloudWatch para que entre en estado `ALARM` cuando la métrica de CloudWatch `disk_used_percent` sea mayor que `80%`.
- [ ] Configurar una alarma de CloudWatch para que entre en estado `ALARM` cuando la métrica de CloudWatch `disk_used` sea mayor que `80%` o cuando la métrica de CloudWatch `disk_free` sea menor que `20%`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps administra una aplicación web que se ejecuta en instancias de Amazon EC2 detrás de un ELB Application Load Balancer (ALB). Las instancias se ejecutan en un grupo de EC2 Auto Scaling. El ingeniero quiere establecer una alarma para cuando todas las instancias de destino asociadas con el `ALB` estén no saludables. ¿Qué condición se debe usar con la alarma?

- [x] `AWS/ApplicationELB HealthyHostCount <= 0`.
- [ ] `AWS/ApplicationELB UnhealthyHostCount >= 1`.
- [ ] `AWS/EC2 StatusCheckFailed <= 0`.
- [ ] `AWS/EC2 StatusCheckFailed >= 1`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa quiere monitorear los grupos de seguridad de sus instancias de Amazon EC2 para asegurarse de que `SSH` no esté abierto al público. Si el puerto está abierto, la empresa necesita cerrarlo lo antes posible. ¿Qué combinación de acciones debe tomar un ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [ ] Agregar una alarma de Amazon CloudWatch para detectar los grupos de seguridad que permiten `SSH`.
- [x] Agregar una regla de AWS Config para detectar los grupos de seguridad que permiten `SSH`.
- [ ] Agregar una plantilla de evaluación a Amazon Inspector para detectar los grupos de seguridad que permiten `SSH`.
- [x] Llamar a un runbook de AWS Systems Manager Automation para cerrar el puerto.
- [ ] Llamar a AWS Systems Manager Run Command para cerrar el puerto.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja una aplicación interna en instancias de Amazon EC2 On-Demand detrás de un Application Load Balancer (ALB). Las instancias están en un grupo de Amazon EC2 Auto Scaling. Los empleados usan la aplicación para proporcionar precios de productos a clientes potenciales. El grupo de Auto Scaling está configurado con una política de escalado dinámico y rastrea el uso promedio de CPU de las instancias. Los empleados han notado que a veces la aplicación se vuelve lenta o no responde. Un ingeniero de CloudOps descubre que algunas instancias están experimentando una alta carga de CPU. El grupo de Auto Scaling no puede escalar hacia afuera porque la empresa está alcanzando la cuota de servicio de instancias de EC2. El ingeniero de CloudOps necesita implementar una solución que proporcione una notificación cuando la empresa alcance el `70%` o más de la cuota de servicio de instancias de EC2. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear una función de AWS Lambda que liste las instancias de EC2, cuente las instancias de EC2, y compare el número total con el valor de cuota aplicado usando la API de Service Quotas. Configurar la función Lambda para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) si la utilización de la cuota es igual o mayor al `70%`. Crear una regla de Amazon EventBridge para invocar la función Lambda.
- [ ] Crear una función de AWS Lambda que liste las instancias de EC2, cuente las instancias de EC2, y compare el número total con el valor de cuota aplicado usando la API de Amazon CloudWatch Metrics. Configurar la función Lambda para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) si la utilización de la cuota es igual o mayor al `70%`. Crear una regla de Amazon EventBridge para invocar la función Lambda.
- [x] Usar la consola de Service Quotas para crear una alarma de Amazon CloudWatch para las instancias de EC2. Configurar la alarma con una utilización de cuota igual o mayor al `70%`. Configurar la alarma para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) cuando la alarma entre en estado `ALARM`.
- [ ] Crear una alarma de Amazon CloudWatch. Configurar la alarma con un umbral del `70%` para la métrica `CPUUtilization` de las instancias de EC2. Configurar la alarma para publicar una notificación de Amazon Simple Notification Service (Amazon SNS) cuando la alarma entre en estado `ALARM`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un equipo de desarrolladores usa varios buckets de Amazon S3 como repositorios centralizados. Usuarios de todo el mundo suben grandes conjuntos de archivos a estos repositorios. Las aplicaciones del equipo de desarrollo procesan estos archivos posteriormente. Un ingeniero de CloudOps configura un nuevo bucket de S3, `DOC-EXAMPLE-BUCKET`, para soportar una nueva carga de trabajo. El nuevo bucket de S3 también recibe cargas regulares de grandes conjuntos de archivos de usuarios de todo el mundo. Cuando el nuevo bucket de S3 entra en producción, el rendimiento de carga desde ciertas áreas geográficas es menor que el rendimiento de carga que proporcionan los buckets de S3 existentes. ¿Qué debe hacer el ingeniero de CloudOps para remediar este problema?

- [ ] Aprovisionar un clúster de Amazon ElastiCache for Redis para el nuevo bucket de S3. Proporcionar a los desarrolladores el endpoint de configuración del clúster para usar en sus llamadas de API.
- [ ] Agregar el nuevo bucket de S3 a una nueva distribución de Amazon CloudFront. Proporcionar a los desarrolladores el nombre de dominio de la nueva distribución para usar en sus llamadas de API.
- [x] Habilitar S3 Transfer Acceleration para el nuevo bucket de S3. Verificar que los desarrolladores estén usando el nombre de endpoint `DOC-EXAMPLE-BUCKET.s3-accelerate.amazonaws.com` en sus llamadas de API.
- [ ] Usar la carga multiparte (multipart upload) de S3 para el nuevo bucket de S3. Verificar que los desarrolladores estén usando nombres de endpoint de S3 específicos de la región, como `DOC-EXAMPLE-BUCKETS3`, `[Region] amazonaws.com`, en sus llamadas de API.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene usuarios que despliegan instancias de Amazon EC2 con más capacidad de rendimiento de disco de la requerida. Un ingeniero de CloudOps necesita revisar todos los volúmenes de Amazon Elastic Block Store (Amazon EBS) asociados con las instancias y crear recomendaciones de optimización de costos basadas en IOPS y rendimiento (throughput). ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Usar los gráficos de monitoreo en la consola de EC2 para ver las métricas de los volúmenes EBS. Revisar el espacio consumido contra el espacio aprovisionado en cada volumen. Identificar cualquier volumen que tenga baja utilización.
- [ ] Detener las instancias de EC2 desde la consola de EC2. Cambiar el tipo de instancia de EC2 a uno optimizado para Amazon EBS. Iniciar las instancias de EC2.
- [x] Habilitar AWS Compute Optimizer. Permitir tiempo suficiente para que se recopilen las métricas. Revisar los hallazgos de Compute Optimizer para los volúmenes EBS.
- [ ] Instalar la herramienta `fio` en las instancias de EC2 y crear un archivo `.cfg` para aproximar las cargas de trabajo requeridas. Usar los resultados del benchmark para evaluar si los volúmenes EBS aprovisionados son del tipo más apropiado.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha creado una puerta de enlace `NAT` en una subred pública en una `VPC`. La `VPC` también contiene una subred privada que incluye instancias de Amazon EC2. Las instancias de EC2 usan la puerta de enlace `NAT` para acceder a internet y descargar parches y actualizaciones. La empresa ha configurado un flow log de `VPC` para la interfaz de red elástica de la puerta de enlace `NAT`. La empresa está publicando la salida en Amazon CloudWatch Logs. Un ingeniero de CloudOps debe identificar los cinco destinos de internet principales con los que se comunican las instancias de EC2 en la subred privada para las descargas. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito de la manera MÁS eficiente operativamente?

- [ ] Usar eventos de AWS CloudTrail Insights para identificar los cinco destinos de internet principales.
- [ ] Usar los registros estándar de Amazon CloudFront (access logs) para identificar los cinco destinos de internet principales.
- [x] Usar CloudWatch Logs Insights para identificar los cinco destinos de internet principales.
- [ ] Cambiar el flow log para publicar registros en Amazon S3. Usar Amazon Athena para consultar los archivos de registro en Amazon S3.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación web de una sola página en AWS. La aplicación usa Amazon CloudFront para entregar contenido estático desde un origen de bucket de Amazon S3. La aplicación también usa un clúster de Amazon Elastic Kubernetes Service (Amazon EKS) para atender llamadas de API. Los usuarios a veces reportan que el sitio web no está operativo, incluso cuando el monitoreo muestra que la página de inicio es alcanzable y que el clúster de EKS está saludable. Un ingeniero de CloudOps debe implementar monitoreo adicional que pueda detectar cuándo el sitio web no está operativo antes de que los usuarios reporten el problema. ¿Qué solución cumple con estos requisitos?

- [x] Crear un canary de monitor de latido (heartbeat monitor) de Amazon CloudWatch Synthetics que apunte al nombre de dominio completamente calificado (FQDN) del sitio web.
- [ ] Crear un canary de API de Amazon CloudWatch Synthetics que monitoree la disponibilidad de los endpoints de API del clúster de EKS.
- [ ] Crear un monitor de aplicación de Amazon CloudWatch RUM que apunte al nombre de dominio completamente calificado (FQDN) del sitio web. Configurar el monitor de aplicación para recopilar telemetría de rendimiento y errores de JavaScript.
- [ ] Crear un monitor de aplicación de Amazon CloudWatch RUM que use los endpoints de API del clúster de EKS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está haciendo la transición desde aplicaciones alojadas en instancias de Amazon EC2. La empresa quiere implementar una arquitectura sin servidor (serverless) que use Amazon S3, Amazon API Gateway, AWS Lambda y Amazon CloudFront. Como parte de esta transición, la empresa tiene direcciones IP elásticas que no están asociadas con ninguna instancia de EC2 después de que estas se terminan. Un ingeniero de CloudOps necesita automatizar el proceso de liberar todas las direcciones IP elásticas no asociadas que permanecen después de que las instancias de EC2 se terminan. ¿Qué solución cumple con este requisito de la manera MÁS eficiente operativamente?

- [x] Activar la regla administrada de AWS Config `eip-attached` para que se ejecute automáticamente cuando ocurran cambios de recursos en la cuenta de AWS. Configurar la remediación automática para la regla. Especificar el runbook de AWS Systems Manager Automation `AWS-ReleaseElasticIP` para la remediación. Especificar un rol apropiado que tenga permisos para la remediación.
- [ ] Crear una función Lambda personalizada que llame a la operación de API `ReleaseAddress` de EC2 y especifique el `AllocationId` de la dirección IP elástica. Invocar la función Lambda usando una regla de Amazon EventBridge. Especificar servicios de AWS como el origen del evento, All Events como el tipo de evento, y AWS Trusted Advisor como el destino.
- [ ] Crear una regla de Amazon EventBridge. Especificar servicios de AWS como el origen del evento, `Instance State-change Notification` como el tipo de evento, y Amazon EC2 como el servicio. Invocar una función Lambda que extraiga la dirección IP elástica de la notificación. Usar AWS CloudFormation para liberar la dirección especificando el `AllocationId` como parámetro de entrada.
- [ ] Crear una función Lambda personalizada que llame a la operación de API `ReleaseAddress` de EC2 y especifique el `AllocationId` de la dirección IP elástica. Invocar la función Lambda usando una regla de Amazon EventBridge. Especificar servicios de AWS como el origen del evento, `Instance State-change Notification` como el tipo de evento, y Amazon EC2 como el servicio.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El uso de servicios de AWS Cloud de una empresa está creciendo rápidamente, por lo que se le ha pedido a un ingeniero de CloudOps que genere detalles del gasto diario para compartir con la gerencia. ¿Qué método debe elegir el ingeniero para producir estos datos?

- [ ] Compartir la factura mensual de AWS con la gerencia.
- [ ] Usar los registros de AWS CloudTrail para acceder a los costos diarios en formato JSON.
- [x] Configurar un Cost and Usage Report diario y descargar la salida desde Amazon S3.
- [ ] Monitorear los costos de AWS con Amazon CloudWatch y crear alarmas y notificaciones de facturación.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Los usuarios están experimentando periódicamente tiempos de respuesta lentos de una base de datos relacional. La base de datos se ejecuta en una instancia ráfaga (burstable) de Amazon EC2 con un volumen de Amazon Elastic Block Store (Amazon EBS) `General Purpose SSD (gp2)` de `350 GB`. Un ingeniero de CloudOps monitorea la instancia de EC2 en Amazon CloudWatch y observa que la métrica `VolumeReadOps` cae a menos del `10%` de su valor máximo durante los períodos de respuesta lenta. ¿Qué debe hacer el ingeniero de CloudOps para asegurar un rendimiento consistentemente alto?

- [ ] Convertir el volumen `gp2` a un volumen EBS `General Purpose SSD (gp3)`.
- [ ] Convertir el volumen `gp2` a un volumen EBS `Cold HDD (sc1)`.
- [ ] Convertir la instancia de EC2 a un tipo de instancia optimizado para memoria.
- [x] Activar el modo ilimitado (unlimited mode) en la instancia de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### AnyCompany ha adquirido Example Corp y está intentando consolidar los sistemas empresariales de ambas compañías. El departamento de TI de AnyCompany necesita integrarse con el sistema de tickets de TI de Example Corp. Un ingeniero de CloudOps debe implementar una solución que use alarmas de Amazon CloudWatch para instancias de Amazon EC2 en la cuenta de AnyCompany para crear nuevos tickets en el sistema de tickets de Example Corp. El sistema de tickets proporciona un endpoint `HTTPS` para la creación de nuevos tickets. El sistema de tickets acepta mensajes en el siguiente formato JSON. ¿Qué enfoque para crear tickets a partir de las alarmas de CloudWatch cumple con estos requisitos con el MENOR tiempo de desarrollo?

![Question 299](images/question299.png)

- [ ] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique EventBridge API destinations como destino. Configurar EventBridge API destinations para enviar eventos al endpoint `HTTPS`. En la regla de EventBridge, crear un input transformer para convertir el origen a una salida compatible con el sistema de tickets.
- [ ] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique un flujo de datos de Amazon Kinesis como destino. Crear una función de AWS Lambda para recibir eventos del flujo de datos de Kinesis. Configurar la función Lambda para iniciar un trabajo de AWS Glue que transforme los datos y reenvíe la salida al endpoint `HTTPS`.
- [x] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique Amazon Simple Notification Service (Amazon SNS) como destino. Configurar Amazon SNS para transformar los eventos y enviarlos al endpoint `HTTPS`.
- [ ] Crear una regla de Amazon EventBridge que filtre los eventos apropiados y especifique una máquina de estados de AWS Step Functions como destino. Crear una función de AWS Lambda y un trabajo de AWS Glue en Step Functions para transformar los eventos y enviarlos al endpoint `HTTPS`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta sus aplicaciones en una gran cantidad de instancias de Amazon EC2. Un ingeniero de CloudOps debe implementar una solución para notificar al equipo de operaciones cada vez que cambie el estado de una instancia de EC2. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear un script que capture los cambios de estado de las instancias y publique una notificación en un tema de Amazon Simple Notification Service (Amazon SNS). Usar AWS Systems Manager Run Command para ejecutar el script en todas las instancias de EC2.
- [x] Crear una regla de evento de Amazon EventBridge que capture los cambios de estado de las instancias de EC2. Establecer un tema de Amazon Simple Notification Service (Amazon SNS) como destino.
- [ ] Crear una regla de evento de Amazon EventBridge que capture los cambios de estado de las instancias de EC2. Establecer como destino una función de AWS Lambda que publique una notificación en un tema de Amazon Simple Notification Service (Amazon SNS).
- [ ] Crear una regla personalizada de AWS Config que evalúe los cambios de estado de las instancias con remediación automática. Usar la regla para invocar una función de AWS Lambda que publique una notificación en un tema de Amazon Simple Notification Service (Amazon SNS).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa necesita hacer cumplir los requisitos de etiquetado para tablas de Amazon DynamoDB en sus cuentas de AWS. Un ingeniero de CloudOps debe implementar una solución para identificar y remediar todas las tablas de DynamoDB que no tengan las etiquetas apropiadas. ¿Qué solución cumple con estos requisitos con el MENOR esfuerzo operativo?

- [ ] Crear una función de AWS Lambda personalizada para evaluar y remediar todas las tablas de DynamoDB. Crear una regla programada de Amazon EventBridge para invocar la función Lambda.
- [ ] Crear una función de AWS Lambda personalizada para evaluar y remediar todas las tablas de DynamoDB. Crear una regla personalizada de AWS Config para invocar la función Lambda.
- [x] Usar la regla administrada de AWS Config `required-tags` para evaluar todas las tablas de DynamoDB en busca de las etiquetas apropiadas. Configurar una acción de remediación automática que use un runbook personalizado de AWS Systems Manager Automation.
- [ ] Crear una regla administrada de Amazon EventBridge para evaluar todas las tablas de DynamoDB en busca de las etiquetas apropiadas. Configurar la regla de EventBridge para ejecutar un runbook personalizado de AWS Systems Manager Automation para la remediación.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa quiere rastrear sus costos de AWS en todas las cuentas miembro que forman parte de una organización en AWS Organizations. Los administradores de las cuentas miembro quieren recibir una notificación cuando los costos estimados superen un monto predeterminado cada mes. Los administradores no pueden configurar una alarma de facturación. Los permisos de IAM para todos los usuarios son correctos. ¿Cuál podría ser la causa de este problema?

- [x] La cuenta de administración/pagadora no tiene activadas las alertas de facturación.
- [ ] La empresa no ha configurado AWS Resource Access Manager (AWS RAM) para compartir información de facturación entre las cuentas miembro y la cuenta de administración/pagadora.
- [ ] Amazon GuardDuty está activado para todas las cuentas.
- [ ] La empresa no ha configurado una regla de AWS Config para monitorear la facturación.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa de servicios financieros está ejecutando software de computación distribuida para administrar una flota de 20 servidores para sus cálculos. Hay 2 nodos de control y 18 nodos trabajadores (worker) que ejecutan los cálculos. Los nodos de control pueden iniciar automáticamente los nodos trabajadores cuando sea necesario. Actualmente, todos los nodos se ejecutan on-demand, y los nodos trabajadores se usan aproximadamente 4 horas cada día. ¿Qué combinación de acciones será MÁS rentable? (Elija dos.)

- [ ] Usar Dedicated Hosts para los nodos de control.
- [x] Usar Instancias Reservadas para los nodos de control.
- [ ] Usar Instancias Reservadas para los nodos trabajadores.
- [ ] Usar Instancias Spot para los nodos de control e Instancias On-Demand si no hay disponibilidad Spot.
- [x] Usar Instancias Spot para los nodos trabajadores e Instancias On-Demand si no hay disponibilidad Spot.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una aplicación web que experimenta problemas de rendimiento varias veces cada noche. Un análisis de causa raíz revela picos en el uso de CPU que duran 5 minutos en una instancia de Amazon EC2 Linux. Se le encarga a un ingeniero de CloudOps encontrar el ID de proceso (PID) del servicio o proceso que está consumiendo más CPU. ¿Cómo puede el ingeniero lograr esto con el MENOR esfuerzo?

- [ ] Configurar una función de AWS Lambda en Python `3.7` para que se ejecute cada minuto y capture el PID y envíe una notificación.
- [x] Configurar el plugin `procstat` para recopilar y enviar métricas de CPU de los procesos en ejecución.
- [ ] Iniciar sesión en la instancia de EC2 Linux usando una clave `.pem` cada noche y luego ejecutar el comando top.
- [ ] Usar la métrica predeterminada de uso de CPU de Amazon CloudWatch para capturar el PID en el panel de CloudWatch.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Se le ha pedido a un ingeniero de CloudOps que configure etiquetas de asignación de costos definidas por el usuario para una nueva cuenta de AWS. La empresa usa AWS Organizations para la administración de cuentas. ¿Qué debe hacer el ingeniero para habilitar las etiquetas de asignación de costos definidas por el usuario?

- [ ] Iniciar sesión en la consola de AWS Billing and Cost Management de la nueva cuenta, y usar el administrador de Cost Allocation Tags para crear las nuevas etiquetas de asignación de costos definidas por el usuario.
- [x] Iniciar sesión en la consola de AWS Billing and Cost Management de la cuenta pagadora, y usar el administrador de Cost Allocation Tags para crear las nuevas etiquetas de asignación de costos definidas por el usuario.
- [ ] Iniciar sesión en la consola de administración de AWS de la nueva cuenta, usar el Tag Editor para crear las nuevas etiquetas definidas por el usuario, luego usar el administrador de Cost Allocation Tags en la nueva cuenta para marcar las etiquetas como etiquetas de asignación de costos.
- [ ] Iniciar sesión en la consola de administración de AWS de la nueva cuenta, usar el Tag Editor para crear las nuevas etiquetas definidas por el usuario, luego usar el administrador de Cost Allocation Tags en la cuenta pagadora para marcar las etiquetas como etiquetas de asignación de costos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un volumen de Amazon EBS adjunto a una instancia de EC2 fue modificado recientemente. Parte de la modificación incluyó aumentar la capacidad de almacenamiento. El ingeniero de CloudOps nota que la capacidad de almacenamiento aumentada no se refleja en el sistema de archivos. ¿Qué paso debe completar el ingeniero para usar la capacidad de almacenamiento aumentada?

- [ ] Reiniciar la instancia de EC2.
- [x] Extender el sistema de archivos del volumen.
- [ ] Desconectar el volumen EBS, redimensionarlo, y volver a conectarlo.
- [ ] Tomar una instantánea de EBS y restaurarla en el volumen más grande.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps es responsable de una gran flota de instancias de EC2 y debe saber si alguna instancia se verá afectada por el próximo mantenimiento de hardware. ¿Qué opción proporcionaría esta información con el MENOR esfuerzo administrativo?

- [ ] Monitorear AWS CloudTrail en busca de llamadas a la API `StopInstances` relacionadas con el mantenimiento próximo.
- [x] Revisar el Personal Health Dashboard en busca de cualquier mantenimiento programado.
- [ ] Desde la consola de administración de AWS, listar cualquier instancia con verificaciones de estado del sistema fallidas.
- [ ] Desplegar una solución de monitoreo de terceros para proporcionar monitoreo en tiempo real de instancias de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa aloja una aplicación web en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias están en un grupo de Amazon EC2 Auto Scaling. Se accede a la aplicación con una URL pública. Un ingeniero de CloudOps necesita implementar una solución de monitoreo que verifique la disponibilidad de la aplicación y siga las mismas rutas y acciones que un cliente. El ingeniero de CloudOps debe recibir una notificación si menos del `95%` de las ejecuciones de monitoreo no encuentran errores. ¿Qué solución cumple con estos requisitos?

- [x] Crear un canary de Amazon CloudWatch Synthetics con un script que siga las rutas del cliente. Programar el canary para que se ejecute en una programación recurrente. Crear una alarma de CloudWatch que publique un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando la métrica `SuccessPercent` sea menor al `95%`.
- [ ] Crear verificaciones de salud (health checks) de Amazon Route 53 que monitoreen la disponibilidad del endpoint. Crear alarmas de Amazon CloudWatch que publiquen un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando la métrica `HealthCheckPercentageHealthy` sea menor al `95%`.
- [ ] Crear una única función de AWS Lambda para verificar si los endpoints están disponibles para cada ruta de cliente. Programar la función Lambda usando Amazon EventBridge (Amazon CloudWatch Events). Configurar la función Lambda para publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando un endpoint devuelva un error.
- [ ] Crear una función de AWS Lambda para cada ruta de cliente para verificar si ese endpoint específico está disponible. Programar las funciones Lambda usando Amazon EventBridge (Amazon CloudWatch Events). Configurar cada función Lambda para publicar una métrica personalizada en Amazon CloudWatch para el estado del endpoint. Crear alarmas de CloudWatch basadas en cada métrica personalizada para publicar un mensaje en un tema de Amazon Simple Notification Service (Amazon SNS) cuando una alarma esté en estado `ALARM`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps que trabaja en una instancia de Amazon EC2 ha configurado incorrectamente el reloj por una hora. La instancia de EC2 está enviando datos a Amazon CloudWatch a través del agente de CloudWatch. Las marcas de tiempo en los registros están 45 minutos en el futuro. ¿Cuál será el resultado de esta configuración?

- [ ] Amazon CloudWatch no capturará los datos porque están en el futuro.
- [x] Amazon CloudWatch aceptará los datos de métrica personalizada y los registrará.
- [ ] El agente de Amazon CloudWatch verificará el servidor de Network Time Protocol (NTP) antes de enviar los datos, y el agente corregirá la hora.
- [ ] El agente de Amazon CloudWatch verificará el servidor de Network Time Protocol (NTP), y el agente no enviará los datos porque están más de 30 minutos en el futuro.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps ha configurado un agente de CloudWatch para enviar métricas personalizadas a Amazon CloudWatch y ahora está ensamblando un panel de CloudWatch para mostrar estas métricas. ¿Qué pasos debe tomar el ingeniero para completar esta tarea?

- [ ] Seleccionar el AWS Namespace, filtrar por nombre de métrica, luego agregar al panel.
- [ ] Agregar un widget de texto, seleccionar la métrica apropiada del namespace personalizado, luego agregar al panel.
- [x] Seleccionar el widget y las métricas apropiadas del namespace personalizado, luego agregar al panel.
- [ ] Abrir la consola de CloudWatch, desde CloudWatch Events, agregar todas las métricas personalizadas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está manteniendo una aplicación que se ejecuta en instancias de Amazon EC2 detrás de un Application Load Balancer (ALB). Los usuarios reportan errores al intentar iniciar la aplicación. El ingeniero nota un aumento en la métrica de Amazon CloudWatch `HTTPCode_ELB_5xx_Count` para el balanceador de carga. ¿Cuál es una posible causa de este aumento?

- [ ] El `ALB` está asociado con subredes privadas dentro de la `VPC`.
- [ ] El `ALB` recibió una solicitud de un cliente, pero el cliente cerró la conexión.
- [ ] El grupo de seguridad del `ALB` no está configurado para permitir tráfico entrante de los usuarios.
- [x] El grupo de destino del `ALB` no contiene instancias de EC2 saludables.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está usando alarmas de Amazon CloudWatch para monitorear cargas de trabajo de Amazon Elastic Kubernetes Service (Amazon EKS). Las alarmas se inician a través de una definición de umbral y no están ayudando a que el clúster de EKS opere de manera más eficiente. Un ingeniero de CloudOps debe implementar una solución que identifique anomalías y genere recomendaciones sobre cómo abordarlas. ¿Qué solución cumple con estos requisitos?

- [ ] Usar la detección de anomalías de CloudWatch para identificar anomalías y proporcionar recomendaciones.
- [x] Usar CloudWatch Container Insights con Amazon DevOps Guru para identificar anomalías y proporcionar recomendaciones.
- [ ] Usar CloudWatch Container Insights para identificar anomalías y proporcionar recomendaciones.
- [ ] Usar la detección de anomalías de CloudWatch con CloudWatch Container Insights para identificar anomalías y proporcionar recomendaciones.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa desplegó recientemente MySQL en una instancia de Amazon EC2 con un volumen de arranque predeterminado. La empresa tiene la intención de restaurar una base de datos de 1.75 TB. Un ingeniero de CloudOps necesita aprovisionar el volumen correcto de Amazon Elastic Block Store (Amazon EBS). La base de datos requerirá un rendimiento de lectura de hasta 10,000 IOPS y no se espera que crezca en tamaño. ¿Qué solución proporcionará el rendimiento requerido al MENOR costo?

- [ ] Desplegar un volumen `Cold HDD (sc1)` de 2 TB.
- [ ] Desplegar un volumen `Throughput Optimized HDD (st1)` de 2 TB.
- [x] Desplegar un volumen `General Purpose SSD (gp3)` de 2 TB. Establecer los IOPS en 10,000.
- [ ] Desplegar un volumen `Provisioned IOPS SSD (io2)` de 2 TB. Establecer los IOPS en 10,000.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una aplicación que se ejecuta en Amazon EC2 permite a los usuarios lanzar trabajos por lotes (batch jobs) para análisis de datos. Los trabajos se ejecutan de forma asíncrona, y se notifica al usuario cuando se completan. Aunque pueden ejecutarse múltiples trabajos simultáneamente, la solicitud de un usuario no necesita cumplirse hasta dentro de 24 horas. Para ejecutar un trabajo, la aplicación lanza una instancia de EC2 adicional que realiza todos los cálculos analíticos. Un trabajo tarda entre 75 y 110 minutos en completarse y no se puede interrumpir. ¿Cuál es la forma MÁS rentable de ejecutar esta carga de trabajo?

- [ ] Ejecutar la aplicación en instancias de EC2 On-Demand. Ejecutar los trabajos en Instancias Spot con una duración especificada.
- [ ] Ejecutar la aplicación en instancias de EC2 Reservadas. Ejecutar los trabajos en AWS Lambda.
- [ ] Ejecutar la aplicación en instancias de EC2 On-Demand. Ejecutar los trabajos en instancias de EC2 On-Demand.
- [x] Ejecutar la aplicación en instancias de EC2 Reservadas. Ejecutar los trabajos en Instancias Spot con una duración especificada.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa de comercio electrónico quiere reducir costos en sus trabajos nocturnos que agregan las ventas del día actual y almacenan los resultados en Amazon S3. Los trabajos actualmente se ejecutan usando múltiples instancias on-demand y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier razón, debe reiniciarse desde el principio. ¿Qué método es el MÁS rentable según estos requisitos?

- [ ] Usar una combinación de Instancias On-Demand y Spot para la ejecución de trabajos.
- [x] Enviar una solicitud de Spot block para usar en la ejecución de trabajos.
- [ ] Comprar Instancias Reservadas para usar en la ejecución de trabajos.
- [ ] Enviar una solicitud de Instancia Spot única (one-time) para la ejecución de trabajos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa quiere reducir costos en trabajos que se pueden completar en cualquier momento. Los trabajos actualmente se ejecutan usando múltiples instancias On-Demand, y tardan un poco menos de 2 horas en completarse. Si un trabajo falla por cualquier razón, se puede reiniciar desde el principio. ¿Qué método es el MÁS rentable según estos requisitos?

- [ ] Comprar Instancias Reservadas para usar en la ejecución de trabajos.
- [ ] Enviar una solicitud de Instancia Spot única (one-time) para la ejecución de trabajos.
- [x] Enviar una solicitud de Spot block para usar en la ejecución de trabajos.
- [ ] Usar una combinación de Instancias On-Demand y Spot para la ejecución de trabajos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita recopilar el contenido de archivos de registro de una aplicación personalizada que está desplegada en cientos de instancias de Amazon EC2 que ejecutan Ubuntu. Los archivos de registro deben almacenarse en Amazon CloudWatch Logs. ¿Cómo debe el ingeniero de CloudOps recopilar los archivos de registro de la aplicación con el MENOR esfuerzo operativo?

- [ ] Configurar el servicio `syslogd` en cada instancia de EC2 para recopilar y enviar los archivos de registro de la aplicación a CloudWatch Logs.
- [ ] Instalar el agente de CloudWatch usando el administrador de paquetes de Amazon Linux en cada instancia de EC2. Configurar cada agente para recopilar los archivos de registro de la aplicación.
- [ ] Instalar el agente de CloudWatch en cada instancia de EC2 usando AWS Systems Manager. Crear una configuración de agente en cada instancia usando el asistente de configuración de CloudWatch. Configurar cada agente para recopilar los archivos de registro de la aplicación.
- [x] Almacenar una configuración del agente de CloudWatch en AWS Systems Manager Parameter Store. Instalar el agente de CloudWatch en cada instancia de EC2 usando Systems Manager. Configurar cada agente para recopilar los archivos de registro de la aplicación.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene un clúster de instancias Spot de Amazon EC2 Linux que leen muchos archivos de, y escriben muchos archivos en, volúmenes de Amazon Elastic Block Store (Amazon EBS) adjuntos. Las instancias de EC2 se inician y se detienen con frecuencia. Como parte del proceso cuando se inicia una instancia de EC2, se restaura un volumen EBS a partir de una instantánea. Los volúmenes EBS que se restauran a partir de instantáneas están experimentando un rendimiento inicial más bajo de lo esperado. La carga de trabajo de la empresa necesita casi todos los IOPS aprovisionados en los volúmenes EBS adjuntos. Las instancias de EC2 no pueden soportar la carga de trabajo cuando el rendimiento de los volúmenes EBS es demasiado bajo. Un ingeniero de CloudOps debe implementar una solución para asegurar que los volúmenes EBS proporcionen el rendimiento esperado cuando se restauren a partir de instantáneas. ¿Qué solución cumple con estos requisitos?

- [x] Configurar la restauración rápida de instantáneas (fast snapshot restore, FSR) en las instantáneas que se usan.
- [ ] Restaurar cada instantánea en un volumen EBS sin cifrar. Cifrar el volumen EBS cuando el rendimiento se estabilice.
- [ ] Formatear los volúmenes EBS como sistemas de archivos XFS antes de restaurar las instantáneas.
- [ ] Aumentar el búfer de lectura anticipada (read-ahead) de Linux a 1 MiB.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Los usuarios del sitio web reportan que las páginas de una aplicación se cargan lentamente al comienzo de la jornada laboral. La aplicación se ejecuta en instancias de Amazon EC2, y los datos se almacenan en una base de datos de Amazon RDS. El ingeniero de CloudOps sospecha que el problema está relacionado con el alto uso de CPU en un componente de esta aplicación. ¿Cómo puede el ingeniero descubrir qué componente está causando el cuello de botella de rendimiento?

- [ ] Usar AWS CloudTrail para revisar el historial de uso de recursos de cada componente.
- [x] Usar métricas de Amazon CloudWatch para examinar el uso de recursos de cada componente.
- [ ] Usar Amazon Inspector para ver los detalles de uso de recursos de cada componente.
- [ ] Usar Amazon CloudWatch Events para examinar los eventos de alto uso de cada componente.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está manteniendo una aplicación web usando una distribución web de Amazon CloudFront, un Application Load Balancer (ALB), Amazon RDS, y Amazon EC2 en una `VPC`. Todos los servicios tienen el registro habilitado. El ingeniero necesita investigar códigos de estado `HTTP` de Capa 7 de la aplicación web. ¿Qué fuentes de registro contienen los códigos de estado? (Elija dos.)

- [ ] `VPC` Flow Logs.
- [ ] Registros de AWS CloudTrail.
- [x] Registros de acceso del `ALB`.
- [x] Registros de acceso de CloudFront.
- [ ] Registros de RDS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Los equipos de desarrollo mantienen varias cargas de trabajo en AWS. La gerencia de la empresa está preocupada por el aumento de costos y quiere que el ingeniero de CloudOps configure alertas para que los equipos sean notificados cuando el gasto se acerque a límites preestablecidos. ¿Qué servicio de AWS satisfará estos requisitos?

- [x] AWS Budgets.
- [ ] AWS Cost Explorer.
- [ ] AWS Trusted Advisor.
- [ ] AWS Cost and Usage Report.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está intentando administrar sus costos en AWS Cloud. Un ingeniero de CloudOps necesita que etiquetas específicas definidas por la empresa y asignadas a recursos aparezcan en el informe de facturación. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Activar las etiquetas como etiquetas de asignación de costos generadas por AWS.
- [x] Activar las etiquetas como etiquetas de asignación de costos definidas por el usuario.
- [ ] Crear una nueva categoría de costos. Seleccionar la dimensión de facturación de cuenta.
- [ ] Crear un nuevo AWS Cost and Usage Report. Incluir los ID de recursos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene un departamento de Ventas y un departamento de Marketing. La empresa usa una cuenta de AWS. Existe la necesidad de determinar qué cargos se generan en la plataforma de AWS por cada departamento. También existe la necesidad de recibir notificaciones cuando se aproxime o se supere un nivel de costo especificado. ¿Qué dos acciones debe tomar un ingeniero de CloudOps para lograr ambos requisitos con el MENOR esfuerzo administrativo? (Elija dos.)

- [ ] Usar AWS Trusted Advisor para obtener un informe que contenga los elementos verificados en el pilar de Optimización de Costos.
- [ ] Descargar el informe de facturación detallado, cargarlo en una base de datos, y hacer coincidir las líneas de partida con una lista de recursos conocidos por departamento.
- [x] Crear un script usando la AWS CLI para aplicar automáticamente etiquetas a los recursos existentes de cada departamento. Programar el script para que se ejecute semanalmente.
- [ ] Usar AWS Organizations para crear una Unidad Organizacional de departamento y permitir que solo el personal autorizado en cada departamento cree recursos.
- [x] Crear un presupuesto (Budget) desde la consola de Billing and Cost Management. Especificar el tipo de presupuesto como Cost, asignar etiquetas para cada departamento, definir notificaciones, y especificar cualquier otra opción según sea necesario.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El director financiero (CFO) de una organización ha notado un aumento en los costos de almacenamiento de Amazon S3 durante los últimos meses. Un ingeniero de CloudOps sospecha que estos costos están relacionados con el almacenamiento de versiones antiguas de objetos de S3 de uno de sus buckets de S3. ¿Qué puede hacer el ingeniero para confirmar esta sospecha?

- [x] Habilitar S3 Inventory y luego consultar el inventario para identificar el almacenamiento total de versiones de objeto anteriores.
- [ ] Usar etiquetas de asignación de costos a nivel de objeto para identificar el almacenamiento total de versiones de objeto anteriores.
- [ ] Habilitar la función de análisis de Amazon S3 para el bucket para identificar el almacenamiento total de versiones de objeto anteriores.
- [ ] Usar métricas de almacenamiento de Amazon CloudWatch para el bucket de S3 para identificar el almacenamiento total de versiones de objeto anteriores.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta una aplicación en instancias de Amazon EC2. Las instancias de EC2 están en un grupo de Auto Scaling y se ejecutan detrás de un Application Load Balancer (ALB). La aplicación experimenta errores cuando el total de solicitudes supera las 100 solicitudes por segundo. Un ingeniero de CloudOps debe recopilar información sobre el total de solicitudes durante un período de 2 semanas para determinar cuándo las solicitudes superaron este umbral. ¿Qué debe hacer el ingeniero de CloudOps para recopilar estos datos?

- [x] Usar la métrica `RequestCount` del `ALB`. Configurar un rango de tiempo de 2 semanas y un período de 1 minuto. Examinar el gráfico para determinar los horarios y volúmenes de tráfico pico.
- [ ] Usar la matemática de métricas de Amazon CloudWatch para generar una suma de los conteos de solicitudes de todas las instancias de EC2 durante un período de 2 semanas. Ordenar por un intervalo de 1 minuto.
- [ ] Crear métricas personalizadas de Amazon CloudWatch en las plantillas de configuración de lanzamiento de EC2 para crear métricas de solicitud agregadas en todas las instancias de EC2.
- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events). Configurar un patrón de coincidencia de eventos de EC2 que cree una métrica basada en solicitudes de EC2. Mostrar los datos en un gráfico.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita crear un informe que muestre cuántos bytes se envían y reciben de cada miembro del grupo de destino para un Application Load Balancer (ALB). ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija dos.)

- [x] Habilitar el registro de acceso para el `ALB`. Guardar los registros en un bucket de Amazon S3.
- [ ] Instalar el agente de Amazon CloudWatch en las instancias del grupo de destino.
- [x] Usar Amazon Athena para consultar los registros del `ALB`. Consultar la tabla. Usar los campos `received_bytes` y `sent_bytes` para calcular el total de bytes agrupados por el campo de puerto de destino.
- [ ] Usar Amazon Athena para consultar los registros del `ALB`. Consultar la tabla. Usar los campos `received_bytes` y `sent_bytes` para calcular el total de bytes agrupados por el campo de puerto de cliente.
- [ ] Crear un panel de Amazon CloudWatch que muestre la estadística Sum de la métrica ProcessedBytes para el `ALB`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa tiene una política que establece que todos los registros de instancias de Amazon EC2 deben publicarse en Amazon CloudWatch Logs. Un ingeniero de CloudOps está solucionando problemas de una instancia de EC2 que ejecuta Amazon Linux 2. La instancia de EC2 no está publicando registros en CloudWatch Logs. El agente de Amazon CloudWatch se está ejecutando en la instancia de EC2, y el archivo de configuración del agente es correcto. ¿Qué debe hacer el ingeniero de CloudOps para resolver el problema?

- [ ] Configurar la AWS CLI en la instancia de EC2. Crear un cron job que llame a la operación de API `PutLogEvents` para enviar los archivos de registro a CloudWatch cada 5 minutos.
- [ ] Inspeccionar el período de retención del grupo de registro de CloudWatch Logs. Asegurarse de que el período de retención esté establecido en un valor mayor a 1 día.
- [ ] Configurar un flujo de datos de Amazon Kinesis que se ejecute en la misma región de AWS que la instancia de EC2. Configurar el agente de CloudWatch en la instancia de EC2 para enviar eventos de CloudWatch al flujo de datos.
- [x] Asegurarse de que el rol de IAM adjunto a la instancia de EC2 tenga permisos en CloudWatch Logs para las acciones `CreateLogGroup`, `CreateLogStream`, `PutLogEvents`, y `DescribeLogStreams`.

**[⬆ Volver arriba](#tabla-de-contenidos)**
