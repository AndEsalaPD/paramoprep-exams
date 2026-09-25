# Interactuar con módulos de Terraform

> **Dominio del examen:** Interactuar con módulos de Terraform | **Peso:** 8-10%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre módulo raíz vs. módulos hijos, sources, inputs/outputs, versionado, convenciones del registry y mejores prácticas de módulos.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Qué es el módulo raíz (root module) en un proyecto de Terraform?

- A. El módulo publicado de nivel superior en el Terraform Registry
- B. El directorio de trabajo donde se ejecutan los comandos de Terraform
- C. Cualquier módulo que define configuraciones de provider
- D. El primer bloque module en orden alfabético en main.tf

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El módulo raíz es la configuración del directorio donde se ejecuta `terraform`; puede invocar módulos hijos.

</details>

---
### Pregunta 2

¿Qué es un módulo hijo (child module)?

- A. Un módulo que no puede definir variables
- B. Un módulo invocado desde otro módulo mediante un bloque `module`
- C. Un módulo almacenado únicamente en GitHub
- D. Una ruta de módulo local obsoleta

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los módulos hijos son invocados por bloques `module` en el módulo raíz o en otro módulo. Encapsulan infraestructura reutilizable.

</details>

---
### Pregunta 3

¿Cómo se referencia un output llamado `vpc_id` de un bloque module con la etiqueta `network`?

- A. output.network.vpc_id
- B. module.network.vpc_id
- C. var.network.vpc_id
- D. data.network.vpc_id

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los outputs de un módulo usan `module.<module_name>.<output_name>`. La etiqueta del módulo proviene de la etiqueta del bloque `module`.

</details>

---
### Pregunta 4

¿Qué valor de `source` referencia un módulo en `./modules/vpc` relativo al módulo que lo invoca?

- A. modules/vpc
- B. ./modules/vpc
- C. local://modules/vpc
- D. path.module/vpc

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los módulos locales usan rutas del sistema de archivos como `./modules/vpc` o `../shared/vpc`. `path.module` se usa dentro de un módulo, no como prefijo de source.

</details>

---
### Pregunta 5

¿Cuál es el formato de source del registry para el namespace `terraform-aws-modules`, nombre `vpc`, provider `aws`?

- A. hashicorp/terraform-aws-modules/vpc
- B. terraform-aws-modules/vpc/aws
- C. registry.terraform.io/vpc/aws
- D. aws/terraform-aws-modules/vpc

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los módulos del registry público usan `namespace/name/provider` (p. ej., `terraform-aws-modules/vpc/aws`).

</details>

---
### Pregunta 6

¿Qué URL de source de módulo usa la sintaxis de subdirectorio de Git?

- A. github.com/org/repo/modules/vpc
- B. github.com/org/repo//modules/vpc
- C. git::github.com/org/repo:modules/vpc
- D. s3::github.com/org/repo/modules/vpc

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La doble barra `//` separa la URL del repositorio de la ruta del subdirectorio dentro del repositorio.

</details>

---
### Pregunta 7

¿Cómo se fija (pin) un módulo del registry público a la versión `5.1.0`?

- A. Agregar version = "5.1.0" dentro del bloque module
- B. Establecer required_version solo en el módulo hijo
- C. Usar terraform init -version 5.1.0
- D. El pinning es automático desde el registry

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los módulos del registry admiten un argumento `version` en el bloque `module`. Siempre fije las versiones para garantizar reproducibilidad.

</details>

---
### Pregunta 8

¿Cuáles son sources de módulos de Terraform válidos? Seleccione todas las que correspondan.

- A. ./modules/vpc
- B. terraform-aws-modules/vpc/aws
- C. github.com/hashicorp/consul//modules/consul-aws
- D. git::https://example.com/vpc.git

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, D**

**Explicación:** Los módulos pueden obtenerse desde rutas locales, el registry público, URLs de GitHub/Git y buckets de S3. Todas las formas listadas son válidas.

</details>

---
### Pregunta 9

¿Qué hace `terraform init` con respecto a los módulos?

- A. Nada; los módulos se cargan solo en el momento del apply
- B. Descarga e instala los módulos declarados en los bloques module
- C. Publica módulos en el registry
- D. Compila los módulos en plugins de provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform init` instala providers, inicializa el backend y descarga los módulos en `.terraform/modules`.

</details>

---
### Pregunta 10

¿En qué se diferencia `terraform get` de `terraform init` respecto a los módulos?

- A. get también instala providers y backends
- B. get descarga o actualiza módulos sin los efectos secundarios de un init completo
- C. get solo funciona con módulos locales
- D. get está obsoleto y fue eliminado en Terraform 1.0

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform get` (o `terraform get -update`) actualiza los módulos. `init` realiza la inicialización completa, incluidos providers y backend.

</details>

---
### Pregunta 11

¿Los módulos hijos heredan automáticamente las configuraciones de provider del módulo raíz?

- A. Sí, todos los providers se transmiten implícitamente
- B. No, los providers deben pasarse explícitamente o configurarse en el módulo hijo
- C. Solo para el provider por defecto
- D. Solo cuando se usan módulos del registry

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Una trampa común del examen: los módulos hijos no heredan las configuraciones de provider. Use el argumento `providers` o `configuration_aliases`.

</details>

---
### Pregunta 12

¿Puede el módulo raíz acceder al valor local interno de un módulo hijo sin un output?

- A. Sí, mediante module.<name>.local.<value>
- B. No, solo los outputs declarados son accesibles fuera del módulo
- C. Sí, si la variable no tiene valor por defecto
- D. Solo en terraform console

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los elementos internos del módulo están encapsulados. Exponga los valores mediante bloques `output` para usarlos fuera del módulo.

</details>

---
### Pregunta 13

¿Qué convención de nombres siguen típicamente los módulos publicados en el registry?

- A. provider-terraform-NAME
- B. terraform-PROVIDER-NAME
- C. NAME-terraform-provider
- D. hashicorp-NAME-provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La convención del registry es `terraform-<PROVIDER>-<NAME>` (p. ej., `terraform-aws-vpc`).

</details>

---
### Pregunta 14

¿Dónde se almacenan en caché localmente los módulos descargados?

- A. .terraform/modules/
- B. modules/.cache/
- C. terraform.tfstate.d/modules/
- D. .terraform/providers/

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los sources de módulos se almacenan en `.terraform/modules/`. Los plugins de provider residen en `.terraform/providers/`.

</details>

---
### Pregunta 15

¿Se puede usar el argumento `version` con un source de módulo de GitHub?

- A. Sí, siempre
- B. No, el pinning de versión aplica a módulos del registry; use refs de Git (ref=) para sources de Git
- C. Solo con sources de S3
- D. Solo en Terraform Enterprise

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El argumento `version` es para módulos del registry. Los sources de Git usan `?ref=<tag>` en la URL para fijar la versión.

</details>

---
### Pregunta 16

¿Qué afirmaciones sobre los inputs y outputs de módulos son verdaderas? Seleccione todas las que correspondan.

- A. Las variables de entrada se establecen mediante argumentos en el bloque module
- B. Los outputs deben declararse para poder referenciarse fuera del módulo
- C. Todas las entradas de variables.tf son automáticamente outputs
- D. module.<name>.<output> referencia un valor de output

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Los inputs se pasan como argumentos del bloque module. Los outputs deben declararse explícitamente. Las variables no se exponen automáticamente como outputs.

</details>

---
### Pregunta 17

¿Qué sucede si se cambia la URL de `source` de un módulo?

- A. Nada hasta el apply
- B. Hay que volver a ejecutar terraform init para instalar el nuevo source
- C. El state se migra automáticamente
- D. El módulo anterior permanece en caché de forma permanente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Cambiar `source` (o la versión) requiere reinicialización para que Terraform descargue el paquete de módulo correcto.

</details>

---
### Pregunta 18

¿Puede un módulo invocar a otro módulo?

- A. No, el anidamiento está limitado a un nivel
- B. Sí, los módulos pueden contener bloques module (módulos anidados)
- C. Solo los módulos raíz pueden anidar
- D. Solo los módulos del registry pueden anidar

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los módulos pueden anidarse de forma arbitraria. Un módulo hijo puede invocar sus propios módulos hijos.

</details>

---
### Pregunta 19

¿Qué es `path.module` dentro de un módulo hijo?

- A. El directorio del módulo raíz
- B. La ruta del sistema de archivos del módulo actual
- C. El namespace del registry
- D. La ruta del backend remoto

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `path.module` es la ruta del módulo cuya configuración se está evaluando; es útil para referenciar archivos dentro del módulo.

</details>

---
### Pregunta 20

¿Qué argumento asigna los providers del módulo padre a un módulo hijo?

- A. provider
- B. providers
- C. alias
- D. solo required_providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El meta-argumento `providers` pasa configuraciones de provider: `providers = { aws = aws.us }`.

</details>

---
### Pregunta 21

Para un source de módulo en S3, ¿qué prefijo es el correcto?

- A. s3://bucket/key
- B. s3::https://s3.amazonaws.com/bucket/key
- C. aws-s3://bucket/key
- D. module-s3://bucket/key

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los sources de módulos en S3 usan el prefijo `s3::` con una URL HTTPS al objeto (a menudo un archivo zip).

</details>

---
### Pregunta 22

¿Cuáles son verdaderas sobre `terraform init` vs `terraform get`? Seleccione todas las que correspondan.

- A. init instala providers
- B. get puede actualizar módulos con -update
- C. init es necesario después de agregar un nuevo bloque module
- D. get configura el backend remoto

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** init se encarga de providers, backend y módulos. `terraform get -update` actualiza los módulos. La configuración del backend es parte de init, no de get.

</details>

---
### Pregunta 23

Si un bloque module omite una variable de entrada requerida, ¿cuándo se detecta el error?

- A. Solo en el momento del apply en la API de la nube
- B. Durante plan o validate, cuando Terraform evalúa la invocación del módulo
- C. Nunca, siempre se aplican los valores por defecto
- D. Solo durante terraform init

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los argumentos requeridos del módulo que faltan se detectan durante validate/plan, cuando Terraform verifica la invocación del módulo contra las definiciones de variables.

</details>

---
### Pregunta 24

¿Pueden dos bloques module usar el mismo `source` con etiquetas diferentes?

- A. No, el source debe ser único por configuración
- B. Sí, etiquetas diferentes crean instancias de módulo separadas
- C. Solo si las versiones difieren
- D. Solo para módulos locales

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La etiqueta del bloque module distingue las instancias. El mismo source puede usarse varias veces con inputs diferentes.

</details>

---
### Pregunta 25

¿Qué archivo de un módulo suele declarar las variables de entrada?

- A. outputs.tf
- B. variables.tf
- C. solo providers.tf
- D. terraform.tfstate

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La convención coloca los bloques `variable` en `variables.tf` (o en cualquier archivo .tf). Los outputs van en `outputs.tf`.

</details>

---
### Pregunta 26

¿Deben los bloques module incluir un argumento `source`?

- A. No, source es opcional para módulos locales
- B. Sí, todo bloque module requiere source
- C. Solo para módulos del registry
- D. Solo cuando se usa count

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `source` es obligatorio: le indica a Terraform desde dónde cargar el módulo.

</details>

---
### Pregunta 27

¿Para qué se usa principalmente un registry de módulos privado?

- A. Almacenar archivos terraform.tfstate
- B. Alojar módulos internos de la organización con versionado y control de acceso
- C. Reemplazar la necesidad de variables
- D. Ejecutar terraform apply solo en la nube

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los registries privados (p. ej., HCP Terraform) alojan módulos internos con el mismo patrón `namespace/name/provider` que el registry público.

</details>

---
### Pregunta 28

¿Qué afirmaciones sobre la herencia de providers son correctas? Seleccione todas las que correspondan.

- A. Los módulos hijos no heredan automáticamente los providers del padre
- B. El meta-argumento providers puede pasar configuraciones de provider explícitas
- C. configuration_aliases permite múltiples configuraciones de provider en un módulo
- D. Los módulos del registry siempre usan automáticamente las credenciales de AWS del módulo raíz

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** Los providers deben pasarse explícitamente o declararse en los módulos. Los módulos del registry no heredan credenciales por arte de magia.

</details>

---
### Pregunta 29

¿Qué define la etiqueta `vpc` del bloque `module "vpc"`?

- A. El namespace del registry
- B. El nombre local usado para referenciar esta instancia del módulo
- C. La etiqueta (tag) del nombre del recurso en la nube
- D. El tipo de provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La cadena entre comillas es el nombre de la instancia del módulo, usado en referencias como `module.vpc.vpc_id`.

</details>

---
### Pregunta 30

¿Se puede referenciar `module.foo.bar` si `bar` es una variable de entrada dentro del módulo foo?

- A. Sí, todas las variables se exportan
- B. No, solo los valores de output son accesibles mediante module.foo
- C. Solo con terraform console
- D. Solo si bar tiene un valor por defecto

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las variables de entrada no son accesibles fuera del módulo. Solo los outputs aparecen en el namespace del módulo.

</details>

---
### Pregunta 31

Al usar un módulo del registry, ¿dónde se evalúa la restricción de `version`?

- A. Contra las versiones disponibles en el registry durante init
- B. Solo durante terraform apply en la nube
- C. Por el plugin del provider
- D. Por terraform fmt

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Durante init, Terraform resuelve la restricción de versión del módulo y descarga la release que coincide.

</details>

---
### Pregunta 32

¿Cuál es el efecto de `terraform init -upgrade` sobre los módulos?

- A. Ignora los módulos por completo
- B. Puede actualizar los módulos a versiones más recientes permitidas por las restricciones de versión
- C. Elimina todos los outputs de los módulos
- D. Publica los módulos en el registry

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-upgrade` vuelve a resolver las versiones de providers y módulos a las más recientes permitidas por las restricciones.

</details>

---
### Pregunta 33

¿Qué forma de source de Git incluye un parámetro de consulta ref explícito?

- A. git::https://example.com/repo.git?ref=v1.2.0
- B. git::https://example.com/repo.git//ref=v1.2.0
- C. github.com/example/repo/ref/v1.2.0
- D. git+ref://example.com/repo

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Fije los sources de módulos Git agregando `?ref=<tag|branch|commit>` a la URL.

</details>

---
### Pregunta 34

¿Pueden los módulos contener bloques `resource`?

- A. No, solo el módulo raíz puede
- B. Sí, los módulos definen recursos como cualquier configuración
- C. Solo data sources
- D. Solo con HCP Terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los módulos son configuración estándar de Terraform que contiene recursos, data sources, variables, outputs, etc.

</details>

---
### Pregunta 35

¿Qué ejemplos de source de módulo son sintácticamente válidos? Seleccione todas las que correspondan.

- A. source = "./modules/network"
- B. source = "terraform-aws-modules/eks/aws"
- C. source = "git::ssh://git@example.com/vpc.git"
- D. source = "module.vpc"

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** `module.vpc` es una sintaxis de referencia, no una ruta de source válida. Las rutas locales, las coordenadas del registry y las URLs de Git son sources válidos.

</details>

---
### Pregunta 36

¿Por qué se deben fijar las versiones de los módulos en producción?

- A. Para acelerar terraform plan
- B. Para garantizar despliegues reproducibles y evitar cambios inesperados en el upstream
- C. Porque los módulos sin versión fija fallan en terraform validate
- D. Para habilitar force-unlock

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las versiones sin fijar o con restricciones laxas pueden traer cambios incompatibles en el siguiente init, causando drift inesperado en la infraestructura.

</details>

---
### Pregunta 37

¿Qué se obtiene si se referencia un output de módulo inexistente?

- A. null silenciosamente
- B. Un error de Terraform durante plan o apply
- C. El valor por defecto de la variable
- D. Una cadena vacía

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Referenciar `module.foo.nonexistent` falla en validate/plan porque el output no está declarado en el módulo hijo.

</details>

---
### Pregunta 38

¿Tiene el módulo raíz un bloque `module` que se invoque a sí mismo?

- A. Sí, es necesario para la inicialización
- B. No, el módulo raíz es implícito y no se declara con un bloque module
- C. Solo en HCP Terraform
- D. Solo cuando se usa count

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El módulo raíz es la configuración del directorio de trabajo. Solo los módulos hijos aparecen en bloques `module`.

</details>

---
### Pregunta 39

¿Pueden los outputs de un módulo usarse en `terraform output` en la raíz?

- A. Solo si se vuelven a exponer mediante un bloque output en la raíz
- B. Automáticamente, todos los outputs de módulos aparecen en la raíz
- C. Nunca
- D. Solo para módulos del registry

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los bloques `output` de la raíz deben exponer los valores explícitamente. Los outputs de módulos no se promueven automáticamente a outputs de la raíz.

</details>

---
### Pregunta 40

¿Qué directorio se crea cuando se descargan módulos durante init?

- A. .terraform/modules/<module_key>/
- B. modules/downloaded/
- C. terraform-modules/
- D. .modules/cache/

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Terraform almacena los módulos extraídos en `.terraform/modules/` con claves internas que se asignan a las invocaciones de módulos.

</details>

---
### Pregunta 41

Al pasar providers a un módulo hijo, ¿qué sucede si no se pasa un provider requerido?

- A. Terraform usa el provider null
- B. Terraform puede fallar porque la configuración de provider del módulo hijo está incompleta
- C. Siempre se usa automáticamente el provider de la raíz
- D. Solo se muestran advertencias

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Sin herencia explícita ni bloques provider dentro del módulo, la falta de asignaciones de provider causa errores de configuración.

</details>

---
### Pregunta 42

¿Qué es verdadero sobre el namespace de un módulo en el Terraform Registry?

- A. Siempre debe ser `hashicorp`
- B. Es la organización o el usuario que publica el módulo (p. ej., terraform-aws-modules)
- C. Coincide con la región del proveedor de nube
- D. Es el número de versión del módulo

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El namespace identifica al publicador. `hashicorp` es solo un namespace entre muchos.

</details>

---
### Pregunta 43

¿Qué prácticas siguen las mejores prácticas de módulos para el examen? Seleccione todas las que correspondan.

- A. Fijar las versiones de los módulos del registry
- B. Exponer solo los valores necesarios mediante outputs
- C. Confiar en la herencia implícita de providers
- D. Usar etiquetas significativas en los bloques module

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Fije las versiones, minimice los outputs expuestos y use etiquetas claras. La herencia implícita de providers es incorrecta: pase los providers explícitamente.

</details>

---
### Pregunta 44

¿Puede `terraform get` instalar providers?

- A. Sí, igual que init
- B. No, se enfoca en la instalación/actualización de módulos
- C. Solo el provider de AWS
- D. Solo con -upgrade

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La instalación de providers es responsabilidad de `terraform init`. `get` está orientado a módulos.

</details>

---
### Pregunta 45

¿Qué archivo de metadatos bloquea las versiones de módulos y providers para lograr ejecuciones consistentes?

- A. .terraform.lock.hcl
- B. terraform.tfvars
- C. modules.lock
- D. solo versions.tf

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** `.terraform.lock.hcl` registra las versiones exactas de los providers (y de los módulos, donde aplique). Inclúyalo en el control de versiones.

</details>

---
### Pregunta 46

En `module "app" { source = "..." }`, ¿es `app` el nombre del módulo en el registry?

- A. Sí
- B. No, es el nombre local de la instancia; el nombre en el registry está en source
- C. Es el nombre del provider
- D. Es el nombre del archivo de state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La etiqueta del bloque es el nombre de instancia que usted elige. La identidad en el registry proviene de la cadena `source`.

</details>

---
### Pregunta 47

¿Están las variables de entrada de los módulos disponibles automáticamente como variables de entorno?

- A. Sí, el prefijo TF_VAR_ aplica globalmente a los inputs de módulos
- B. No, los inputs de módulos se establecen solo mediante el bloque module, salvo que se use TF_VAR para variables del módulo raíz
- C. Solo en HCP Terraform
- D. Solo para variables de tipo string

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** TF_VAR_ aplica a las variables del módulo raíz. Los inputs de los módulos hijos se pasan explícitamente en el bloque module.

</details>

---
### Pregunta 48

¿Qué sucede al eliminar un bloque module de la configuración?

- A. Nada
- B. El siguiente plan propone destruir los recursos que gestionaba ese módulo (a menos que se muevan o se eliminen del state)
- C. terraform init falla permanentemente
- D. Los archivos del módulo en .terraform/modules se eliminan del disco inmediatamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Eliminar la invocación de un módulo significa que Terraform deja de gestionar esos recursos: el plan muestra destrucciones a menos que se usen operaciones sobre el state.

</details>

---
### Pregunta 49

¿Puede una misma configuración usar sources de módulos locales y del registry?

- A. No, todos los módulos deben compartir un mismo tipo de source
- B. Sí, cada bloque module tiene su propio source
- C. Solo en workspaces separados
- D. Solo con terraform cloud

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Distintos bloques `module` pueden combinar libremente sources de rutas locales, registry, Git y S3.

</details>

---
### Pregunta 50

¿Cuál es el tercer componente en las coordenadas `namespace/name/provider` del registry?

- A. La versión de Terraform
- B. El provider implícito del módulo (p. ej., aws)
- C. La región de AWS
- D. El nombre del output del módulo

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El tercer segmento es el tipo de provider al que apunta el módulo (p. ej., `aws`, `google`, `azurerm`).

</details>

---
### Pregunta 51

¿Por qué usar módulos en lugar de copiar archivos .tf?

- A. Los módulos se ejecutan más rápido que los recursos sueltos
- B. Los módulos permiten reutilización, encapsulación e interfaces consistentes mediante inputs/outputs
- C. Los módulos no usan state
- D. Los módulos reemplazan a los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los módulos empaquetan patrones de infraestructura para su reutilización y mantienen contratos claros mediante variables y outputs.

</details>

---
### Pregunta 52

Después de clonar un repositorio con módulos, ¿qué comando se debe ejecutar primero?

- A. terraform apply
- B. terraform init
- C. terraform destroy
- D. terraform graph

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Init descarga los módulos y providers antes de que plan/apply puedan tener éxito.

</details>

---
### Pregunta 53

¿Puede la `version` de un módulo usar operadores de restricción como `~> 5.0`?

- A. No, solo versiones exactas
- B. Sí, version admite sintaxis de restricciones como los providers
- C. Solo en required_providers
- D. Solo para módulos locales

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los argumentos version de los módulos aceptan restricciones de versión (p. ej., `~> 5.0`, `>= 4.0, < 6.0`) para módulos del registry.

</details>

---
### Pregunta 54

¿Qué hace `terraform init -reconfigure` respecto a los módulos?

- A. Omite por completo la descarga de módulos
- B. Reinicializa el backend sin solicitar migración; aun así procesa la instalación de módulos como en init
- C. Elimina todos los outputs de módulos del state
- D. Publica los módulos en un registry privado

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-reconfigure` ignora la migración del backend y reinicializa. Los módulos se siguen instalando durante init como de costumbre.

</details>

---
### Pregunta 55

¿Puede un módulo exponer valores sensibles mediante outputs?

- A. No, los outputs no pueden ser sensibles
- B. Sí, usando `sensitive = true` en el bloque output
- C. Solo los módulos raíz pueden marcar la sensibilidad
- D. La sensibilidad es automática para todas las contraseñas

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los outputs de módulos admiten `sensitive = true`, lo que oculta los valores en la salida de la CLI pero permite seguir usándolos en la configuración.

</details>

---
### Pregunta 56

¿Para qué se usa el meta-argumento `count` en un bloque module?

- A. Contar recursos solo en el state
- B. Crear múltiples instancias del mismo módulo desde un solo bloque
- C. Fijar versiones de módulos
- D. Reemplazar terraform.workspace

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `count` (o `for_each`) en un bloque module crea múltiples instancias del módulo, referenciadas como `module.name[0]`, etc.

</details>

---
### Pregunta 57

¿Cómo se referencia un output de una instancia de módulo creada con `count`?

- A. solo module.vpc.output_name
- B. module.vpc[0].output_name
- C. count.module.vpc.output_name
- D. module.output_name[0]

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las instancias de módulo indexadas usan notación de corchetes: `module.<name>[<index>].<output>`.

</details>

---
### Pregunta 58

¿`terraform get -update` reinstala los providers?

- A. Sí, igual que init -upgrade
- B. No, actualiza los paquetes de módulos sin un init completo
- C. Solo actualiza .terraform.lock.hcl
- D. Elimina la configuración del backend

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `get -update` actualiza los módulos para que coincidan con los sources/restricciones; la gestión de providers sigue siendo trabajo de init.

</details>

---
### Pregunta 59

Cuando un módulo raíz define `source = "./modules/app"`, ¿desde dónde se resuelve esa ruta?

- A. El directorio del módulo hijo
- B. El directorio que contiene el bloque module (el invocador), normalmente la raíz
- C. El directorio de instalación de Terraform
- D. La raíz del bucket del backend remoto

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las rutas locales relativas en `source` se resuelven desde el directorio del módulo que invoca, no desde el módulo hijo.

</details>

---
### Pregunta 60

¿Qué sucede si dos bloques module usan el mismo nombre de etiqueta?

- A. Terraform los fusiona
- B. Terraform reporta un error de nombre de módulo duplicado
- C. El segundo sobrescribe al primero silenciosamente
- D. Solo se descarga el primero

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las etiquetas de los bloques module deben ser únicas dentro de un módulo. Las etiquetas duplicadas causan un error de configuración.

</details>

---
