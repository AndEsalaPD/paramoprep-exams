# Uso de la CLI de Terraform (fuera del flujo de trabajo principal)

> **Dominio del examen:** Uso de la CLI de Terraform (fuera del flujo de trabajo principal) | **Peso:** 8-10%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre workspaces, import, bloques moved, logging, graph, console, taint/replace, force-unlock, provisioners y bloques dynamic.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Qué administra el comando `terraform workspace`?

- A. Las credenciales del backend remoto para HCP Terraform
- B. Múltiples archivos de state aislados dentro del mismo directorio de configuración
- C. Copias separadas de todos los archivos de configuración .tf por entorno
- D. Las versiones de los plugins de provider para cada etapa de despliegue

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los workspaces de la CLI aíslan el state (terraform.tfstate.d/<name>/) mientras comparten la misma configuración. No son árboles de configuración separados ni objetos de workspace de HCP.

</details>

---
### Pregunta 2

¿Qué comando crea un nuevo workspace de la CLI de Terraform llamado `staging`?

- A. terraform workspace create staging
- B. terraform workspace new staging
- C. terraform workspace add staging
- D. terraform workspace init staging

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El subcomando es `new`, no `create` ni `add`. `terraform workspace new staging` crea el nuevo workspace y cambia a él.

</details>

---
### Pregunta 3

¿Cómo se cambia el workspace activo de la CLI a `prod`?

- A. terraform workspace use prod
- B. terraform workspace switch prod
- C. terraform workspace select prod
- D. terraform workspace set prod

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: C**

**Explicación:** `terraform workspace select <name>` cambia el workspace activo. No existen los subcomandos `use`, `switch` ni `set`.

</details>

---
### Pregunta 4

¿Qué muestra `terraform workspace show`?

- A. Una lista de todos los workspaces con un asterisco en el actual
- B. El nombre del workspace actualmente seleccionado
- C. El contenido detallado del state del workspace actual
- D. Las sobrescrituras de variables específicas del workspace desde terraform.tfvars

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `show` imprime únicamente el nombre del workspace actual. Use `terraform workspace list` para ver todos los workspaces.

</details>

---
### Pregunta 5

En una configuración HCL, ¿qué devuelve `terraform.workspace`?

- A. La ruta del sistema de archivos al archivo de state del workspace activo
- B. El nombre del workspace de la CLI actualmente seleccionado
- C. El slug del workspace de HCP Terraform configurado en el backend
- D. El nombre de workspace predeterminado de terraform.tfvars

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform.workspace` es una expresión integrada que devuelve el nombre del workspace actual de la CLI (p. ej., `default`, `dev`, `prod`).

</details>

---
### Pregunta 6

¿Qué sucede al eliminar el workspace activo con `terraform workspace delete`?

- A. Terraform selecciona automáticamente `default` y elimina el workspace
- B. El comando falla; primero debe cambiar a otro workspace antes de eliminarlo
- C. Todos los recursos de ese workspace se destruyen automáticamente
- D. El workspace se archiva pero el state se conserva

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** No se puede eliminar el workspace que se está usando actualmente. Primero seleccione otro workspace y luego elimine.

</details>

---
### Pregunta 7

¿Dónde se almacena el state de un workspace de la CLI que no es el predeterminado, llamado `dev`?

- A. En un subdirectorio `dev/` separado que contiene sus propios archivos .tf
- B. En `terraform.tfstate.d/dev/terraform.tfstate`
- C. En el backend remoto, bajo una clave de workspace que coincide con `dev`
- D. En `.terraform/workspaces/dev/terraform.tfstate` solo para backends locales

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los workspaces de la CLI almacenan el state en `terraform.tfstate.d/<workspace>/`. El workspace predeterminado usa `terraform.tfstate` en la raíz.

</details>

---
### Pregunta 8

¿Cuáles de los siguientes son subcomandos válidos de `terraform workspace`? Seleccione todas las que correspondan.

- A. list
- B. new
- C. rename
- D. delete

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Los subcomandos válidos son `list`, `new`, `select`, `show` y `delete`. No existe un subcomando `rename` ni `create`.

</details>

---
### Pregunta 9

¿Cuál es el nombre del workspace de la CLI predeterminado cuando no se ha creado ninguno?

- A. main
- B. default
- C. production
- D. root

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Toda configuración comienza en el workspace `default` hasta que se crean y seleccionan otros.

</details>

---
### Pregunta 10

¿Pueden dos workspaces de la CLI en el mismo directorio usar versiones de provider diferentes de forma simultánea?

- A. Sí, cada workspace mantiene su propio archivo de lock de providers
- B. No, las versiones de provider se definen en la configuración compartida y en el archivo de lock del directorio
- C. Sí, pero solo cuando se usa un backend remoto
- D. Solo si cada workspace tiene su propio bloque backend

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los workspaces aíslan el state, no la configuración. Todos los workspaces comparten los mismos archivos .tf y el mismo `.terraform.lock.hcl`.

</details>

---
### Pregunta 11

¿Cuál es la sintaxis tradicional de la CLI para importar una instancia existente de AWS al state?

- A. terraform import -id=i-abc123 aws_instance.web
- B. terraform import aws_instance.web i-abc123
- C. terraform state import aws_instance.web i-abc123
- D. terraform plan -import aws_instance.web i-abc123

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform import <resource_address> <resource_id>` agrega un recurso existente al state. Primero va la dirección y luego el ID del proveedor de nube.

</details>

---
### Pregunta 12

¿Qué declara un bloque `import` en la configuración?

- A. Que Terraform debe exportar el state a un archivo después de apply
- B. La dirección del recurso de destino y el ID en la nube para una importación basada en plan
- C. Una URL de origen de module para importar módulos del registry
- D. Que un recurso debe destruirse antes de recrearse

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los bloques import (`import { to = ..., id = ... }`) declaran la intención; Terraform realiza la importación durante plan/apply cuando se usa el flujo de trabajo moderno.

</details>

---
### Pregunta 13

¿Qué opción genera la configuración de los recursos declarados en bloques `import`?

- A. terraform apply -generate-config
- B. terraform plan -generate-config-out=generated.tf
- C. terraform import -config-out=generated.tf
- D. terraform console -generate-config

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform plan -generate-config-out=<file>` produce bloques de recursos sugeridos para los destinos de importación, lo que reduce la escritura manual de HCL.

</details>

---
### Pregunta 14

¿`terraform import` (CLI) modifica sus archivos de configuración .tf?

- A. Sí, escribe automáticamente un bloque resource equivalente
- B. No, solo actualiza el state; debe escribir la configuración por separado
- C. Sí, pero solo cuando se usa -generate-config-out
- D. Modifica variables.tf con el ID importado

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La importación por CLI solo actualiza el state. Aún necesita la configuración correspondiente. La importación basada en plan con `-generate-config-out` puede ayudar a generar la configuración.

</details>

---
### Pregunta 15

Después de agregar un bloque `import`, ¿qué comando aplica la importación como parte del flujo de trabajo normal?

- A. terraform import apply
- B. terraform apply (después de que plan muestre la acción de importación)
- C. terraform init -import
- D. terraform validate -import

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Con bloques import, `terraform plan` muestra una vista previa de la importación y `terraform apply` la ejecuta; no se requiere un comando de importación aparte.

</details>

---
### Pregunta 16

¿Qué afirmaciones sobre la importación en Terraform son correctas? Seleccione todas las que correspondan.

- A. Import incorpora la infraestructura existente a la administración de Terraform
- B. La importación por CLI requiere que usted escriba la configuración de recurso correspondiente
- C. Los bloques import se evalúan durante plan y apply
- D. Import destruye y recrea automáticamente el recurso

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** Import asocia los recursos existentes con el state sin recrearlos. La configuración debe coincidir con el recurso real. Los bloques import se integran con plan/apply; no destruyen recursos.

</details>

---
### Pregunta 17

¿Cuál es el propósito principal de un bloque `moved`?

- A. Migrar el state entre backends remotos
- B. Registrar cambios de dirección de recursos sin destruir y recrear
- C. Mover archivos .tf a un directorio de module en disco
- D. Transferir la propiedad de un recurso a otra cuenta de AWS

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `moved { from = ... to = ... }` le indica a Terraform que el recurso fue renombrado o reubicado en la configuración, y actualiza en el lugar el mapeo del state.

</details>

---
### Pregunta 18

Al refactorizar `aws_instance.web` hacia `module.compute.aws_instance.web`, ¿qué bloque evita el reemplazo?

- A. import { to = module.compute.aws_instance.web id = ... }
- B. moved { from = aws_instance.web to = module.compute.aws_instance.web }
- C. terraform state replace aws_instance.web module.compute.aws_instance.web
- D. lifecycle { prevent_destroy = true }

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Un bloque `moved` actualiza el seguimiento del state cuando cambian las direcciones. `terraform state mv` es el equivalente en la CLI.

</details>

---
### Pregunta 19

¿Los bloques `moved` cambian la infraestructura real en la nube?

- A. Sí, desencadenan una actualización de API en el lugar
- B. No, solo actualizan cómo Terraform asigna las direcciones de configuración al state
- C. Sí, recrean los recursos con nombres nuevos
- D. Solo cuando se combinan con terraform taint

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los bloques `moved` son un mecanismo de refactorización de state/configuración. No llaman a las API de la nube para modificar recursos.

</details>

---
### Pregunta 20

¿Qué variable de entorno habilita el registro de depuración de Terraform?

- A. TF_DEBUG
- B. TF_LOG
- C. TF_TRACE
- D. TERRAFORM_LOG_LEVEL

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Establezca `TF_LOG` en TRACE, DEBUG, INFO, WARN o ERROR. `TF_DEBUG` no es una variable estándar de Terraform.

</details>

---
### Pregunta 21

¿Cuál es el nivel válido más detallado de `TF_LOG`?

- A. DEBUG
- B. VERBOSE
- C. TRACE
- D. DETAIL

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: C**

**Explicación:** Los niveles válidos, del más al menos detallado, son: TRACE, DEBUG, INFO, WARN, ERROR. TRACE ofrece el mayor detalle.

</details>

---
### Pregunta 22

¿Cuáles son valores válidos para la variable de entorno `TF_LOG`? Seleccione todas las que correspondan.

- A. TRACE
- B. DEBUG
- C. VERBOSE
- D. ERROR

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Los niveles válidos de TF_LOG son TRACE, DEBUG, INFO, WARN y ERROR. VERBOSE no es un nivel reconocido.

</details>

---
### Pregunta 23

¿Qué logra establecer `TF_LOG_PATH=./debug.log`?

- A. Redirige las llamadas a la API del provider a un registro de proxy
- B. Escribe la salida de registro de Terraform en el archivo especificado
- C. Almacena el plan de ejecución en un archivo de registro
- D. Habilita únicamente el diagnóstico del locking del state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `TF_LOG_PATH` dirige la salida de registro a un archivo. También debe establecer `TF_LOG` en un nivel para que se genere el registro.

</details>

---
### Pregunta 24

¿Cómo se desactiva el registro de Terraform después de haberlo habilitado?

- A. Solo con unset TF_LOG_PATH
- B. Estableciendo TF_LOG en una cadena vacía o eliminando TF_LOG (unset)
- C. Ejecutando terraform init -no-log
- D. Eliminando el directorio .terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Establecer `TF_LOG=""` o eliminar `TF_LOG` desactiva el registro. TF_LOG_PATH por sí solo no habilita el registro sin TF_LOG.

</details>

---
### Pregunta 25

¿Qué formato produce `terraform graph` de forma predeterminada?

- A. Árbol de dependencias en JSON
- B. Lenguaje de descripción de grafos DOT
- C. Inventario de recursos en YAML
- D. Jerarquía con sangría en texto plano

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform graph` genera un grafo de dependencias en formato DOT, adecuado para renderizarse con Graphviz (`dot`).

</details>

---
### Pregunta 26

¿Qué permite evaluar `terraform console`?

- A. Comandos de shell en el servidor aprovisionado
- B. Expresiones HCL contra el state y la configuración actuales
- C. Credenciales de API del provider de forma interactiva
- D. Scripts de migración del backend remoto

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform console` es un REPL interactivo para probar expresiones, funciones y referencias como `var.name` o `aws_instance.web.id`.

</details>

---
### Pregunta 27

¿Debe ejecutar `terraform apply` antes de usar `terraform console` para hacer referencia a recursos administrados?

- A. Sí, console solo funciona después de apply
- B. No, pero los recursos deben existir en el state (normalmente después de al menos un apply)
- C. No, console simula sin ningún state
- D. Sí, y debe actualizar (refresh) el state cada vez

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Console lee el state y la configuración actuales. Los recursos deben estar en el state para devolver valores reales de atributos.

</details>

---
### Pregunta 28

¿Cuál es el reemplazo moderno de `terraform taint`?

- A. terraform untaint
- B. terraform apply -replace=<address>
- C. terraform destroy -target
- D. terraform state rm

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform taint` está obsoleto (deprecated). Use `terraform apply -replace=<resource_address>` o `-replace` en plan para forzar el reemplazo.

</details>

---
### Pregunta 29

¿Para qué marcaba un recurso `terraform taint`?

- A. Eliminación permanente del state sin cambios en la nube
- B. Destrucción y recreación forzadas en el siguiente apply
- C. Modo de solo lectura durante plan
- D. Exclusión de todos los planes futuros

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Tainting marcaba un recurso para su reemplazo en el siguiente apply. `-replace` logra lo mismo de forma declarativa.

</details>

---
### Pregunta 30

¿Qué hace `terraform untaint` sobre un recurso marcado como tainted?

- A. Elimina el recurso de la nube
- B. Quita la marca de taint para que no se reemplace de forma forzada
- C. Mueve el recurso a una nueva dirección
- D. Desbloquea un lock de state atascado

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform untaint <address>` eliminaba la marca de taint. Tanto taint como untaint están obsoletos en favor de `-replace`.

</details>

---
### Pregunta 31

¿Qué afirmaciones sobre taint y replace son verdaderas? Seleccione todas las que correspondan.

- A. `terraform taint` está obsoleto
- B. `-replace` se puede pasar a `terraform apply`
- C. `terraform untaint` fuerza la recreación inmediata
- D. Tainting marcaba un recurso para su reemplazo en el siguiente apply

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Taint/untaint están obsoletos. `-replace` en apply (o plan) fuerza el reemplazo. Untaint eliminaba la marca de taint; no recreaba los recursos.

</details>

---
### Pregunta 32

¿Cuándo se debe usar `terraform force-unlock`?

- A. Cuando las credenciales del provider han expirado
- B. Cuando un ID de lock de state obsoleto bloquea las operaciones tras un proceso que falló
- C. Para desbloquear archivos de variables cifrados
- D. Para omitir las verificaciones de permisos del workspace

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform force-unlock <LOCK_ID>` libera manualmente un lock de state dejado por una operación interrumpida. Úselo solo cuando esté seguro de que ningún otro proceso mantiene el lock.

</details>

---
### Pregunta 33

¿Qué argumento requiere `terraform force-unlock`?

- A. El nombre del bucket del backend
- B. El ID del lock que aparece en el mensaje de error
- C. El nombre del workspace que se desbloqueará
- D. El alias del provider que se restablecerá

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El comando requiere el ID del lock que aparece en el error de bloqueo (p. ej., el UUID del lock de DynamoDB). Un desbloqueo indebido puede corromper ejecuciones concurrentes.

</details>

---
### Pregunta 34

¿Qué provisioner ejecuta un comando en la máquina donde se ejecuta Terraform?

- A. remote-exec
- B. local-exec
- C. file
- D. connection

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `local-exec` se ejecuta en el host de Terraform. `remote-exec` y `file` se ejecutan en el recurso mediante un bloque `connection`.

</details>

---
### Pregunta 35

Dentro de un bloque provisioner, ¿a qué hace referencia `self`?

- A. A la configuración de provider del módulo raíz
- B. Al recurso al que está asociado el provisioner
- C. Al ID de proceso de la CLI de Terraform
- D. Al objeto del backend de state remoto

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `self` hace referencia a los atributos del recurso padre (p. ej., `self.public_ip`) dentro de los bloques provisioner y connection.

</details>

---
### Pregunta 36

¿Qué provisioner copia archivos a un recurso remoto?

- A. local-exec
- B. remote-exec
- C. file
- D. null_resource

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: C**

**Explicación:** El provisioner `file` carga archivos al host remoto definido en el bloque `connection`.

</details>

---
### Pregunta 37

¿Por qué HashiCorp desaconseja los provisioners?

- A. No están soportados en Terraform 1.0+
- B. No se rastrean por completo en el state y rompen el modelo declarativo
- C. Solo funcionan con el backend local
- D. Requieren HCP Terraform Enterprise

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los provisioners ejecutan scripts imperativos, pueden fallar de forma independiente del ciclo de vida del recurso y son un último recurso. Prefiera cloud-init, user_data o herramientas de administración de configuración.

</details>

---
### Pregunta 38

¿Cuáles son tipos válidos de provisioner de Terraform? Seleccione todas las que correspondan.

- A. local-exec
- B. remote-exec
- C. shell-exec
- D. file

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Los tres tipos de provisioner integrados son `local-exec`, `remote-exec` y `file`. No existe un provisioner `shell-exec`.

</details>

---
### Pregunta 39

¿Qué debe definirse para que los provisioners `remote-exec` y `file` puedan conectarse?

- A. Un bloque `backend`
- B. Un bloque `connection`
- C. Un bloque `import`
- D. Un bloque `moved`

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los provisioners remotos requieren un bloque `connection` (SSH, WinRM, etc.) que especifique el host, el usuario y las credenciales, a menudo usando `self` para el host.

</details>

---
### Pregunta 40

¿Cuándo se ejecutan los provisioners con respecto a la creación del recurso?

- A. Antes de que el recurso se planifique
- B. Después de que el recurso se crea (en la creación, de forma predeterminada)
- C. Solo durante terraform destroy
- D. Durante terraform validate

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los provisioners se ejecutan en eventos del ciclo de vida (de forma predeterminada: después de la creación). También pueden configurarse para la destrucción con `when = destroy`.

</details>

---
### Pregunta 41

¿Cuál es el propósito de un bloque `dynamic` en Terraform?

- A. Generar la configuración del provider en tiempo de ejecución
- B. Generar repetidamente bloques anidados a partir de una variable compleja o una colección
- C. Descargar módulos dinámicamente desde el registry
- D. Cambiar de backend según el nombre del workspace

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los bloques dynamic iteran sobre una colección para producir bloques anidados repetidos (p. ej., varias reglas `ingress` en un grupo de seguridad).

</details>

---
### Pregunta 42

¿Qué meta-argumento es obligatorio dentro de un bloque `dynamic`?

- A. for_each
- B. iterator (opcional, pero `for_each` es obligatorio en el bloque dynamic)
- C. solo count
- D. source

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Un bloque `dynamic` requiere `for_each` y un bloque `content`. Un `iterator` opcional cambia el nombre de la variable del ciclo.

</details>

---
### Pregunta 43

En un bloque dynamic, ¿dónde se define el cuerpo del bloque anidado que se repite?

- A. Dentro de un bloque `repeat`
- B. Dentro del bloque `content`
- C. Directamente dentro de la etiqueta de `dynamic`
- D. Dentro de un archivo .tfvars aparte

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El bloque `content` contiene la plantilla del bloque anidado y usa el iterator (por defecto `dynamic`) para hacer referencia a cada elemento.

</details>

---
### Pregunta 44

¿Qué afirmaciones sobre los bloques dynamic son correctas? Seleccione todas las que correspondan.

- A. Reducen la duplicación en bloques anidados repetidos
- B. Requieren un bloque `content`
- C. Pueden reemplazar la necesidad de cualquier bloque resource
- D. Usan `for_each` para iterar una colección

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Los bloques dynamic generan bloques anidados a partir de colecciones. No reemplazan por completo los bloques resource de nivel superior.

</details>

---
### Pregunta 45

¿Se puede usar `terraform workspace select` para cambiar entre workspaces remotos de HCP Terraform?

- A. Sí, configura el workspace del backend cloud
- B. No, los workspaces de la CLI son un aislamiento de state local; los workspaces de HCP se configuran en el bloque backend
- C. Sí, pero solo después de terraform login
- D. Solo cuando TF_WORKSPACE está definido

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Una trampa común del examen: los comandos `terraform workspace` de la CLI administran archivos de state de workspaces locales, no la selección de workspace de HCP Terraform (que se hace mediante la configuración del backend).

</details>

---
### Pregunta 46

¿Qué indica un asterisco (*) en la salida de `terraform workspace list`?

- A. El workspace cuyo último apply falló
- B. El workspace actualmente seleccionado
- C. El workspace con el archivo de state más grande
- D. Solo el workspace predeterminado

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El asterisco marca el workspace activo en la salida de la lista.

</details>

---
### Pregunta 47

¿Se puede eliminar el workspace `default`?

- A. Sí, con terraform workspace delete default
- B. No, el workspace predeterminado no se puede eliminar
- C. Sí, pero solo cuando existe otro workspace
- D. Solo con la opción -force

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El workspace `default` siempre existe y no se puede eliminar. Puede eliminar otros workspaces después de cambiar a uno distinto.

</details>

---
### Pregunta 48

¿La importación basada en plan con bloques `import` requiere una ejecución aparte de `terraform import` en la CLI?

- A. Sí, siempre
- B. No, la importación se gestiona mediante plan y apply
- C. Solo para módulos
- D. Solo cuando se usa el backend local

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los bloques import modernos se integran en el flujo de trabajo estándar; no se requiere una importación separada por CLI al usar este enfoque.

</details>

---
### Pregunta 49

Si se ejecuta `terraform graph` antes de `terraform init`, ¿qué sucede?

- A. Descarga los providers automáticamente
- B. Puede fallar o producir una salida incompleta porque los providers no están instalados
- C. Grafica solo los módulos
- D. Produce un grafo vacío correctamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Graph depende de la configuración inicializada y de los esquemas de los providers. Ejecute `terraform init` primero.

</details>

---
### Pregunta 50

¿Qué símbolo del plan indica que un recurso se actualizará en el lugar?

- A. ~
- B. +
- C. -
- D. -/+

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** `~` significa actualización en el lugar. `+` crear, `-` destruir, `-/+` reemplazar, `<=` leer un data source.

</details>

---
### Pregunta 51

¿Cuál es un riesgo clave de usar `terraform force-unlock` de forma incorrecta?

- A. Elimina todas las copias de seguridad del state
- B. Las operaciones concurrentes podrían corromper el state si otro proceso aún mantiene el lock
- C. Revoca las credenciales de API de la nube
- D. Elimina todos los recursos de la configuración

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Force-unlock solo debe usarse cuando se tiene la certeza de que el proceso que mantenía el lock falló. De lo contrario, podrían ejecutarse dos apply simultáneamente.

</details>

---
### Pregunta 52

¿Se pueden declarar provisioners directamente dentro de un bloque `module`?

- A. Sí, los bloques module admiten provisioners en línea
- B. No, los provisioners pertenecen a los recursos, no a los bloques module
- C. Solo en módulos raíz
- D. Solo con el provider null

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los provisioners se asocian a bloques `resource` o `data` (normalmente recursos), no a bloques `module`.

</details>

---
### Pregunta 53

¿Qué sucede si un provisioner falla durante apply?

- A. Terraform reintenta automáticamente tres veces
- B. Terraform marca el recurso como tainted (comportamiento heredado) y el apply falla
- C. El recurso se elimina del state
- D. Terraform continúa silenciosamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La falla de un provisioner hace fallar el apply. Históricamente Terraform marcaba el recurso como tainted; con los flujos de trabajo modernos es posible que necesite `-replace` para reintentar.

</details>

---
### Pregunta 54

¿Qué expresión es válida dentro de `terraform console`?

- A. var.instance_type
- B. terraform apply
- C. provider "aws" {}
- D. resource "aws_instance" "web" {}

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Console evalúa expresiones; no bloques de configuración completos ni comandos de la CLI.

</details>

---
### Pregunta 55

Al usar bloques `moved`, ¿debe ejecutar algún comando especial además de plan y apply?

- A. Sí, terraform state mv siempre es obligatorio
- B. No, los bloques moved se procesan durante plan
- C. Sí, terraform refactor
- D. Sí, terraform init -migrate-moved

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform 1.1+ procesa los bloques `moved` automáticamente durante la planificación; no se necesita un comando de refactorización aparte.

</details>

---
### Pregunta 56

¿Se pueden usar bloques `dynamic` en el nivel raíz de un bloque resource (no anidados)?

- A. Sí, para cualquier atributo
- B. No, los bloques dynamic solo generan tipos de bloques anidados
- C. Solo con el provider aws
- D. Solo dentro de módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los bloques dynamic envuelven tipos de bloques anidados (p. ej., `ingress` en grupos de seguridad), no argumentos escalares simples.

</details>

---
### Pregunta 57

¿Qué enfatiza `terraform graph -type=plan` en comparación con el grafo predeterminado?

- A. Solo los nodos de provider
- B. Los recursos con cambios planificados en lugar del grafo de dependencias completo
- C. Los metadatos del registry de módulos
- D. El historial de locks del state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La opción `-type` cambia la salida del grafo; `plan` se centra en los recursos afectados por el contexto del plan actual.

</details>

---
### Pregunta 58

Al usar bloques `import`, ¿puede Terraform generar automáticamente la configuración de los recursos?

- A. Nunca
- B. Sí, al usar `terraform plan -generate-config-out=<file>`
- C. Solo mediante terraform console
- D. Solo para importaciones de módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Plan con `-generate-config-out` escribe en el archivo especificado el HCL sugerido para los recursos importados.

</details>

---
### Pregunta 59

¿Qué hook del ciclo de vida puede ejecutar un provisioner cuando se destruye un recurso?

- A. when = destroy en el bloque provisioner
- B. on_destroy en el bloque resource
- C. terraform destroy -provisioner
- D. prevent_destroy = true

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los provisioners aceptan `when = destroy` para ejecutarse durante la destrucción del recurso (poco común; sigue siendo desaconsejado).

</details>

---
### Pregunta 60

En un bloque dynamic, ¿cuál es el nombre predeterminado del iterator si se omite `iterator`?

- A. item
- B. each
- C. La etiqueta del bloque dynamic (p. ej., ingress para `dynamic "ingress"`)
- D. self

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: C**

**Explicación:** Si se omite, el objeto iterador recibe el nombre de la etiqueta del bloque dynamic y se accede a él como `ingress.value`, etc.

</details>

---
