# Implementar y mantener el estado (State)

> **Dominio del examen:** Implement and Maintain State | **Peso:** 12-15%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre por qué existe el state, los datos sensibles, los backends remotos, el locking, los subcomandos de state, refresh-only y la migración de backend.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Por qué Terraform mantiene un archivo de state?

- A. Para almacenar los binarios de los plugins de provider
- B. Para asociar la configuración con los IDs de los recursos reales y rastrear metadatos
- C. Para reemplazar la necesidad de los providers
- D. Para cifrar todas las credenciales de las APIs de la nube

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El state asocia las direcciones de Terraform con los IDs reales de los recursos, almacena metadatos y dependencias, guarda en caché los atributos y permite la colaboración mediante backends remotos.

</details>

---
### Pregunta 2

¿Cuál NO es una razón principal por la que Terraform mantiene el state?

- A. Asociar los recursos de la configuración con los IDs de la infraestructura real
- B. Guardar en caché los atributos de los recursos para mejorar el rendimiento
- C. Almacenar el código fuente de los providers para uso sin conexión
- D. Permitir la colaboración en equipo mediante remote state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: C**

**Explicación:** El state asocia, guarda en caché y permite la colaboración. Los plugins de provider viven en .terraform/, no en el state.

</details>

---
### Pregunta 3

¿Qué mejora la caché del state de Terraform?

- A. Solo la velocidad de descarga de los providers
- B. El rendimiento, al almacenar los atributos de los recursos que Terraform ya conoce
- C. La validación de la sintaxis HCL
- D. La resolución de versiones de los módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los atributos en caché reducen las llamadas repetidas a la API durante las operaciones de plan/apply.

</details>

---
### Pregunta 4

¿Cómo ayuda principalmente el remote state a que los equipos colaboren?

- A. Compilando HCL a JSON automáticamente
- B. Proporcionando una vista compartida y consistente de la infraestructura administrada
- C. Eliminando la necesidad de control de versiones
- D. Ejecutando apply localmente en la laptop de cada ingeniero

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los backends remotos permiten que los equipos compartan un único state autoritativo, de modo que todos planifiquen sobre la misma realidad.

</details>

---
### Pregunta 5

¿Cuál de las siguientes opciones rastrea el state de Terraform?

- A. Solo los nombres de los recursos de la configuración
- B. IDs de recursos, dependencias y metadatos del provider
- C. Solo los valores de los outputs
- D. Solo los valores por defecto de las variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El state registra los IDs de los recursos, los grafos de dependencias, la información de serial/versión y el linaje del provider.

</details>

---
### Pregunta 6

Sin un archivo de state, ¿qué problema enfrentaría Terraform en el siguiente plan?

- A. No podría descargar los providers
- B. No sabría qué recursos reales corresponden a las direcciones de la configuración
- C. Omitiría la validación
- D. Siempre destruiría todos los recursos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El state es la capa de asociación entre las direcciones de HCL y los identificadores de la infraestructura real.

</details>

---
### Pregunta 7

Los metadatos del state son útiles porque permiten a Terraform:

- A. Omitir por completo la fase de plan
- B. Entender las dependencias entre recursos durante los recorridos del grafo
- C. Escribir módulos automáticamente
- D. Evitar la autenticación del provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los metadatos de dependencias determinan el orden correcto de creación, actualización y destrucción.

</details>

---
### Pregunta 8

¿Qué afirmación sobre el state y el rendimiento es correcta?

- A. El state no tiene ningún rol en el rendimiento
- B. El state guarda en caché los atributos conocidos para que Terraform evite consultas redundantes cuando sea posible
- C. El state deshabilita la caché de los providers
- D. El state solo afecta las operaciones de destroy

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los valores en caché aceleran la planificación al reducir los viajes de ida y vuelta a la API.

</details>

---
### Pregunta 9

¿Cómo se almacenan los datos sensibles dentro del archivo de state de Terraform?

- A. Siempre cifrados e ilegibles en el archivo
- B. En texto plano, a menos que el backend cifre en reposo
- C. Solo como hashes bcrypt
- D. Solo en variables de entorno, nunca en el state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform marca los valores como sensibles en la salida de la CLI, pero el state en sí almacena los valores en texto plano. Cifre los backends y restrinja el acceso.

</details>

---
### Pregunta 10

¿Cómo afecta al almacenamiento del state marcar una variable como sensitive?

- A. Impide que el valor se escriba en el state
- B. Oculta el valor en los logs/salida de la CLI, pero el valor aún puede existir en el state
- C. Cifra automáticamente el valor en el state
- D. Elimina la variable de la configuración

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** sensitive afecta la visualización/redacción en la CLI; el state aún puede contener el secreto en texto plano.

</details>

---
### Pregunta 11

¿Cuál es una buena práctica para los secretos en el state de Terraform?

- A. Hacer commit del state en Git como respaldo
- B. Usar backends remotos con cifrado en reposo y controles de acceso estrictos
- C. Almacenar los secretos solo en comentarios
- D. Deshabilitar el state locking

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Cifre el remote state, restrinja IAM/el acceso y nunca haga commit de los archivos de state.

</details>

---
### Pregunta 12

Un output está marcado con sensitive=true. ¿Dónde podría aparecer aún el valor en texto plano?

- A. En ningún lugar; Terraform nunca lo persiste
- B. En el archivo de state
- C. Solo en la salida de terraform validate
- D. Solo en .terraform.lock.hcl

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los outputs sensibles se redactan en la CLI, pero aún pueden almacenarse en el state.

</details>

---
### Pregunta 13

¿Qué trampa del examen es correcta respecto a los recursos sensibles?

- A. sensitive = true en una variable la elimina del state
- B. El state siempre almacena los valores de los atributos en texto plano en disco
- C. Los backends de remote state nunca almacenan secretos
- D. terraform show nunca revela valores sensibles del state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Trampa del examen: los indicadores sensitive afectan la visualización, no la persistencia del state. Cifre siempre los backends.

</details>

---
### Pregunta 14

En un backend remoto de AWS S3, ¿qué configuración habilita el state locking con DynamoDB?

- A. encrypt = true
- B. dynamodb_table = "locks-table"
- C. acl = "private"
- D. versioning = true

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** dynamodb_table apunta a la tabla de DynamoDB usada como almacén de IDs de lock para operaciones concurrentes.

</details>

---
### Pregunta 15

¿Qué hace encrypt = true en un backend de S3?

- A. Cifra los plugins de provider
- B. Habilita el cifrado del lado del servidor para el objeto de state en S3
- C. Cifra los archivos fuente HCL
- D. Reemplaza la necesidad del locking con DynamoDB

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** encrypt habilita SSE para el objeto de state en reposo en S3.

</details>

---
### Pregunta 16

¿Qué par es una configuración común de backend remoto en producción en AWS?

- A. S3 para almacenar el state y DynamoDB para el locking
- B. EC2 para almacenar el state y RDS para el locking
- C. Lambda para almacenar el state y SNS para el locking
- D. CloudWatch para almacenar el state e IAM para el locking

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** S3 almacena el state; DynamoDB proporciona escrituras condicionales para los IDs de lock.

</details>

---
### Pregunta 17

La configuración del backend de S3 pertenece a qué bloque?

- A. provider "aws"
- B. terraform { backend "s3" { ... } }
- C. resource "aws_s3_bucket"
- D. variable "backend"

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La configuración del backend se declara dentro de terraform { backend "s3" { ... } }.

</details>

---
### Pregunta 18

¿Puede la configuración del backend usar variables arbitrarias de Terraform directamente?

- A. Sí, siempre
- B. No; los bloques backend no pueden referenciar variables ni outputs de módulos
- C. Solo para el nombre del bucket
- D. Solo en Terraform 1.5+

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los bloques backend deben configurarse de forma estática o usar archivos/flags -backend-config en init.

</details>

---
### Pregunta 19

¿Por qué es importante el state locking?

- A. Acelera terraform fmt
- B. Evita que las operaciones apply concurrentes corrompan el state
- C. Cifra las variables
- D. Valida los esquemas de los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los locks garantizan que solo un escritor modifique el state a la vez.

</details>

---
### Pregunta 20

¿Qué sucede si un segundo usuario ejecuta terraform apply mientras hay un lock activo?

- A. El apply continúa normalmente
- B. Terraform se bloquea con un error de lock hasta que el lock se libere
- C. Terraform elimina el lock automáticamente
- D. Terraform migra el state silenciosamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los escritores concurrentes se bloquean para evitar la corrupción del state.

</details>

---
### Pregunta 21

¿Qué comando libera manualmente un lock de state atascado?

- A. terraform unlock
- B. terraform force-unlock <LOCK_ID>
- C. terraform state rm --unlock
- D. terraform init -unlock

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** force-unlock solo debe usarse cuando está seguro de que no hay otra operación en ejecución.

</details>

---
### Pregunta 22

¿Cuándo es apropiado usar terraform force-unlock?

- A. Siempre que apply sea lento
- B. Cuando un lock permanece tras un proceso que falló y no hay otra operación activa
- C. Antes de cada plan
- D. Para eludir las políticas de Sentinel

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Úselo solo cuando el proceso que mantenía el lock ya no exista; forzar el desbloqueo durante ejecuciones activas arriesga la corrupción.

</details>

---
### Pregunta 23

Comportamiento por defecto del backend local respecto al locking:

- A. Usa DynamoDB automáticamente
- B. No proporciona un locking real para escenarios de equipo
- C. Usa locks de Git
- D. Requiere Consul

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El state local en disco no tiene un lock distribuido; los equipos deben usar backends remotos con locking.

</details>

---
### Pregunta 24

¿Qué hace terraform state list?

- A. Destruye todos los recursos listados
- B. Lista las direcciones de los recursos rastreados actualmente en el state
- C. Lista todos los archivos .tf
- D. Lista los mirrors de providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** state list imprime las direcciones de los recursos en el state actual.

</details>

---
### Pregunta 25

¿Qué hace terraform state show <address>?

- A. Muestra los atributos actuales del state del recurso para esa dirección
- B. Muestra el README del provider
- C. Muestra solo el archivo de plan
- D. Elimina el recurso de la nube

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** state show muestra los atributos almacenados de una dirección de recurso.

</details>

---
### Pregunta 26

terraform state pull se usa para:

- A. Subir el state local al remoto
- B. Descargar el state remoto y enviarlo a stdout
- C. Eliminar el state remoto
- D. Importar un recurso

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** state pull obtiene el state remoto para inspección o respaldo.

</details>

---
### Pregunta 27

terraform state push se considera peligroso porque:

- A. Siempre destruye recursos
- B. Puede sobrescribir el state remoto con el state local, eludiendo las verificaciones de seguridad normales
- C. Elimina los locks de forma permanente
- D. Deshabilita los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Push puede pisar el state remoto; úselo solo en escenarios de recuperación controlados.

</details>

---
### Pregunta 28

terraform state replace-provider se usa cuando:

- A. Se renombra un recurso en la configuración
- B. Se migran los registros del state de un origen de provider a otro
- C. Se destruye un provider
- D. Se bloquea el state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** replace-provider reescribe las direcciones de provider en el state durante las migraciones de origen de provider.

</details>

---
### Pregunta 29

¿Qué comando muestra el state o un archivo de plan guardado en formato legible?

- A. terraform graph
- B. terraform show
- C. terraform get
- D. terraform providers mirror

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** terraform show presenta el state o un archivo de plan en un formato legible.

</details>

---
### Pregunta 30

terraform show plan.tfplan muestra:

- A. Solo las versiones de los providers
- B. El contenido de un archivo de plan guardado
- C. Solo los outputs
- D. Solo las variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Pase un archivo de plan guardado para inspeccionar los cambios planificados sin conexión.

</details>

---
### Pregunta 31

¿Qué hace terraform state rm <address>?

- A. Destruye el recurso real en la nube y lo elimina del state
- B. Elimina el recurso solo del state; el recurso real sigue existiendo
- C. Elimina el bloque de configuración .tf
- D. Reemplaza el provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** state rm deja de administrar el recurso; NO destruye la infraestructura. Trampa clásica del examen.

</details>

---
### Pregunta 32

Después de terraform state rm, la infraestructura real:

- A. Siempre se elimina
- B. Sigue existiendo pero ya no está administrada por Terraform
- C. Se importa automáticamente
- D. Queda marcada como tainted

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El recurso queda huérfano desde la perspectiva de Terraform.

</details>

---
### Pregunta 33

¿Por qué podría usar terraform state rm?

- A. Para eliminar recursos de la nube de forma segura
- B. Para dejar de administrar un recurso sin destruirlo
- C. Para renombrar recursos
- D. Para actualizar (refresh) el state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Es útil al transferir recursos a otro equipo o al corregir importaciones erróneas sin destruir.

</details>

---
### Pregunta 34

terraform state mv se usa principalmente para:

- A. Destruir y recrear recursos
- B. Renombrar o mover la dirección de un recurso en el state sin cambiar la infraestructura real
- C. Descargar providers
- D. Cambiar el tipo de backend automáticamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** state mv actualiza las direcciones en el state para refactorizaciones sin cambios en la API.

</details>

---
### Pregunta 35

Al refactorizar el nombre de un recurso en HCL, ¿qué evita destruir y recrear?

- A. Solo editar el nombre sin ninguna acción sobre el state
- B. terraform state mv old.address new.address (o bloques moved en la configuración)
- C. terraform destroy
- D. terraform taint

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** state mv (o los bloques moved) preserva el recurso real mientras actualiza el seguimiento.

</details>

---
### Pregunta 36

terraform state mv afecta:

- A. Solo la asociación de direcciones en el archivo de state
- B. El ID real del recurso en la nube
- C. Las versiones de los plugins de provider
- D. El nombre del bucket del backend

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** mv cambia la dirección de seguimiento de Terraform, no el identificador del recurso real.

</details>

---
### Pregunta 37

¿Qué comando es el reemplazo recomendado del terraform refresh obsoleto?

- A. terraform plan -refresh-only
- B. terraform apply -auto-approve
- C. terraform validate
- D. terraform fmt

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** plan -refresh-only previsualiza la reconciliación del drift; apply -refresh-only aplica solo los cambios de refresh.

</details>

---
### Pregunta 38

¿Qué hace terraform plan -refresh-only?

- A. Crea solo recursos nuevos
- B. Actualiza el state desde la infraestructura real y muestra el drift sin otros cambios planificados
- C. Elimina todos los recursos
- D. Da formato a la configuración

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El modo refresh-only sincroniza el state con la realidad e informa las diferencias.

</details>

---
### Pregunta 39

terraform refresh es:

- A. El comando preferido del flujo de trabajo moderno
- B. Obsoleto en favor de plan/apply -refresh-only
- C. Requerido antes de cada init
- D. Idéntico a terraform destroy

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Enfoque del examen: refresh está obsoleto; use las variantes -refresh-only.

</details>

---
### Pregunta 40

terraform apply -refresh-only:

- A. Aplicará todos los cambios de configuración pendientes
- B. Aplicará solo los cambios de refresh del state para que coincida con la infraestructura real
- C. Omitirá las actualizaciones del state
- D. Eliminará los locks

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Actualiza el state para reflejar los atributos del mundo real sin otros cambios.

</details>

---
### Pregunta 41

El backend local por defecto almacena el state:

- A. Solo en HCP Terraform
- B. Como terraform.tfstate en el directorio de trabajo
- C. Dentro de los binarios del provider
- D. Solo en RAM

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El backend local escribe terraform.tfstate (y su respaldo) de forma local.

</details>

---
### Pregunta 42

Una desventaja clave del state local para los equipos es:

- A. No puede funcionar con providers
- B. No tiene locking compartido ni colaboración integrados entre máquinas
- C. Deshabilita los módulos
- D. Impide el uso de variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los archivos locales son difíciles de compartir de forma segura; los backends remotos resuelven la colaboración.

</details>

---
### Pregunta 43

Los backends remotos proporcionan principalmente:

- A. Generación automática de HCL
- B. Almacenamiento centralizado y duradero y, a menudo, locking para el state
- C. Estimación de costos gratuita en local
- D. Ejecución local de Sentinel

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El almacenamiento remoto junto con el locking sustenta los flujos de trabajo en equipo.

</details>

---
### Pregunta 44

Después de cambiar la configuración del backend, ¿qué comando migra el state existente?

- A. terraform apply -migrate
- B. terraform init -migrate-state
- C. terraform state mv --migrate
- D. terraform get -migrate

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** init -migrate-state copia el state al nuevo backend durante la reinicialización.

</details>

---
### Pregunta 45

terraform init -migrate-state le solicita confirmación cuando:

- A. Faltan providers
- B. Terraform detecta un state existente que debería moverse a un nuevo backend
- C. Hay variables sin definir
- D. Cambian los nombres de los módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Durante los cambios de backend, init ofrece migrar el state existente al nuevo backend.

</details>

---
### Pregunta 46

La migración de backend con -migrate-state copia:

- A. Solo los archivos .tf
- B. El state existente al backend recién configurado
- C. Los plugins de provider a S3
- D. Solo las entradas de la tabla de locks

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La migración transfiere el contenido del state para que el seguimiento continúe sin interrupciones.

</details>

---
### Pregunta 47

¿Debe hacerse commit de terraform.tfstate en el control de versiones?

- A. Sí, siempre
- B. No; puede contener secretos y es específico de cada entorno
- C. Solo si está cifrado con gpg
- D. Solo para módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Nunca haga commit del state; use backends remotos y gestión de secretos.

</details>

---
### Pregunta 48

terraform.tfstate.backup se crea:

- A. Antes de las operaciones que modifican el state, como copia de seguridad
- B. Solo durante fmt
- C. Solo en HCP Terraform
- D. Nunca

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Terraform mantiene un respaldo antes de reescribir el state.

</details>

---
### Pregunta 49

¿Qué archivo relacionado con las dependencias debe someterse a commit?

- A. .terraform/
- B. .terraform.lock.hcl
- C. terraform.tfstate
- D. terraform.tfstate.backup

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El archivo de lock fija las versiones de los providers; los archivos de state no deben someterse a commit.

</details>

---
### Pregunta 50

El state locking con DynamoDB se basa en:

- A. Escrituras condicionales / registros de lock identificados por un ID de lock
- B. Solo el versionado de objetos de S3
- C. Hooks de Git
- D. Nombres de workspace de terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** DynamoDB almacena los metadatos del lock; S3 por sí solo no proporciona locking de Terraform.

</details>

---
### Pregunta 51

Si dos apply se ejecutan de forma concurrente sin locking, el riesgo es:

- A. Un fmt más lento
- B. Corrupción del state o pérdida de actualizaciones
- C. Fallo en la descarga de providers
- D. HCL inválido

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las condiciones de carrera pueden corromper la única fuente de verdad.

</details>

---
### Pregunta 52

terraform state show es diferente de terraform show porque state show:

- A. Muestra una dirección de recurso del state; terraform show puede mostrar el state completo o un archivo de plan
- B. Siempre destruye recursos
- C. Solo funciona de forma remota
- D. Requiere -replace

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** state show apunta a una sola dirección; terraform show es más amplio.

</details>

---
### Pregunta 53

Para inspeccionar el state actual completo en la terminal, use:

- A. Solo terraform state list
- B. terraform show
- C. terraform validate
- D. terraform fmt -check

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** terraform show imprime el state en formato legible (o un plan si se le pasa un archivo de plan).

</details>

---
### Pregunta 54

terraform show -json genera:

- A. Solo arte ASCII
- B. Una representación JSON del state o del plan
- C. Licencias de los providers
- D. Solo variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El formato JSON es útil para herramientas y pipelines de CI.

</details>

---
### Pregunta 55

¿Por qué Terraform mantiene el state? (Seleccione todas las que correspondan.)

- A. Asociar las direcciones de la configuración con los IDs reales de los recursos
- B. Almacenar los binarios de los plugins de provider para uso sin conexión
- C. Guardar en caché los atributos de los recursos para mejorar el rendimiento
- D. Rastrear metadatos y dependencias
- E. Permitir la colaboración mediante remote state compartido

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, C, D, E**

**Explicación:** El state asocia, guarda en caché, rastrea metadatos/dependencias y permite la colaboración. Los binarios de provider no se almacenan en el state.

</details>

---
### Pregunta 56

¿Qué afirmaciones sobre los datos sensibles y el state son verdaderas? (Seleccione todas las que correspondan.)

- A. El state puede contener secretos en texto plano en disco
- B. sensitive = true impide que los valores se almacenen alguna vez en el state
- C. Cifrar los backends remotos ayuda a proteger los datos en reposo
- D. terraform.tfstate no debe someterse a commit en el VCS
- E. Los indicadores sensitive afectan principalmente la redacción en la CLI

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, C, D, E**

**Explicación:** Las marcas sensitive redactan la salida de la CLI; los valores aún pueden estar en texto plano en el state. Cifre los backends y nunca haga commit del state.

</details>

---
### Pregunta 57

¿Qué subcomandos de terraform state son válidos? (Seleccione todas las que correspondan.)

- A. terraform state list
- B. terraform state show
- C. terraform state mv
- D. terraform state destroy
- E. terraform state replace-provider

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** Los subcomandos válidos incluyen list, show, mv, rm, pull, push, replace-provider. No existe state destroy.

</details>

---
### Pregunta 58

¿Qué afirmaciones sobre el state locking son correctas? (Seleccione todas las que correspondan.)

- A. El locking evita que las escrituras concurrentes corrompan el state
- B. S3 por sí solo proporciona locking nativo de Terraform sin DynamoDB
- C. terraform force-unlock debe usarse con cautela
- D. Los backends locales ofrecen locking distribuido para equipos por defecto
- E. Un lock atascado por un proceso que falló puede requerir force-unlock

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, C, E**

**Explicación:** S3 necesita DynamoDB (u otro mecanismo) para el locking; los backends locales carecen de locking para equipos.

</details>

---
### Pregunta 59

¿Qué pares son correctos para las operaciones de state? (Seleccione todas las que correspondan.)

- A. state rm — elimina solo del state, no destruye
- B. state mv — refactoriza direcciones sin destruir los recursos reales
- C. state rm — destruye el recurso en la nube y lo elimina del state
- D. state push — puede sobrescribir el remote state de forma peligrosa
- E. import — incorpora infraestructura existente a la administración de Terraform

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D, E**

**Explicación:** state rm NO destruye. import administra infraestructura existente. state push es peligroso.

</details>

---
### Pregunta 60

¿Qué afirmaciones sobre refresh y los backends son verdaderas? (Seleccione todas las que correspondan.)

- A. terraform refresh está obsoleto
- B. plan -refresh-only previsualiza la reconciliación del drift
- C. init -migrate-state mueve el state al cambiar de backend
- D. Los backends remotos ayudan a los equipos a compartir el state
- E. Los bloques backend pueden referenciar var.backend_name directamente

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, D**

**Explicación:** Los bloques backend no pueden referenciar variables. Refresh está obsoleto; use -refresh-only.

</details>

---
