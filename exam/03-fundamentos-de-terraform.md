# Comprender los fundamentos de Terraform

> **Dominio del examen:** Comprender los fundamentos de Terraform | **Peso:** 10-12%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre la sintaxis de HCL, la estructura del proyecto, los providers, el versionado, el bloque terraform y los conceptos de inicialización.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Qué significa HCL en Terraform?

- A. HashiCorp Configuration Language
- B. Hypertext Cloud Language
- C. Hosted Compute Layer
- D. Hardware Control Logic

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** HCL es HashiCorp Configuration Language, diseñado para la configuración estructurada, incluido Terraform.

</details>

---
### Pregunta 2

¿Qué archivo suele contener las definiciones principales de recursos?

- A. outputs.tf
- B. main.tf
- C. terraform.tfstate
- D. .terraform.lock.hcl

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** main.tf tradicionalmente contiene los recursos principales, aunque Terraform carga todos los archivos .tf del directorio.

</details>

---
### Pregunta 3

¿Dónde se declaran normalmente las variables de entrada?

- A. variables.tf
- B. terraform.tfstate
- C. .terraform/providers/
- D. solo terraform.tfplan

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** variables.tf (o cualquier archivo .tf) declara los bloques variable; los valores pueden provenir de archivos tfvars o de la CLI.

</details>

---
### Pregunta 4

¿Cuál es el propósito de outputs.tf?

- A. Declarar valores de salida (output) que se exponen después del apply
- B. Almacenar los binarios de los plugins de provider
- C. Bloquear automáticamente las versiones de los providers
- D. Reemplazar la necesidad de variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los bloques output exponen valores seleccionados (p. ej., IPs, IDs) después de los cambios en la infraestructura.

</details>

---
### Pregunta 5

terraform.tfvars se usa comúnmente para:

- A. Asignar valores a las variables de entrada
- B. Almacenar el remote state
- C. Descargar plugins de provider
- D. Reemplazar terraform init

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los archivos tfvars proporcionan los valores de las variables; Terraform carga automáticamente terraform.tfvars si está presente.

</details>

---
### Pregunta 6

El archivo providers.tf normalmente contiene:

- A. Bloques de configuración de provider
- B. Solo definiciones de output
- C. El archivo de state en JSON
- D. Binarios compilados de Go

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La configuración del provider (región, alias de credenciales) suele colocarse en providers.tf por organización.

</details>

---
### Pregunta 7

versions.tf comúnmente contiene:

- A. El bloque terraform con required_version y required_providers
- B. Solo claves privadas SSH
- C. El estado en tiempo de ejecución de todos los recursos
- D. Hosts del inventario de Ansible

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las restricciones de versión de la CLI de Terraform y de los providers se declaran en el bloque terraform.

</details>

---
### Pregunta 8

¿Qué se almacena en el directorio .terraform/?

- A. Los plugins de provider descargados y las fuentes de módulos después de init
- B. Solo metadatos del repositorio Git
- C. Secretos de producción que deben ser confirmados en el repositorio
- D. Siempre el archivo de remote state autoritativo

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** .terraform/ es creado por init y contiene los plugins y las cachés de módulos; generalmente no se confirma en el repositorio.

</details>

---
### Pregunta 9

¿Cuál es el propósito de .terraform.lock.hcl?

- A. Fijar las versiones de dependencias de provider para que init sea consistente entre máquinas
- B. Almacenar contraseñas en texto plano para los providers
- C. Reemplazar terraform.tfstate
- D. Formatear automáticamente los archivos HCL

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El archivo de lock registra las versiones de provider seleccionadas y sus checksums; confírmelo en el VCS para mantener la consistencia.

</details>

---
### Pregunta 10

¿Qué archivos normalmente deben confirmarse en el control de versiones? (Seleccione todas las que correspondan.)

- A. Archivos de configuración *.tf
- B. .terraform.lock.hcl
- C. El directorio .terraform/
- D. terraform.tfvars (si no contiene secretos) o usar un tfvars de ejemplo
- E. terraform.tfstate que contiene datos sensibles

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Confirme el código y el archivo de lock. No confirme .terraform/ ni un state sin protección que contenga secretos.

</details>

---
### Pregunta 11

¿Qué comando muestra la versión instalada de la CLI de Terraform?

- A. terraform init
- B. terraform version
- C. terraform providers
- D. terraform show

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** terraform version imprime la versión de la CLI y puede mostrar los requisitos de providers cuando se ejecuta dentro de un directorio.

</details>

---
### Pregunta 12

La configuración de Terraform puede escribirse como:

- A. Solo archivos .tf binarios
- B. Archivos .tf o archivos .tf.json
- C. Solo libros de Excel
- D. Solo YAML de CloudFormation

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform acepta HCL nativo (.tf) o sintaxis JSON (.tf.json) con una estructura equivalente.

</details>

---
### Pregunta 13

En un bloque provider, ¿qué se configura?

- A. Ajustes de un plugin de provider, como la región o las credenciales
- B. Solo valores de output
- C. Solo las claves de cifrado del backend de state
- D. URLs remotas de Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los bloques provider configuran el comportamiento del plugin (región, endpoints, alias, etc.).

</details>

---
### Pregunta 14

required_providers dentro de terraform {} especifica:

- A. Qué plugins de provider y restricciones de versión se necesitan
- B. La lista de recursos a destruir
- C. Las rutas de los playbooks de Ansible
- D. Los nombres de los stacks de CloudFormation

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** required_providers declara las fuentes de los providers y las restricciones de versión para la configuración.

</details>

---
### Pregunta 15

La restricción de versión '= 1.6.0' significa:

- A. Exactamente la versión 1.6.0
- B. 1.6.0 o cualquier versión más reciente
- C. Cualquier versión anterior a 1.6.0
- D. Aproximadamente 1.6.x pero menor que 2.0

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El operador igual fija una versión exacta.

</details>

---
### Pregunta 16

La restricción de versión '>= 1.0' significa:

- A. Solo versiones anteriores a 1.0
- B. La versión 1.0 y cualquier versión más reciente
- C. Exactamente 1.0 únicamente
- D. No se permite ninguna versión

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** >= establece una versión mínima sin límite superior, a menos que se combine con otra restricción.

</details>

---
### Pregunta 17

La restricción de versión '~> 5.0' para un provider significa:

- A. >= 5.0 y < 6.0
- B. Exactamente 5.0 únicamente
- C. Cualquier versión, incluidas la 6.0 y la 7.0
- D. Solo versiones 4.x

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La restricción pesimista ~> 5.0 permite actualizaciones 5.x pero no el salto de versión mayor a 6.0.

</details>

---
### Pregunta 18

¿Qué operador se conoce como operador de restricción pesimista?

- A. ~>
- B. =>
- C. ==
- D. <>

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** ~> se conoce comúnmente como pesimista; permite actualizaciones de parche/menores dentro del límite especificado.

</details>

---
### Pregunta 19

Terraform carga la configuración desde:

- A. Solo main.tf, ignorando los demás archivos
- B. Todos los archivos .tf y .tf.json del directorio de trabajo (salvo que se excluyan)
- C. Solo los archivos llamados terraform.tfvars
- D. Solo el archivo de state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform fusiona todos los archivos de configuración del directorio del módulo en una sola configuración.

</details>

---
### Pregunta 20

¿Qué afirmaciones sobre .terraform/ frente a .terraform.lock.hcl son correctas? (Seleccione todas las que correspondan.)

- A. .terraform/ es generado por terraform init
- B. .terraform.lock.hcl debe confirmarse en el repositorio para mantener la consistencia del equipo
- C. .terraform/ normalmente debe ir en gitignore
- D. .terraform.lock.hcl contiene los binarios de plugins descargados
- E. Ambos pueden eliminarse en cualquier momento sin volver a ejecutar init

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** .terraform/ contiene los plugins/módulos y es regenerado por init. El archivo de lock fija las versiones y debe confirmarse en el repositorio. El archivo de lock no contiene binarios.

</details>

---
### Pregunta 21

Una dirección de origen de provider 'hashicorp/aws' indica:

- A. El namespace y el tipo del provider en el registry
- B. El nombre de un rol de Ansible
- C. Un ID de stack de CloudFormation
- D. Solo una rama de Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los orígenes de provider usan el formato namespace/tipo, p. ej., hashicorp/aws en required_providers.

</details>

---
### Pregunta 22

¿Qué archivo NO debe confirmarse en el repositorio si contiene secretos?

- A. terraform.tfvars con credenciales en texto plano
- B. variables.tf solo con declaraciones
- C. main.tf con bloques resource
- D. .terraform.lock.hcl

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los tfvars con secretos deben excluirse o usar una inyección segura de secretos; los archivos de lock y las declaraciones son seguros de confirmar.

</details>

---
### Pregunta 23

La sintaxis de HCL usa bloques como:

- A. resource "aws_instance" "web" { ... }
- B. CREATE INSTANCE web IN aws;
- C. solo JSON sin comillas
- D. Etiquetas HTML para los recursos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los recursos usan sintaxis de bloque: tipo de bloque, etiquetas entre comillas y argumentos entre llaves.

</details>

---
### Pregunta 24

terraform.tfstate generalmente debería:

- A. No confirmarse en un VCS público porque puede contener datos sensibles
- B. Confirmarse siempre sin cifrar
- C. Reemplazar todos los archivos .tf
- D. Editarse manualmente como flujo de trabajo principal

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El state puede contener secretos y se gestiona mediante backends; evite confirmar un state sin protección.

</details>

---
### Pregunta 25

required_version en terraform {} restringe:

- A. La versión de la CLI de Terraform que puede ejecutar la configuración
- B. Solo las versiones de la API de AWS
- C. Solo las versiones del cliente Git
- D. Solo los mirrors de descarga de providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** required_version establece las versiones aceptables de la CLI de Terraform para el código.

</details>

---
### Pregunta 26

Si se menciona ~/.terraform.d/plugins, se relaciona con:

- A. Ubicaciones de mirror en el sistema de archivos para plugins de provider (configuraciones avanzadas)
- B. La ubicación predeterminada de terraform.tfstate
- C. El archivo de contraseña de Ansible Vault
- D. La caché de plantillas de CloudFormation

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los mirrors de plugins personalizados pueden usar rutas del sistema de archivos; normalmente init descarga en .terraform/.

</details>

---
### Pregunta 27

Los archivos de Terraform con sintaxis JSON usan la extensión:

- A. .tf.json
- B. solo .hcl
- C. .yaml.tf
- D. .cfjson

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los proyectos generados por máquina o que prefieren JSON usan archivos .tf.json.

</details>

---
### Pregunta 28

¿Cuál es HCL válido para un fragmento de bloque terraform?

- A. terraform { required_version = ">= 1.0" }
- B. terraform => required_version: 1.0
- C. TERRAFORM BEGIN VERSION 1.0 END
- D. terraform(required_version=1.0)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los bloques terraform usan llaves y asignaciones con = en la sintaxis de HCL.

</details>

---
### Pregunta 29

¿Qué restricciones de versión permiten Terraform 1.5.9 pero NO 2.0.0? (Seleccione todas las que correspondan.)

- A. ~> 1.5
- B. >= 1.0, < 2.0
- C. = 1.5.9
- D. >= 1.0
- E. ~> 1.0

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** ~> 1.5 permite solo 1.5.x. >=1.0,<2.0 y ~>1.0 limitan por debajo de 2.0. =1.5.9 permite solo ese parche. >=1.0 por sí solo permitiría 2.0.0.

</details>

---
### Pregunta 30

La configuración de alias de provider permite:

- A. Múltiples configuraciones del mismo provider (p. ej., múltiples regiones)
- B. Eliminar el state automáticamente
- C. Omitir terraform init
- D. Usar HCL sin bloques

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los alias permiten definir múltiples bloques provider del mismo tipo para distintas configuraciones.

</details>

---
### Pregunta 31

Después de clonar un repositorio, los compañeros de equipo obtienen versiones de provider consistentes principalmente mediante:

- A. Confirmar .terraform.lock.hcl en el repositorio y ejecutar terraform init
- B. Confirmar el directorio .terraform/ con binarios
- C. Eliminar versions.tf
- D. Evitar required_providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El archivo de lock junto con init garantiza selecciones de provider consistentes según los checksums por plataforma.

</details>

---
### Pregunta 32

variables.tf contiene:

- A. Bloques variable con tipos, descripciones y valores predeterminados
- B. Solo plugins de provider
- C. Datos del remote state del backend
- D. Archivos de plan generados con terraform plan -out

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las variables de entrada se declaran con bloques variable, idealmente sin asignarles secretos de producción.

</details>

---
### Pregunta 33

outputs.tf expone valores como:

- A. load_balancer_dns_name después del apply
- B. Solo las rutas de los zip de plugins de provider
- C. SHAs de commits de Git automáticamente
- D. Solo grupos del inventario de Ansible

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los outputs presentan atributos útiles para usuarios u otros sistemas después del apply.

</details>

---
### Pregunta 34

¿Qué directorio aparece después de terraform init?

- A. .terraform/
- B. .git/hooks/
- C. node_modules/
- D. ansible/roles/ automáticamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** init crea .terraform/ con las instalaciones de providers y módulos.

</details>

---
### Pregunta 35

Una trampa común del examen: todos los archivos .tf deben llamarse main.tf. Afirmación correcta:

- A. Terraform carga todos los archivos .tf; los nombres son convenciones de organización
- B. Solo se lee main.tf
- C. las variables deben estar solo en main.tf
- D. los outputs deben estar solo en providers.tf

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los nombres de archivo son convenciones para facilitar la lectura; Terraform fusiona todos los archivos .tf.

</details>

---
### Pregunta 36

Las restricciones de versión en required_providers ayudan a:

- A. Evitar que actualizaciones inesperadas de versión mayor del provider rompan la configuración
- B. Eliminar la necesidad de terraform plan
- C. Eliminar los requisitos de autenticación
- D. Confirmar automáticamente el state en Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las restricciones de versión gestionan las versiones de provider compatibles.

</details>

---
### Pregunta 37

terraform version en un directorio configurado también puede mostrar:

- A. Los requisitos de providers del bloque terraform
- B. El contenido completo del archivo de state
- C. Todas las contraseñas de la cuenta de AWS
- D. Los resultados de un playbook de Ansible

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** terraform version puede informar las versiones requeridas de Terraform y de los providers según la configuración.

</details>

---
### Pregunta 38

Las cadenas de texto en HCL pueden definirse con:

- A. Comillas dobles para cadenas estándar
- B. Únicamente comillas simples, de forma exclusiva
- C. Solo comillas invertidas, que están prohibidas
- D. Solo entidades HTML

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** HCL usa principalmente cadenas con comillas dobles; también se admiten heredocs.

</details>

---
### Pregunta 39

¿Cuáles pertenecen al bloque terraform {}? (Seleccione todas las que correspondan.)

- A. required_version
- B. required_providers
- C. configuración del backend
- D. bloques resource "aws_instance"
- E. la configuración de región de provider "aws"

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** terraform {} contiene la versión de la CLI, los providers y la configuración del backend. Los recursos van en bloques resource; los ajustes del provider van en bloques provider.

</details>

---
### Pregunta 40

Los argumentos de configuración de un provider suelen ser:

- A. Específicos de cada provider (p. ej., region para AWS)
- B. Idénticos para todos los providers
- C. Siempre opcionales y sin efecto
- D. Solo se establecen en terraform.tfstate

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El esquema de cada provider define sus propios atributos de configuración.

</details>

---
### Pregunta 41

Los archivos .tf.json son útiles cuando:

- A. La configuración es generada programáticamente por otra herramienta
- B. Se desea únicamente HCL escrito a mano
- C. Se debe evitar terraform init
- D. Se necesita almacenar secretos binarios en Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La sintaxis JSON es adecuada para configuraciones generadas por máquina; HCL es más amigable para las personas.

</details>

---
### Pregunta 42

Se desaconseja confirmar .terraform/ en el repositorio porque:

- A. Es grande, específico de la plataforma y reproducible mediante init
- B. No contiene datos útiles
- C. Impide las descargas de providers para siempre
- D. HashiCorp exige que sea público

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los plugins pueden volver a descargarse; los binarios inflan los repositorios y pueden diferir según el sistema operativo/arquitectura.

</details>

---
### Pregunta 43

La restricción pesimista '~> 1.0' para la CLI de Terraform permite:

- A. 1.9.x pero no 2.0.0
- B. 2.5.0
- C. 0.14.0
- D. Solo exactamente 1.0.0

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** ~> 1.0 significa >= 1.0 y < 2.0, lo que permite cualquier release 1.x.

</details>

---
### Pregunta 44

¿Qué archivo separa las declaraciones de variables de las asignaciones?

- A. variables.tf declara; terraform.tfvars asigna valores
- B. outputs.tf declara y asigna variables
- C. providers.tf almacena solo el state
- D. versions.tf almacena solo secretos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las declaraciones y los valores son conceptos separados; las asignaciones también pueden provenir de la CLI o de variables de entorno.

</details>

---
### Pregunta 45

terraform init usa required_providers para:

- A. Seleccionar y descargar los plugins de provider adecuados
- B. Aplicar los cambios de inmediato sin plan
- C. Formatear todos los archivos JSON
- D. Eliminar siempre .terraform.lock.hcl

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Init lee los requisitos de los providers e instala los plugins que coinciden según las restricciones y el archivo de lock.

</details>

---
### Pregunta 46

Un bloque provider sin alias usa:

- A. La configuración de provider predeterminada para ese tipo
- B. Ningún provider jamás
- C. Solo módulos
- D. Solo data sources

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los bloques provider sin alias configuran la instancia predeterminada que usan los recursos, a menos que se sobrescriba.

</details>

---
### Pregunta 47

¿Cuál NO es un archivo estándar de un proyecto Terraform?

- A. main.tf
- B. terraform.tfstate
- C. variables.tf
- D. outputs.tf

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** tfstate se genera en tiempo de ejecución; los demás son archivos de configuración escritos por el autor (tfstate no es configuración fuente).

</details>

---
### Pregunta 48

¿Qué afirmaciones sobre los bloques provider son VERDADERAS? (Seleccione todas las que correspondan.)

- A. Configuran el comportamiento del plugin de provider
- B. Pueden usar alias para múltiples configuraciones
- C. Reemplazan por completo a required_providers
- D. Son independientes de los bloques resource
- E. Siempre deben estar solo en main.tf

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Los bloques provider configuran los plugins y pueden usar alias. required_providers sigue declarando los orígenes y las versiones. La ubicación en archivos es una convención.

</details>

---
### Pregunta 49

La restricción de versión '>= 1.2, < 2.0' significa:

- A. 1.2 <= versión < 2.0
- B. Solo exactamente 1.2
- C. Cualquier versión, incluida la 3.0
- D. Ninguna versión la cumple

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las restricciones compuestas combinan límites inferior y superior.

</details>

---
### Pregunta 50

Los comentarios en HCL pueden escribirse como:

- A. # comentario de línea o // comentario de línea
- B. solo <!-- comentarios HTML -->
- C. solo comentarios de bloque de C /* prohibido */
- D. no se permiten comentarios

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** HCL admite comentarios de línea con # y //; también se admiten comentarios de bloque /* */.

</details>

---
### Pregunta 51

terraform.tfvars.json es:

- A. Un archivo de valores de variables en formato JSON que Terraform puede cargar
- B. El archivo de lock de providers
- C. Un reemplazo de terraform init
- D. Solo un respaldo del state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los valores de las variables pueden suministrarse mediante tfvars en HCL o tfvars.json.

</details>

---
### Pregunta 52

Si se omite required_providers pero existen bloques provider, Terraform moderno:

- A. Sigue esperando que los requisitos de providers se declaren en el bloque terraform (mejor práctica desde Terraform 0.13+)
- B. No puede ejecutarse en absoluto, jamás
- C. Usa Ansible automáticamente
- D. Ignora los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Terraform 0.13+ requiere direcciones de origen de provider explícitas en required_providers por claridad.

</details>

---
### Pregunta 53

El archivo de lock se actualiza cuando:

- A. Se ejecuta terraform init con cambios en las versiones de provider o con -upgrade
- B. Se ejecuta solo terraform fmt
- C. Se ejecuta solo terraform version
- D. Se edita README.md

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Init selecciona las versiones de provider y registra los checksums en .terraform.lock.hcl.

</details>

---
### Pregunta 54

¿Qué práctica favorece el uso consistente de la CLI de Terraform en todo el equipo?

- A. Documentar required_version y hacerlo cumplir en CI
- B. Que cada desarrollador use versiones aleatorias de la CLI sin verificaciones
- C. Eliminar versions.tf
- D. Confirmar solo los binarios de .terraform/

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** required_version junto con las verificaciones en CI alinea las versiones de la CLI entre los compañeros de equipo.

</details>

---
### Pregunta 55

Los outputs se definen con:

- A. output "name" { value = ... }
- B. solo variable "name" { value = ... }
- C. provider "name" { output = ... }
- D. resource "output" "name" {}

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los bloques output usan la palabra clave output con una etiqueta de nombre y el argumento value.

</details>

---
### Pregunta 56

Una trampa: terraform.tfvars es obligatorio en todos los proyectos. La realidad:

- A. Las variables pueden usar valores predeterminados, -var en la CLI u otros archivos tfvars; terraform.tfvars es opcional
- B. Terraform no puede ejecutarse sin tfvars
- C. tfvars reemplaza a providers.tf
- D. tfvars almacena los checksums del lock

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** terraform.tfvars se carga automáticamente si está presente, pero no es obligatorio.

</details>

---
### Pregunta 57

¿Qué afirmaciones sobre los fundamentos de Terraform son verdaderas? (Seleccione todas las que correspondan.)

- A. HCL es el lenguaje de configuración principal
- B. .terraform.lock.hcl debe confirmarse en el repositorio
- C. terraform.tfstate debe manejarse con cuidado y no confirmarse a la ligera
- D. Los bloques provider siempre pertenecen dentro de bloques resource
- E. ~> es una restricción de versión pesimista

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** HCL, confirmar el archivo de lock, el manejo cuidadoso del state y el ~> pesimista son conceptos básicos fundamentales. Los bloques provider son construcciones hermanas, no anidadas dentro de los recursos.

</details>

---
### Pregunta 58

¿Qué comando debe ejecutarse antes de plan/apply en un nuevo directorio de trabajo?

- A. terraform init
- B. terraform destroy
- C. solo terraform login
- D. solo terraform graph

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** init descarga los providers/módulos y prepara el backend antes de los demás comandos del flujo de trabajo.

</details>

---
### Pregunta 59

¿Qué tipo de bloque se usa para declarar variables?

- A. variable "name" { ... }
- B. solo output "name" { ... }
- C. solo provider "name" { ... }
- D. terraform "name" { ... }

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las variables de entrada se declaran con bloques variable; los outputs y los providers usan sus propios tipos de bloque.

</details>

---
### Pregunta 60

El argumento source en required_providers identifica:

- A. La dirección del provider en el registry (namespace/nombre)
- B. La rama de Git para terraform.tfstate
- C. El correo raíz de la cuenta de AWS
- D. Solo la ruta local a terraform.tfvars

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** source especifica la ubicación del provider en el registry, p. ej., hashicorp/aws.

</details>

---
