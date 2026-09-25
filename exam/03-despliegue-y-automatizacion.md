# Dominio 3: Despliegue, aprovisionamiento y automatización (22 %)

Preguntas de práctica AWS Certified CloudOps Engineer – Associate (SOA-C03) — 55 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [Una empresa administra muchas cuentas mediante una única organización en AWS Organizations. La organización tiene todas las funciones habilitadas. La empresa quiere activar AWS Config en todas las cuentas de la organización y en todas las regiones de AWS. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?](#una-empresa-administra-muchas-cuentas-mediante-una-única-organización-en-aws-organizations-la-organización-tiene-todas-las-funciones-habilitadas-la-empresa-quiere-activar-aws-config-en-todas-las-cuentas-de-la-organización-y-en-todas-las-regiones-de-aws-qué-debe-hacer-un-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-de-la-manera-más-eficiente-operativamente) |
| 2 | [El ingeniero de CloudOps de una empresa implementa cuatro nuevas instancias de Amazon EC2 utilizando la Amazon Machine Image (AMI) estándar de Amazon Linux 2. La empresa necesita poder usar AWS Systems Manager para administrar las instancias. El ingeniero de CloudOps observa que las instancias no aparecen en la consola de Systems Manager. ¿Qué debe hacer el ingeniero de CloudOps para resolver este problema?](#el-ingeniero-de-cloudops-de-una-empresa-implementa-cuatro-nuevas-instancias-de-amazon-ec2-utilizando-la-amazon-machine-image-ami-estándar-de-amazon-linux-2-la-empresa-necesita-poder-usar-aws-systems-manager-para-administrar-las-instancias-el-ingeniero-de-cloudops-observa-que-las-instancias-no-aparecen-en-la-consola-de-systems-manager-qué-debe-hacer-el-ingeniero-de-cloudops-para-resolver-este-problema) |
| 3 | [Un ingeniero de CloudOps quiere cargar un archivo de 1 TB de tamaño desde un entorno on-premises a un bucket de Amazon S3 usando cargas multiparte (multipart uploads). ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#un-ingeniero-de-cloudops-quiere-cargar-un-archivo-de-1-tb-de-tamaño-desde-un-entorno-on-premises-a-un-bucket-de-amazon-s3-usando-cargas-multiparte-multipart-uploads-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 4 | [Un ingeniero de CloudOps quiere administrar una aplicación de servidor web con AWS Elastic Beanstalk. El servicio de Elastic Beanstalk debe mantener siempre la capacidad completa durante las nuevas implementaciones. ¿Qué políticas de despliegue satisfacen este requisito? (Seleccione DOS.)](#un-ingeniero-de-cloudops-quiere-administrar-una-aplicación-de-servidor-web-con-aws-elastic-beanstalk-el-servicio-de-elastic-beanstalk-debe-mantener-siempre-la-capacidad-completa-durante-las-nuevas-implementaciones-qué-políticas-de-despliegue-satisfacen-este-requisito-seleccione-dos) |
| 5 | [Una empresa crea imágenes AMI personalizadas lanzando nuevas instancias de Amazon EC2 desde una plantilla de AWS CloudFormation; instala y configura el software necesario mediante AWS OpsWorks y luego toma imágenes de cada instancia de EC2. El proceso de instalación y configuración del software puede tardar entre 2 y 3 horas, pero a veces el proceso se detiene por errores de instalación. El ingeniero de CloudOps debe modificar la plantilla de CloudFormation para que, si el proceso se detiene, todo el stack falle y se revierta (rollback). Con base en estos requisitos, ¿qué se debe agregar a la plantilla?](#una-empresa-crea-imágenes-ami-personalizadas-lanzando-nuevas-instancias-de-amazon-ec2-desde-una-plantilla-de-aws-cloudformation-instala-y-configura-el-software-necesario-mediante-aws-opsworks-y-luego-toma-imágenes-de-cada-instancia-de-ec2-el-proceso-de-instalación-y-configuración-del-software-puede-tardar-entre-2-y-3-horas-pero-a-veces-el-proceso-se-detiene-por-errores-de-instalación-el-ingeniero-de-cloudops-debe-modificar-la-plantilla-de-cloudformation-para-que-si-el-proceso-se-detiene-todo-el-stack-falle-y-se-revierta-rollback-con-base-en-estos-requisitos-qué-se-debe-agregar-a-la-plantilla) |
| 6 | [Un ingeniero de CloudOps aplica la siguiente política a un stack de AWS CloudFormation. ¿Cuál es el resultado de esta política?](#un-ingeniero-de-cloudops-aplica-la-siguiente-política-a-un-stack-de-aws-cloudformation-cuál-es-el-resultado-de-esta-política) |
| 7 | [Una empresa ejecuta un sitio web en instancias de Amazon EC2 dentro de un grupo de Auto Scaling. Cuando aumenta el tráfico del sitio web, las instancias adicionales tardan varios minutos en estar disponibles debido a un script de datos de usuario (user data) de larga duración que instala software. Un ingeniero de CloudOps debe reducir el tiempo necesario para que las nuevas instancias estén disponibles. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-ejecuta-un-sitio-web-en-instancias-de-amazon-ec2-dentro-de-un-grupo-de-auto-scaling-cuando-aumenta-el-tráfico-del-sitio-web-las-instancias-adicionales-tardan-varios-minutos-en-estar-disponibles-debido-a-un-script-de-datos-de-usuario-user-data-de-larga-duración-que-instala-software-un-ingeniero-de-cloudops-debe-reducir-el-tiempo-necesario-para-que-las-nuevas-instancias-estén-disponibles-qué-acción-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 8 | [Una empresa usa AWS Organizations. Un ingeniero de CloudOps quiere usar AWS Compute Optimizer y políticas de etiquetas (tag policies) de AWS en la cuenta de administración para gobernar todas las cuentas miembro de la familia de facturación. El ingeniero de CloudOps navega a la consola de AWS Organizations pero no puede activar las políticas de etiquetas desde la cuenta de administración. ¿Cuál podría ser la razón de este problema?](#una-empresa-usa-aws-organizations-un-ingeniero-de-cloudops-quiere-usar-aws-compute-optimizer-y-políticas-de-etiquetas-tag-policies-de-aws-en-la-cuenta-de-administración-para-gobernar-todas-las-cuentas-miembro-de-la-familia-de-facturación-el-ingeniero-de-cloudops-navega-a-la-consola-de-aws-organizations-pero-no-puede-activar-las-políticas-de-etiquetas-desde-la-cuenta-de-administración-cuál-podría-ser-la-razón-de-este-problema) |
| 9 | [Una empresa está ampliando su uso de servicios de AWS en toda su cartera. La empresa quiere aprovisionar cuentas de AWS para cada equipo, con el fin de garantizar la separación de los procesos de negocio por motivos de cumplimiento de seguridad y facturación. La creación y configuración inicial (bootstrapping) de las cuentas debe realizarse de forma escalable y eficiente, de modo que las nuevas cuentas se creen con una línea base definida y con barreras de gobernanza (guardrails) implementadas. Un ingeniero de CloudOps necesita diseñar un proceso de aprovisionamiento que ahorre tiempo y recursos. ¿Qué acción se debe tomar para cumplir con estos requisitos?](#una-empresa-está-ampliando-su-uso-de-servicios-de-aws-en-toda-su-cartera-la-empresa-quiere-aprovisionar-cuentas-de-aws-para-cada-equipo-con-el-fin-de-garantizar-la-separación-de-los-procesos-de-negocio-por-motivos-de-cumplimiento-de-seguridad-y-facturación-la-creación-y-configuración-inicial-bootstrapping-de-las-cuentas-debe-realizarse-de-forma-escalable-y-eficiente-de-modo-que-las-nuevas-cuentas-se-creen-con-una-línea-base-definida-y-con-barreras-de-gobernanza-guardrails-implementadas-un-ingeniero-de-cloudops-necesita-diseñar-un-proceso-de-aprovisionamiento-que-ahorre-tiempo-y-recursos-qué-acción-se-debe-tomar-para-cumplir-con-estos-requisitos) |
| 10 | [Un ingeniero de CloudOps está usando AWS Systems Manager Patch Manager para aplicar parches a una flota de instancias de Amazon EC2. El ingeniero de CloudOps ha configurado una línea base de parches (patch baseline) y una ventana de mantenimiento. El ingeniero de CloudOps también ha usado una etiqueta de instancia para identificar cuáles instancias parchear. El ingeniero de CloudOps debe darle a Systems Manager la capacidad de acceder a las instancias de EC2. ¿Qué acción adicional debe realizar el ingeniero de CloudOps para cumplir con este requisito?](#un-ingeniero-de-cloudops-está-usando-aws-systems-manager-patch-manager-para-aplicar-parches-a-una-flota-de-instancias-de-amazon-ec2-el-ingeniero-de-cloudops-ha-configurado-una-línea-base-de-parches-patch-baseline-y-una-ventana-de-mantenimiento-el-ingeniero-de-cloudops-también-ha-usado-una-etiqueta-de-instancia-para-identificar-cuáles-instancias-parchear-el-ingeniero-de-cloudops-debe-darle-a-systems-manager-la-capacidad-de-acceder-a-las-instancias-de-ec2-qué-acción-adicional-debe-realizar-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 11 | [Un ingeniero de CloudOps ha creado un portafolio de AWS Service Catalog y lo ha compartido con una segunda cuenta de AWS de la empresa. La segunda cuenta está controlada por otro ingeniero. ¿Qué acción podrá realizar el ingeniero de la segunda cuenta?](#un-ingeniero-de-cloudops-ha-creado-un-portafolio-de-aws-service-catalog-y-lo-ha-compartido-con-una-segunda-cuenta-de-aws-de-la-empresa-la-segunda-cuenta-está-controlada-por-otro-ingeniero-qué-acción-podrá-realizar-el-ingeniero-de-la-segunda-cuenta) |
| 12 | [Una empresa está ampliando su flota de instancias de Amazon EC2 antes de un aumento esperado de tráfico. Cuando un ingeniero de CloudOps intenta agregar más instancias, se devuelve un error `InstanceLimitExceeded`. ¿Qué debe hacer el ingeniero de CloudOps para resolver este error?](#una-empresa-está-ampliando-su-flota-de-instancias-de-amazon-ec2-antes-de-un-aumento-esperado-de-tráfico-cuando-un-ingeniero-de-cloudops-intenta-agregar-más-instancias-se-devuelve-un-error-instancelimitexceeded-qué-debe-hacer-el-ingeniero-de-cloudops-para-resolver-este-error) |
| 13 | [Una empresa usa una cola estándar de Amazon Simple Queue Service (Amazon SQS) con su aplicación. La aplicación envía mensajes a la cola con cuerpos de mensaje únicos. La empresa decide cambiar a una cola SQS FIFO. ¿Qué debe hacer la empresa para migrar a una cola SQS FIFO?](#una-empresa-usa-una-cola-estándar-de-amazon-simple-queue-service-amazon-sqs-con-su-aplicación-la-aplicación-envía-mensajes-a-la-cola-con-cuerpos-de-mensaje-únicos-la-empresa-decide-cambiar-a-una-cola-sqs-fifo-qué-debe-hacer-la-empresa-para-migrar-a-una-cola-sqs-fifo) |
| 14 | [Un ingeniero de CloudOps creó una plantilla de AWS CloudFormation que aprovisiona instancias de Amazon EC2, un Elastic Load Balancer (ELB) y una instancia de base de datos de Amazon RDS. Durante la creación del stack, la creación de las instancias de EC2 y del ELB es exitosa. Sin embargo, la creación de la instancia de base de datos falla. ¿Cuál es el comportamiento predeterminado de CloudFormation en este escenario?](#un-ingeniero-de-cloudops-creó-una-plantilla-de-aws-cloudformation-que-aprovisiona-instancias-de-amazon-ec2-un-elastic-load-balancer-elb-y-una-instancia-de-base-de-datos-de-amazon-rds-durante-la-creación-del-stack-la-creación-de-las-instancias-de-ec2-y-del-elb-es-exitosa-sin-embargo-la-creación-de-la-instancia-de-base-de-datos-falla-cuál-es-el-comportamiento-predeterminado-de-cloudformation-en-este-escenario) |
| 15 | [Un ingeniero de CloudOps crea un clúster de Amazon Elastic Kubernetes Service (Amazon EKS) que usa AWS Fargate. El clúster se despliega con éxito. El ingeniero de CloudOps necesita administrar el clúster usando la herramienta de línea de comandos `kubectl`. ¿Cuál de los siguientes debe configurarse en la máquina del ingeniero de CloudOps para que `kubectl` pueda comunicarse con el servidor de la API del clúster?](#un-ingeniero-de-cloudops-crea-un-clúster-de-amazon-elastic-kubernetes-service-amazon-eks-que-usa-aws-fargate-el-clúster-se-despliega-con-éxito-el-ingeniero-de-cloudops-necesita-administrar-el-clúster-usando-la-herramienta-de-línea-de-comandos-kubectl-cuál-de-los-siguientes-debe-configurarse-en-la-máquina-del-ingeniero-de-cloudops-para-que-kubectl-pueda-comunicarse-con-el-servidor-de-la-api-del-clúster) |
| 16 | [Una empresa de desarrollo de software tiene varios desarrolladores que trabajan en el mismo producto. Cada desarrollador debe tener su propio entorno de desarrollo, y estos entornos de desarrollo deben ser idénticos. Cada entorno de desarrollo consiste en instancias de Amazon EC2 y una instancia de base de datos de Amazon RDS. Los entornos de desarrollo deben crearse solo cuando sea necesario y deben terminarse cada noche para minimizar costos. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#una-empresa-de-desarrollo-de-software-tiene-varios-desarrolladores-que-trabajan-en-el-mismo-producto-cada-desarrollador-debe-tener-su-propio-entorno-de-desarrollo-y-estos-entornos-de-desarrollo-deben-ser-idénticos-cada-entorno-de-desarrollo-consiste-en-instancias-de-amazon-ec2-y-una-instancia-de-base-de-datos-de-amazon-rds-los-entornos-de-desarrollo-deben-crearse-solo-cuando-sea-necesario-y-deben-terminarse-cada-noche-para-minimizar-costos-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 17 | [Una empresa adquirió recientemente otra corporación junto con todas las cuentas de AWS de esa corporación. Un analista financiero necesita los datos de costos de estas cuentas. Un ingeniero de CloudOps usa Cost Explorer para generar informes de costos y uso. El ingeniero de CloudOps observa que `No Tagkey` representa el `20%` del costo mensual. ¿Qué debe hacer el ingeniero de CloudOps para etiquetar los recursos de `No Tagkey`?](#una-empresa-adquirió-recientemente-otra-corporación-junto-con-todas-las-cuentas-de-aws-de-esa-corporación-un-analista-financiero-necesita-los-datos-de-costos-de-estas-cuentas-un-ingeniero-de-cloudops-usa-cost-explorer-para-generar-informes-de-costos-y-uso-el-ingeniero-de-cloudops-observa-que-no-tagkey-representa-el-20-del-costo-mensual-qué-debe-hacer-el-ingeniero-de-cloudops-para-etiquetar-los-recursos-de-no-tagkey) |
| 18 | [Un ingeniero de CloudOps está solucionando problemas de una plantilla de AWS CloudFormation mediante la cual se crean múltiples instancias de Amazon EC2. La plantilla funciona en `us-east-1`, pero falla en `us-west-2` con el código de error: `AMI [ami-12345678] does not exist`. ¿Cómo debe asegurarse el ingeniero de que la plantilla de AWS CloudFormation funcione en todas las regiones?](#un-ingeniero-de-cloudops-está-solucionando-problemas-de-una-plantilla-de-aws-cloudformation-mediante-la-cual-se-crean-múltiples-instancias-de-amazon-ec2-la-plantilla-funciona-en-us-east-1-pero-falla-en-us-west-2-con-el-código-de-error-ami-ami-12345678-does-not-exist-cómo-debe-asegurarse-el-ingeniero-de-que-la-plantilla-de-aws-cloudformation-funcione-en-todas-las-regiones) |
| 19 | [Un ingeniero de CloudOps desarrolló un script de Python que usa el AWS SDK para realizar varias tareas de mantenimiento. El script necesita ejecutarse automáticamente cada noche. ¿Cuál es la solución MÁS eficiente operativamente que cumple con este requisito?](#un-ingeniero-de-cloudops-desarrolló-un-script-de-python-que-usa-el-aws-sdk-para-realizar-varias-tareas-de-mantenimiento-el-script-necesita-ejecutarse-automáticamente-cada-noche-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-este-requisito) |
| 20 | [Una empresa usa plantillas de AWS CloudFormation para desplegar infraestructura en la nube. Un análisis de todas las plantillas de la empresa muestra que la empresa ha declarado los mismos componentes en múltiples plantillas. Un ingeniero de CloudOps necesita crear plantillas dedicadas que tengan sus propios parámetros y condiciones para estos componentes comunes. ¿Qué solución cumple con este requisito?](#una-empresa-usa-plantillas-de-aws-cloudformation-para-desplegar-infraestructura-en-la-nube-un-análisis-de-todas-las-plantillas-de-la-empresa-muestra-que-la-empresa-ha-declarado-los-mismos-componentes-en-múltiples-plantillas-un-ingeniero-de-cloudops-necesita-crear-plantillas-dedicadas-que-tengan-sus-propios-parámetros-y-condiciones-para-estos-componentes-comunes-qué-solución-cumple-con-este-requisito) |
| 21 | [Una auditoría reciente encontró que la mayoría de los recursos pertenecientes al equipo de desarrollo estaban en violación de los estándares de cumplimiento de parches. Los recursos estaban correctamente etiquetados. ¿Qué servicio se debe usar para remediar rápidamente el problema y devolver los recursos al cumplimiento?](#una-auditoría-reciente-encontró-que-la-mayoría-de-los-recursos-pertenecientes-al-equipo-de-desarrollo-estaban-en-violación-de-los-estándares-de-cumplimiento-de-parches-los-recursos-estaban-correctamente-etiquetados-qué-servicio-se-debe-usar-para-remediar-rápidamente-el-problema-y-devolver-los-recursos-al-cumplimiento) |
| 22 | [Un ingeniero de CloudOps tiene muchas instancias de Amazon EC2 con Windows que necesitan compartir un sistema de archivos entre nodos. El ingeniero de CloudOps crea un recurso compartido de archivos de Amazon Elastic File System (Amazon EFS). Después de crear el recurso compartido, el ingeniero de CloudOps tiene problemas para montarlo en las instancias de EC2. ¿Qué acción debe tomar el ingeniero de CloudOps para que las instancias de EC2 puedan compartir los archivos?](#un-ingeniero-de-cloudops-tiene-muchas-instancias-de-amazon-ec2-con-windows-que-necesitan-compartir-un-sistema-de-archivos-entre-nodos-el-ingeniero-de-cloudops-crea-un-recurso-compartido-de-archivos-de-amazon-elastic-file-system-amazon-efs-después-de-crear-el-recurso-compartido-el-ingeniero-de-cloudops-tiene-problemas-para-montarlo-en-las-instancias-de-ec2-qué-acción-debe-tomar-el-ingeniero-de-cloudops-para-que-las-instancias-de-ec2-puedan-compartir-los-archivos) |
| 23 | [Una empresa usa una plantilla de AWS CloudFormation para aprovisionar una instancia de Amazon EC2 y una instancia de base de datos de Amazon RDS. Un ingeniero de CloudOps debe actualizar la plantilla para asegurarse de que la instancia de base de datos se cree antes de que se lance la instancia de EC2. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?](#una-empresa-usa-una-plantilla-de-aws-cloudformation-para-aprovisionar-una-instancia-de-amazon-ec2-y-una-instancia-de-base-de-datos-de-amazon-rds-un-ingeniero-de-cloudops-debe-actualizar-la-plantilla-para-asegurarse-de-que-la-instancia-de-base-de-datos-se-cree-antes-de-que-se-lance-la-instancia-de-ec2-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-este-requisito) |
| 24 | [Una empresa usa AWS CloudFormation para desplegar la infraestructura de su aplicación. Recientemente, un usuario cambió accidentalmente una propiedad de una base de datos en una plantilla de CloudFormation y realizó una actualización del stack que causó una interrupción en la aplicación. Un ingeniero de CloudOps debe determinar cómo modificar el proceso de despliegue para permitir que el equipo de DevOps continúe desplegando la infraestructura, pero evitando modificaciones accidentales a recursos específicos. ¿Qué solución cumple con estos requisitos?](#una-empresa-usa-aws-cloudformation-para-desplegar-la-infraestructura-de-su-aplicación-recientemente-un-usuario-cambió-accidentalmente-una-propiedad-de-una-base-de-datos-en-una-plantilla-de-cloudformation-y-realizó-una-actualización-del-stack-que-causó-una-interrupción-en-la-aplicación-un-ingeniero-de-cloudops-debe-determinar-cómo-modificar-el-proceso-de-despliegue-para-permitir-que-el-equipo-de-devops-continúe-desplegando-la-infraestructura-pero-evitando-modificaciones-accidentales-a-recursos-específicos-qué-solución-cumple-con-estos-requisitos) |
| 25 | [Un ingeniero de CloudOps tiene una plantilla de AWS CloudFormation de la infraestructura existente de la empresa en `us-west-2`. El ingeniero intenta usar la plantilla para lanzar un nuevo stack en `eu-west-1`, pero el stack solo se despliega parcialmente, recibe un mensaje de error y luego se revierte (rollback). ¿Por qué fallaría esta plantilla al desplegarse? (Seleccione DOS.)](#un-ingeniero-de-cloudops-tiene-una-plantilla-de-aws-cloudformation-de-la-infraestructura-existente-de-la-empresa-en-us-west-2-el-ingeniero-intenta-usar-la-plantilla-para-lanzar-un-nuevo-stack-en-eu-west-1-pero-el-stack-solo-se-despliega-parcialmente-recibe-un-mensaje-de-error-y-luego-se-revierte-rollback-por-qué-fallaría-esta-plantilla-al-desplegarse-seleccione-dos) |
| 26 | [Una empresa usa AWS CloudFormation para desplegar su infraestructura. La empresa recientemente retiró una aplicación. Un ingeniero de operaciones en la nube inicia la eliminación de un stack de CloudFormation, y el stack queda atascado en estado `DELETE_FAILED`. Un ingeniero de CloudOps descubre que el stack había desplegado un grupo de seguridad. Ese grupo de seguridad es referenciado por otros grupos de seguridad en el entorno. El ingeniero de CloudOps necesita eliminar el stack sin afectar otras aplicaciones. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?](#una-empresa-usa-aws-cloudformation-para-desplegar-su-infraestructura-la-empresa-recientemente-retiró-una-aplicación-un-ingeniero-de-operaciones-en-la-nube-inicia-la-eliminación-de-un-stack-de-cloudformation-y-el-stack-queda-atascado-en-estado-delete_failed-un-ingeniero-de-cloudops-descubre-que-el-stack-había-desplegado-un-grupo-de-seguridad-ese-grupo-de-seguridad-es-referenciado-por-otros-grupos-de-seguridad-en-el-entorno-el-ingeniero-de-cloudops-necesita-eliminar-el-stack-sin-afectar-otras-aplicaciones-qué-solución-cumple-con-estos-requisitos-de-la-manera-más-eficiente-operativamente) |
| 27 | [Un ingeniero de CloudOps crea una plantilla de AWS CloudFormation para definir una pila de aplicación que puede desplegarse en múltiples regiones de AWS. El ingeniero de CloudOps también crea un dashboard de Amazon CloudWatch usando la consola de administración de AWS. Cada despliegue de la aplicación requiere su propio dashboard de CloudWatch. ¿Cómo puede el ingeniero de CloudOps automatizar la creación del dashboard de CloudWatch cada vez que se despliega la aplicación?](#un-ingeniero-de-cloudops-crea-una-plantilla-de-aws-cloudformation-para-definir-una-pila-de-aplicación-que-puede-desplegarse-en-múltiples-regiones-de-aws-el-ingeniero-de-cloudops-también-crea-un-dashboard-de-amazon-cloudwatch-usando-la-consola-de-administración-de-aws-cada-despliegue-de-la-aplicación-requiere-su-propio-dashboard-de-cloudwatch-cómo-puede-el-ingeniero-de-cloudops-automatizar-la-creación-del-dashboard-de-cloudwatch-cada-vez-que-se-despliega-la-aplicación) |
| 28 | [Un ingeniero de CloudOps ha desplegado con éxito una `VPC` con una plantilla de AWS CloudFormation. El ingeniero de CloudOps quiere desplegar la misma plantilla en múltiples cuentas administradas a través de AWS Organizations. ¿Qué solución cumple con este requisito con el MENOR esfuerzo operativo?](#un-ingeniero-de-cloudops-ha-desplegado-con-éxito-una-vpc-con-una-plantilla-de-aws-cloudformation-el-ingeniero-de-cloudops-quiere-desplegar-la-misma-plantilla-en-múltiples-cuentas-administradas-a-través-de-aws-organizations-qué-solución-cumple-con-este-requisito-con-el-menor-esfuerzo-operativo) |
| 29 | [Un ingeniero de CloudOps es responsable de administrar la infraestructura en la nube de una empresa con AWS CloudFormation. El ingeniero de CloudOps necesita crear un único recurso que consista en múltiples servicios de AWS. El recurso debe admitir su creación y eliminación a través de la consola de CloudFormation. ¿Qué tipo de recurso de CloudFormation debe crear el ingeniero de CloudOps para cumplir con estos requisitos?](#un-ingeniero-de-cloudops-es-responsable-de-administrar-la-infraestructura-en-la-nube-de-una-empresa-con-aws-cloudformation-el-ingeniero-de-cloudops-necesita-crear-un-único-recurso-que-consista-en-múltiples-servicios-de-aws-el-recurso-debe-admitir-su-creación-y-eliminación-a-través-de-la-consola-de-cloudformation-qué-tipo-de-recurso-de-cloudformation-debe-crear-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos) |
| 30 | [Un ingeniero de CloudOps está usando `StackSets` de AWS CloudFormation para crear recursos de AWS en dos regiones de AWS dentro de la misma cuenta de AWS. Una operación de stack falla en una región y devuelve el estado de instancia de stack `OUTDATED`. ¿Cuál es la causa de esta falla?](#un-ingeniero-de-cloudops-está-usando-stacksets-de-aws-cloudformation-para-crear-recursos-de-aws-en-dos-regiones-de-aws-dentro-de-la-misma-cuenta-de-aws-una-operación-de-stack-falla-en-una-región-y-devuelve-el-estado-de-instancia-de-stack-outdated-cuál-es-la-causa-de-esta-falla) |
| 31 | [A un ingeniero de CloudOps se le asigna la tarea de desplegar la infraestructura de una empresa como código. El ingeniero de CloudOps quiere escribir una única plantilla que pueda reutilizarse para múltiples entornos. ¿Cómo debe el ingeniero de CloudOps usar AWS CloudFormation para crear una solución?](#a-un-ingeniero-de-cloudops-se-le-asigna-la-tarea-de-desplegar-la-infraestructura-de-una-empresa-como-código-el-ingeniero-de-cloudops-quiere-escribir-una-única-plantilla-que-pueda-reutilizarse-para-múltiples-entornos-cómo-debe-el-ingeniero-de-cloudops-usar-aws-cloudformation-para-crear-una-solución) |
| 32 | [Un ingeniero de CloudOps está intentando desplegar recursos usando una plantilla de AWS CloudFormation. Una instancia de Amazon EC2 que está definida en la plantilla no logra iniciarse y produce un error `InsufficientInstanceCapacity`. ¿Qué acciones debe tomar el ingeniero de CloudOps para resolver este error? (Elija dos.)](#un-ingeniero-de-cloudops-está-intentando-desplegar-recursos-usando-una-plantilla-de-aws-cloudformation-una-instancia-de-amazon-ec2-que-está-definida-en-la-plantilla-no-logra-iniciarse-y-produce-un-error-insufficientinstancecapacity-qué-acciones-debe-tomar-el-ingeniero-de-cloudops-para-resolver-este-error-elija-dos) |
| 33 | [Un ingeniero de CloudOps está examinando la siguiente plantilla de AWS CloudFormation. ¿Por qué fallará la creación del stack?](#un-ingeniero-de-cloudops-está-examinando-la-siguiente-plantilla-de-aws-cloudformation-por-qué-fallará-la-creación-del-stack) |
| 34 | [Una empresa usa un portafolio de AWS Service Catalog para crear y administrar recursos. Un ingeniero de CloudOps debe crear una réplica de la infraestructura de AWS existente de la empresa en una nueva cuenta de AWS. ¿Cuál es la forma MÁS eficiente operativamente de cumplir con este requisito?](#una-empresa-usa-un-portafolio-de-aws-service-catalog-para-crear-y-administrar-recursos-un-ingeniero-de-cloudops-debe-crear-una-réplica-de-la-infraestructura-de-aws-existente-de-la-empresa-en-una-nueva-cuenta-de-aws-cuál-es-la-forma-más-eficiente-operativamente-de-cumplir-con-este-requisito) |
| 35 | [Un ingeniero de CloudOps ha usado AWS CloudFormation para desplegar una aplicación sin servidor (serverless) en una `VPC` de producción. La aplicación consiste en una función de AWS Lambda, una tabla de Amazon DynamoDB y una API de Amazon API Gateway. El ingeniero de CloudOps debe eliminar el stack de AWS CloudFormation sin eliminar la tabla de DynamoDB. ¿Qué acción debe tomar el ingeniero de CloudOps antes de eliminar el stack de AWS CloudFormation?](#un-ingeniero-de-cloudops-ha-usado-aws-cloudformation-para-desplegar-una-aplicación-sin-servidor-serverless-en-una-vpc-de-producción-la-aplicación-consiste-en-una-función-de-aws-lambda-una-tabla-de-amazon-dynamodb-y-una-api-de-amazon-api-gateway-el-ingeniero-de-cloudops-debe-eliminar-el-stack-de-aws-cloudformation-sin-eliminar-la-tabla-de-dynamodb-qué-acción-debe-tomar-el-ingeniero-de-cloudops-antes-de-eliminar-el-stack-de-aws-cloudformation) |
| 36 | [Un ingeniero de CloudOps debe idear una estrategia para hacer cumplir el etiquetado de todas las instancias de EC2 y volúmenes de Amazon Elastic Block Store (Amazon EBS). ¿Qué acción puede tomar el ingeniero para implementar esto en tiempo real?](#un-ingeniero-de-cloudops-debe-idear-una-estrategia-para-hacer-cumplir-el-etiquetado-de-todas-las-instancias-de-ec2-y-volúmenes-de-amazon-elastic-block-store-amazon-ebs-qué-acción-puede-tomar-el-ingeniero-para-implementar-esto-en-tiempo-real) |
| 37 | [Una empresa global opera desde cinco regiones de AWS. Un ingeniero de CloudOps quiere identificar todas las instancias de Amazon EC2 de la empresa, tanto etiquetadas como sin etiquetar. La empresa requiere que la salida muestre el ID de instancia y las etiquetas. ¿Cuál es la forma MÁS eficiente operativamente para que el ingeniero de CloudOps cumpla con estos requisitos?](#una-empresa-global-opera-desde-cinco-regiones-de-aws-un-ingeniero-de-cloudops-quiere-identificar-todas-las-instancias-de-amazon-ec2-de-la-empresa-tanto-etiquetadas-como-sin-etiquetar-la-empresa-requiere-que-la-salida-muestre-el-id-de-instancia-y-las-etiquetas-cuál-es-la-forma-más-eficiente-operativamente-para-que-el-ingeniero-de-cloudops-cumpla-con-estos-requisitos) |
| 38 | [Un ingeniero de CloudOps necesita eliminar un stack de AWS CloudFormation que ya no está en uso. El stack de CloudFormation está en el estado `DELETE_FAILED`. El ingeniero de CloudOps ha validado los permisos requeridos para eliminar el stack de CloudFormation. ¿Cuáles de las siguientes son posibles causas del estado `DELETE_FAILED`? (Elija dos.)](#un-ingeniero-de-cloudops-necesita-eliminar-un-stack-de-aws-cloudformation-que-ya-no-está-en-uso-el-stack-de-cloudformation-está-en-el-estado-delete_failed-el-ingeniero-de-cloudops-ha-validado-los-permisos-requeridos-para-eliminar-el-stack-de-cloudformation-cuáles-de-las-siguientes-son-posibles-causas-del-estado-delete_failed-elija-dos) |
| 39 | [Una empresa ha desplegado una aplicación en AWS. La aplicación se ejecuta en una flota de instancias de Amazon EC2 Linux que están en un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para usar plantillas de lanzamiento (launch templates). Las plantillas de lanzamiento lanzan instancias de EC2 respaldadas por Amazon Elastic Block Store (Amazon EBS) que usan volúmenes EBS `General Purpose SSD (gp3)` para almacenamiento primario. Un ingeniero de CloudOps necesita implementar una solución para asegurar que todas las instancias de EC2 puedan compartir los mismos archivos subyacentes. La solución también debe asegurar que los datos sean consistentes. ¿Qué solución cumple con estos requisitos?](#una-empresa-ha-desplegado-una-aplicación-en-aws-la-aplicación-se-ejecuta-en-una-flota-de-instancias-de-amazon-ec2-linux-que-están-en-un-grupo-de-auto-scaling-el-grupo-de-auto-scaling-está-configurado-para-usar-plantillas-de-lanzamiento-launch-templates-las-plantillas-de-lanzamiento-lanzan-instancias-de-ec2-respaldadas-por-amazon-elastic-block-store-amazon-ebs-que-usan-volúmenes-ebs-general-purpose-ssd-gp3-para-almacenamiento-primario-un-ingeniero-de-cloudops-necesita-implementar-una-solución-para-asegurar-que-todas-las-instancias-de-ec2-puedan-compartir-los-mismos-archivos-subyacentes-la-solución-también-debe-asegurar-que-los-datos-sean-consistentes-qué-solución-cumple-con-estos-requisitos) |
| 40 | [Una aplicación que se ejecuta en instancias de Amazon EC2 en un grupo de Auto Scaling en múltiples Zonas de disponibilidad se desplegó usando una plantilla de AWS CloudFormation. El equipo de SysOps ha parcheado la versión de la Amazon Machine Image (AMI) y debe actualizar todas las instancias de EC2 para usar la nueva AMI. ¿Cómo puede el ingeniero de CloudOps usar CloudFormation para aplicar la nueva AMI mientras mantiene un nivel mínimo de instancias activas para garantizar la continuidad del servicio?](#una-aplicación-que-se-ejecuta-en-instancias-de-amazon-ec2-en-un-grupo-de-auto-scaling-en-múltiples-zonas-de-disponibilidad-se-desplegó-usando-una-plantilla-de-aws-cloudformation-el-equipo-de-sysops-ha-parcheado-la-versión-de-la-amazon-machine-image-ami-y-debe-actualizar-todas-las-instancias-de-ec2-para-usar-la-nueva-ami-cómo-puede-el-ingeniero-de-cloudops-usar-cloudformation-para-aplicar-la-nueva-ami-mientras-mantiene-un-nivel-mínimo-de-instancias-activas-para-garantizar-la-continuidad-del-servicio) |
| 41 | [Un ingeniero de CloudOps quiere usar AWS Systems Manager Patch Manager para automatizar el proceso de aplicar parches a instancias de Amazon EC2 Windows. El ingeniero de CloudOps quiere asegurarse de que los parches se aprueben automáticamente 2 días después de la fecha de lanzamiento para las instancias de desarrollo. Los parches también deben aprobarse automáticamente 5 días después de la fecha de lanzamiento para las instancias de producción. El mantenimiento debe ocurrir solo durante una ventana de 2 horas para todas las instancias. ¿Qué solución cumple con estos requisitos?](#un-ingeniero-de-cloudops-quiere-usar-aws-systems-manager-patch-manager-para-automatizar-el-proceso-de-aplicar-parches-a-instancias-de-amazon-ec2-windows-el-ingeniero-de-cloudops-quiere-asegurarse-de-que-los-parches-se-aprueben-automáticamente-2-días-después-de-la-fecha-de-lanzamiento-para-las-instancias-de-desarrollo-los-parches-también-deben-aprobarse-automáticamente-5-días-después-de-la-fecha-de-lanzamiento-para-las-instancias-de-producción-el-mantenimiento-debe-ocurrir-solo-durante-una-ventana-de-2-horas-para-todas-las-instancias-qué-solución-cumple-con-estos-requisitos) |
| 42 | [Un ingeniero de CloudOps es responsable de más de `50` instancias de Amazon EC2 desplegadas en una única cuenta de AWS de producción. Las instancias de EC2 ejecutan varios sistemas operativos diferentes. Los estándares de la empresa requieren que el parchado se complete al menos una vez al mes. El ingeniero de CloudOps quiere usar AWS Systems Manager para reducir el número de horas que la empresa dedica al parchado del sistema operativo cada mes. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija tres.)](#un-ingeniero-de-cloudops-es-responsable-de-más-de-50-instancias-de-amazon-ec2-desplegadas-en-una-única-cuenta-de-aws-de-producción-las-instancias-de-ec2-ejecutan-varios-sistemas-operativos-diferentes-los-estándares-de-la-empresa-requieren-que-el-parchado-se-complete-al-menos-una-vez-al-mes-el-ingeniero-de-cloudops-quiere-usar-aws-systems-manager-para-reducir-el-número-de-horas-que-la-empresa-dedica-al-parchado-del-sistema-operativo-cada-mes-qué-combinación-de-pasos-debe-tomar-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-elija-tres) |
| 43 | [Una organización está ejecutando múltiples aplicaciones para sus clientes. Cada aplicación se despliega ejecutando una plantilla base de AWS CloudFormation que configura una nueva `VPC`. Todas las aplicaciones se ejecutan en la misma cuenta de AWS y región de AWS. Un ingeniero de CloudOps ha notado que al intentar desplegar el mismo stack de AWS CloudFormation, este falla al desplegarse. ¿Cuál es probablemente el problema?](#una-organización-está-ejecutando-múltiples-aplicaciones-para-sus-clientes-cada-aplicación-se-despliega-ejecutando-una-plantilla-base-de-aws-cloudformation-que-configura-una-nueva-vpc-todas-las-aplicaciones-se-ejecutan-en-la-misma-cuenta-de-aws-y-región-de-aws-un-ingeniero-de-cloudops-ha-notado-que-al-intentar-desplegar-el-mismo-stack-de-aws-cloudformation-este-falla-al-desplegarse-cuál-es-probablemente-el-problema) |
| 44 | [Se le ha encomendado a un ingeniero de CloudOps desplegar la infraestructura de una empresa como código. El ingeniero quiere escribir una única plantilla que pueda reutilizarse para múltiples entornos de una manera segura y repetible. ¿Cuál es la forma recomendada de usar AWS CloudFormation para cumplir con este requisito?](#se-le-ha-encomendado-a-un-ingeniero-de-cloudops-desplegar-la-infraestructura-de-una-empresa-como-código-el-ingeniero-quiere-escribir-una-única-plantilla-que-pueda-reutilizarse-para-múltiples-entornos-de-una-manera-segura-y-repetible-cuál-es-la-forma-recomendada-de-usar-aws-cloudformation-para-cumplir-con-este-requisito) |
| 45 | [Un ingeniero de CloudOps está creando recursos a partir de una plantilla de AWS CloudFormation que define un grupo de Auto Scaling de instancias de Amazon EC2. La plantilla de lanzamiento del grupo de Auto Scaling aprovisiona cada instancia de EC2 usando un script de datos de usuario. La creación del recurso de grupo de Auto Scaling está fallando debido a un error. La condición de espera (wait condition) no está recibiendo el número requerido de señales. ¿Cómo debe el ingeniero de CloudOps resolver este error?](#un-ingeniero-de-cloudops-está-creando-recursos-a-partir-de-una-plantilla-de-aws-cloudformation-que-define-un-grupo-de-auto-scaling-de-instancias-de-amazon-ec2-la-plantilla-de-lanzamiento-del-grupo-de-auto-scaling-aprovisiona-cada-instancia-de-ec2-usando-un-script-de-datos-de-usuario-la-creación-del-recurso-de-grupo-de-auto-scaling-está-fallando-debido-a-un-error-la-condición-de-espera-wait-condition-no-está-recibiendo-el-número-requerido-de-señales-cómo-debe-el-ingeniero-de-cloudops-resolver-este-error) |
| 46 | [Un ingeniero de CloudOps necesita crear una réplica de la infraestructura de AWS existente de una empresa en una nueva cuenta de AWS. Actualmente, se usa un portafolio de AWS Service Catalog para crear y administrar recursos. ¿Cuál es la forma MÁS eficiente de lograr esto?](#un-ingeniero-de-cloudops-necesita-crear-una-réplica-de-la-infraestructura-de-aws-existente-de-una-empresa-en-una-nueva-cuenta-de-aws-actualmente-se-usa-un-portafolio-de-aws-service-catalog-para-crear-y-administrar-recursos-cuál-es-la-forma-más-eficiente-de-lograr-esto) |
| 47 | [El ingeniero de CloudOps de una empresa administra una flota de cientos de instancias de Amazon EC2 que ejecutan cargas de trabajo basadas en Windows y cargas de trabajo basadas en Linux. Cada instancia de EC2 tiene una etiqueta que identifica su sistema operativo. Todas las instancias de EC2 ejecutan AWS Systems Manager Session Manager. Se reporta una vulnerabilidad de día cero, y no hay parches disponibles. El equipo de seguridad de la empresa proporciona código para todos los sistemas operativos relevantes para reducir el riesgo de la vulnerabilidad. El ingeniero de CloudOps necesita implementar el código en las instancias de EC2 y debe proporcionar un informe que muestre que el código se ejecutó exitosamente en todas las instancias. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos lo más rápido posible?](#el-ingeniero-de-cloudops-de-una-empresa-administra-una-flota-de-cientos-de-instancias-de-amazon-ec2-que-ejecutan-cargas-de-trabajo-basadas-en-windows-y-cargas-de-trabajo-basadas-en-linux-cada-instancia-de-ec2-tiene-una-etiqueta-que-identifica-su-sistema-operativo-todas-las-instancias-de-ec2-ejecutan-aws-systems-manager-session-manager-se-reporta-una-vulnerabilidad-de-día-cero-y-no-hay-parches-disponibles-el-equipo-de-seguridad-de-la-empresa-proporciona-código-para-todos-los-sistemas-operativos-relevantes-para-reducir-el-riesgo-de-la-vulnerabilidad-el-ingeniero-de-cloudops-necesita-implementar-el-código-en-las-instancias-de-ec2-y-debe-proporcionar-un-informe-que-muestre-que-el-código-se-ejecutó-exitosamente-en-todas-las-instancias-qué-debe-hacer-el-ingeniero-de-cloudops-para-cumplir-con-estos-requisitos-lo-más-rápido-posible) |
| 48 | [Una empresa ha desarrollado un servicio que se despliega en una flota de instancias de Amazon EC2 basadas en Linux que están en un grupo de Auto Scaling. El servicio falla ocasionalmente de manera inesperada debido a un error en el código de la aplicación. El equipo de ingeniería de la empresa determina que resolver la causa subyacente de la falla del servicio podría tomar varias semanas. Un ingeniero de CloudOps necesita crear una solución para automatizar la recuperación si el servicio falla en cualquiera de las instancias de EC2. ¿Qué soluciones cumplen con este requisito? (Elija dos.)](#una-empresa-ha-desarrollado-un-servicio-que-se-despliega-en-una-flota-de-instancias-de-amazon-ec2-basadas-en-linux-que-están-en-un-grupo-de-auto-scaling-el-servicio-falla-ocasionalmente-de-manera-inesperada-debido-a-un-error-en-el-código-de-la-aplicación-el-equipo-de-ingeniería-de-la-empresa-determina-que-resolver-la-causa-subyacente-de-la-falla-del-servicio-podría-tomar-varias-semanas-un-ingeniero-de-cloudops-necesita-crear-una-solución-para-automatizar-la-recuperación-si-el-servicio-falla-en-cualquiera-de-las-instancias-de-ec2-qué-soluciones-cumplen-con-este-requisito-elija-dos) |
| 49 | [Un ingeniero de CloudOps necesita automatizar la invocación de una función de AWS Lambda. La función Lambda debe ejecutarse al final de cada día para generar un informe sobre datos almacenados en un bucket de Amazon S3. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?](#un-ingeniero-de-cloudops-necesita-automatizar-la-invocación-de-una-función-de-aws-lambda-la-función-lambda-debe-ejecutarse-al-final-de-cada-día-para-generar-un-informe-sobre-datos-almacenados-en-un-bucket-de-amazon-s3-cuál-es-la-solución-más-eficiente-operativamente-que-cumple-con-estos-requisitos) |
| 50 | [La infraestructura de la aplicación de una empresa se desplegó usando AWS CloudFormation y consiste en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias se ejecutan en un grupo de EC2 Auto Scaling en múltiples Zonas de disponibilidad. Al lanzar una nueva versión de la aplicación, el despliegue de actualización debe evitar cambios de `DNS` y permitir reversión (rollback). ¿Qué solución debe usar un ingeniero de CloudOps para cumplir con los requisitos de despliegue de este nuevo lanzamiento?](#la-infraestructura-de-la-aplicación-de-una-empresa-se-desplegó-usando-aws-cloudformation-y-consiste-en-instancias-de-amazon-ec2-detrás-de-un-application-load-balancer-las-instancias-se-ejecutan-en-un-grupo-de-ec2-auto-scaling-en-múltiples-zonas-de-disponibilidad-al-lanzar-una-nueva-versión-de-la-aplicación-el-despliegue-de-actualización-debe-evitar-cambios-de-dns-y-permitir-reversión-rollback-qué-solución-debe-usar-un-ingeniero-de-cloudops-para-cumplir-con-los-requisitos-de-despliegue-de-este-nuevo-lanzamiento) |
| 51 | [Una empresa usa un bucket de Amazon S3 para almacenar archivos de datos. El bucket de S3 contiene cientos de objetos. La empresa necesita reemplazar una etiqueta en todos los objetos del bucket de S3 por otra etiqueta. ¿Cuál es la forma MÁS eficiente operativamente de cumplir con este requisito?](#una-empresa-usa-un-bucket-de-amazon-s3-para-almacenar-archivos-de-datos-el-bucket-de-s3-contiene-cientos-de-objetos-la-empresa-necesita-reemplazar-una-etiqueta-en-todos-los-objetos-del-bucket-de-s3-por-otra-etiqueta-cuál-es-la-forma-más-eficiente-operativamente-de-cumplir-con-este-requisito) |
| 52 | [Un equipo de aplicaciones le ha pedido a un ingeniero de CloudOps que aprovisione un entorno adicional para una aplicación en cuatro regiones adicionales. La aplicación se ejecuta en más de 100 instancias en `us-east-1`, usando AMI completamente preparadas (fully baked). Se ha creado una plantilla de AWS CloudFormation para desplegar recursos en `us-east-1`. ¿Qué debe hacer el ingeniero de CloudOps para aprovisionar la aplicación rápidamente?](#un-equipo-de-aplicaciones-le-ha-pedido-a-un-ingeniero-de-cloudops-que-aprovisione-un-entorno-adicional-para-una-aplicación-en-cuatro-regiones-adicionales-la-aplicación-se-ejecuta-en-más-de-100-instancias-en-us-east-1-usando-ami-completamente-preparadas-fully-baked-se-ha-creado-una-plantilla-de-aws-cloudformation-para-desplegar-recursos-en-us-east-1-qué-debe-hacer-el-ingeniero-de-cloudops-para-aprovisionar-la-aplicación-rápidamente) |
| 53 | [Una empresa planea expandirse a una región adicional de AWS con fines de recuperación ante desastres. La empresa usa AWS CloudFormation, y su infraestructura está bien definida como código. La empresa quisiera reutilizar la mayor cantidad posible de su código existente al desplegar recursos en regiones adicionales. Un ingeniero de CloudOps está revisando cómo se seleccionan las Amazon Machine Images (AMI) en AWS CloudFormation, pero tiene problemas para hacer que el mismo stack funcione en la nueva región. ¿Qué acción facilitaría la administración de múltiples regiones?](#una-empresa-planea-expandirse-a-una-región-adicional-de-aws-con-fines-de-recuperación-ante-desastres-la-empresa-usa-aws-cloudformation-y-su-infraestructura-está-bien-definida-como-código-la-empresa-quisiera-reutilizar-la-mayor-cantidad-posible-de-su-código-existente-al-desplegar-recursos-en-regiones-adicionales-un-ingeniero-de-cloudops-está-revisando-cómo-se-seleccionan-las-amazon-machine-images-ami-en-aws-cloudformation-pero-tiene-problemas-para-hacer-que-el-mismo-stack-funcione-en-la-nueva-región-qué-acción-facilitaría-la-administración-de-múltiples-regiones) |
| 54 | [Un ingeniero de CloudOps está administrando una cuenta de AWS donde los desarrolladores están autorizados a lanzar instancias de Amazon EC2 para probar código nuevo. Para limitar los costos, el ingeniero debe asegurarse de que las instancias de EC2 en la cuenta se terminen 24 horas después del lanzamiento. ¿Cómo debe el ingeniero cumplir con estos requisitos?](#un-ingeniero-de-cloudops-está-administrando-una-cuenta-de-aws-donde-los-desarrolladores-están-autorizados-a-lanzar-instancias-de-amazon-ec2-para-probar-código-nuevo-para-limitar-los-costos-el-ingeniero-debe-asegurarse-de-que-las-instancias-de-ec2-en-la-cuenta-se-terminen-24-horas-después-del-lanzamiento-cómo-debe-el-ingeniero-cumplir-con-estos-requisitos) |
| 55 | [El ingeniero de CloudOps de una empresa administra una flota de instancias de Amazon EC2 Windows que se ejecutan en una única cuenta de AWS. Las instancias tienen una etiqueta que incluye una clave `OS` y un valor `Windows`. La empresa usa AWS Systems Manager para parchar las instancias. La empresa ha instalado el agente de Amazon CloudWatch en las instancias, pero la configuración es inconsistente. El ingeniero de CloudOps necesita reconfigurar cada instancia para usar la misma configuración predefinida de CloudWatch. ¿Qué combinación de pasos cumple con estos requisitos? (Elija dos.)](#el-ingeniero-de-cloudops-de-una-empresa-administra-una-flota-de-instancias-de-amazon-ec2-windows-que-se-ejecutan-en-una-única-cuenta-de-aws-las-instancias-tienen-una-etiqueta-que-incluye-una-clave-os-y-un-valor-windows-la-empresa-usa-aws-systems-manager-para-parchar-las-instancias-la-empresa-ha-instalado-el-agente-de-amazon-cloudwatch-en-las-instancias-pero-la-configuración-es-inconsistente-el-ingeniero-de-cloudops-necesita-reconfigurar-cada-instancia-para-usar-la-misma-configuración-predefinida-de-cloudwatch-qué-combinación-de-pasos-cumple-con-estos-requisitos-elija-dos) |

### Una empresa administra muchas cuentas mediante una única organización en AWS Organizations. La organización tiene todas las funciones habilitadas. La empresa quiere activar AWS Config en todas las cuentas de la organización y en todas las regiones de AWS. ¿Qué debe hacer un ingeniero de CloudOps para cumplir con estos requisitos de la manera MÁS eficiente operativamente?

- [x] Usar `StackSets` de AWS CloudFormation para implementar instancias de stack que activen AWS Config en todas las cuentas y en todas las regiones.
- [ ] Usar `StackSets` de AWS CloudFormation para implementar políticas de stack que activen AWS Config en todas las cuentas y en todas las regiones.
- [ ] Usar Políticas de Control de Servicio (SCP) para configurar AWS Config en todas las cuentas y en todas las regiones.
- [ ] Crear un script que use la AWS CLI para activar AWS Config en todas las cuentas de la organización. Ejecutar el script desde la cuenta de administración de la organización.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El ingeniero de CloudOps de una empresa implementa cuatro nuevas instancias de Amazon EC2 utilizando la Amazon Machine Image (AMI) estándar de Amazon Linux 2. La empresa necesita poder usar AWS Systems Manager para administrar las instancias. El ingeniero de CloudOps observa que las instancias no aparecen en la consola de Systems Manager. ¿Qué debe hacer el ingeniero de CloudOps para resolver este problema?

- [ ] Conectarse a cada instancia mediante `SSH`. Instalar el Systems Manager Agent en cada instancia. Configurar el Systems Manager Agent para que se inicie automáticamente cuando las instancias arranquen.
- [ ] Usar AWS Certificate Manager (ACM) para crear un certificado TLS. Importar el certificado a cada instancia. Configurar el Systems Manager Agent para que use el certificado TLS en las comunicaciones seguras.
- [ ] Conectarse a cada instancia mediante `SSH`. Crear una cuenta `ssm-user`. Agregar la cuenta `ssm-user` al directorio `/etcsudoers`.
- [x] Adjuntar un perfil de instancia de IAM a las instancias. Asegurarse de que el perfil de instancia contenga la política `AmazonSSMManagedinstanceCore`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps quiere cargar un archivo de 1 TB de tamaño desde un entorno on-premises a un bucket de Amazon S3 usando cargas multiparte (multipart uploads). ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Cargar el archivo usando la consola de S3.
- [ ] Usar el comando `s3api copy-object`.
- [ ] Usar el comando `s3api put-object`.
- [x] Usar el comando `s3 cp`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps quiere administrar una aplicación de servidor web con AWS Elastic Beanstalk. El servicio de Elastic Beanstalk debe mantener siempre la capacidad completa durante las nuevas implementaciones. ¿Qué políticas de despliegue satisfacen este requisito? (Seleccione DOS.)

- [ ] Todo a la vez (All at once).
- [x] Inmutable (Immutable).
- [ ] Reconstrucción (Rebuild).
- [ ] Continuo (Rolling).
- [x] Continuo con lote adicional (Rolling with additional batch).

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa crea imágenes AMI personalizadas lanzando nuevas instancias de Amazon EC2 desde una plantilla de AWS CloudFormation; instala y configura el software necesario mediante AWS OpsWorks y luego toma imágenes de cada instancia de EC2. El proceso de instalación y configuración del software puede tardar entre 2 y 3 horas, pero a veces el proceso se detiene por errores de instalación. El ingeniero de CloudOps debe modificar la plantilla de CloudFormation para que, si el proceso se detiene, todo el stack falle y se revierta (rollback). Con base en estos requisitos, ¿qué se debe agregar a la plantilla?

- [ ] `Conditions` con un tiempo de espera (timeout) configurado en 4 horas.
- [x] `CreationPolicy` con un tiempo de espera configurado en 4 horas.
- [ ] `DependsOn` con un tiempo de espera configurado en 4 horas.
- [ ] `Metadata` con un tiempo de espera configurado en 4 horas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps aplica la siguiente política a un stack de AWS CloudFormation. ¿Cuál es el resultado de esta política?

![Question 35](images/question35.jpg)

- [ ] Los usuarios que asuman un rol de IAM con un ID lógico que comience con `Production` no podrán ejecutar el comando `update-stack`.
- [x] Los usuarios pueden actualizar todos los recursos del stack, excepto los recursos cuyo ID lógico comience con `Production`.
- [ ] Los usuarios pueden actualizar todos los recursos del stack, excepto los recursos cuyo atributo comience con `Production`.
- [ ] Los usuarios de un grupo de IAM con un ID lógico que comience con `Production` no podrán ejecutar el comando `update-stack`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ejecuta un sitio web en instancias de Amazon EC2 dentro de un grupo de Auto Scaling. Cuando aumenta el tráfico del sitio web, las instancias adicionales tardan varios minutos en estar disponibles debido a un script de datos de usuario (user data) de larga duración que instala software. Un ingeniero de CloudOps debe reducir el tiempo necesario para que las nuevas instancias estén disponibles. ¿Qué acción debe tomar el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Reducir los umbrales de escalado para que las instancias se agreguen antes de que aumente el tráfico.
- [ ] Comprar Instancias Reservadas para cubrir el `100%` de la capacidad máxima del grupo de Auto Scaling.
- [ ] Actualizar el grupo de Auto Scaling para lanzar instancias de un tipo optimizado para almacenamiento.
- [x] Usar EC2 Image Builder para preparar una Amazon Machine Image (AMI) con el software preinstalado.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa AWS Organizations. Un ingeniero de CloudOps quiere usar AWS Compute Optimizer y políticas de etiquetas (tag policies) de AWS en la cuenta de administración para gobernar todas las cuentas miembro de la familia de facturación. El ingeniero de CloudOps navega a la consola de AWS Organizations pero no puede activar las políticas de etiquetas desde la cuenta de administración. ¿Cuál podría ser la razón de este problema?

- [x] No se han habilitado todas las funciones (all features) en la organización.
- [ ] No se ha habilitado la facturación consolidada.
- [ ] Las cuentas miembro no tienen etiquetas habilitadas para la asignación de costos.
- [ ] Las cuentas miembro no han habilitado manualmente el acceso de confianza (trusted access) para Compute Optimizer.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está ampliando su uso de servicios de AWS en toda su cartera. La empresa quiere aprovisionar cuentas de AWS para cada equipo, con el fin de garantizar la separación de los procesos de negocio por motivos de cumplimiento de seguridad y facturación. La creación y configuración inicial (bootstrapping) de las cuentas debe realizarse de forma escalable y eficiente, de modo que las nuevas cuentas se creen con una línea base definida y con barreras de gobernanza (guardrails) implementadas. Un ingeniero de CloudOps necesita diseñar un proceso de aprovisionamiento que ahorre tiempo y recursos. ¿Qué acción se debe tomar para cumplir con estos requisitos?

- [ ] Automatizar usando AWS Elastic Beanstalk para aprovisionar las cuentas de AWS, configurar la infraestructura e integrarse con AWS Organizations.
- [ ] Crear scripts de configuración inicial (bootstrapping) en AWS OpsWorks y combinarlos con plantillas de AWS CloudFormation para aprovisionar cuentas e infraestructura.
- [ ] Usar AWS Config para aprovisionar cuentas y desplegar instancias usando AWS Service Catalog.
- [x] Usar AWS Control Tower para crear una plantilla en Account Factory y usar la plantilla para aprovisionar nuevas cuentas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está usando AWS Systems Manager Patch Manager para aplicar parches a una flota de instancias de Amazon EC2. El ingeniero de CloudOps ha configurado una línea base de parches (patch baseline) y una ventana de mantenimiento. El ingeniero de CloudOps también ha usado una etiqueta de instancia para identificar cuáles instancias parchear. El ingeniero de CloudOps debe darle a Systems Manager la capacidad de acceder a las instancias de EC2. ¿Qué acción adicional debe realizar el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Agregar una regla de entrada al grupo de seguridad de las instancias.
- [x] Adjuntar un perfil de instancia de IAM con acceso a Systems Manager a las instancias.
- [ ] Crear una activación de Systems Manager y luego activar la flota de instancias.
- [ ] Especificar manualmente las instancias a parchear en lugar de usar selección basada en etiquetas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps ha creado un portafolio de AWS Service Catalog y lo ha compartido con una segunda cuenta de AWS de la empresa. La segunda cuenta está controlada por otro ingeniero. ¿Qué acción podrá realizar el ingeniero de la segunda cuenta?

- [x] Agregar un producto del portafolio importado a un portafolio local.
- [ ] Agregar nuevos productos al portafolio importado.
- [ ] Cambiar el rol de lanzamiento (launch role) de los productos contenidos en el portafolio importado.
- [ ] Personalizar los productos del portafolio importado.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa está ampliando su flota de instancias de Amazon EC2 antes de un aumento esperado de tráfico. Cuando un ingeniero de CloudOps intenta agregar más instancias, se devuelve un error `InstanceLimitExceeded`. ¿Qué debe hacer el ingeniero de CloudOps para resolver este error?

- [ ] Agregar un bloque `CIDR` adicional a la `VPC`.
- [ ] Lanzar las instancias de EC2 en una Zona de disponibilidad diferente.
- [ ] Lanzar nuevas instancias de EC2 en otra `VPC`.
- [x] Usar Service Quotas para solicitar un aumento de cuota de EC2.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa una cola estándar de Amazon Simple Queue Service (Amazon SQS) con su aplicación. La aplicación envía mensajes a la cola con cuerpos de mensaje únicos. La empresa decide cambiar a una cola SQS FIFO. ¿Qué debe hacer la empresa para migrar a una cola SQS FIFO?

- [x] Crear una nueva cola SQS FIFO. Activar la deduplicación basada en contenido en la nueva cola FIFO. Actualizar la aplicación para incluir un ID de grupo de mensajes (message group ID) en los mensajes.
- [ ] Crear una nueva cola SQS FIFO. Actualizar la aplicación para incluir el parámetro `DelaySeconds` en los mensajes.
- [ ] Modificar el tipo de cola de SQS estándar a SQS FIFO. Desactivar la deduplicación basada en contenido en la cola. Actualizar la aplicación para incluir un ID de grupo de mensajes en los mensajes.
- [ ] Modificar el tipo de cola de SQS estándar a SQS FIFO. Actualizar la aplicación para enviar mensajes con cuerpos de mensaje idénticos e incluir el parámetro `DelaySeconds` en los mensajes.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps creó una plantilla de AWS CloudFormation que aprovisiona instancias de Amazon EC2, un Elastic Load Balancer (ELB) y una instancia de base de datos de Amazon RDS. Durante la creación del stack, la creación de las instancias de EC2 y del ELB es exitosa. Sin embargo, la creación de la instancia de base de datos falla. ¿Cuál es el comportamiento predeterminado de CloudFormation en este escenario?

- [ ] CloudFormation revertirá (rollback) el stack y lo eliminará.
- [x] CloudFormation revertirá el stack pero no lo eliminará.
- [ ] CloudFormation le pedirá al usuario que decida entre revertir el stack o continuar.
- [ ] CloudFormation completará el stack exitosamente pero reportará un estado fallido para la instancia de base de datos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps crea un clúster de Amazon Elastic Kubernetes Service (Amazon EKS) que usa AWS Fargate. El clúster se despliega con éxito. El ingeniero de CloudOps necesita administrar el clúster usando la herramienta de línea de comandos `kubectl`. ¿Cuál de los siguientes debe configurarse en la máquina del ingeniero de CloudOps para que `kubectl` pueda comunicarse con el servidor de la API del clúster?

- [x] El archivo `kubeconfig`.
- [ ] El complemento de Amazon EKS `kube-proxy`.
- [ ] El perfil de Fargate.
- [ ] El archivo `eks-connector.yaml`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa de desarrollo de software tiene varios desarrolladores que trabajan en el mismo producto. Cada desarrollador debe tener su propio entorno de desarrollo, y estos entornos de desarrollo deben ser idénticos. Cada entorno de desarrollo consiste en instancias de Amazon EC2 y una instancia de base de datos de Amazon RDS. Los entornos de desarrollo deben crearse solo cuando sea necesario y deben terminarse cada noche para minimizar costos. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Dar a los desarrolladores acceso a la misma plantilla de AWS CloudFormation para que puedan aprovisionar su entorno de desarrollo cuando sea necesario. Programar un cron job nocturno en cada instancia de desarrollo para detener todos los procesos en ejecución y reducir el uso de CPU a casi cero.
- [x] Dar a los desarrolladores acceso a la misma plantilla de AWS CloudFormation para que puedan aprovisionar su entorno de desarrollo cuando sea necesario. Programar una regla nocturna de Amazon EventBridge (Amazon CloudWatch Events) para invocar una función de AWS Lambda que elimine los stacks de AWS CloudFormation.
- [ ] Dar a los desarrolladores comandos de la CLI para que puedan aprovisionar su propio entorno de desarrollo cuando sea necesario. Programar una regla nocturna de Amazon EventBridge (Amazon CloudWatch Events) para invocar una función de AWS Lambda que termine todas las instancias de EC2 y la instancia de base de datos.
- [ ] Dar a los desarrolladores comandos de la CLI para que puedan aprovisionar su propio entorno de desarrollo cuando sea necesario. Programar una regla nocturna de Amazon EventBridge (Amazon CloudWatch Events) para que AWS CloudFormation elimine todos los recursos del entorno de desarrollo.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa adquirió recientemente otra corporación junto con todas las cuentas de AWS de esa corporación. Un analista financiero necesita los datos de costos de estas cuentas. Un ingeniero de CloudOps usa Cost Explorer para generar informes de costos y uso. El ingeniero de CloudOps observa que `No Tagkey` representa el `20%` del costo mensual. ¿Qué debe hacer el ingeniero de CloudOps para etiquetar los recursos de `No Tagkey`?

- [ ] Agregar las cuentas a AWS Organizations. Usar una Política de Control de Servicio (SCP) para etiquetar todos los recursos sin etiquetar.
- [ ] Usar una regla de AWS Config para encontrar los recursos sin etiquetar. Configurar la acción de remediación para terminar los recursos.
- [ ] Usar Cost Explorer para encontrar y etiquetar todos los recursos sin etiquetar.
- [x] Usar Tag Editor para encontrar y etiquetar todos los recursos sin etiquetar.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está solucionando problemas de una plantilla de AWS CloudFormation mediante la cual se crean múltiples instancias de Amazon EC2. La plantilla funciona en `us-east-1`, pero falla en `us-west-2` con el código de error: `AMI [ami-12345678] does not exist`. ¿Cómo debe asegurarse el ingeniero de que la plantilla de AWS CloudFormation funcione en todas las regiones?

- [ ] Copiar la Amazon Machine Image (AMI) de la región de origen a la región de destino y asignarle el mismo ID.
- [ ] Editar la plantilla de AWS CloudFormation para especificar el código de región como parte del ID de AMI totalmente calificado.
- [ ] Editar la plantilla de AWS CloudFormation para ofrecer al usuario una lista desplegable de todas las AMIs usando el control `AWS::EC2::AMI::ImageID`.
- [x] Modificar la plantilla de AWS CloudFormation incluyendo los IDs de AMI en la sección `Mappings`. Referenciar el mapeo apropiado dentro de la plantilla para obtener el ID de AMI correcto.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps desarrolló un script de Python que usa el AWS SDK para realizar varias tareas de mantenimiento. El script necesita ejecutarse automáticamente cada noche. ¿Cuál es la solución MÁS eficiente operativamente que cumple con este requisito?

- [x] Convertir el script de Python en una función de AWS Lambda. Usar una regla de Amazon EventBridge (Amazon CloudWatch Events) para invocar la función cada noche.
- [ ] Convertir el script de Python en una función de AWS Lambda. Usar AWS CloudTrail para invocar la función cada noche.
- [ ] Desplegar el script de Python en una instancia de Amazon EC2. Usar Amazon EventBridge (Amazon CloudWatch Events) para programar el inicio y detención de la instancia cada noche.
- [ ] Desplegar el script de Python en una instancia de Amazon EC2. Usar AWS Systems Manager para programar el inicio y detención de la instancia cada noche.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa plantillas de AWS CloudFormation para desplegar infraestructura en la nube. Un análisis de todas las plantillas de la empresa muestra que la empresa ha declarado los mismos componentes en múltiples plantillas. Un ingeniero de CloudOps necesita crear plantillas dedicadas que tengan sus propios parámetros y condiciones para estos componentes comunes. ¿Qué solución cumple con este requisito?

- [ ] Desarrollar un conjunto de cambios (change set) de CloudFormation.
- [ ] Desarrollar macros de CloudFormation.
- [x] Desarrollar stacks anidados (nested stacks) de CloudFormation.
- [ ] Desarrollar conjuntos de stacks (stack sets) de CloudFormation.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una auditoría reciente encontró que la mayoría de los recursos pertenecientes al equipo de desarrollo estaban en violación de los estándares de cumplimiento de parches. Los recursos estaban correctamente etiquetados. ¿Qué servicio se debe usar para remediar rápidamente el problema y devolver los recursos al cumplimiento?

- [ ] AWS Config.
- [ ] Amazon Inspector.
- [ ] AWS Trusted Advisor.
- [x] AWS Systems Manager.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps tiene muchas instancias de Amazon EC2 con Windows que necesitan compartir un sistema de archivos entre nodos. El ingeniero de CloudOps crea un recurso compartido de archivos de Amazon Elastic File System (Amazon EFS). Después de crear el recurso compartido, el ingeniero de CloudOps tiene problemas para montarlo en las instancias de EC2. ¿Qué acción debe tomar el ingeniero de CloudOps para que las instancias de EC2 puedan compartir los archivos?

- [x] Eliminar el recurso compartido de EFS. Crear un recurso compartido de archivos de Amazon FSx for Windows File Server para las instancias de EC2.
- [ ] Usar las credenciales de IAM correctas para montar el recurso compartido de EFS.
- [ ] Configurar soporte para NFSv4 en el sistema operativo Windows que se ejecuta en las instancias de EC2.
- [ ] Permitir el puerto correcto para NFS a través del grupo de seguridad y la `ACL` de red.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa una plantilla de AWS CloudFormation para aprovisionar una instancia de Amazon EC2 y una instancia de base de datos de Amazon RDS. Un ingeniero de CloudOps debe actualizar la plantilla para asegurarse de que la instancia de base de datos se cree antes de que se lance la instancia de EC2. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con este requisito?

- [ ] Agregar una condición de espera (wait condition) a la plantilla. Actualizar el script de datos de usuario (user data) de la instancia de EC2 para enviar una señal después de que la instancia de EC2 se inicie.
- [x] Agregar el atributo `DependsOn` al recurso de la instancia de EC2, y proporcionar el nombre lógico del recurso de RDS.
- [ ] Cambiar el orden de los recursos en la plantilla para que el recurso de RDS se liste antes que el recurso de la instancia de EC2.
- [ ] Crear múltiples plantillas. Usar `StackSets` de AWS CloudFormation para esperar a que un stack se complete antes de crear el segundo stack.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa AWS CloudFormation para desplegar la infraestructura de su aplicación. Recientemente, un usuario cambió accidentalmente una propiedad de una base de datos en una plantilla de CloudFormation y realizó una actualización del stack que causó una interrupción en la aplicación. Un ingeniero de CloudOps debe determinar cómo modificar el proceso de despliegue para permitir que el equipo de DevOps continúe desplegando la infraestructura, pero evitando modificaciones accidentales a recursos específicos. ¿Qué solución cumple con estos requisitos?

- [ ] Configurar una regla de AWS Config para alertar según los cambios en cualquier stack de CloudFormation. Una función de AWS Lambda puede entonces describir el stack para determinar si se modificó algún recurso protegido y cancelar la operación.
- [ ] Configurar un evento de Amazon CloudWatch Events con una regla que se active según cualquier llamada a la API de CloudFormation. Una función de AWS Lambda puede entonces describir el stack para determinar si se modificó algún recurso protegido y cancelar la operación.
- [x] Lanzar las plantillas de CloudFormation usando una política de stack (stack policy) con un permiso explícito (allow) para todos los recursos y una denegación explícita (deny) de los recursos protegidos con una acción de `Update:*`.
- [ ] Adjuntar una política de IAM al rol del equipo de DevOps que impida que un stack de CloudFormation se actualice, con una condición basada en los Amazon Resource Names (ARNs) específicos de los recursos protegidos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps tiene una plantilla de AWS CloudFormation de la infraestructura existente de la empresa en `us-west-2`. El ingeniero intenta usar la plantilla para lanzar un nuevo stack en `eu-west-1`, pero el stack solo se despliega parcialmente, recibe un mensaje de error y luego se revierte (rollback). ¿Por qué fallaría esta plantilla al desplegarse? (Seleccione DOS.)

- [ ] La plantilla referenciaba un usuario de IAM que no está disponible en `eu-west-1`.
- [x] La plantilla referenciaba una Amazon Machine Image (AMI) que no está disponible en `eu-west-1`.
- [ ] La plantilla no tenía el nivel adecuado de permisos para desplegar los recursos.
- [x] La plantilla solicitaba servicios que no existen en `eu-west-1`.
- [ ] Las plantillas de CloudFormation solo pueden usarse para actualizar servicios existentes.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa AWS CloudFormation para desplegar su infraestructura. La empresa recientemente retiró una aplicación. Un ingeniero de operaciones en la nube inicia la eliminación de un stack de CloudFormation, y el stack queda atascado en estado `DELETE_FAILED`. Un ingeniero de CloudOps descubre que el stack había desplegado un grupo de seguridad. Ese grupo de seguridad es referenciado por otros grupos de seguridad en el entorno. El ingeniero de CloudOps necesita eliminar el stack sin afectar otras aplicaciones. ¿Qué solución cumple con estos requisitos de la manera MÁS eficiente operativamente?

- [ ] Crear un nuevo grupo de seguridad con un nombre diferente. Aplicar reglas idénticas al nuevo grupo de seguridad. Reemplazar todos los demás grupos de seguridad que referencien al nuevo grupo de seguridad. Eliminar el stack.
- [ ] Crear un conjunto de cambios (change set) de CloudFormation para eliminar el grupo de seguridad. Desplegar el conjunto de cambios.
- [x] Eliminar el stack nuevamente. Especificar que el grupo de seguridad se conserve (retained).
- [ ] Realizar una detección de deriva (drift detection) de CloudFormation. Eliminar el stack.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps crea una plantilla de AWS CloudFormation para definir una pila de aplicación que puede desplegarse en múltiples regiones de AWS. El ingeniero de CloudOps también crea un dashboard de Amazon CloudWatch usando la consola de administración de AWS. Cada despliegue de la aplicación requiere su propio dashboard de CloudWatch. ¿Cómo puede el ingeniero de CloudOps automatizar la creación del dashboard de CloudWatch cada vez que se despliega la aplicación?

- [ ] Crear un script usando la AWS CLI para ejecutar el comando `aws cloudformation put-dashboard` con el nombre del dashboard. Ejecutar el comando cada vez que se cree un nuevo stack de CloudFormation.
- [x] Exportar el dashboard de CloudWatch existente como JSON. Actualizar la plantilla de CloudFormation para definir un recurso `AWS::CloudWatch::Dashboard`. Incluir el JSON exportado en la propiedad `DashboardBody` del recurso.
- [ ] Actualizar la plantilla de CloudFormation para definir un recurso `AWS::CloudWatch::Dashboard`. Usar la función intrínseca Ref para referenciar el ID del dashboard de CloudWatch existente.
- [ ] Actualizar la plantilla de CloudFormation para definir un recurso `AWS::CloudWatch::Dashboard`. Especificar el nombre del dashboard existente en la propiedad `DashboardName`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps ha desplegado con éxito una `VPC` con una plantilla de AWS CloudFormation. El ingeniero de CloudOps quiere desplegar la misma plantilla en múltiples cuentas administradas a través de AWS Organizations. ¿Qué solución cumple con este requisito con el MENOR esfuerzo operativo?

- [ ] Asumir el rol de IAM `OrganizationAccountAccessRole` desde la cuenta de administración. Desplegar la plantilla en cada una de las cuentas.
- [ ] Crear una función de AWS Lambda para asumir un rol en cada cuenta. Desplegar la plantilla usando la llamada a la API `CreateStack` de AWS CloudFormation.
- [ ] Crear una función de AWS Lambda para consultar una lista de cuentas. Desplegar la plantilla usando la llamada a la API `CreateStack` de AWS CloudFormation.
- [x] Usar `StackSets` de AWS CloudFormation desde la cuenta de administración para desplegar la plantilla en cada una de las cuentas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps es responsable de administrar la infraestructura en la nube de una empresa con AWS CloudFormation. El ingeniero de CloudOps necesita crear un único recurso que consista en múltiples servicios de AWS. El recurso debe admitir su creación y eliminación a través de la consola de CloudFormation. ¿Qué tipo de recurso de CloudFormation debe crear el ingeniero de CloudOps para cumplir con estos requisitos?

- [ ] `AWS::EC2::Instance` con un script de ayuda `cfn-init`.
- [ ] `AWS::OpsWorks::Instance`.
- [ ] `AWS::SSM::Document`.
- [x] `Custom::MyCustomType`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está usando `StackSets` de AWS CloudFormation para crear recursos de AWS en dos regiones de AWS dentro de la misma cuenta de AWS. Una operación de stack falla en una región y devuelve el estado de instancia de stack `OUTDATED`. ¿Cuál es la causa de esta falla?

- [ ] La plantilla de CloudFormation cambió en el disco local y no ha sido enviada a CloudFormation.
- [x] La plantilla de CloudFormation está intentando crear un recurso global que no es único.
- [ ] El stack aún no ha sido desplegado en la región.
- [ ] El ingeniero de CloudOps está usando una versión antigua de la API de CloudFormation.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### A un ingeniero de CloudOps se le asigna la tarea de desplegar la infraestructura de una empresa como código. El ingeniero de CloudOps quiere escribir una única plantilla que pueda reutilizarse para múltiples entornos. ¿Cómo debe el ingeniero de CloudOps usar AWS CloudFormation para crear una solución?

- [ ] Usar datos de usuario (user data) de Amazon EC2 en una plantilla de CloudFormation.
- [ ] Usar stacks anidados (nested stacks) para aprovisionar recursos.
- [x] Usar parámetros en una plantilla de CloudFormation.
- [ ] Usar políticas de stack para aprovisionar recursos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está intentando desplegar recursos usando una plantilla de AWS CloudFormation. Una instancia de Amazon EC2 que está definida en la plantilla no logra iniciarse y produce un error `InsufficientInstanceCapacity`. ¿Qué acciones debe tomar el ingeniero de CloudOps para resolver este error? (Elija dos.)

- [ ] Crear una plantilla de AWS CloudFormation separada para la instancia de EC2.
- [x] Modificar la plantilla de AWS CloudFormation para no especificar una Zona de disponibilidad para la instancia de EC2.
- [x] Modificar la plantilla de AWS CloudFormation para usar un tipo de instancia de EC2 diferente.
- [ ] Usar una Amazon Machine Image (AMI) diferente para la instancia de EC2.
- [ ] Usar el comando `validate-template` de la AWS CLI antes de crear un stack a partir de la plantilla.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está examinando la siguiente plantilla de AWS CloudFormation. ¿Por qué fallará la creación del stack?

![Question 201](images/question201.jpg)

- [ ] Se omitió la sección `Outputs` de la plantilla de CloudFormation.
- [ ] Se omitió la sección `Parameters` de la plantilla de CloudFormation.
- [x] `PrivateDnsName` no se puede configurar desde una plantilla de CloudFormation.
- [ ] No se especificó la `VPC` en la plantilla de CloudFormation.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa un portafolio de AWS Service Catalog para crear y administrar recursos. Un ingeniero de CloudOps debe crear una réplica de la infraestructura de AWS existente de la empresa en una nueva cuenta de AWS. ¿Cuál es la forma MÁS eficiente operativamente de cumplir con este requisito?

- [ ] Crear una plantilla de AWS CloudFormation para usar el portafolio de AWS Service Catalog en la nueva cuenta de AWS.
- [ ] En la nueva cuenta de AWS, crear manualmente un portafolio de AWS Service Catalog que duplique el portafolio original.
- [ ] Ejecutar una función de AWS Lambda para crear un nuevo portafolio de AWS Service Catalog basado en la salida de la operación de API `DescribePortfolio`.
- [x] Compartir el portafolio de AWS Service Catalog con la nueva cuenta de AWS. Importar el portafolio a la nueva cuenta de AWS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps ha usado AWS CloudFormation para desplegar una aplicación sin servidor (serverless) en una `VPC` de producción. La aplicación consiste en una función de AWS Lambda, una tabla de Amazon DynamoDB y una API de Amazon API Gateway. El ingeniero de CloudOps debe eliminar el stack de AWS CloudFormation sin eliminar la tabla de DynamoDB. ¿Qué acción debe tomar el ingeniero de CloudOps antes de eliminar el stack de AWS CloudFormation?

- [x] Agregar una política de eliminación `Retain` al recurso de DynamoDB en el stack de AWS CloudFormation.
- [ ] Agregar una política de eliminación `Snapshot` al recurso de DynamoDB en el stack de AWS CloudFormation.
- [ ] Habilitar la protección contra terminación en el stack de AWS CloudFormation.
- [ ] Actualizar la política de IAM de la aplicación con una declaración `Deny` para la acción `dynamodb:DeleteTable`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps debe idear una estrategia para hacer cumplir el etiquetado de todas las instancias de EC2 y volúmenes de Amazon Elastic Block Store (Amazon EBS). ¿Qué acción puede tomar el ingeniero para implementar esto en tiempo real?

- [ ] Usar el AWS Tag Editor para buscar manualmente recursos sin etiquetar y luego etiquetarlos correctamente en el editor.
- [x] Configurar AWS Service Catalog con la regla de biblioteca `TagOptions` que hace cumplir una taxonomía de etiquetado proactivamente cuando se lanzan instancias y volúmenes.
- [ ] En un script de PowerShell o shell, verificar elementos sin etiquetar usando la acción de API de etiquetado de recursos `GetResources`, y luego etiquetar manualmente los elementos reportados.
- [ ] Lanzar elementos usando la API de AWS. Usar la acción de API `TagResources` para aplicar las etiquetas requeridas cuando se lancen las instancias y volúmenes.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa global opera desde cinco regiones de AWS. Un ingeniero de CloudOps quiere identificar todas las instancias de Amazon EC2 de la empresa, tanto etiquetadas como sin etiquetar. La empresa requiere que la salida muestre el ID de instancia y las etiquetas. ¿Cuál es la forma MÁS eficiente operativamente para que el ingeniero de CloudOps cumpla con estos requisitos?

- [ ] Crear un grupo de recursos basado en etiquetas en AWS Resource Groups.
- [ ] Usar AWS Trusted Advisor. Exportar los resultados de la verificación de instancias On-Demand de EC2 desde Trusted Advisor.
- [ ] Usar Cost Explorer. Elegir un tipo de servicio de EC2-Instances, y agrupar por recurso.
- [x] Usar Tag Editor en AWS Resource Groups. Seleccionar todas las regiones, y elegir un tipo de recurso `AWS::EC2::Instance`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita eliminar un stack de AWS CloudFormation que ya no está en uso. El stack de CloudFormation está en el estado `DELETE_FAILED`. El ingeniero de CloudOps ha validado los permisos requeridos para eliminar el stack de CloudFormation. ¿Cuáles de las siguientes son posibles causas del estado `DELETE_FAILED`? (Elija dos.)

- [ ] El tiempo de espera (timeout) configurado para eliminar el stack era demasiado bajo para que se completara la operación de eliminación.
- [ ] El stack contiene stacks anidados (nested stacks) que deben eliminarse manualmente primero.
- [ ] El stack se desplegó con la opción `--disable-rollback`.
- [x] Hay recursos adicionales asociados con un grupo de seguridad en el stack.
- [x] Hay buckets de Amazon S3 en el stack que todavía contienen objetos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha desplegado una aplicación en AWS. La aplicación se ejecuta en una flota de instancias de Amazon EC2 Linux que están en un grupo de Auto Scaling. El grupo de Auto Scaling está configurado para usar plantillas de lanzamiento (launch templates). Las plantillas de lanzamiento lanzan instancias de EC2 respaldadas por Amazon Elastic Block Store (Amazon EBS) que usan volúmenes EBS `General Purpose SSD (gp3)` para almacenamiento primario. Un ingeniero de CloudOps necesita implementar una solución para asegurar que todas las instancias de EC2 puedan compartir los mismos archivos subyacentes. La solución también debe asegurar que los datos sean consistentes. ¿Qué solución cumple con estos requisitos?

- [x] Crear un sistema de archivos de Amazon Elastic File System (Amazon EFS). Crear una nueva versión de la plantilla de lanzamiento que incluya datos de usuario (user data) que monten el sistema de archivos EFS. Actualizar el grupo de Auto Scaling para usar la nueva versión de la plantilla de lanzamiento a fin de ciclar instancias de EC2 más nuevas y terminar las instancias de EC2 más antiguas.
- [ ] Habilitar Multi-Attach en los volúmenes EBS. Crear una nueva versión de la plantilla de lanzamiento que incluya datos de usuario que monten el volumen EBS. Actualizar el grupo de Auto Scaling para usar la nueva versión de la plantilla a fin de ciclar instancias de EC2 más nuevas y terminar las instancias de EC2 más antiguas.
- [ ] Crear un cron job que sincronice los datos entre los volúmenes EBS para todas las instancias de EC2 en el grupo de Auto Scaling. Crear un lifecycle hook durante el lanzamiento de instancias para configurar el cron job en todas las instancias de EC2. Rotar las instancias de EC2 más antiguas.
- [ ] Crear una nueva versión de la plantilla de lanzamiento que cree un sistema de archivos de Amazon Elastic File System (Amazon EFS). Actualizar el grupo de Auto Scaling para usar la nueva versión de la plantilla a fin de ciclar instancias de EC2 más nuevas y terminar las instancias de EC2 más antiguas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una aplicación que se ejecuta en instancias de Amazon EC2 en un grupo de Auto Scaling en múltiples Zonas de disponibilidad se desplegó usando una plantilla de AWS CloudFormation. El equipo de SysOps ha parcheado la versión de la Amazon Machine Image (AMI) y debe actualizar todas las instancias de EC2 para usar la nueva AMI. ¿Cómo puede el ingeniero de CloudOps usar CloudFormation para aplicar la nueva AMI mientras mantiene un nivel mínimo de instancias activas para garantizar la continuidad del servicio?

- [ ] Ejecutar el comando `update-stack` de aws cloudformation con la opción `rollback-configuration`.
- [ ] Actualizar la plantilla de CloudFormation con el nuevo ID de AMI, luego reiniciar las instancias de EC2.
- [ ] Desplegar un segundo stack de CloudFormation y usar Amazon Route 53 para redirigir el tráfico al nuevo stack.
- [x] Establecer una política `AutoScalingRollingUpdate` en la plantilla de CloudFormation para actualizar el stack.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps quiere usar AWS Systems Manager Patch Manager para automatizar el proceso de aplicar parches a instancias de Amazon EC2 Windows. El ingeniero de CloudOps quiere asegurarse de que los parches se aprueben automáticamente 2 días después de la fecha de lanzamiento para las instancias de desarrollo. Los parches también deben aprobarse automáticamente 5 días después de la fecha de lanzamiento para las instancias de producción. El mantenimiento debe ocurrir solo durante una ventana de 2 horas para todas las instancias. ¿Qué solución cumple con estos requisitos?

- [ ] Usar etiquetas para identificar las instancias de desarrollo y producción. En Patch Manager, crear dos grupos de parches y una línea base de parches. Agregar un retraso de aprobación automática a cada grupo de parches. Crear una única ventana de mantenimiento.
- [x] Usar etiquetas para identificar las instancias de desarrollo y producción. En Patch Manager, crear dos grupos de parches y dos líneas base de parches. Especificar un retraso de aprobación automática en cada una de las líneas base de parches. Crear una única ventana de mantenimiento.
- [ ] Usar etiquetas para identificar las instancias de desarrollo y producción. En Patch Manager, crear dos grupos de parches y una línea base de parches. Crear dos ventanas de mantenimiento separadas, cada una con un retraso de aprobación automática.
- [ ] Usar etiquetas para identificar las instancias de desarrollo. En Patch Manager, crear un grupo de parches y una línea base de parches. Especificar retrasos de aprobación automática en la línea base de parches. Agregar las instancias de desarrollo al nuevo grupo de parches. Usar líneas base de parches predefinidas de Patch Manager para todas las instancias restantes. Crear una única ventana de mantenimiento.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps es responsable de más de `50` instancias de Amazon EC2 desplegadas en una única cuenta de AWS de producción. Las instancias de EC2 ejecutan varios sistemas operativos diferentes. Los estándares de la empresa requieren que el parchado se complete al menos una vez al mes. El ingeniero de CloudOps quiere usar AWS Systems Manager para reducir el número de horas que la empresa dedica al parchado del sistema operativo cada mes. ¿Qué combinación de pasos debe tomar el ingeniero de CloudOps para cumplir con estos requisitos? (Elija tres.)

- [x] Agrupar instancias de EC2 similares en grupos de recursos usando AWS Resource Groups.
- [ ] Crear una programación en Systems Manager Patch Manager. Especificar el grupo de recursos apropiado como el destino.
- [x] Especificar runbooks de Systems Manager Automation para parchar los sistemas operativos. Registrar los runbooks como tareas en la ventana de mantenimiento. Especificar el grupo de recursos apropiado como el destino.
- [ ] Crear un runbook de Systems Manager Automation para monitorear y controlar el estado de los parches requeridos. Aplicar el runbook a Systems Manager Patch Manager.
- [x] Crear una única ventana de mantenimiento de Systems Manager para cada grupo de recursos.
- [ ] Configurar Systems Manager Fleet Manager para aplicar un runbook de Systems Manager Automation al grupo de recursos apropiado.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una organización está ejecutando múltiples aplicaciones para sus clientes. Cada aplicación se despliega ejecutando una plantilla base de AWS CloudFormation que configura una nueva `VPC`. Todas las aplicaciones se ejecutan en la misma cuenta de AWS y región de AWS. Un ingeniero de CloudOps ha notado que al intentar desplegar el mismo stack de AWS CloudFormation, este falla al desplegarse. ¿Cuál es probablemente el problema?

- [ ] La Amazon Machine Image usada no está disponible en esa región.
- [ ] La plantilla de AWS CloudFormation necesita actualizarse a la última versión.
- [ ] Los parámetros de configuración de la `VPC` han cambiado y deben actualizarse en la plantilla.
- [x] La cuenta ha alcanzado el límite predeterminado de `VPC` permitidas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Se le ha encomendado a un ingeniero de CloudOps desplegar la infraestructura de una empresa como código. El ingeniero quiere escribir una única plantilla que pueda reutilizarse para múltiples entornos de una manera segura y repetible. ¿Cuál es la forma recomendada de usar AWS CloudFormation para cumplir con este requisito?

- [x] Usar parámetros para aprovisionar los recursos.
- [ ] Usar stacks anidados (nested stacks) para aprovisionar los recursos.
- [ ] Usar datos de usuario (user data) de Amazon EC2 para aprovisionar los recursos.
- [ ] Usar políticas de stack para aprovisionar los recursos.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está creando recursos a partir de una plantilla de AWS CloudFormation que define un grupo de Auto Scaling de instancias de Amazon EC2. La plantilla de lanzamiento del grupo de Auto Scaling aprovisiona cada instancia de EC2 usando un script de datos de usuario. La creación del recurso de grupo de Auto Scaling está fallando debido a un error. La condición de espera (wait condition) no está recibiendo el número requerido de señales. ¿Cómo debe el ingeniero de CloudOps resolver este error?

- [x] Ejecutar `cfn-signal` al finalizar el script de datos de usuario.
- [ ] Modificar el grupo de seguridad de las instancias de EC2 para permitir tráfico saliente en el puerto `443`.
- [ ] Reducir el valor de `DesiredCapacity` del grupo de Auto Scaling en la plantilla de CloudFormation.
- [ ] Establecer la propiedad `AssociatePublicIpAddress` en `True` en la plantilla de lanzamiento del grupo de Auto Scaling.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita crear una réplica de la infraestructura de AWS existente de una empresa en una nueva cuenta de AWS. Actualmente, se usa un portafolio de AWS Service Catalog para crear y administrar recursos. ¿Cuál es la forma MÁS eficiente de lograr esto?

- [ ] Crear una plantilla de AWS CloudFormation para usar el portafolio de AWS Service Catalog en la nueva cuenta de AWS.
- [ ] Crear manualmente un portafolio de AWS Service Catalog en la nueva cuenta de AWS que duplique el portafolio original.
- [ ] Ejecutar una función de AWS Lambda para crear un nuevo portafolio de AWS Service Catalog basado en la salida de la operación de API `DescribePortfolio`.
- [x] Compartir el portafolio de AWS Service Catalog con las otras cuentas de AWS e importar el portafolio a las otras cuentas de AWS.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El ingeniero de CloudOps de una empresa administra una flota de cientos de instancias de Amazon EC2 que ejecutan cargas de trabajo basadas en Windows y cargas de trabajo basadas en Linux. Cada instancia de EC2 tiene una etiqueta que identifica su sistema operativo. Todas las instancias de EC2 ejecutan AWS Systems Manager Session Manager. Se reporta una vulnerabilidad de día cero, y no hay parches disponibles. El equipo de seguridad de la empresa proporciona código para todos los sistemas operativos relevantes para reducir el riesgo de la vulnerabilidad. El ingeniero de CloudOps necesita implementar el código en las instancias de EC2 y debe proporcionar un informe que muestre que el código se ejecutó exitosamente en todas las instancias. ¿Qué debe hacer el ingeniero de CloudOps para cumplir con estos requisitos lo más rápido posible?

- [x] Usar Systems Manager Run Command. Elegir el documento `AWS-RunShellScript` o el documento `AWS-RunPowerShellScript`. Configurar Run Command con el código del equipo de seguridad. Especificar la etiqueta del sistema operativo en el parámetro Targets. Ejecutar el comando. Proporcionar el historial de comandos como evidencia al equipo de seguridad.
- [ ] Crear una función de AWS Lambda que se conecte a las instancias de EC2 a través de Session Manager. Configurar la función Lambda para identificar el sistema operativo, ejecutar el código del equipo de seguridad, y devolver los resultados a una instancia de base de datos de Amazon RDS. Consultar la instancia de base de datos para obtener los resultados. Proporcionar los resultados como evidencia al equipo de seguridad.
- [ ] Iniciar sesión en cada instancia de EC2. Ejecutar el código del equipo de seguridad en cada instancia de EC2. Copiar y pegar los resultados de cada ejecución en una única hoja de cálculo. Proporcionar la hoja de cálculo como evidencia al equipo de seguridad.
- [ ] Actualizar las plantillas de lanzamiento de las instancias de EC2 para incluir el código del equipo de seguridad en los datos de usuario. Volver a lanzar las instancias de EC2 usando las plantillas de lanzamiento actualizadas. Recuperar los registros de instancia de EC2 de cada instancia. Proporcionar los registros de instancia de EC2 como evidencia al equipo de seguridad.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa ha desarrollado un servicio que se despliega en una flota de instancias de Amazon EC2 basadas en Linux que están en un grupo de Auto Scaling. El servicio falla ocasionalmente de manera inesperada debido a un error en el código de la aplicación. El equipo de ingeniería de la empresa determina que resolver la causa subyacente de la falla del servicio podría tomar varias semanas. Un ingeniero de CloudOps necesita crear una solución para automatizar la recuperación si el servicio falla en cualquiera de las instancias de EC2. ¿Qué soluciones cumplen con este requisito? (Elija dos.)

- [ ] Instalar el agente de Amazon CloudWatch en las instancias de EC2. Configurar el agente de CloudWatch para monitorear el servicio. Establecer la acción de CloudWatch para reiniciar si falla la verificación de salud del servicio.
- [ ] Etiquetar las instancias de EC2. Crear una función de AWS Lambda que use AWS Systems Manager Session Manager para iniciar sesión en las instancias de EC2 etiquetadas y reiniciar el servicio. Programar la función Lambda para que se ejecute cada 5 minutos.
- [x] Etiquetar las instancias de EC2. Usar AWS Systems Manager State Manager para crear una asociación que use el documento `AWS-RunShellScript`. Configurar el comando de asociación con un script que verifique si el servicio se está ejecutando y que lo inicie si no lo está. Para los destinos, especificar la etiqueta de la instancia de EC2. Programar la asociación para que se ejecute cada 5 minutos.
- [x] Actualizar los datos de usuario de EC2 especificados en la plantilla de lanzamiento del grupo de Auto Scaling para incluir un script que se ejecute en una programación cron cada 5 minutos. Configurar el script para verificar si el servicio se está ejecutando y para iniciarlo si no lo está. Volver a desplegar todas las instancias de EC2 en el grupo de Auto Scaling con la plantilla de lanzamiento actualizada.
- [ ] Actualizar los datos de usuario de EC2 especificados en la plantilla de lanzamiento del grupo de Auto Scaling para asegurar que el servicio se ejecute durante el inicio. Volver a desplegar todas las instancias de EC2 en el grupo de Auto Scaling con la plantilla de lanzamiento actualizada.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps necesita automatizar la invocación de una función de AWS Lambda. La función Lambda debe ejecutarse al final de cada día para generar un informe sobre datos almacenados en un bucket de Amazon S3. ¿Cuál es la solución MÁS eficiente operativamente que cumple con estos requisitos?

- [ ] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que tenga un patrón de evento para Amazon S3 y la función Lambda como destino.
- [x] Crear una regla de Amazon EventBridge (Amazon CloudWatch Events) que tenga una programación y la función Lambda como destino.
- [ ] Crear una notificación de eventos de S3 para invocar la función Lambda cada vez que los objetos cambien en el bucket de S3.
- [ ] Desplegar una instancia de Amazon EC2 con un cron job para invocar la función Lambda.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### La infraestructura de la aplicación de una empresa se desplegó usando AWS CloudFormation y consiste en instancias de Amazon EC2 detrás de un Application Load Balancer. Las instancias se ejecutan en un grupo de EC2 Auto Scaling en múltiples Zonas de disponibilidad. Al lanzar una nueva versión de la aplicación, el despliegue de actualización debe evitar cambios de `DNS` y permitir reversión (rollback). ¿Qué solución debe usar un ingeniero de CloudOps para cumplir con los requisitos de despliegue de este nuevo lanzamiento?

- [ ] Configurar el grupo de Auto Scaling para usar lifecycle hooks. Desplegar nuevas instancias con la nueva versión de la aplicación. Completar la acción del lifecycle hook una vez que estén saludables.
- [ ] Crear una nueva Amazon Machine Image (AMI) que contenga el código actualizado. Crear una configuración de lanzamiento con la AMI. Actualizar el grupo de Auto Scaling para usar la nueva configuración de lanzamiento.
- [ ] Desplegar un segundo stack de CloudFormation. Esperar a que la aplicación esté disponible. Cambiar al nuevo Application Load Balancer.
- [x] Modificar la plantilla de CloudFormation para usar una política `AutoScalingReplacingUpdate`. Actualizar el stack. Realizar una segunda actualización con el nuevo lanzamiento.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa usa un bucket de Amazon S3 para almacenar archivos de datos. El bucket de S3 contiene cientos de objetos. La empresa necesita reemplazar una etiqueta en todos los objetos del bucket de S3 por otra etiqueta. ¿Cuál es la forma MÁS eficiente operativamente de cumplir con este requisito?

- [x] Usar S3 Batch Operations. Especificar la operación para reemplazar todas las etiquetas de objeto.
- [ ] Usar la AWS CLI para obtener las etiquetas de cada objeto. Guardar las etiquetas en una lista. Usar S3 Batch Operations. Especificar la operación para eliminar todas las etiquetas de objeto. Usar la AWS CLI y la lista para volver a etiquetar los objetos.
- [ ] Usar la AWS CLI para obtener las etiquetas de cada objeto. Guardar las etiquetas en una lista. Usar la AWS CLI y la lista para eliminar las etiquetas de objeto. Usar la AWS CLI y la lista para volver a etiquetar los objetos.
- [ ] Usar la AWS CLI para copiar los objetos a otro bucket de S3. Agregar la nueva etiqueta a los objetos copiados. Eliminar los objetos originales.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un equipo de aplicaciones le ha pedido a un ingeniero de CloudOps que aprovisione un entorno adicional para una aplicación en cuatro regiones adicionales. La aplicación se ejecuta en más de 100 instancias en `us-east-1`, usando AMI completamente preparadas (fully baked). Se ha creado una plantilla de AWS CloudFormation para desplegar recursos en `us-east-1`. ¿Qué debe hacer el ingeniero de CloudOps para aprovisionar la aplicación rápidamente?

- [x] Copiar la AMI a cada región usando `aws ec2 copy-image`. Actualizar el mapeo de CloudFormation para incluir mapeos para las AMI copiadas.
- [ ] Crear una instantánea de la instancia en ejecución y copiar la instantánea a las otras regiones. Crear una AMI a partir de las instantáneas. Actualizar la plantilla de CloudFormation para cada región para usar la nueva AMI.
- [ ] Ejecutar la plantilla de CloudFormation existente en cada región adicional basándose en el éxito de la plantilla usada actualmente en `us-east-1`.
- [ ] Actualizar la plantilla de CloudFormation para incluir las regiones adicionales en el grupo de Auto Scaling. Actualizar el stack existente en `us-east-1`.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Una empresa planea expandirse a una región adicional de AWS con fines de recuperación ante desastres. La empresa usa AWS CloudFormation, y su infraestructura está bien definida como código. La empresa quisiera reutilizar la mayor cantidad posible de su código existente al desplegar recursos en regiones adicionales. Un ingeniero de CloudOps está revisando cómo se seleccionan las Amazon Machine Images (AMI) en AWS CloudFormation, pero tiene problemas para hacer que el mismo stack funcione en la nueva región. ¿Qué acción facilitaría la administración de múltiples regiones?

- [ ] Nombrar cada AMI en la nueva región exactamente igual que la AMI equivalente en la primera región.
- [ ] Duplicar el stack para que se puedan codificar nombres de AMI únicos en el stack apropiado.
- [ ] Crear un alias para cada AMI de modo que se pueda hacer referencia a una AMI por un nombre común entre regiones.
- [x] Crear una sección `Mappings` en el stack, y definir las asociaciones de región a AMI.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### Un ingeniero de CloudOps está administrando una cuenta de AWS donde los desarrolladores están autorizados a lanzar instancias de Amazon EC2 para probar código nuevo. Para limitar los costos, el ingeniero debe asegurarse de que las instancias de EC2 en la cuenta se terminen 24 horas después del lanzamiento. ¿Cómo debe el ingeniero cumplir con estos requisitos?

- [ ] Crear una alarma de Amazon CloudWatch basada en la métrica `CPUUtilization`. Cuando la métrica sea `0%` durante 24 horas, activar una acción para terminar la instancia de EC2 cuando se active la alarma.
- [x] Crear una función de AWS Lambda para verificar todas las instancias de EC2 y terminar las instancias que se ejecuten por más de 24 horas. Activar la función con un evento de Amazon CloudWatch Events cada 15 minutos.
- [ ] Agregar una acción a AWS Trusted Advisor para apagar instancias de EC2 según la verificación Low Utilization Amazon EC2 Instances, terminando las instancias identificadas por Trusted Advisor como en ejecución por más de 24 horas.
- [ ] Instalar el agente unificado de Amazon CloudWatch en cada instancia de EC2. Configurar el agente para terminar las instancias después de que se hayan ejecutado durante 24 horas.

**[⬆ Volver arriba](#tabla-de-contenidos)**

### El ingeniero de CloudOps de una empresa administra una flota de instancias de Amazon EC2 Windows que se ejecutan en una única cuenta de AWS. Las instancias tienen una etiqueta que incluye una clave `OS` y un valor `Windows`. La empresa usa AWS Systems Manager para parchar las instancias. La empresa ha instalado el agente de Amazon CloudWatch en las instancias, pero la configuración es inconsistente. El ingeniero de CloudOps necesita reconfigurar cada instancia para usar la misma configuración predefinida de CloudWatch. ¿Qué combinación de pasos cumple con estos requisitos? (Elija dos.)

- [ ] Almacenar el archivo de configuración del agente de CloudWatch en un bucket de Amazon S3.
- [ ] Almacenar el contenido del archivo de configuración del agente de CloudWatch en Systems Manager OpsCenter.
- [x] Almacenar el contenido del archivo de configuración del agente de CloudWatch en Systems Manager Parameter Store.
- [x] Crear una asociación de Systems Manager State Manager para ejecutar el documento de Systems Manager Run Command `AmazonCloudWatch-ManageAgent`. Seleccionar Systems Manager como fuente de configuración opcional. Dirigir a las instancias según los valores de etiqueta.
- [ ] Crear una asociación de Systems Manager State Manager para ejecutar el documento de Systems Manager Run Command `AmazonCloudWatch-ManageAgent`. Configurar el documento para usar la ubicación del bucket de S3 como fuente de configuración. Dirigir a las instancias según el valor de etiqueta.

**[⬆ Volver arriba](#tabla-de-contenidos)**
