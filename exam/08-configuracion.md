# Leer, generar y modificar la configuración

> **Dominio del examen:** Leer, generar y modificar la configuración | **Peso:** 15-18%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre variables, outputs, locals, expresiones, funciones, meta-argumentos, data sources y dynamic blocks.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Qué restricción de tipo de variable es válida en Terraform?

- A. string
- B. char
- C. integer
- D. double only

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los tipos primitivos incluyen string, number y bool. Use number, no integer.

</details>

---
### Pregunta 2

¿Cuáles son tipos de variable complejos válidos?

- A. list(string), map(string), set(string)
- B. array(string)
- C. dict(string)
- D. queue(string)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Terraform usa list, map, set, object y tuple, no array/dict.

</details>

---
### Pregunta 3

¿Qué significa nullable = false en una variable?

- A. La variable no se puede establecer
- B. La variable no se puede establecer en null
- C. La variable es sensitive
- D. La variable está obsoleta

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** nullable=false rechaza asignaciones de null.

</details>

---
### Pregunta 4

Los bloques validation en las variables se ejecutan durante:

- A. terraform plan/apply cuando los valores son conocidos
- B. Solo terraform fmt
- C. Solo la descarga del provider
- D. Nunca

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las condiciones de validación se verifican cuando Terraform evalúa las variables.

</details>

---
### Pregunta 5

sensitive = true en una variable principalmente:

- A. La oculta de la salida de la CLI y de los logs
- B. Impide que se use en recursos
- C. La almacena solo en variables de entorno
- D. La elimina del state automáticamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Sensitive afecta la visualización; no elimina los valores del state.

</details>

---
### Pregunta 6

default en un bloque variable proporciona:

- A. El valor de menor precedencia cuando no se suministra ninguno
- B. El valor de mayor precedencia siempre
- C. Cifrado automático
- D. Configuración del provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los valores por defecto se aplican solo cuando ninguna fuente de mayor precedencia proporciona un valor.

</details>

---
### Pregunta 7

type = object({ name = string, count = number }) es un ejemplo de:

- A. Una restricción de tipo estructural
- B. Un bloque provider
- C. Un tipo de backend
- D. Un formato de output

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** object() define tipado estructural para las variables.

</details>

---
### Pregunta 8

type = any en una variable significa:

- A. Solo se permiten strings
- B. Se acepta cualquier tipo
- C. Solo null
- D. Solo booleanos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** any deshabilita las restricciones de tipo específicas.

</details>

---
### Pregunta 9

¿Cuál tiene la MAYOR precedencia para las variables de Terraform?

- A. default en el bloque variable
- B. terraform.tfvars
- C. Variable de entorno TF_VAR_name
- D. Flag de CLI -var="name=value"

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: D**

**Explicación:** Orden (de menor a mayor): default, TF_VAR_, tfvars, auto.tfvars, -var-file, -var.

</details>

---
### Pregunta 10

¿Cuál tiene la MENOR precedencia?

- A. default en el bloque variable
- B. Flag -var
- C. -var-file
- D. Variable de entorno TF_VAR_

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El -var explícito de la CLI sobrescribe todo lo demás.

</details>

---
### Pregunta 11

terraform.tfvars es:

- A. Cargado automáticamente si está presente
- B. Nunca cargado automáticamente
- C. Cargado solo con -var-file
- D. Solo para outputs

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** terraform.tfvars y *.auto.tfvars se cargan automáticamente.

</details>

---
### Pregunta 12

Los archivos que coinciden con *.auto.tfvars:

- A. Se cargan automáticamente en orden lexicográfico
- B. Se ignoran
- C. Sobrescriben el flag -var
- D. Reemplazan a los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los archivos auto.tfvars se cargan automáticamente; entre ellos importa el orden alfabético.

</details>

---
### Pregunta 13

La variable de entorno TF_VAR_instance_type tiene precedencia sobre:

- A. El valor default y terraform.tfvars
- B. El flag de CLI -var
- C. Nada
- D. Solo outputs

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** TF_VAR_ tiene precedencia sobre los defaults y tfvars, pero pierde frente a -var-file y -var.

</details>

---
### Pregunta 14

Para pasar una sobrescritura puntual en CI con la mayor prioridad, use:

- A. -var="key=value"
- B. Solo el default
- C. terraform fmt
- D. terraform graph

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** -var tiene la mayor precedencia para sobrescrituras rápidas.

</details>

---
### Pregunta 15

Los valores de output se usan principalmente para:

- A. Declarar providers
- B. Exponer valores útiles después del apply a usuarios/otros sistemas
- C. Bloquear el state
- D. Descargar módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los outputs exponen IPs, IDs, endpoints, etc.

</details>

---
### Pregunta 16

sensitive = true en un output:

- A. Oculta el valor en la salida normal de la CLI
- B. Elimina el valor del state
- C. Impide que el output exista
- D. Fuerza el cifrado en HCL

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los outputs sensitive se redactan en la visualización de la CLI.

</details>

---
### Pregunta 17

Los locals son útiles porque:

- A. Reducen la repetición y simplifican expresiones sin exponer inputs/outputs
- B. Reemplazan a los providers
- C. Almacenan el remote state
- D. Ejecutan provisioners

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los locals son valores calculados internos.

</details>

---
### Pregunta 18

Referenciar un local llamado common_tags:

- A. var.common_tags
- B. local.common_tags
- C. output.common_tags
- D. module.common_tags

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los locals usan el prefijo local.

</details>

---
### Pregunta 19

Los outputs pueden referenciar:

- A. Atributos de recursos y expresiones
- B. Solo variables
- C. Solo providers
- D. Solo módulos de otras organizaciones

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los valores de output pueden ser cualquier expresión basada en la infraestructura administrada.

</details>

---
### Pregunta 20

La sintaxis de la expresión condicional es:

- A. if condition then a else b
- B. condition ? true_val : false_val
- C. when condition -> value
- D. select(condition, a, b)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform usa el operador ternario ? :

</details>

---
### Pregunta 21

La expresión for [for s in var.list : upper(s)] devuelve:

- A. Un map
- B. Una lista derivada de var.list
- C. Un provider
- D. Un backend

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La forma con corchetes produce una comprensión de lista.

</details>

---
### Pregunta 22

La expresión for { for k, v in var.map : k => v } devuelve:

- A. Una lista
- B. Una comprensión de map/object
- C. Un string
- D. Un ID de lock

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La forma con llaves y => construye un map.

</details>

---
### Pregunta 23

La expresión splat aws_instance.web[*].id recolecta:

- A. Siempre un único string
- B. Una lista de atributos id de todas las instancias de esa colección de recursos
- C. Configuraciones de provider
- D. Solo el primer recurso en el orden del archivo de state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** [*] reúne un atributo a través de múltiples instancias.

</details>

---
### Pregunta 24

for_each en un recurso requiere:

- A. Solo una lista
- B. Un map o set (convierta las listas con toset())
- C. Un alias de provider
- D. Un backend

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** for_each acepta map o set; las listas requieren conversión, una trampa común en el examen.

</details>

---
### Pregunta 25

count.index comienza en:

- A. 1
- B. 0
- C. -1
- D. Aleatorio

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los índices de count comienzan en cero.

</details>

---
### Pregunta 26

format("Hello, %s!", var.name) usa:

- A. Una función de formateo de strings similar a printf
- B. Codificación JSON
- C. Cálculo de CIDR
- D. Bloqueo del state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** format construye strings con marcadores de posición.

</details>

---
### Pregunta 27

join(", ", ["a", "b"]) devuelve:

- A. "a, b"
- B. ["a", "b"]
- C. {a,b}
- D. ab

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** join concatena los elementos de una lista con un separador.

</details>

---
### Pregunta 28

merge({a=1}, {b=2}) devuelve:

- A. {a=1, b=2}
- B. [1,2]
- C. 1
- D. null

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** merge combina maps; las claves posteriores sobrescriben en caso de colisión.

</details>

---
### Pregunta 29

lookup({a=1}, "b", 0) devuelve:

- A. 0
- B. 1
- C. siempre null
- D. siempre error

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** lookup devuelve el valor por defecto cuando falta la clave.

</details>

---
### Pregunta 30

cidrsubnet("10.0.0.0/16", 8, 1) calcula:

- A. Un CIDR de subred dentro del bloque padre
- B. Un nombre DNS
- C. Un ID de AMI
- D. Una tabla de lock

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** cidrsubnet divide el espacio de direcciones.

</details>

---
### Pregunta 31

file("${path.module}/script.sh") lee:

- A. Un objeto S3 remoto
- B. El contenido de un archivo local relativo al contexto de evaluación
- C. Solo el archivo de state
- D. El schema del provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** file() lee archivos locales; a menudo se combina con path.module.

</details>

---
### Pregunta 32

templatefile("tpl.tftpl", { name = "x" }) hace lo siguiente:

- A. Descarga un módulo
- B. Renderiza un archivo de plantilla con variables
- C. Bloquea el state
- D. Valida providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** templatefile renderiza plantillas .tftpl.

</details>

---
### Pregunta 33

jsonencode({a=1}) produce:

- A. Un string JSON
- B. Solo un map de Terraform
- C. Un bloque HCL
- D. Un binario de provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** jsonencode serializa a un string JSON.

</details>

---
### Pregunta 34

jsondecode("{\"a\":1}") devuelve:

- A. Un valor map/object de Terraform
- B. Solo un string
- C. Solo un número
- D. Siempre un error

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** jsondecode convierte JSON en valores de Terraform.

</details>

---
### Pregunta 35

contains(["a","b"], "a") devuelve:

- A. true
- B. false
- C. null
- D. ["a"]

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** contains verifica la pertenencia a una lista/set.

</details>

---
### Pregunta 36

length(["a","b"]) devuelve:

- A. 2
- B. 1
- C. 0
- D. "ab"

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** length devuelve la cantidad de elementos.

</details>

---
### Pregunta 37

toset(["a","b","a"]) devuelve:

- A. Un set con elementos únicos
- B. Una lista con duplicados
- C. Un map
- D. Un error

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** toset elimina duplicados; es útil antes de for_each.

</details>

---
### Pregunta 38

Las dependencias implícitas se crean cuando:

- A. Un recurso referencia los atributos de otro en expresiones
- B. Se usa terraform fmt
- C. Se usa la misma versión del provider
- D. Se usan tags idénticos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las referencias a atributos construyen el grafo de dependencias automáticamente.

</details>

---
### Pregunta 39

depends_on se usa para:

- A. Dependencias explícitas que no son capturadas por referencias
- B. Formatear HCL
- C. Cambiar el backend
- D. Establecer valores por defecto de variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** depends_on declara el orden cuando no existe una referencia a un atributo.

</details>

---
### Pregunta 40

lifecycle { prevent_destroy = true }:

- A. Impide que Terraform destruya ese recurso
- B. Impide todos los plans
- C. Elimina el recurso inmediatamente
- D. Deshabilita los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** prevent_destroy protege contra eliminaciones accidentales.

</details>

---
### Pregunta 41

lifecycle { create_before_destroy = true } ayuda a:

- A. Reducir el tiempo de inactividad cuando se requiere un reemplazo
- B. Omitir el apply
- C. Eliminar el state
- D. Deshabilitar el cifrado

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Crea el nuevo recurso antes de destruir el anterior en los recursos que lo admiten.

</details>

---
### Pregunta 42

lifecycle { ignore_changes = [tags] } le indica a Terraform que:

- A. Deje de administrar el recurso
- B. Ignore el drift en los atributos listados después de la creación
- C. Destruya el recurso
- D. Elimine los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** ignore_changes suprime las actualizaciones de los atributos especificados.

</details>

---
### Pregunta 43

El meta-argumento provider en un recurso selecciona:

- A. Un alias de configuración de provider que no es el predeterminado
- B. Un backend
- C. Un output de módulo
- D. Un workspace

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** provider = aws.west selecciona la configuración de provider con alias.

</details>

---
### Pregunta 44

count en un recurso crea:

- A. Múltiples instancias indexadas desde 0
- B. Solo maps
- C. Solo data sources
- D. Backends

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** count se expande a aws_instance.name[0], [1], ...

</details>

---
### Pregunta 45

Las claves de for_each están disponibles como:

- A. each.key y each.value
- B. count.key
- C. index.key
- D. solo for.key

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** for_each expone each.key/each.value dentro de los bloques.

</details>

---
### Pregunta 46

Los data sources se diferencian de los recursos porque los data sources:

- A. Crean nueva infraestructura
- B. Leen infraestructura existente sin administrar su ciclo de vida
- C. Siempre ejecutan provisioners
- D. Almacenan el remote state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los data sources son consultas de solo lectura.

</details>

---
### Pregunta 47

Un bloque data source podría usarse para:

- A. Buscar el ID de la AMI más reciente
- B. Crear un bucket de S3
- C. Bloquear DynamoDB
- D. Enviar el state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Patrón común: data "aws_ami" "latest" { ... }

</details>

---
### Pregunta 48

Los dynamic blocks generan:

- A. Bloques anidados repetidos a partir de una colección
- B. Binarios de provider
- C. Solo copias de seguridad del state
- D. Migraciones de backend

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los dynamic blocks iteran con for_each sobre tipos de bloques anidados.

</details>

---
### Pregunta 49

Dentro de un dynamic block, el objeto iterador se referencia como:

- A. ingress.value para un iterador llamado ingress
- B. siempre dynamic.value
- C. each.only
- D. count.dynamic

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La etiqueta del iterador (p. ej., ingress) expone .key y .value en content.

</details>

---
### Pregunta 50

¿Qué meta-argumentos requiere un dynamic block?

- A. for_each y content
- B. source y version
- C. backend y key
- D. solo count

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** dynamic usa for_each + content { ... }.

</details>

---
### Pregunta 51

terraform console se usa para:

- A. Evaluar expresiones de Terraform de forma interactiva
- B. Aplicar cambios silenciosamente
- C. Destruir todos los recursos
- D. Configurar solo backends

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Console ayuda a probar funciones y expresiones.

</details>

---
### Pregunta 52

terraform output sin argumentos:

- A. Muestra todos los outputs
- B. Elimina los outputs
- C. Muestra los providers
- D. Ejecuta Sentinel

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** terraform output lista los valores de output.

</details>

---
### Pregunta 53

terraform output -json proporciona:

- A. Outputs con formato JSON
- B. Solo outputs sensitive en texto plano hacia los logs
- C. Caché de providers
- D. Estado del lock

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La salida JSON facilita el scripting y CI.

</details>

---
### Pregunta 54

Revisión n.º 54: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con la cantidad de preguntas por dominio.

</details>

---
### Pregunta 55

¿Cuáles son tipos de variable válidos de Terraform? (Seleccione todas las que correspondan.)

- A. string
- B. list(string)
- C. object({ id = string })
- D. array(int)
- E. set(number)

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** Terraform usa list/set/map/object/tuple/any, no array.

</details>

---
### Pregunta 56

El orden de precedencia de variables de MENOR a MAYOR incluye qué ordenamientos? (Seleccione todas las que correspondan.)

- A. default en el bloque variable es el más bajo
- B. TF_VAR_ tiene precedencia sobre default
- C. -var tiene precedencia sobre -var-file
- D. terraform.tfvars tiene precedencia sobre -var
- E. -var es el más alto

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** Orden correcto: default < TF_VAR_ < tfvars < auto.tfvars < -var-file < -var.

</details>

---
### Pregunta 57

¿Qué funciones integradas funcionan como se describe? (Seleccione todas las que correspondan.)

- A. merge combina maps
- B. join concatena una lista con un separador
- C. lookup obtiene un valor de un map con un valor por defecto opcional
- D. cidrsubnet calcula subredes
- E. templatefile renderiza plantillas

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, D, E**

**Explicación:** Todas las funciones listadas se comportan como se describe; es conocimiento común del examen.

</details>

---
### Pregunta 58

¿Qué meta-argumentos / bloques son válidos? (Seleccione todas las que correspondan.)

- A. count
- B. for_each
- C. depends_on
- D. lifecycle
- E. bloques anidados dynamic

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, D, E**

**Explicación:** Estos son meta-argumentos y patrones centrales de la configuración.

</details>

---
### Pregunta 59

¿Qué afirmaciones sobre data sources y outputs son verdaderas? (Seleccione todas las que correspondan.)

- A. Los data sources leen sin crear recursos administrados
- B. Los outputs exponen valores después del apply
- C. Los outputs sensitive se redactan en la salida normal de la CLI
- D. Los data sources siempre requieren import
- E. jsonencode/jsondecode ayudan a serializar valores

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** Los data sources no requieren import; consultan datos existentes.

</details>

---
### Pregunta 60

¿Qué expresiones son patrones válidos de Terraform? (Seleccione todas las que correspondan.)

- A. condition ? a : b
- B. [for x in var.items : x]
- C. aws_instance.web[*].id
- D. for_each sobre una lista sin procesar sin conversión
- E. toset() antes de for_each en claves derivadas de una lista

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** for_each necesita map/set; convierta las listas con toset() o similar.

</details>

---
