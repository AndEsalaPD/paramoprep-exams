# Dominio 3: Despliegue (24 %)

Preguntas de práctica AWS Certified Developer Associate (DVA-C02) — 74 preguntas.

## Tabla de contenidos

| No. | Preguntas |
| --- | --------- |
| 1 | [Una empresa utiliza una herramienta de terceros para compilar, agrupar y empaquetar sus aplicaciones de forma local (on-premises) y almacenarlas localmente. La empresa utiliza instancias de Amazon EC2 para ejecutar sus aplicaciones front-end. ¿Cómo se puede implementar una aplicación desde el sistema de control de código fuente en las instancias EC2?](#una-empresa-utiliza-una-herramienta-de-terceros-para-compilar-agrupar-y-empaquetar-sus-aplicaciones-de-forma-local-on-premises-y-almacenarlas-localmente-la-empresa-utiliza-instancias-de-amazon-ec2-para-ejecutar-sus-aplicaciones-front-end-cómo-se-puede-implementar-una-aplicación-desde-el-sistema-de-control-de-código-fuente-en-las-instancias-ec2) |
| 2 | [Un desarrollador debe ampliar una aplicación existente basada en AWS Serverless Application Model (AWS SAM). El desarrollador ha utilizado AWS SAM CLI para crear el proyecto. El proyecto contiene diferentes funciones de AWS Lambda. ¿Qué combinación de comandos debe usar el desarrollador para volver a implementar la aplicación de AWS SAM? (Seleccione DOS)](#un-desarrollador-debe-ampliar-una-aplicación-existente-basada-en-aws-serverless-application-model-aws-sam-el-desarrollador-ha-utilizado-aws-sam-cli-para-crear-el-proyecto-el-proyecto-contiene-diferentes-funciones-de-aws-lambda-qué-combinación-de-comandos-debe-usar-el-desarrollador-para-volver-a-implementar-la-aplicación-de-aws-sam-seleccione-dos) |
| 3 | [Una aplicación implementada en AWS Elastic Beanstalk experimenta mayores tasas de error durante las implementaciones de nuevas versiones de la aplicación, lo que resulta en una degradación del servicio para los usuarios. El equipo de desarrollo cree que esto se debe a la reducción de capacidad durante los pasos de la implementación. El equipo desea cambiar la configuración de la política de implementación del entorno a una opción que mantenga la capacidad total durante la implementación utilizando las instancias existentes. ¿Qué política de implementación cumplirá con estos requisitos utilizando las instancias existentes?](#una-aplicación-implementada-en-aws-elastic-beanstalk-experimenta-mayores-tasas-de-error-durante-las-implementaciones-de-nuevas-versiones-de-la-aplicación-lo-que-resulta-en-una-degradación-del-servicio-para-los-usuarios-el-equipo-de-desarrollo-cree-que-esto-se-debe-a-la-reducción-de-capacidad-durante-los-pasos-de-la-implementación-el-equipo-desea-cambiar-la-configuración-de-la-política-de-implementación-del-entorno-a-una-opción-que-mantenga-la-capacidad-total-durante-la-implementación-utilizando-las-instancias-existentes-qué-política-de-implementación-cumplirá-con-estos-requisitos-utilizando-las-instancias-existentes) |
| 4 | [Un desarrollador está realizando cambios en una aplicación personalizada que actualmente utiliza AWS Elastic Beanstalk. Una vez que el desarrollador completa los cambios, ¿qué soluciones actualizarán el entorno de Elastic Beanstalk con la nueva versión de la aplicación? (Elija DOS)](#un-desarrollador-está-realizando-cambios-en-una-aplicación-personalizada-que-actualmente-utiliza-aws-elastic-beanstalk-una-vez-que-el-desarrollador-completa-los-cambios-qué-soluciones-actualizarán-el-entorno-de-elastic-beanstalk-con-la-nueva-versión-de-la-aplicación-elija-dos) |
| 5 | [Un desarrollador necesita implementar una nueva versión en una aplicación de AWS Elastic Beanstalk. ¿Cómo puede el desarrollador lograr esta tarea?](#un-desarrollador-necesita-implementar-una-nueva-versión-en-una-aplicación-de-aws-elastic-beanstalk-cómo-puede-el-desarrollador-lograr-esta-tarea) |
| 6 | [Un desarrollador desea tener la capacidad de revertir a una versión anterior de una función de AWS Lambda en caso de errores causados por un nuevo despliegue. ¿Cómo puede lograrlo el desarrollador con un impacto MÍNIMO en los usuarios?](#un-desarrollador-desea-tener-la-capacidad-de-revertir-a-una-versión-anterior-de-una-función-de-aws-lambda-en-caso-de-errores-causados-por-un-nuevo-despliegue-cómo-puede-lograrlo-el-desarrollador-con-un-impacto-mínimo-en-los-usuarios) |
| 7 | [Una aplicación contiene dos componentes: uno que maneja las solicitudes HTTP y otro que maneja tareas de procesamiento en segundo plano. Cada componente debe escalar de forma independiente. El desarrollador desea desplegar esta aplicación utilizando AWS Elastic Beanstalk. ¿Cómo se debe desplegar esta aplicación, según estos requisitos?](#una-aplicación-contiene-dos-componentes-uno-que-maneja-las-solicitudes-http-y-otro-que-maneja-tareas-de-procesamiento-en-segundo-plano-cada-componente-debe-escalar-de-forma-independiente-el-desarrollador-desea-desplegar-esta-aplicación-utilizando-aws-elastic-beanstalk-cómo-se-debe-desplegar-esta-aplicación-según-estos-requisitos) |
| 8 | [Una empresa utiliza plantillas de AWS CloudFormation para desplegar recursos de AWS. La empresa necesita actualizar una de sus pilas de AWS CloudFormation. ¿Qué puede hacer la empresa para saber cómo afectarán los cambios a los recursos que se están ejecutando?](#una-empresa-utiliza-plantillas-de-aws-cloudformation-para-desplegar-recursos-de-aws-la-empresa-necesita-actualizar-una-de-sus-pilas-de-aws-cloudformation-qué-puede-hacer-la-empresa-para-saber-cómo-afectarán-los-cambios-a-los-recursos-que-se-están-ejecutando) |
| 9 | [Un desarrollador está creando una aplicación web sin servidor y mantiene diferentes ramas de código. El desarrollador desea evitar actualizar el endpoint de destino de Amazon API Gateway cada vez que se realiza un nuevo push de código. ¿Qué solución permitiría al desarrollador realizar un push de código de manera eficiente, sin necesidad de actualizar API Gateway?](#un-desarrollador-está-creando-una-aplicación-web-sin-servidor-y-mantiene-diferentes-ramas-de-código-el-desarrollador-desea-evitar-actualizar-el-endpoint-de-destino-de-amazon-api-gateway-cada-vez-que-se-realiza-un-nuevo-push-de-código-qué-solución-permitiría-al-desarrollador-realizar-un-push-de-código-de-manera-eficiente-sin-necesidad-de-actualizar-api-gateway) |
| 10 | [Una empresa de publicidad tiene un sitio web dinámico con mucho tráfico. La empresa desea migrar la infraestructura del sitio web a AWS para que AWS se encargue de todo excepto del desarrollo del sitio web. ¿Qué solución cumple MEJOR con estos requisitos?](#una-empresa-de-publicidad-tiene-un-sitio-web-dinámico-con-mucho-tráfico-la-empresa-desea-migrar-la-infraestructura-del-sitio-web-a-aws-para-que-aws-se-encargue-de-todo-excepto-del-desarrollo-del-sitio-web-qué-solución-cumple-mejor-con-estos-requisitos) |
| 11 | [El flujo de trabajo del proceso de lanzamiento de una aplicación requiere una aprobación manual antes de que el código se despliegue en el entorno de producción. ¿Cuál es la MEJOR manera de lograr esto utilizando AWS CodePipeline?](#el-flujo-de-trabajo-del-proceso-de-lanzamiento-de-una-aplicación-requiere-una-aprobación-manual-antes-de-que-el-código-se-despliegue-en-el-entorno-de-producción-cuál-es-la-mejor-manera-de-lograr-esto-utilizando-aws-codepipeline) |
| 12 | [Un desarrollador ha escrito una aplicación sin servidor utilizando varios servicios de AWS. La lógica de negocio está escrita como una función de Lambda que tiene dependencias de bibliotecas de terceros. Los endpoints de la función de Lambda se expondrán mediante Amazon API Gateway. La función de Lambda escribirá la información en Amazon DynamoDB. El desarrollador está listo para desplegar la aplicación, pero debe tener la capacidad de revertir. ¿Cómo se puede automatizar este despliegue, según estos requisitos?](#un-desarrollador-ha-escrito-una-aplicación-sin-servidor-utilizando-varios-servicios-de-aws-la-lógica-de-negocio-está-escrita-como-una-función-de-lambda-que-tiene-dependencias-de-bibliotecas-de-terceros-los-endpoints-de-la-función-de-lambda-se-expondrán-mediante-amazon-api-gateway-la-función-de-lambda-escribirá-la-información-en-amazon-dynamodb-el-desarrollador-está-listo-para-desplegar-la-aplicación-pero-debe-tener-la-capacidad-de-revertir-cómo-se-puede-automatizar-este-despliegue-según-estos-requisitos) |
| 13 | [Dado el código fuente de una función de AWS Lambda en el archivo local `store.py` que contiene una función handler llamada `get_store` y la siguiente plantilla de AWS CloudFormation. ¿Qué se debe hacer para preparar la plantilla de modo que pueda desplegarse usando el comando de la AWS CLI `aws cloudformation deploy`?](#dado-el-código-fuente-de-una-función-de-aws-lambda-en-el-archivo-local-storepy-que-contiene-una-función-handler-llamada-get_store-y-la-siguiente-plantilla-de-aws-cloudformation-qué-se-debe-hacer-para-preparar-la-plantilla-de-modo-que-pueda-desplegarse-usando-el-comando-de-la-aws-cli-aws-cloudformation-deploy) |
| 14 | [Un desarrollador ha creado una función de Lambda grande y el despliegue está fallando con el siguiente error: `ClientError: An error occurred (InvalidParameterValueException) when calling the CreateFunction operation: Unzipped size must be smaller than XXXXXXXXX bytes.`, donde `XXXXXXXXX` es el límite actual de Lambda. ¿Qué puede hacer el desarrollador para solucionar este problema?](#un-desarrollador-ha-creado-una-función-de-lambda-grande-y-el-despliegue-está-fallando-con-el-siguiente-error-clienterror-an-error-occurred-invalidparametervalueexception-when-calling-the-createfunction-operation-unzipped-size-must-be-smaller-than-xxxxxxxxx-bytes-donde-xxxxxxxxx-es-el-límite-actual-de-lambda-qué-puede-hacer-el-desarrollador-para-solucionar-este-problema) |
| 15 | [Un desarrollador está escribiendo una aplicación basada en Linux para ejecutarse en AWS Elastic Beanstalk. Los requisitos de la aplicación establecen que esta debe mantener su capacidad completa durante las actualizaciones y, al mismo tiempo, minimizar el costo. ¿Qué tipo de política de despliegue de Elastic Beanstalk debería especificar el desarrollador para el entorno?](#un-desarrollador-está-escribiendo-una-aplicación-basada-en-linux-para-ejecutarse-en-aws-elastic-beanstalk-los-requisitos-de-la-aplicación-establecen-que-esta-debe-mantener-su-capacidad-completa-durante-las-actualizaciones-y-al-mismo-tiempo-minimizar-el-costo-qué-tipo-de-política-de-despliegue-de-elastic-beanstalk-debería-especificar-el-desarrollador-para-el-entorno) |
| 16 | [¿Dónde debe colocarse el archivo `appspec.yml` para que AWS CodeDeploy funcione?](#dónde-debe-colocarse-el-archivo-appspecyml-para-que-aws-codedeploy-funcione) |
| 17 | [Un desarrollador está creando una función Lambda y usará bibliotecas externas que no están incluidas en las bibliotecas estándar de Lambda. ¿Qué acción minimizaría el tiempo de cómputo de Lambda consumido?](#un-desarrollador-está-creando-una-función-lambda-y-usará-bibliotecas-externas-que-no-están-incluidas-en-las-bibliotecas-estándar-de-lambda-qué-acción-minimizaría-el-tiempo-de-cómputo-de-lambda-consumido) |
| 18 | [Un cliente quiere desplegar su código fuente en un entorno de AWS Elastic Beanstalk. El cliente necesita realizar el despliegue con una interrupción mínima y solo debe usar instancias existentes para conservar los registros de acceso de la aplicación. ¿Qué política de despliegue cumpliría con estos requisitos?](#un-cliente-quiere-desplegar-su-código-fuente-en-un-entorno-de-aws-elastic-beanstalk-el-cliente-necesita-realizar-el-despliegue-con-una-interrupción-mínima-y-solo-debe-usar-instancias-existentes-para-conservar-los-registros-de-acceso-de-la-aplicación-qué-política-de-despliegue-cumpliría-con-estos-requisitos) |
| 19 | [Una función Lambda se empaqueta para su despliegue en múltiples entornos, incluidos desarrollo, pruebas, producción, etc. Cada entorno tiene un conjunto único de recursos, como bases de datos, etc. ¿Cómo puede la función Lambda usar los recursos del entorno actual?](#una-función-lambda-se-empaqueta-para-su-despliegue-en-múltiples-entornos-incluidos-desarrollo-pruebas-producción-etc-cada-entorno-tiene-un-conjunto-único-de-recursos-como-bases-de-datos-etc-cómo-puede-la-función-lambda-usar-los-recursos-del-entorno-actual) |
| 20 | [Una empresa quiere implementar integración continua para sus cargas de trabajo en AWS. La empresa quiere activar pruebas unitarias en su pipeline para los commits en su repositorio de código, y quiere recibir notificaciones de los eventos de falla en el pipeline. ¿Cómo se pueden cumplir estos requisitos?](#una-empresa-quiere-implementar-integración-continua-para-sus-cargas-de-trabajo-en-aws-la-empresa-quiere-activar-pruebas-unitarias-en-su-pipeline-para-los-commits-en-su-repositorio-de-código-y-quiere-recibir-notificaciones-de-los-eventos-de-falla-en-el-pipeline-cómo-se-pueden-cumplir-estos-requisitos) |
| 21 | [Para un despliegue con AWS CodeDeploy, ¿cuál es el orden de ejecución de los hooks en los despliegues in-place?](#para-un-despliegue-con-aws-codedeploy-cuál-es-el-orden-de-ejecución-de-los-hooks-en-los-despliegues-in-place) |
| 22 | [¿Cuáles son los pasos para usar la AWS CLI para lanzar una aplicación sin servidor basada en plantillas?](#cuáles-son-los-pasos-para-usar-la-aws-cli-para-lanzar-una-aplicación-sin-servidor-basada-en-plantillas) |
| 23 | [Una empresa ha desarrollado una nueva aplicación sin servidor usando funciones de AWS Lambda que se desplegará usando la CLI de AWS Serverless Application Model (AWS SAM). ¿Qué paso debería completar el desarrollador antes de desplegar la aplicación?](#una-empresa-ha-desarrollado-una-nueva-aplicación-sin-servidor-usando-funciones-de-aws-lambda-que-se-desplegará-usando-la-cli-de-aws-serverless-application-model-aws-sam-qué-paso-debería-completar-el-desarrollador-antes-de-desplegar-la-aplicación) |
| 24 | [Un desarrollador está actualizando una aplicación implementada en AWS Elastic Beanstalk. La nueva versión es incompatible con la versión anterior. Para implementar la actualización con éxito, se debe realizar un cambio total a la nueva versión actualizada en todas las instancias al mismo tiempo, con la capacidad de revertir los cambios en caso de que falle el despliegue de la nueva versión. ¿Cómo se puede lograr esto con la MENOR cantidad de tiempo de inactividad?](#un-desarrollador-está-actualizando-una-aplicación-implementada-en-aws-elastic-beanstalk-la-nueva-versión-es-incompatible-con-la-versión-anterior-para-implementar-la-actualización-con-éxito-se-debe-realizar-un-cambio-total-a-la-nueva-versión-actualizada-en-todas-las-instancias-al-mismo-tiempo-con-la-capacidad-de-revertir-los-cambios-en-caso-de-que-falle-el-despliegue-de-la-nueva-versión-cómo-se-puede-lograr-esto-con-la-menor-cantidad-de-tiempo-de-inactividad) |
| 25 | [Dada la siguiente plantilla de AWS CloudFormation. ¿Cuál es la forma MÁS eficiente de hacer referencia al nuevo bucket de Amazon S3 desde otra plantilla de AWS CloudFormation?](#dada-la-siguiente-plantilla-de-aws-cloudformation-cuál-es-la-forma-más-eficiente-de-hacer-referencia-al-nuevo-bucket-de-amazon-s3-desde-otra-plantilla-de-aws-cloudformation) |
| 26 | [Un desarrollador está usando AWS CodeDeploy para implementar una aplicación que se ejecuta en Amazon EC2. El desarrollador quiere cambiar los permisos de archivo de un archivo de despliegue específico. ¿Qué evento del ciclo de vida debe usar el desarrollador para cumplir con este requisito?](#un-desarrollador-está-usando-aws-codedeploy-para-implementar-una-aplicación-que-se-ejecuta-en-amazon-ec2-el-desarrollador-quiere-cambiar-los-permisos-de-archivo-de-un-archivo-de-despliegue-específico-qué-evento-del-ciclo-de-vida-debe-usar-el-desarrollador-para-cumplir-con-este-requisito) |
| 27 | [Un desarrollador está creando un script para automatizar el proceso de despliegue de una aplicación sin servidor. El desarrollador quiere usar una plantilla existente de AWS Serverless Application Model (AWS SAM) para la aplicación. ¿Qué debe usar el desarrollador para el proyecto? (Elija DOS)](#un-desarrollador-está-creando-un-script-para-automatizar-el-proceso-de-despliegue-de-una-aplicación-sin-servidor-el-desarrollador-quiere-usar-una-plantilla-existente-de-aws-serverless-application-model-aws-sam-para-la-aplicación-qué-debe-usar-el-desarrollador-para-el-proyecto-elija-dos) |
| 28 | [Un equipo de desarrollo usa AWS Elastic Beanstalk para el despliegue de aplicaciones. El equipo ha configurado la política de ciclo de vida de versiones de la aplicación para limitar el número de versiones de la aplicación a 25. Sin embargo, incluso con la política de ciclo de vida, el source bundle se elimina del bucket de origen de Amazon S3. ¿Qué debe hacer un desarrollador en la configuración del ciclo de vida de versiones de la aplicación de Elastic Beanstalk para conservar el código fuente en el bucket de S3?](#un-equipo-de-desarrollo-usa-aws-elastic-beanstalk-para-el-despliegue-de-aplicaciones-el-equipo-ha-configurado-la-política-de-ciclo-de-vida-de-versiones-de-la-aplicación-para-limitar-el-número-de-versiones-de-la-aplicación-a-25-sin-embargo-incluso-con-la-política-de-ciclo-de-vida-el-source-bundle-se-elimina-del-bucket-de-origen-de-amazon-s3-qué-debe-hacer-un-desarrollador-en-la-configuración-del-ciclo-de-vida-de-versiones-de-la-aplicación-de-elastic-beanstalk-para-conservar-el-código-fuente-en-el-bucket-de-s3) |
| 29 | [A un desarrollador se le proporciona una URL de clonación HTTPS para un repositorio de AWS CodeCommit. ¿Qué es necesario configurar antes de clonar este repositorio?](#a-un-desarrollador-se-le-proporciona-una-url-de-clonación-https-para-un-repositorio-de-aws-codecommit-qué-es-necesario-configurar-antes-de-clonar-este-repositorio) |
| 30 | [Un desarrollador convirtió un programa existente en una función de AWS Lambda en la consola. El programa se ejecuta correctamente en una laptop local, pero muestra un error `Unable to import module` al probarse en la consola de Lambda. ¿Cuál de las siguientes acciones puede corregir el error?](#un-desarrollador-convirtió-un-programa-existente-en-una-función-de-aws-lambda-en-la-consola-el-programa-se-ejecuta-correctamente-en-una-laptop-local-pero-muestra-un-error-unable-to-import-module-al-probarse-en-la-consola-de-lambda-cuál-de-las-siguientes-acciones-puede-corregir-el-error) |
| 31 | [Un desarrollador necesita administrar la infraestructura de AWS como código y debe poder desplegar múltiples copias idénticas de la infraestructura, preparar cambios (stage) y revertir a versiones anteriores. ¿Qué enfoque cumple con estos requisitos?](#un-desarrollador-necesita-administrar-la-infraestructura-de-aws-como-código-y-debe-poder-desplegar-múltiples-copias-idénticas-de-la-infraestructura-preparar-cambios-stage-y-revertir-a-versiones-anteriores-qué-enfoque-cumple-con-estos-requisitos) |
| 32 | [Un desarrollador necesita desplegar una aplicación que se ejecuta en AWS Fargate usando Amazon ECS. La aplicación tiene variables de entorno que deben pasarse a un contenedor para que la aplicación se inicialice. ¿Cómo se deben pasar las variables de entorno al contenedor?](#un-desarrollador-necesita-desplegar-una-aplicación-que-se-ejecuta-en-aws-fargate-usando-amazon-ecs-la-aplicación-tiene-variables-de-entorno-que-deben-pasarse-a-un-contenedor-para-que-la-aplicación-se-inicialice-cómo-se-deben-pasar-las-variables-de-entorno-al-contenedor) |
| 33 | [Una empresa ejecuta pipelines de integración continua/entrega continua (CI/CD) para su aplicación en AWS CodePipeline. Un desarrollador debe escribir pruebas unitarias y ejecutarlas como parte de los pipelines antes de preparar (staging) los artefactos para pruebas. ¿Cómo debería incorporar el desarrollador las pruebas unitarias como parte de los pipelines de CI/CD?](#una-empresa-ejecuta-pipelines-de-integración-continuaentrega-continua-cicd-para-su-aplicación-en-aws-codepipeline-un-desarrollador-debe-escribir-pruebas-unitarias-y-ejecutarlas-como-parte-de-los-pipelines-antes-de-preparar-staging-los-artefactos-para-pruebas-cómo-debería-incorporar-el-desarrollador-las-pruebas-unitarias-como-parte-de-los-pipelines-de-cicd) |
| 34 | [Un desarrollador ha escrito código para una aplicación y quiere compartirlo con otros desarrolladores del equipo para recibir comentarios. El código compartido de la aplicación debe almacenarse a largo plazo con múltiples versiones y seguimiento de cambios por lotes. ¿Qué servicio de AWS debería usar el desarrollador?](#un-desarrollador-ha-escrito-código-para-una-aplicación-y-quiere-compartirlo-con-otros-desarrolladores-del-equipo-para-recibir-comentarios-el-código-compartido-de-la-aplicación-debe-almacenarse-a-largo-plazo-con-múltiples-versiones-y-seguimiento-de-cambios-por-lotes-qué-servicio-de-aws-debería-usar-el-desarrollador) |
| 35 | [Un desarrollador está preparando un paquete de despliegue con AWS CloudFormation. El paquete consta de dos plantillas separadas: una para la infraestructura y otra para la aplicación. La aplicación debe estar dentro de la VPC creada a partir de la plantilla de infraestructura. ¿Cómo puede la pila de la aplicación hacer referencia a la VPC creada a partir de la plantilla de infraestructura?](#un-desarrollador-está-preparando-un-paquete-de-despliegue-con-aws-cloudformation-el-paquete-consta-de-dos-plantillas-separadas-una-para-la-infraestructura-y-otra-para-la-aplicación-la-aplicación-debe-estar-dentro-de-la-vpc-creada-a-partir-de-la-plantilla-de-infraestructura-cómo-puede-la-pila-de-la-aplicación-hacer-referencia-a-la-vpc-creada-a-partir-de-la-plantilla-de-infraestructura) |
| 36 | [Un equipo de desarrollo decide adoptar un proceso de integración continua/entrega continua (CI/CD) usando AWS CodePipeline y AWS CodeCommit para una nueva aplicación. Sin embargo, la gerencia quiere que una persona revise y apruebe el código antes de que se despliegue en producción. ¿Cómo puede el equipo de desarrollo agregar un aprobador manual al pipeline de CI/CD?](#un-equipo-de-desarrollo-decide-adoptar-un-proceso-de-integración-continuaentrega-continua-cicd-usando-aws-codepipeline-y-aws-codecommit-para-una-nueva-aplicación-sin-embargo-la-gerencia-quiere-que-una-persona-revise-y-apruebe-el-código-antes-de-que-se-despliegue-en-producción-cómo-puede-el-equipo-de-desarrollo-agregar-un-aprobador-manual-al-pipeline-de-cicd) |
| 37 | [Una empresa ha implementado AWS CodeDeploy como parte de su stack de CI/CD nativo de la nube. La empresa habilita los rollbacks automáticos al desplegar una nueva versión de una aplicación web popular in-place en Amazon EC2. ¿Qué ocurre si el despliegue de la nueva versión falla debido a una regresión de código?](#una-empresa-ha-implementado-aws-codedeploy-como-parte-de-su-stack-de-cicd-nativo-de-la-nube-la-empresa-habilita-los-rollbacks-automáticos-al-desplegar-una-nueva-versión-de-una-aplicación-web-popular-in-place-en-amazon-ec2-qué-ocurre-si-el-despliegue-de-la-nueva-versión-falla-debido-a-una-regresión-de-código) |
| 38 | [Una empresa ha implementado AWS CodePipeline para automatizar sus pipelines de lanzamiento. El equipo de desarrollo está escribiendo una función de AWS Lambda que enviará notificaciones sobre los cambios de estado de cada una de las acciones en las etapas. ¿Qué pasos se deben seguir para asociar la función de Lambda con la fuente de eventos?](#una-empresa-ha-implementado-aws-codepipeline-para-automatizar-sus-pipelines-de-lanzamiento-el-equipo-de-desarrollo-está-escribiendo-una-función-de-aws-lambda-que-enviará-notificaciones-sobre-los-cambios-de-estado-de-cada-una-de-las-acciones-en-las-etapas-qué-pasos-se-deben-seguir-para-asociar-la-función-de-lambda-con-la-fuente-de-eventos) |
| 39 | [Un Developer ha creado una aplicación que se ejecuta en AWS Lambda usando AWS Serverless Application Model (AWS SAM). ¿Cuál es el orden de ejecución correcto para desplegar la aplicación con éxito?](#un-developer-ha-creado-una-aplicación-que-se-ejecuta-en-aws-lambda-usando-aws-serverless-application-model-aws-sam-cuál-es-el-orden-de-ejecución-correcto-para-desplegar-la-aplicación-con-éxito) |
| 40 | [Un equipo de desarrollo quiere compilar y desplegar de inmediato una aplicación siempre que haya un cambio en el código fuente. ¿Qué enfoques se podrían usar para activar el despliegue? (Elija DOS)](#un-equipo-de-desarrollo-quiere-compilar-y-desplegar-de-inmediato-una-aplicación-siempre-que-haya-un-cambio-en-el-código-fuente-qué-enfoques-se-podrían-usar-para-activar-el-despliegue-elija-dos) |
| 41 | [Una empresa minorista en línea ha desplegado una aplicación sin servidor con AWS Lambda, Amazon API Gateway, Amazon S3 y Amazon DynamoDB usando AWS CloudFormation. La empresa lanzó una nueva versión con mejoras importantes en la función de Lambda y desplegó el lanzamiento en producción. Posteriormente, la aplicación dejó de funcionar. ¿Qué solución debería restablecer la aplicación lo más rápido posible?](#una-empresa-minorista-en-línea-ha-desplegado-una-aplicación-sin-servidor-con-aws-lambda-amazon-api-gateway-amazon-s3-y-amazon-dynamodb-usando-aws-cloudformation-la-empresa-lanzó-una-nueva-versión-con-mejoras-importantes-en-la-función-de-lambda-y-desplegó-el-lanzamiento-en-producción-posteriormente-la-aplicación-dejó-de-funcionar-qué-solución-debería-restablecer-la-aplicación-lo-más-rápido-posible) |
| 42 | [Una empresa está creando un servicio REST usando Amazon API Gateway con integración de AWS Lambda. El servicio debe ejecutar diferentes versiones con fines de prueba. ¿Cuál sería la MEJOR forma de lograrlo?](#una-empresa-está-creando-un-servicio-rest-usando-amazon-api-gateway-con-integración-de-aws-lambda-el-servicio-debe-ejecutar-diferentes-versiones-con-fines-de-prueba-cuál-sería-la-mejor-forma-de-lograrlo) |
| 43 | [Un equipo de Desarrollo desea migrar el código de su aplicación existente de un repositorio de GitHub a AWS CodeCommit. ¿Qué es necesario crear antes de poder migrar un repositorio clonado a CodeCommit mediante HTTPS?](#un-equipo-de-desarrollo-desea-migrar-el-código-de-su-aplicación-existente-de-un-repositorio-de-github-a-aws-codecommit-qué-es-necesario-crear-antes-de-poder-migrar-un-repositorio-clonado-a-codecommit-mediante-https) |
| 44 | [¿Cuáles de las siguientes plataformas son compatibles con Elastic Beanstalk? (Elija DOS)](#cuáles-de-las-siguientes-plataformas-son-compatibles-con-elastic-beanstalk-elija-dos) |
| 45 | [¿Qué fragmento de código a continuación devuelve la URL de un sitio web con balanceo de carga creado en CloudFormation con un recurso `AWS::ElasticLoadBalancing::LoadBalancer` de nombre `ElasticLoad Balancer`?](#qué-fragmento-de-código-a-continuación-devuelve-la-url-de-un-sitio-web-con-balanceo-de-carga-creado-en-cloudformation-con-un-recurso-awselasticloadbalancingloadbalancer-de-nombre-elasticload-balancer) |
| 46 | [¿Qué sucede, por defecto, cuando no se puede crear uno de los recursos de un stack de CloudFormation?](#qué-sucede-por-defecto-cuando-no-se-puede-crear-uno-de-los-recursos-de-un-stack-de-cloudformation) |
| 47 | [Las instancias de EC2 se lanzan a partir de Amazon Machine Images (AMIs). Una AMI pública determinada puede:](#las-instancias-de-ec2-se-lanzan-a-partir-de-amazon-machine-images-amis-una-ami-pública-determinada-puede) |
| 48 | [¿Qué productos y características de AWS pueden ser desplegados por Elastic Beanstalk? (Elija TRES)](#qué-productos-y-características-de-aws-pueden-ser-desplegados-por-elastic-beanstalk-elija-tres) |
| 49 | [Un equipo de desarrolladores debe migrar una aplicación que se ejecuta dentro de un entorno de AWS Elastic Beanstalk de un Classic Load Balancer a un Application Load Balancer. ¿Qué pasos se deben seguir para lograr la tarea usando la AWS Management Console?](#un-equipo-de-desarrolladores-debe-migrar-una-aplicación-que-se-ejecuta-dentro-de-un-entorno-de-aws-elastic-beanstalk-de-un-classic-load-balancer-a-un-application-load-balancer-qué-pasos-se-deben-seguir-para-lograr-la-tarea-usando-la-aws-management-console) |
| 50 | [Una empresa necesita un sistema de control de versiones para el desarrollo colaborativo de software. Las características del sistema deben incluir lo siguiente: soporte para lotes de cambios en múltiples archivos, ramificación (branching) en paralelo y seguimiento de versiones. ¿Qué servicio de AWS cumplirá estos requisitos?](#una-empresa-necesita-un-sistema-de-control-de-versiones-para-el-desarrollo-colaborativo-de-software-las-características-del-sistema-deben-incluir-lo-siguiente-soporte-para-lotes-de-cambios-en-múltiples-archivos-ramificación-branching-en-paralelo-y-seguimiento-de-versiones-qué-servicio-de-aws-cumplirá-estos-requisitos) |
| 51 | [Una empresa utiliza sistemas de integración continua y entrega continua. Un desarrollador ahora necesita automatizar el despliegue de un paquete de software tanto en instancias de Amazon EC2 como en servidores virtuales que se ejecutan on-premises. ¿Qué servicio de AWS se debe usar para lograrlo?](#una-empresa-utiliza-sistemas-de-integración-continua-y-entrega-continua-un-desarrollador-ahora-necesita-automatizar-el-despliegue-de-un-paquete-de-software-tanto-en-instancias-de-amazon-ec2-como-en-servidores-virtuales-que-se-ejecutan-on-premises-qué-servicio-de-aws-se-debe-usar-para-lograrlo) |
| 52 | [Un desarrollador está intentando desplegar una aplicación serverless usando AWS CodeDeploy. La aplicación fue actualizada y necesita volver a desplegarse. ¿Qué archivo necesita actualizar el desarrollador para propagar ese cambio a través de CodeDeploy?](#un-desarrollador-está-intentando-desplegar-una-aplicación-serverless-usando-aws-codedeploy-la-aplicación-fue-actualizada-y-necesita-volver-a-desplegarse-qué-archivo-necesita-actualizar-el-desarrollador-para-propagar-ese-cambio-a-través-de-codedeploy) |
| 53 | [Un desarrollador está creando una plantilla que usa AWS CloudFormation para desplegar una aplicación. Esta aplicación es serverless y utiliza Amazon API Gateway, Amazon DynamoDB y AWS Lambda. ¿Qué herramienta debe usar el desarrollador para definir una sintaxis simplificada que exprese recursos serverless?](#un-desarrollador-está-creando-una-plantilla-que-usa-aws-cloudformation-para-desplegar-una-aplicación-esta-aplicación-es-serverless-y-utiliza-amazon-api-gateway-amazon-dynamodb-y-aws-lambda-qué-herramienta-debe-usar-el-desarrollador-para-definir-una-sintaxis-simplificada-que-exprese-recursos-serverless) |
| 54 | [Para incluir objetos definidos por AWS Serverless Application Model (SAM) en una plantilla de AWS CloudFormation, además de `Resources`, ¿qué sección DEBE incluirse en la raíz del documento?](#para-incluir-objetos-definidos-por-aws-serverless-application-model-sam-en-una-plantilla-de-aws-cloudformation-además-de-resources-qué-sección-debe-incluirse-en-la-raíz-del-documento) |
| 55 | [Un desarrollador creó especificaciones de configuración para una aplicación de AWS Elastic Beanstalk en un archivo llamado healthcheckurl.yaml en el `.ebextensions/directory` del paquete de origen de su aplicación. El archivo contiene lo siguiente: Después de que la aplicación se inicia, el health check no se ejecuta en la ruta correcta, aunque esta es válida. ¿Qué se puede hacer para corregir este archivo de configuración?](#un-desarrollador-creó-especificaciones-de-configuración-para-una-aplicación-de-aws-elastic-beanstalk-en-un-archivo-llamado-healthcheckurlyaml-en-el-ebextensionsdirectory-del-paquete-de-origen-de-su-aplicación-el-archivo-contiene-lo-siguiente-después-de-que-la-aplicación-se-inicia-el-health-check-no-se-ejecuta-en-la-ruta-correcta-aunque-esta-es-válida-qué-se-puede-hacer-para-corregir-este-archivo-de-configuración) |
| 56 | [Una empresa tiene tres entornos distintos: Development, QA y Production. La empresa quiere implementar su código primero en el entorno de Development, luego en QA y después en Production. ¿Qué servicio de AWS se puede usar para cumplir este requisito?](#una-empresa-tiene-tres-entornos-distintos-development-qa-y-production-la-empresa-quiere-implementar-su-código-primero-en-el-entorno-de-development-luego-en-qa-y-después-en-production-qué-servicio-de-aws-se-puede-usar-para-cumplir-este-requisito) |
| 57 | [En un entorno Docker multicontenedor en AWS Elastic Beanstalk, ¿qué se requiere para configurar las instancias de contenedor del entorno?](#en-un-entorno-docker-multicontenedor-en-aws-elastic-beanstalk-qué-se-requiere-para-configurar-las-instancias-de-contenedor-del-entorno) |
| 58 | [Una empresa tiene un sitio web desarrollado en PHP y WordPress que se lanza mediante AWS Elastic Beanstalk. Hay una nueva versión del sitio web que se debe implementar en el entorno de Elastic Beanstalk. La empresa no puede tolerar que el sitio web quede fuera de línea si falla una actualización. Los despliegues deben tener un impacto mínimo y permitir un rollback lo antes posible. ¿Qué método de despliegue se debe usar?](#una-empresa-tiene-un-sitio-web-desarrollado-en-php-y-wordpress-que-se-lanza-mediante-aws-elastic-beanstalk-hay-una-nueva-versión-del-sitio-web-que-se-debe-implementar-en-el-entorno-de-elastic-beanstalk-la-empresa-no-puede-tolerar-que-el-sitio-web-quede-fuera-de-línea-si-falla-una-actualización-los-despliegues-deben-tener-un-impacto-mínimo-y-permitir-un-rollback-lo-antes-posible-qué-método-de-despliegue-se-debe-usar) |
| 59 | [Un desarrollador escribe una función de AWS Lambda y carga el código en un archivo `.ZIP` en Amazon S3. El desarrollador realiza cambios en el código y carga un nuevo archivo `.ZIP` en Amazon S3. Sin embargo, Lambda ejecuta el código anterior. ¿Cómo puede el desarrollador solucionarlo de la forma MENOS disruptiva?](#un-desarrollador-escribe-una-función-de-aws-lambda-y-carga-el-código-en-un-archivo-zip-en-amazon-s3-el-desarrollador-realiza-cambios-en-el-código-y-carga-un-nuevo-archivo-zip-en-amazon-s3-sin-embargo-lambda-ejecuta-el-código-anterior-cómo-puede-el-desarrollador-solucionarlo-de-la-forma-menos-disruptiva) |
| 60 | [A un desarrollador se le ha pedido realizar cambios en el código fuente de una función de AWS Lambda. La función se administra mediante una plantilla de AWS CloudFormation. La plantilla está configurada para cargar el código fuente desde un bucket de Amazon S3. El desarrollador creó manualmente un paquete de despliegue en un archivo `.ZIP` que contiene los cambios y colocó el archivo en la ubicación correcta de Amazon S3. Cuando se invoca la función, los cambios de código no se han aplicado. ¿Qué paso se requiere para actualizar la función con los cambios?](#a-un-desarrollador-se-le-ha-pedido-realizar-cambios-en-el-código-fuente-de-una-función-de-aws-lambda-la-función-se-administra-mediante-una-plantilla-de-aws-cloudformation-la-plantilla-está-configurada-para-cargar-el-código-fuente-desde-un-bucket-de-amazon-s3-el-desarrollador-creó-manualmente-un-paquete-de-despliegue-en-un-archivo-zip-que-contiene-los-cambios-y-colocó-el-archivo-en-la-ubicación-correcta-de-amazon-s3-cuando-se-invoca-la-función-los-cambios-de-código-no-se-han-aplicado-qué-paso-se-requiere-para-actualizar-la-función-con-los-cambios) |
| 61 | [Una aplicación de AWS Elastic Beanstalk necesita implementarse en varias regiones y requiere una Amazon Machine Image (AMI) diferente en cada región. ¿Qué clave de la plantilla de AWS CloudFormation se puede usar para especificar la AMI correcta para cada región?](#una-aplicación-de-aws-elastic-beanstalk-necesita-implementarse-en-varias-regiones-y-requiere-una-amazon-machine-image-ami-diferente-en-cada-región-qué-clave-de-la-plantilla-de-aws-cloudformation-se-puede-usar-para-especificar-la-ami-correcta-para-cada-región) |
| 62 | [Un desarrollador debe implementar una nueva función de AWS Lambda mediante una plantilla de AWS CloudFormation. ¿Qué procedimientos implementarán una función Lambda? (Seleccione DOS)](#un-desarrollador-debe-implementar-una-nueva-función-de-aws-lambda-mediante-una-plantilla-de-aws-cloudformation-qué-procedimientos-implementarán-una-función-lambda-seleccione-dos) |
| 63 | [¿Cómo se deben utilizar las bibliotecas personalizadas en AWS Lambda?](#cómo-se-deben-utilizar-las-bibliotecas-personalizadas-en-aws-lambda) |
| 64 | [Un desarrollador está escribiendo un microservicio de procesamiento de imágenes en AWS Lambda. El servicio depende de varias bibliotecas que no están disponibles en el entorno de ejecución de Lambda. ¿Qué estrategia debe seguir el desarrollador para crear el paquete de despliegue de Lambda?](#un-desarrollador-está-escribiendo-un-microservicio-de-procesamiento-de-imágenes-en-aws-lambda-el-servicio-depende-de-varias-bibliotecas-que-no-están-disponibles-en-el-entorno-de-ejecución-de-lambda-qué-estrategia-debe-seguir-el-desarrollador-para-crear-el-paquete-de-despliegue-de-lambda) |
| 65 | [Una empresa necesita un servicio de control de código fuente totalmente administrado que funcione en AWS. El servicio debe garantizar que el control de revisiones sincronice múltiples repositorios distribuidos intercambiando conjuntos de cambios de par a par (peer-to-peer). Todos los usuarios necesitan trabajar de forma productiva incluso cuando no están conectados a una red. ¿Qué servicio de control de código fuente se debe usar?](#una-empresa-necesita-un-servicio-de-control-de-código-fuente-totalmente-administrado-que-funcione-en-aws-el-servicio-debe-garantizar-que-el-control-de-revisiones-sincronice-múltiples-repositorios-distribuidos-intercambiando-conjuntos-de-cambios-de-par-a-par-peer-to-peer-todos-los-usuarios-necesitan-trabajar-de-forma-productiva-incluso-cuando-no-están-conectados-a-una-red-qué-servicio-de-control-de-código-fuente-se-debe-usar) |
| 66 | [Una empresa tiene múltiples desarrolladores ubicados en todo el mundo que actualizan código de forma incremental para un proyecto de desarrollo. Cuando los desarrolladores cargan código de forma concurrente, la conexión a internet es lenta y toma mucho tiempo cargar el código para desplegarlo en AWS Elastic Beanstalk. ¿Qué paso dará como resultado un tiempo mínimo de carga y despliegue con la MENOR cantidad de esfuerzo administrativo?](#una-empresa-tiene-múltiples-desarrolladores-ubicados-en-todo-el-mundo-que-actualizan-código-de-forma-incremental-para-un-proyecto-de-desarrollo-cuando-los-desarrolladores-cargan-código-de-forma-concurrente-la-conexión-a-internet-es-lenta-y-toma-mucho-tiempo-cargar-el-código-para-desplegarlo-en-aws-elastic-beanstalk-qué-paso-dará-como-resultado-un-tiempo-mínimo-de-carga-y-despliegue-con-la-menor-cantidad-de-esfuerzo-administrativo) |
| 67 | [Una empresa tiene una plantilla de AWS CloudFormation almacenada como un solo archivo. La plantilla puede lanzar y crear una pila de infraestructura completa. ¿Qué mejor práctica aumentaría la mantenibilidad de la plantilla?](#una-empresa-tiene-una-plantilla-de-aws-cloudformation-almacenada-como-un-solo-archivo-la-plantilla-puede-lanzar-y-crear-una-pila-de-infraestructura-completa-qué-mejor-práctica-aumentaría-la-mantenibilidad-de-la-plantilla) |
| 68 | [AWS CodeBuild compila el código de una aplicación, crea la imagen de Docker, la envía a Amazon Elastic Container Registry (Amazon ECR) y etiqueta la imagen con un identificador único. Si los desarrolladores ya tienen la AWS CLI configurada en sus estaciones de trabajo, ¿cómo se pueden descargar (pull) las imágenes de Docker a las estaciones de trabajo?](#aws-codebuild-compila-el-código-de-una-aplicación-crea-la-imagen-de-docker-la-envía-a-amazon-elastic-container-registry-amazon-ecr-y-etiqueta-la-imagen-con-un-identificador-único-si-los-desarrolladores-ya-tienen-la-aws-cli-configurada-en-sus-estaciones-de-trabajo-cómo-se-pueden-descargar-pull-las-imágenes-de-docker-a-las-estaciones-de-trabajo) |
| 69 | [Un desarrollador ha creado una aplicación web y quiere desplegarla rápidamente en un servidor Tomcat en AWS. El desarrollador quiere evitar tener que administrar la infraestructura subyacente. ¿Cuál es la forma más fácil de desplegar la aplicación, según estos requisitos?](#un-desarrollador-ha-creado-una-aplicación-web-y-quiere-desplegarla-rápidamente-en-un-servidor-tomcat-en-aws-el-desarrollador-quiere-evitar-tener-que-administrar-la-infraestructura-subyacente-cuál-es-la-forma-más-fácil-de-desplegar-la-aplicación-según-estos-requisitos) |
| 70 | [Un equipo de desarrollo está usando AWS Elastic Beanstalk para desplegar una aplicación de dos capas que consta de una capa web con balanceo de carga y una capa de base de datos de Amazon RDS en producción. El equipo desea separar la instancia de RDS de Elastic Beanstalk. ¿Cómo se puede lograr esto?](#un-equipo-de-desarrollo-está-usando-aws-elastic-beanstalk-para-desplegar-una-aplicación-de-dos-capas-que-consta-de-una-capa-web-con-balanceo-de-carga-y-una-capa-de-base-de-datos-de-amazon-rds-en-producción-el-equipo-desea-separar-la-instancia-de-rds-de-elastic-beanstalk-cómo-se-puede-lograr-esto) |
| 71 | [Cuando un desarrollador intenta ejecutar un proyecto de AWS CodeBuild, este genera un error porque la longitud de todas las variables de entorno excede el límite del máximo combinado de caracteres. ¿Cuál es la solución recomendada?](#cuando-un-desarrollador-intenta-ejecutar-un-proyecto-de-aws-codebuild-este-genera-un-error-porque-la-longitud-de-todas-las-variables-de-entorno-excede-el-límite-del-máximo-combinado-de-caracteres-cuál-es-la-solución-recomendada) |
| 72 | [Un desarrollador debe desplegar de manera repetida y consistente una API RESTful sin servidor en AWS. ¿Qué técnicas funcionarán? (Elija DOS)](#un-desarrollador-debe-desplegar-de-manera-repetida-y-consistente-una-api-restful-sin-servidor-en-aws-qué-técnicas-funcionarán-elija-dos) |
| 73 | [Una empresa está usando Amazon API Gateway para administrar el acceso a un conjunto de microservicios implementados como funciones de AWS Lambda. Tras un reporte de error, la empresa realiza un cambio menor que rompe la compatibilidad en una de las APIs. Para evitar afectar a los clientes existentes cuando se despliegue la nueva API, la empresa quiere dar a los clientes seis meses para migrar de v1 a v2. ¿Qué enfoque debe usar el desarrollador para manejar este cambio?](#una-empresa-está-usando-amazon-api-gateway-para-administrar-el-acceso-a-un-conjunto-de-microservicios-implementados-como-funciones-de-aws-lambda-tras-un-reporte-de-error-la-empresa-realiza-un-cambio-menor-que-rompe-la-compatibilidad-en-una-de-las-apis-para-evitar-afectar-a-los-clientes-existentes-cuando-se-despliegue-la-nueva-api-la-empresa-quiere-dar-a-los-clientes-seis-meses-para-migrar-de-v1-a-v2-qué-enfoque-debe-usar-el-desarrollador-para-manejar-este-cambio) |
| 74 | [¿Dónde debe colocarse un archivo de configuración de Elastic Beanstalk llamado `healthcheckur1.config` en el paquete de código fuente de la aplicación?](#dónde-debe-colocarse-un-archivo-de-configuración-de-elastic-beanstalk-llamado-healthcheckur1config-en-el-paquete-de-código-fuente-de-la-aplicación) |

### Una empresa utiliza una herramienta de terceros para compilar, agrupar y empaquetar sus aplicaciones de forma local (on-premises) y almacenarlas localmente. La empresa utiliza instancias de Amazon EC2 para ejecutar sus aplicaciones front-end. ¿Cómo se puede implementar una aplicación desde el sistema de control de código fuente en las instancias EC2?

- [ ] Usar AWS CodeDeploy y apuntarlo al almacenamiento local para implementar directamente un paquete en formato zip, tar o tar.gz.
- [x] Cargar el paquete en un bucket de Amazon S3 y especificar la ubicación de S3 al realizar una implementación con AWS CodeDeploy.
- [ ] Crear un repositorio con AWS CodeCommit para activar automáticamente una implementación en las instancias EC2.
- [ ] Usar AWS CodeBuild para implementar automáticamente la última compilación en las últimas instancias EC2.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe ampliar una aplicación existente basada en AWS Serverless Application Model (AWS SAM). El desarrollador ha utilizado AWS SAM CLI para crear el proyecto. El proyecto contiene diferentes funciones de AWS Lambda. ¿Qué combinación de comandos debe usar el desarrollador para volver a implementar la aplicación de AWS SAM? (Seleccione DOS)

- [ ] `sam init`.
- [ ] `sam validate`.
- [x] `sam build`.
- [x] `sam deploy`.
- [ ] `sam publish`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación implementada en AWS Elastic Beanstalk experimenta mayores tasas de error durante las implementaciones de nuevas versiones de la aplicación, lo que resulta en una degradación del servicio para los usuarios. El equipo de desarrollo cree que esto se debe a la reducción de capacidad durante los pasos de la implementación. El equipo desea cambiar la configuración de la política de implementación del entorno a una opción que mantenga la capacidad total durante la implementación utilizando las instancias existentes. ¿Qué política de implementación cumplirá con estos requisitos utilizando las instancias existentes?

- [ ] All at once.
- [ ] Rolling.
- [x] Rolling with additional batch.
- [ ] Immutable.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está realizando cambios en una aplicación personalizada que actualmente utiliza AWS Elastic Beanstalk. Una vez que el desarrollador completa los cambios, ¿qué soluciones actualizarán el entorno de Elastic Beanstalk con la nueva versión de la aplicación? (Elija DOS)

- [x] Empaquetar el código de la aplicación en un archivo `.zip`, cargarlo y luego implementar la aplicación empaquetada desde la AWS Management Console.
- [ ] Empaquetar el código de la aplicación en un archivo `.tar`, crear una nueva versión de la aplicación desde la AWS Management Console y luego actualizar el entorno mediante AWS CLI.
- [ ] Empaquetar el código de la aplicación en un archivo `.tar`, y cargar e implementar la aplicación empaquetada desde la AWS Management Console.
- [x] Empaquetar el código de la aplicación en un archivo `.zip`, crear una nueva versión de la aplicación a partir de la aplicación empaquetada mediante AWS CLI y luego actualizar el entorno mediante AWS CLI.
- [ ] Empaquetar el código de la aplicación en un archivo `.zip`, crear una nueva versión de la aplicación desde la AWS Management Console y luego reconstruir el entorno mediante AWS CLI.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita implementar una nueva versión en una aplicación de AWS Elastic Beanstalk. ¿Cómo puede el desarrollador lograr esta tarea?

- [x] Cargar e implementar la nueva versión de la aplicación en la consola de Elastic Beanstalk.
- [ ] Usar el comando de CLI eb init para implementar una nueva versión.
- [ ] Terminar el entorno actual de Elastic Beanstalk y crear uno nuevo.
- [ ] Modificar la carpeta ebextensions para agregar una opción source a services.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador desea tener la capacidad de revertir a una versión anterior de una función de AWS Lambda en caso de errores causados por un nuevo despliegue. ¿Cómo puede lograrlo el desarrollador con un impacto MÍNIMO en los usuarios?

- [ ] Cambiar la aplicación para que use un alias que apunte a la versión actual. Desplegar la nueva versión del código. Actualizar el alias para que use la versión recién desplegada. Si se encuentran demasiados errores, apuntar el alias de nuevo a la versión anterior.
- [x] Cambiar la aplicación para que use un alias que apunte a la versión actual. Desplegar la nueva versión del código. Actualizar el alias para dirigir el 10 % de los usuarios a la versión recién desplegada. Si se encuentran demasiados errores, enviar el 100 % del tráfico a la versión anterior.
- [ ] No realizar ningún cambio en la aplicación. Desplegar la nueva versión del código. Si se encuentran demasiados errores, apuntar la aplicación de nuevo a la versión anterior usando el número de versión en el Amazon Resource Name (ARN).
- [ ] Crear tres alias: new, existing y router. Apuntar el alias existing a la versión actual. Hacer que el alias router dirija el 100 % de los usuarios al alias existing. Actualizar la aplicación para que use el alias router. Desplegar la nueva versión del código. Apuntar el alias new a esta versión. Actualizar el alias router para dirigir el 10 % de los usuarios al alias new. Si se encuentran demasiados errores, enviar el 100 % del tráfico al alias existing.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación contiene dos componentes: uno que maneja las solicitudes HTTP y otro que maneja tareas de procesamiento en segundo plano. Cada componente debe escalar de forma independiente. El desarrollador desea desplegar esta aplicación utilizando AWS Elastic Beanstalk. ¿Cómo se debe desplegar esta aplicación, según estos requisitos?

- [ ] Desplegar la aplicación en un único entorno de Elastic Beanstalk.
- [x] Desplegar cada componente en un entorno de Elastic Beanstalk independiente.
- [ ] Usar varios entornos de Elastic Beanstalk para el componente HTTP, pero un solo entorno para el componente de tareas en segundo plano.
- [ ] Usar varios entornos de Elastic Beanstalk para el componente de tareas en segundo plano, pero un solo entorno para el componente HTTP.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa utiliza plantillas de AWS CloudFormation para desplegar recursos de AWS. La empresa necesita actualizar una de sus pilas de AWS CloudFormation. ¿Qué puede hacer la empresa para saber cómo afectarán los cambios a los recursos que se están ejecutando?

- [x] Investigar los change sets.
- [ ] Investigar las stack policies.
- [ ] Investigar la sección `Metadata`.
- [ ] Investigar la sección `Resources`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una aplicación web sin servidor y mantiene diferentes ramas de código. El desarrollador desea evitar actualizar el endpoint de destino de Amazon API Gateway cada vez que se realiza un nuevo push de código. ¿Qué solución permitiría al desarrollador realizar un push de código de manera eficiente, sin necesidad de actualizar API Gateway?

- [ ] Asociar diferentes funciones de AWS Lambda a un endpoint de destino de API Gateway.
- [ ] Crear diferentes stages en API Gateway y luego asociar API Gateway con AWS Lambda.
- [x] Crear alias y versiones en AWS Lambda.
- [ ] Etiquetar (tag) las funciones de AWS Lambda con nombres diferentes.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa de publicidad tiene un sitio web dinámico con mucho tráfico. La empresa desea migrar la infraestructura del sitio web a AWS para que AWS se encargue de todo excepto del desarrollo del sitio web. ¿Qué solución cumple MEJOR con estos requisitos?

- [ ] Usar AWS VM Import para migrar una imagen de servidor web a AWS. Lanzar la imagen en una instancia de Amazon EC2 optimizada para cómputo.
- [ ] Lanzar varias instancias de Amazon Lightsail detrás de un balanceador de carga. Configurar el sitio web en esas instancias.
- [x] Desplegar el código del sitio web en un entorno de AWS Elastic Beanstalk. Usar Auto Scaling para escalar el número de instancias.
- [ ] Usar Amazon S3 para alojar el sitio web. Usar Amazon CloudFornt para entregar el contenido a escala.

**[⬆ Back to Top](#tabla-de-contenidos)**

### El flujo de trabajo del proceso de lanzamiento de una aplicación requiere una aprobación manual antes de que el código se despliegue en el entorno de producción. ¿Cuál es la MEJOR manera de lograr esto utilizando AWS CodePipeline?

- [ ] Usar varios pipelines para permitir la aprobación.
- [x] Usar una acción de aprobación en un stage.
- [ ] Deshabilitar la transición del stage para permitir la aprobación manual.
- [ ] Deshabilitar un stage justo antes del stage de despliegue.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha escrito una aplicación sin servidor utilizando varios servicios de AWS. La lógica de negocio está escrita como una función de Lambda que tiene dependencias de bibliotecas de terceros. Los endpoints de la función de Lambda se expondrán mediante Amazon API Gateway. La función de Lambda escribirá la información en Amazon DynamoDB. El desarrollador está listo para desplegar la aplicación, pero debe tener la capacidad de revertir. ¿Cómo se puede automatizar este despliegue, según estos requisitos?

- [ ] Desplegar usando las operaciones de la API de Amazon Lambda para crear la función de Lambda proporcionando un paquete de despliegue.
- [ ] Usar una plantilla de AWS CloudFormation y usar la sintaxis de CloudFormation para definir el recurso de la función de Lambda en la plantilla.
- [x] Usar una sintaxis que cumpla con el Serverless Application Model en la plantilla de AWS CloudFormation para definir el recurso de la función de Lambda.
- [ ] Crear un script de bash que use la AWS CLI para empaquetar y desplegar la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Dado el código fuente de una función de AWS Lambda en el archivo local `store.py` que contiene una función handler llamada `get_store` y la siguiente plantilla de AWS CloudFormation. ¿Qué se debe hacer para preparar la plantilla de modo que pueda desplegarse usando el comando de la AWS CLI `aws cloudformation deploy`?

![Question 59](images/question59.jpg)

- [ ] Usar AWS CloudFormation compile para codificar en base64 e incrustar el archivo fuente en una plantilla de CloudFormation modificada.
- [x] Usar AWS CloudFormation package para cargar el código fuente en un bucket de Amazon S3 y producir una plantilla de CloudFormation modificada.
- [ ] Usar AWS Lambda zip para empaquetar el archivo fuente junto con la plantilla de CloudFormation y desplegar el archivo zip resultante.
- [ ] Usar AWS Serverless `create-package` para incrustar el archivo fuente directamente en la plantilla de CloudFormation existente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha creado una función de Lambda grande y el despliegue está fallando con el siguiente error: `ClientError: An error occurred (InvalidParameterValueException) when calling the CreateFunction operation: Unzipped size must be smaller than XXXXXXXXX bytes.`, donde `XXXXXXXXX` es el límite actual de Lambda. ¿Qué puede hacer el desarrollador para solucionar este problema?

- [ ] Enviar una solicitud de aumento de límite a AWS Support para aumentar la función al tamaño necesario.
- [ ] Usar un algoritmo de compresión más eficiente que `ZIP`.
- [x] Dividir la función en varias funciones de Lambda más pequeñas.
- [ ] Comprimir el archivo `ZIP` dos veces con ZIP para comprimirlo aún más.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo una aplicación basada en Linux para ejecutarse en AWS Elastic Beanstalk. Los requisitos de la aplicación establecen que esta debe mantener su capacidad completa durante las actualizaciones y, al mismo tiempo, minimizar el costo. ¿Qué tipo de política de despliegue de Elastic Beanstalk debería especificar el desarrollador para el entorno?

- [ ] Immutable.
- [ ] Rolling.
- [ ] All at Once.
- [x] Rolling with additional batch.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Dónde debe colocarse el archivo `appspec.yml` para que AWS CodeDeploy funcione?

- [x] En la raíz de la estructura de directorios del código fuente de la aplicación.
- [ ] En la carpeta `bin` junto con todo el código compilado.
- [ ] En un bucket de S3.
- [ ] En la misma carpeta que los archivos de configuración de la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una función Lambda y usará bibliotecas externas que no están incluidas en las bibliotecas estándar de Lambda. ¿Qué acción minimizaría el tiempo de cómputo de Lambda consumido?

- [ ] Instalar las dependencias y bibliotecas externas al inicio de la función Lambda.
- [ ] Crear un paquete de despliegue de Lambda que incluya las bibliotecas externas.
- [ ] Copiar las bibliotecas externas a Amazon S3 y hacer referencia a ellas desde la ubicación de S3.
- [x] Instalar las bibliotecas externas en una Lambda Layer para que estén disponibles para todas las funciones Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un cliente quiere desplegar su código fuente en un entorno de AWS Elastic Beanstalk. El cliente necesita realizar el despliegue con una interrupción mínima y solo debe usar instancias existentes para conservar los registros de acceso de la aplicación. ¿Qué política de despliegue cumpliría con estos requisitos?

- [x] Rolling.
- [ ] All at once.
- [ ] Rolling with an additional batch.
- [ ] Immutable.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una función Lambda se empaqueta para su despliegue en múltiples entornos, incluidos desarrollo, pruebas, producción, etc. Cada entorno tiene un conjunto único de recursos, como bases de datos, etc. ¿Cómo puede la función Lambda usar los recursos del entorno actual?

- [ ] Aplicar tags a las funciones Lambda.
- [ ] Codificar los recursos directamente en el código fuente.
- [x] Usar variables de entorno para las funciones Lambda.
- [ ] Usar una función separada para desarrollo y producción.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa quiere implementar integración continua para sus cargas de trabajo en AWS. La empresa quiere activar pruebas unitarias en su pipeline para los commits en su repositorio de código, y quiere recibir notificaciones de los eventos de falla en el pipeline. ¿Cómo se pueden cumplir estos requisitos?

- [x] Almacenar el código fuente en AWS CodeCommit. Crear un CodePipeline para automatizar las pruebas unitarias. Usar Amazon SNS para activar las notificaciones de los eventos de falla.
- [ ] Almacenar el código fuente en GitHub. Crear un CodePipeline para automatizar las pruebas unitarias. Usar Amazon SES para activar las notificaciones de los eventos de falla.
- [ ] Almacenar el código fuente en GitHub. Crear un CodePipeline para automatizar las pruebas unitarias. Usar Amazon CloudWatch para activar las notificaciones de los eventos de falla.
- [ ] Almacenar el código fuente en AWS CodeCommit. Crear un CodePipeline para automatizar las pruebas unitarias. Usar Amazon CloudWatch para activar la notificación de los eventos de falla.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Para un despliegue con AWS CodeDeploy, ¿cuál es el orden de ejecución de los hooks en los despliegues in-place?

- [ ] Before Install -> Application Stop -> Application Start -> After Install.
- [x] Application Stop -> Before Install -> After Install -> Application Start.
- [ ] Before Install -> Application Stop -> Validate Service -> Application Start.
- [ ] Application Stop -> Before Install -> Validate Service -> Application Start.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles son los pasos para usar la AWS CLI para lanzar una aplicación sin servidor basada en plantillas?

- [ ] Usar AWS CloudFormation get-template y luego CloudFormation execute-change-set.
- [ ] Usar AWS CloudFormation validate-template y luego CloudFormation create-change-set.
- [x] Usar AWS CloudFormation package y luego CloudFormation deploy.
- [ ] Usar AWS CloudFormation create-stack y luego CloudFormation update-stack.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ha desarrollado una nueva aplicación sin servidor usando funciones de AWS Lambda que se desplegará usando la CLI de AWS Serverless Application Model (AWS SAM). ¿Qué paso debería completar el desarrollador antes de desplegar la aplicación?

- [ ] Comprimir la aplicación en un archivo `.zip` y cargarlo en AWS Lambda.
- [ ] Probar la nueva función de AWS Lambda rastreándola primero en AWS X-Ray.
- [x] Empaquetar la aplicación sin servidor usando SAM package.
- [ ] Crear el entorno de la aplicación usando el comando `eb create my-env`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está actualizando una aplicación implementada en AWS Elastic Beanstalk. La nueva versión es incompatible con la versión anterior. Para implementar la actualización con éxito, se debe realizar un cambio total a la nueva versión actualizada en todas las instancias al mismo tiempo, con la capacidad de revertir los cambios en caso de que falle el despliegue de la nueva versión. ¿Cómo se puede lograr esto con la MENOR cantidad de tiempo de inactividad?

- [ ] Usar la política de despliegue All at once de Elastic Beanstalk para actualizar todas las instancias simultáneamente.
- [ ] Realizar un despliegue Rolling with additional batch de Elastic Beanstalk.
- [x] Implementar la nueva versión en un nuevo entorno de Elastic Beanstalk e intercambiar las URL de los entornos.
- [ ] Realizar un despliegue Rolling de Elastic Beanstalk.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Dada la siguiente plantilla de AWS CloudFormation. ¿Cuál es la forma MÁS eficiente de hacer referencia al nuevo bucket de Amazon S3 desde otra plantilla de AWS CloudFormation?

![Question 130](images/question130.jpg)

- [x] Agregar una declaración `Export` a la sección `Outputs` de la plantilla original y usar `ImportValue` en las otras plantillas.
- [ ] Agregar `Exported: true` a `Content.Bucket` en la plantilla original y usar `ImportResource` en las otras plantillas.
- [ ] Crear un recurso personalizado de AWS CloudFormation que obtenga el nombre del bucket del recurso `ContentBucket` del primer stack.
- [ ] Usar `Fn::Include` para incluir la plantilla existente en las otras plantillas y usar directamente el recurso `ContentBucket`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está usando AWS CodeDeploy para implementar una aplicación que se ejecuta en Amazon EC2. El desarrollador quiere cambiar los permisos de archivo de un archivo de despliegue específico. ¿Qué evento del ciclo de vida debe usar el desarrollador para cumplir con este requisito?

- [x] AfterInstall.
- [ ] DownloadBundle.
- [ ] BeforeInstall.
- [ ] ValidateService.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando un script para automatizar el proceso de despliegue de una aplicación sin servidor. El desarrollador quiere usar una plantilla existente de AWS Serverless Application Model (AWS SAM) para la aplicación. ¿Qué debe usar el desarrollador para el proyecto? (Elija DOS)

- [x] Llamar a `aws cloudformation package` para crear el paquete de despliegue. Llamar a `aws cloudformation deploy` para desplegar el paquete posteriormente.
- [x] Llamar a `sam package` para crear el paquete de despliegue. Llamar a `sam deploy` para desplegar el paquete posteriormente.
- [ ] Llamar a `aws s3 cp` para cargar la plantilla de AWS SAM en Amazon S3. Llamar a `aws lambda update-function-code` para crear la aplicación.
- [ ] Crear un paquete `ZIP` localmente y llamar a `aws serverlessrepo create-application` para crear la aplicación.
- [ ] Crear un paquete `ZIP` y cargarlo en Amazon S3. Llamar a `aws cloudformation create-stack` para crear la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo usa AWS Elastic Beanstalk para el despliegue de aplicaciones. El equipo ha configurado la política de ciclo de vida de versiones de la aplicación para limitar el número de versiones de la aplicación a 25. Sin embargo, incluso con la política de ciclo de vida, el source bundle se elimina del bucket de origen de Amazon S3. ¿Qué debe hacer un desarrollador en la configuración del ciclo de vida de versiones de la aplicación de Elastic Beanstalk para conservar el código fuente en el bucket de S3?

- [ ] Cambiar la configuración Set the application versions limit by total count a cero.
- [ ] Deshabilitar la configuración de la política Lifecycle.
- [ ] Cambiar la configuración Set the application version limit by age a cero.
- [x] Establecer Retention en Retain source bundle in S3.

**[⬆ Back to Top](#tabla-de-contenidos)**

### A un desarrollador se le proporciona una URL de clonación HTTPS para un repositorio de AWS CodeCommit. ¿Qué es necesario configurar antes de clonar este repositorio?

- [ ] Usar AWS KMS para configurar claves públicas y privadas para usar con AWS CodeCommit.
- [x] Configurar el Git credential helper para usar un perfil de credenciales de AWS y habilitar el helper para enviar la ruta de los repositorios.
- [ ] Usar AWS Certificate Manager para aprovisionar certificados SSL/TLS públicos y privados.
- [ ] Generar claves de cifrado con AWS CloudHSM y luego exportar la clave para usarla con AWS CodeCommit.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador convirtió un programa existente en una función de AWS Lambda en la consola. El programa se ejecuta correctamente en una laptop local, pero muestra un error `Unable to import module` al probarse en la consola de Lambda. ¿Cuál de las siguientes acciones puede corregir el error?

- [x] Instalar el módulo faltante y especificar el directorio actual como destino. Crear un archivo `ZIP` que incluya todos los archivos del directorio actual y cargar el archivo `ZIP`.
- [ ] Instalar el módulo faltante en un directorio lib. Crear un archivo `ZIP` que incluya todos los archivos del directorio lib y cargar el archivo `ZIP` como archivo de dependencias.
- [ ] En el código de Lambda, invocar un comando de Linux para instalar los módulos faltantes en el directorio `/usr/lib directory`.
- [ ] En la consola de Lambda, crear un entorno `LB_LIBRARY_PATH` y especificar el valor para el plan de bibliotecas del sistema.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita administrar la infraestructura de AWS como código y debe poder desplegar múltiples copias idénticas de la infraestructura, preparar cambios (stage) y revertir a versiones anteriores. ¿Qué enfoque cumple con estos requisitos?

- [ ] Usar informes de asignación de costos y AWS OpsWorks para desplegar y administrar la infraestructura.
- [ ] Usar métricas y alertas de Amazon CloudWatch junto con el etiquetado de recursos para desplegar y administrar la infraestructura.
- [ ] Usar AWS Elastic Beanstalk y AWS CodeCommit para desplegar y administrar la infraestructura.
- [x] Usar AWS CloudFormation y AWS CodeCommit para desplegar y administrar la infraestructura.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador necesita desplegar una aplicación que se ejecuta en AWS Fargate usando Amazon ECS. La aplicación tiene variables de entorno que deben pasarse a un contenedor para que la aplicación se inicialice. ¿Cómo se deben pasar las variables de entorno al contenedor?

- [ ] Definir un arreglo que incluya las variables de entorno bajo el parámetro environment dentro de la service definition.
- [x] Definir un arreglo que incluya las variables de entorno bajo el parámetro environment dentro de la task definition.
- [ ] Definir un arreglo que incluya las variables de entorno bajo el parámetro entryPoint dentro de la task definition.
- [ ] Definir un arreglo que incluya las variables de entorno bajo el parámetro entryPoint dentro de la service definition.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ejecuta pipelines de integración continua/entrega continua (CI/CD) para su aplicación en AWS CodePipeline. Un desarrollador debe escribir pruebas unitarias y ejecutarlas como parte de los pipelines antes de preparar (staging) los artefactos para pruebas. ¿Cómo debería incorporar el desarrollador las pruebas unitarias como parte de los pipelines de CI/CD?

- [ ] Crear un pipeline de CodePipeline independiente para ejecutar las pruebas unitarias.
- [x] Actualizar la especificación de AWS CodeBuild para incluir una fase que ejecute las pruebas unitarias.
- [ ] Instalar el agente de AWS CodeDeploy en una instancia de Amazon EC2 para ejecutar las pruebas unitarias.
- [ ] Crear una rama de pruebas en AWS CodeCommit para ejecutar las pruebas unitarias.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha escrito código para una aplicación y quiere compartirlo con otros desarrolladores del equipo para recibir comentarios. El código compartido de la aplicación debe almacenarse a largo plazo con múltiples versiones y seguimiento de cambios por lotes. ¿Qué servicio de AWS debería usar el desarrollador?

- [ ] AWS CodeBuild.
- [ ] Amazon S3.
- [x] AWS CodeCommit.
- [ ] AWS Cloud9.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está preparando un paquete de despliegue con AWS CloudFormation. El paquete consta de dos plantillas separadas: una para la infraestructura y otra para la aplicación. La aplicación debe estar dentro de la VPC creada a partir de la plantilla de infraestructura. ¿Cómo puede la pila de la aplicación hacer referencia a la VPC creada a partir de la plantilla de infraestructura?

- [ ] Usar la función Ref para importar la VPC a la pila de la aplicación desde la plantilla de infraestructura.
- [x] Usar el indicador export en la plantilla de infraestructura y luego usar la función `Fn::ImportValue` en la plantilla de la aplicación.
- [ ] Usar el atributo `DependsOn` para especificar que la instancia de la aplicación depende de la VPC en la plantilla de la aplicación.
- [ ] Usar la función `Fn::GetAtt` para incluir el atributo de la VPC en la plantilla de la aplicación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo decide adoptar un proceso de integración continua/entrega continua (CI/CD) usando AWS CodePipeline y AWS CodeCommit para una nueva aplicación. Sin embargo, la gerencia quiere que una persona revise y apruebe el código antes de que se despliegue en producción. ¿Cómo puede el equipo de desarrollo agregar un aprobador manual al pipeline de CI/CD?

- [ ] Usar AWS SES para enviar un correo electrónico a los aprobadores cuando se requiera su acción. Desarrollar una aplicación sencilla que permita a los aprobadores aceptar o rechazar una compilación. Invocar una función de AWS Lambda para avanzar el pipeline cuando se acepte una compilación.
- [ ] Si se aprueba, agregar una etiqueta (tag) de aprobado al enviar los cambios al repositorio de CodeCommit. CodePipeline continuará compilando y desplegando los commits aprobados sin interrupción.
- [ ] Agregar un paso de aprobación a CodeCommit. Los commits no se guardarán hasta que se aprueben.
- [x] Agregar una acción de aprobación al pipeline. Configurar la acción de aprobación para que publique en un tema de Amazon SNS cuando se requiera aprobación. La ejecución del pipeline se detendrá y esperará una aprobación.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ha implementado AWS CodeDeploy como parte de su stack de CI/CD nativo de la nube. La empresa habilita los rollbacks automáticos al desplegar una nueva versión de una aplicación web popular in-place en Amazon EC2. ¿Qué ocurre si el despliegue de la nueva versión falla debido a una regresión de código?

- [ ] El último despliegue válido conocido se restaura automáticamente usando la instantánea almacenada en Amazon S3.
- [ ] CodeDeploy vuelve a cambiar los registros alias de Amazon Route 53 al despliegue green válido conocido y termina el despliegue blue fallido.
- [x] Se realiza un nuevo despliegue de la última versión conocida de la aplicación con un nuevo ID de despliegue.
- [ ] AWS CodePipeline promueve a producción el despliegue más reciente con estado SUCCEEDED.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa ha implementado AWS CodePipeline para automatizar sus pipelines de lanzamiento. El equipo de desarrollo está escribiendo una función de AWS Lambda que enviará notificaciones sobre los cambios de estado de cada una de las acciones en las etapas. ¿Qué pasos se deben seguir para asociar la función de Lambda con la fuente de eventos?

- [ ] Crear un trigger que invoque la función de Lambda desde la consola de Lambda seleccionando CodePipeline como fuente de eventos.
- [x] Crear un event trigger y especificar la función de Lambda desde la consola de CodePipeline.
- [ ] Crear una alarma de Amazon CloudWatch que monitoree los cambios de estado en Code Pipeline y active la función de Lambda.
- [ ] Crear una regla de Amazon CloudWatch Events que use CodePipeline como fuente de eventos.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un Developer ha creado una aplicación que se ejecuta en AWS Lambda usando AWS Serverless Application Model (AWS SAM). ¿Cuál es el orden de ejecución correcto para desplegar la aplicación con éxito?

- [ ] 1. Compilar (build) la plantilla de SAM en Amazon EC2. 2. Empaquetar (package) la plantilla de SAM en almacenamiento de Amazon EBS. 3. Desplegar (deploy) la plantilla de SAM desde Amazon EBS.
- [x] 1. Compilar (build) la plantilla de SAM localmente. 2. Empaquetar (package) la plantilla de SAM en Amazon S3. 3. Desplegar (deploy) la plantilla de SAM desde Amazon S3.
- [ ] 1. Compilar (build) la plantilla de SAM localmente. 2. Desplegar (deploy) la plantilla de SAM desde Amazon S3. 3. Empaquetar (package) la plantilla de SAM para su uso.
- [ ] 1. Compilar (build) la plantilla de SAM localmente. 2. Empaquetar (package) la plantilla de SAM desde AWS CodeCommit. 3. Desplegar (deploy) la plantilla de SAM en CodeCommit.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo quiere compilar y desplegar de inmediato una aplicación siempre que haya un cambio en el código fuente. ¿Qué enfoques se podrían usar para activar el despliegue? (Elija DOS)

- [x] Almacenar el código fuente en un bucket de Amazon S3. Configurar AWS CodePipeline para que se inicie siempre que cambie un archivo en el bucket.
- [ ] Almacenar el código fuente en un volumen cifrado de Amazon EBS. Configurar AWS CodePipeline para que se inicie siempre que cambie un archivo en el volumen.
- [x] Almacenar el código fuente en un repositorio de AWS CodeCommit. Configurar AWS CodePipeline para que se inicie siempre que se confirme un cambio en el repositorio.
- [ ] Almacenar el código fuente en un bucket de Amazon S3. Configurar AWS CodePipeline para que se inicie cada 15 minutos.
- [ ] Almacenar el código fuente en el almacenamiento efímero de una instancia de Amazon EC2. Configurar la instancia para que inicie AWS CodePipeline siempre que haya cambios en el código fuente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa minorista en línea ha desplegado una aplicación sin servidor con AWS Lambda, Amazon API Gateway, Amazon S3 y Amazon DynamoDB usando AWS CloudFormation. La empresa lanzó una nueva versión con mejoras importantes en la función de Lambda y desplegó el lanzamiento en producción. Posteriormente, la aplicación dejó de funcionar. ¿Qué solución debería restablecer la aplicación lo más rápido posible?

- [ ] Volver a desplegar la aplicación en Amazon EC2 para que la función de Lambda pueda resolver las dependencias.
- [ ] Migrar DynamoDB a Amazon RDS y volver a desplegar la función de Lambda.
- [x] Revertir (roll back) la función de Lambda a la versión anterior.
- [ ] Desplegar la última función de Lambda en una Región diferente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está creando un servicio REST usando Amazon API Gateway con integración de AWS Lambda. El servicio debe ejecutar diferentes versiones con fines de prueba. ¿Cuál sería la MEJOR forma de lograrlo?

- [ ] Usar un encabezado `x-Version` para indicar qué versión se está llamando y pasar ese encabezado a la(s) función(es) Lambda.
- [ ] Crear un Lambda authorizer de API Gateway para enrutar a los clientes de la API a la versión correcta de la API.
- [ ] Crear una resource policy de API Gateway para aislar las versiones y proporcionar contexto a la(s) función(es) Lambda.
- [x] Desplegar las versiones de la API como stages únicos con endpoints únicos y usar stage variables para proporcionar contexto adicional.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de Desarrollo desea migrar el código de su aplicación existente de un repositorio de GitHub a AWS CodeCommit. ¿Qué es necesario crear antes de poder migrar un repositorio clonado a CodeCommit mediante HTTPS?

- [ ] Un token de autenticación seguro de GitHub.
- [ ] Un archivo de clave SSH pública y privada.
- [x] Un conjunto de credenciales de Git generadas desde IAM.
- [ ] Un rol de IAM de Amazon EC2 con permisos de CodeCommit.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cuáles de las siguientes plataformas son compatibles con Elastic Beanstalk? (Elija DOS)

- [x] Apache Tomcat.
- [x] .NET.
- [ ] IBM Websphere.
- [ ] Oracle JBoss.
- [ ] Jetty.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué fragmento de código a continuación devuelve la URL de un sitio web con balanceo de carga creado en CloudFormation con un recurso `AWS::ElasticLoadBalancing::LoadBalancer` de nombre `ElasticLoad Balancer`?

- [x] `"Fn::Join":[ "".["http://", {Fn::GetAtt": [ "ElasticLoadBalancer","DNSName"]}]]`.
- [ ] `"Fn::Join":[ "".["http://", {Fn::GetAtt": [ "ElasticLoadBalancer","Url"]}]]`.
- [ ] `"Fn::Join":[ "".["http://", {"Ref : "ElasticLoadBalancerUrl"}]]`.
- [ ] `"Fn::Join":[ "".["http://", {"Ref : "ElasticLoadBalancer","DNSName"}]]`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué sucede, por defecto, cuando no se puede crear uno de los recursos de un stack de CloudFormation?

- [ ] Los recursos creados previamente se conservan pero la creación del stack termina.
- [x] Los recursos creados previamente se eliminan y la creación del stack termina.
- [ ] La creación del stack continúa y los resultados finales indican qué pasos fallaron.
- [ ] Las plantillas de CloudFormation se analizan por adelantado, por lo que se garantiza que la creación del stack tendrá éxito.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Las instancias de EC2 se lanzan a partir de Amazon Machine Images (AMIs). Una AMI pública determinada puede:

- [ ] Usarse para lanzar instancias de EC2 en cualquier región de AWS.
- [ ] Usarse únicamente para lanzar instancias de EC2 en el mismo país en el que está almacenada la AMI.
- [x] Usarse únicamente para lanzar instancias de EC2 en la misma región de AWS en la que está almacenada la AMI.
- [ ] Usarse únicamente para lanzar instancias de EC2 en la misma zona de disponibilidad de AWS en la que está almacenada la AMI.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Qué productos y características de AWS pueden ser desplegados por Elastic Beanstalk? (Elija TRES)

- [x] Auto scaling groups.
- [ ] Route 53 hosted zones.
- [x] Elastic Load Balancers.
- [x] Instancias de RDS.
- [ ] Direcciones Elastic IP.
- [ ] Colas de SQS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrolladores debe migrar una aplicación que se ejecuta dentro de un entorno de AWS Elastic Beanstalk de un Classic Load Balancer a un Application Load Balancer. ¿Qué pasos se deben seguir para lograr la tarea usando la AWS Management Console?

- [x] 1. Actualizar el código de la aplicación en el despliegue existente. 2. Seleccionar un nuevo tipo de load balancer antes de ejecutar el despliegue. 3. Desplegar la nueva versión del código de la aplicación en el entorno.
- [ ] 1. Crear un nuevo entorno con las mismas configuraciones excepto el tipo de load balancer. 2. Desplegar la misma versión de la aplicación utilizada en el entorno original. 3. Ejecutar la acción `swap-environment-cnames`.
- [ ] 1. Clonar el entorno existente, cambiando el tipo de load balancer asociado. 2. Desplegar la misma versión de la aplicación utilizada en el entorno original. 3. Ejecutar la acción `swap-environment-cnames`.
- [ ] 1. Editar las definiciones del entorno en el despliegue existente. 2. Cambiar el tipo de load balancer asociado según los requisitos. 3. Reconstruir el entorno con el nuevo tipo de load balancer.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa necesita un sistema de control de versiones para el desarrollo colaborativo de software. Las características del sistema deben incluir lo siguiente: soporte para lotes de cambios en múltiples archivos, ramificación (branching) en paralelo y seguimiento de versiones. ¿Qué servicio de AWS cumplirá estos requisitos?

- [ ] AWS CodePipeline.
- [ ] Amazon S3.
- [ ] AWS Code Build.
- [x] AWS CodeCommit.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa utiliza sistemas de integración continua y entrega continua. Un desarrollador ahora necesita automatizar el despliegue de un paquete de software tanto en instancias de Amazon EC2 como en servidores virtuales que se ejecutan on-premises. ¿Qué servicio de AWS se debe usar para lograrlo?

- [ ] AWS CodePipeline.
- [ ] AWS CodeBuild.
- [ ] AWS Elastic Beanstalk.
- [x] AWS CodeDeploy.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está intentando desplegar una aplicación serverless usando AWS CodeDeploy. La aplicación fue actualizada y necesita volver a desplegarse. ¿Qué archivo necesita actualizar el desarrollador para propagar ese cambio a través de CodeDeploy?

- [ ] `dockerrun.aws.json`.
- [ ] `buildspec.yml`.
- [x] `appspec.yml`.
- [ ] `ebextensions.config`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está creando una plantilla que usa AWS CloudFormation para desplegar una aplicación. Esta aplicación es serverless y utiliza Amazon API Gateway, Amazon DynamoDB y AWS Lambda. ¿Qué herramienta debe usar el desarrollador para definir una sintaxis simplificada que exprese recursos serverless?

- [ ] Funciones intrínsecas serverless de CloudFormation.
- [ ] AWS serverless express.
- [x] Un AWS serverless application model.
- [ ] Un plugin serverless de CloudFormation.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Para incluir objetos definidos por AWS Serverless Application Model (SAM) en una plantilla de AWS CloudFormation, además de `Resources`, ¿qué sección DEBE incluirse en la raíz del documento?

- [ ] `Conditions`.
- [ ] `Globals`.
- [x] `Transform`.
- [ ] `Properties`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador creó especificaciones de configuración para una aplicación de AWS Elastic Beanstalk en un archivo llamado healthcheckurl.yaml en el `.ebextensions/directory` del paquete de origen de su aplicación. El archivo contiene lo siguiente: Después de que la aplicación se inicia, el health check no se ejecuta en la ruta correcta, aunque esta es válida. ¿Qué se puede hacer para corregir este archivo de configuración?

![Question 297](images/question297.jpeg)

- [ ] Convertir el archivo a formato JSON.
- [x] Renombrar el archivo con la extensión `.config`.
- [ ] Cambiar la sección de configuración de `options_settings` a resources.
- [ ] Cambiar el namespace de las option settings a un namespace personalizado.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene tres entornos distintos: Development, QA y Production. La empresa quiere implementar su código primero en el entorno de Development, luego en QA y después en Production. ¿Qué servicio de AWS se puede usar para cumplir este requisito?

- [ ] Usar AWS CodeCommit para crear varios repositorios para implementar la aplicación.
- [ ] Usar AWS CodeBuild para crear, configurar e implementar varios proyectos de compilación de la aplicación.
- [ ] Usar AWS Data Pipeline para crear varios aprovisionamientos de data pipeline para implementar la aplicación.
- [x] Usar AWS CodeDeploy para crear varios deployment groups.

**[⬆ Back to Top](#tabla-de-contenidos)**

### En un entorno Docker multicontenedor en AWS Elastic Beanstalk, ¿qué se requiere para configurar las instancias de contenedor del entorno?

- [x] Una task definition de Amazon ECS.
- [ ] Un clúster de Amazon ECS.
- [ ] Un Dockerfile en un paquete de la aplicación.
- [ ] Una CLI para Elastic Beanstalk.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene un sitio web desarrollado en PHP y WordPress que se lanza mediante AWS Elastic Beanstalk. Hay una nueva versión del sitio web que se debe implementar en el entorno de Elastic Beanstalk. La empresa no puede tolerar que el sitio web quede fuera de línea si falla una actualización. Los despliegues deben tener un impacto mínimo y permitir un rollback lo antes posible. ¿Qué método de despliegue se debe usar?

- [ ] All at once.
- [ ] Rolling.
- [ ] Snapshots.
- [x] Immutable.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador escribe una función de AWS Lambda y carga el código en un archivo `.ZIP` en Amazon S3. El desarrollador realiza cambios en el código y carga un nuevo archivo `.ZIP` en Amazon S3. Sin embargo, Lambda ejecuta el código anterior. ¿Cómo puede el desarrollador solucionarlo de la forma MENOS disruptiva?

- [ ] Crear otra función Lambda y especificar el nuevo archivo `.ZIP`.
- [x] Llamar a la API `update-function-code`.
- [ ] Eliminar primero el archivo `.ZIP` anterior y luego agregar el nuevo archivo `.ZIP`.
- [ ] Llamar a la API `create-alias`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### A un desarrollador se le ha pedido realizar cambios en el código fuente de una función de AWS Lambda. La función se administra mediante una plantilla de AWS CloudFormation. La plantilla está configurada para cargar el código fuente desde un bucket de Amazon S3. El desarrollador creó manualmente un paquete de despliegue en un archivo `.ZIP` que contiene los cambios y colocó el archivo en la ubicación correcta de Amazon S3. Cuando se invoca la función, los cambios de código no se han aplicado. ¿Qué paso se requiere para actualizar la función con los cambios?

- [ ] Eliminar el archivo `.ZIP` en S3 y volver a cargarlo usando un nombre de clave de objeto diferente.
- [x] Actualizar el stack de CloudFormation con los valores correctos para las propiedades de código de la función S3Bucket, S3Key o S3ObjectVersion.
- [ ] Asegurarse de que el código fuente de la función esté codificado en base64 antes de cargar el paquete de despliegue en S3.
- [ ] Modificar el rol de ejecución de la función Lambda para permitir el permiso de acceso a S3 al archivo `.ZIP` del paquete de despliegue.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una aplicación de AWS Elastic Beanstalk necesita implementarse en varias regiones y requiere una Amazon Machine Image (AMI) diferente en cada región. ¿Qué clave de la plantilla de AWS CloudFormation se puede usar para especificar la AMI correcta para cada región?

- [ ] `Parameters`.
- [ ] `Outputs`.
- [x] `Mappings`.
- [ ] `Resources`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe implementar una nueva función de AWS Lambda mediante una plantilla de AWS CloudFormation. ¿Qué procedimientos implementarán una función Lambda? (Seleccione DOS)

- [ ] Cargar el código en un repositorio de AWS CodeCommit y luego agregar una referencia a él en un recurso `AWS::Lambda::Function` de la plantilla.
- [x] Crear un recurso `AWS::Lambda::Function` en la plantilla y luego escribir el código directamente dentro de la plantilla de CloudFormation.
- [x] Cargar un archivo `.ZIP` que contenga el código de la función en Amazon S3 y luego agregar una referencia a él en un recurso `AWS::Lambda::Function` de la plantilla.
- [ ] Cargar un archivo `.ZIP` en AWS CloudFormation que contenga el código de la función y luego agregar una referencia a él en un recurso `AWS::Lambda::Function` de la plantilla.
- [ ] Cargar el código de la función en un repositorio Git privado y luego agregar una referencia a él en un recurso `AWS::Lambda::Function` de la plantilla.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Cómo se deben utilizar las bibliotecas personalizadas en AWS Lambda?

- [ ] Alojar la biblioteca en Amazon S3 y hacer referencia a ella desde la función Lambda.
- [x] Instalar la biblioteca localmente y cargar un archivo `ZIP` de la función Lambda.
- [ ] Importar el blueprint de Lambda necesario al crear la función.
- [ ] Modificar el runtime de la función para incluir la biblioteca necesaria.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador está escribiendo un microservicio de procesamiento de imágenes en AWS Lambda. El servicio depende de varias bibliotecas que no están disponibles en el entorno de ejecución de Lambda. ¿Qué estrategia debe seguir el desarrollador para crear el paquete de despliegue de Lambda?

- [x] Crear un archivo `ZIP` con el código fuente y todas las bibliotecas dependientes.
- [ ] Crear un archivo `ZIP` con el código fuente y un script que instale las bibliotecas dependientes en tiempo de ejecución.
- [ ] Crear un archivo `ZIP` con el código fuente. Colocar las bibliotecas dependientes en un bucket de Amazon S3 indicado por la variable de entorno de Lambda `LD_LIBRARY_PATH`.
- [ ] Crear un archivo `ZIP` con el código fuente y un archivo buildspec.yaml que instale las bibliotecas dependientes en AWS Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa necesita un servicio de control de código fuente totalmente administrado que funcione en AWS. El servicio debe garantizar que el control de revisiones sincronice múltiples repositorios distribuidos intercambiando conjuntos de cambios de par a par (peer-to-peer). Todos los usuarios necesitan trabajar de forma productiva incluso cuando no están conectados a una red. ¿Qué servicio de control de código fuente se debe usar?

- [ ] Subversion.
- [ ] AWS CodeBuild.
- [x] AWS CodeCommit.
- [ ] AWS CodeStar.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene múltiples desarrolladores ubicados en todo el mundo que actualizan código de forma incremental para un proyecto de desarrollo. Cuando los desarrolladores cargan código de forma concurrente, la conexión a internet es lenta y toma mucho tiempo cargar el código para desplegarlo en AWS Elastic Beanstalk. ¿Qué paso dará como resultado un tiempo mínimo de carga y despliegue con la MENOR cantidad de esfuerzo administrativo?

- [ ] Permitir que los desarrolladores carguen el código a un bucket de Amazon S3 y lo desplieguen directamente en Elastic Beanstalk.
- [ ] Permitir que los desarrolladores carguen el código a un servidor FTP central para desplegar la aplicación en Elastic Beanstalk.
- [x] Crear un repositorio de AWS CodeCommit, permitir que los desarrolladores confirmen (commit) código en él y luego desplegar el código directamente en Elastic Beanstalk.
- [ ] Crear un repositorio de código en una instancia de Amazon EC2 para que todos los desarrolladores puedan actualizar el código, y desplegar la aplicación desde la instancia a Elastic Beanstalk.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa tiene una plantilla de AWS CloudFormation almacenada como un solo archivo. La plantilla puede lanzar y crear una pila de infraestructura completa. ¿Qué mejor práctica aumentaría la mantenibilidad de la plantilla?

- [x] Usar nested stacks para patrones de plantilla comunes.
- [ ] Incrustar credenciales para evitar errores de escritura.
- [ ] Eliminar los mappings para disminuir la cantidad de variables.
- [ ] Usar `AWS::Include` para referenciar archivos de plantilla alojados públicamente.

**[⬆ Back to Top](#tabla-de-contenidos)**

### AWS CodeBuild compila el código de una aplicación, crea la imagen de Docker, la envía a Amazon Elastic Container Registry (Amazon ECR) y etiqueta la imagen con un identificador único. Si los desarrolladores ya tienen la AWS CLI configurada en sus estaciones de trabajo, ¿cómo se pueden descargar (pull) las imágenes de Docker a las estaciones de trabajo?

- [ ] Ejecutar lo siguiente: `docker pull REPOSITORY URI : TAG`.
- [x] Ejecutar la salida del siguiente comando: `aws ecr get-login` y luego ejecutar: `docker pull REPOSITORY URI : TAG`.
- [ ] Ejecutar lo siguiente: `aws ecr get-login` y luego ejecutar: `docker pull REPOSITORY URI : TAG`.
- [ ] Ejecutar la salida del siguiente comando: `aws ecr get-download-url-for-layer` y luego ejecutar: `docker pull REPOSITORY URI : TAG`.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador ha creado una aplicación web y quiere desplegarla rápidamente en un servidor Tomcat en AWS. El desarrollador quiere evitar tener que administrar la infraestructura subyacente. ¿Cuál es la forma más fácil de desplegar la aplicación, según estos requisitos?

- [ ] AWS CloudFormation.
- [x] AWS Elastic Beanstalk.
- [ ] Amazon S3.
- [ ] AWS CodePipeline

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un equipo de desarrollo está usando AWS Elastic Beanstalk para desplegar una aplicación de dos capas que consta de una capa web con balanceo de carga y una capa de base de datos de Amazon RDS en producción. El equipo desea separar la instancia de RDS de Elastic Beanstalk. ¿Cómo se puede lograr esto?

- [ ] Usar la CLI de Elastic Beanstalk para desasociar la base de datos.
- [ ] Usar el AWS CLI para desasociar la base de datos.
- [ ] Cambiar la política de despliegue para desasociar la base de datos.
- [x] Recrear un nuevo entorno de Elastic Beanstalk sin Amazon RDS.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Cuando un desarrollador intenta ejecutar un proyecto de AWS CodeBuild, este genera un error porque la longitud de todas las variables de entorno excede el límite del máximo combinado de caracteres. ¿Cuál es la solución recomendada?

- [ ] Agregar el comando export `LC_ALL="en_US.utf8"` a la sección `pre_build` para asegurar la localización `POSIX`.
- [ ] Usar Amazon Cognito para almacenar pares clave-valor para un gran número de variables de entorno.
- [ ] Actualizar la configuración del proyecto de compilación para usar un bucket de Amazon S3 para un gran número de variables de entorno.
- [x] Usar AWS Systems Manager Parameter Store para almacenar un gran número de variables de entorno.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Un desarrollador debe desplegar de manera repetida y consistente una API RESTful sin servidor en AWS. ¿Qué técnicas funcionarán? (Elija DOS)

- [ ] Definir un archivo Swagger. Usar AWS Elastic Beanstalk para desplegar el archivo Swagger.
- [ ] Definir un archivo Swagger. Usar AWS CodeDeploy para desplegar el archivo Swagger.
- [x] Desplegar una plantilla de SAM con una definición de Swagger en línea.
- [x] Definir un archivo Swagger. Desplegar una plantilla de SAM que haga referencia al archivo Swagger.
- [ ] Definir una definición de Swagger en línea en una función Lambda. Invocar la función Lambda.

**[⬆ Back to Top](#tabla-de-contenidos)**

### Una empresa está usando Amazon API Gateway para administrar el acceso a un conjunto de microservicios implementados como funciones de AWS Lambda. Tras un reporte de error, la empresa realiza un cambio menor que rompe la compatibilidad en una de las APIs. Para evitar afectar a los clientes existentes cuando se despliegue la nueva API, la empresa quiere dar a los clientes seis meses para migrar de v1 a v2. ¿Qué enfoque debe usar el desarrollador para manejar este cambio?

- [ ] Actualizar la función Lambda subyacente y proporcionar a los clientes la nueva URL de invocación de Lambda.
- [ ] Usar API Gateway para propagar automáticamente el cambio a los clientes, especificando 180 días en el parámetro de despliegue por fases.
- [x] Usar API Gateway para desplegar un nuevo stage llamado v2 en la API y proporcionar a los usuarios su URL.
- [ ] Actualizar la función Lambda subyacente y crear una distribución de Amazon CloudFront con la función Lambda actualizada como su origen.

**[⬆ Back to Top](#tabla-de-contenidos)**

### ¿Dónde debe colocarse un archivo de configuración de Elastic Beanstalk llamado `healthcheckur1.config` en el paquete de código fuente de la aplicación?

- [ ] En el `root` de la aplicación.
- [ ] En la carpeta `bin`.
- [ ] En `healthcheckur1.config.ebextension` bajo `root`.
- [x] En la carpeta `.ebextensions`.

**[⬆ Back to Top](#tabla-de-contenidos)**
