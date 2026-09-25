# Comprender el propósito de Terraform (frente a otras herramientas de IaC)

> **Dominio del examen:** Comprender el propósito de Terraform (frente a otras herramientas de IaC) | **Peso:** 7-9%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre el rol de Terraform frente a Ansible, CloudFormation y Pulumi; el modelo de providers; las ventajas del multi-cloud; y la propuesta de valor central.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Cuál es el enfoque principal de Terraform en comparación con Ansible?

- A. Gestión de configuración y ejecución de comandos ad hoc sobre hosts existentes
- B. Aprovisionamiento y gestión del ciclo de vida de la infraestructura mediante configuración declarativa
- C. Despliegue de aplicaciones de escritorio de Windows únicamente
- D. Agregación de logs en tiempo real únicamente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform se enfoca en aprovisionar infraestructura de nube y de red; Ansible se enfoca más en la gestión de configuración.

</details>

---
### Pregunta 2

Ansible se describe generalmente como:

- A. Una herramienta de aprovisionamiento en la nube exclusivamente declarativa, sin tareas procedimentales
- B. Una herramienta de gestión de configuración basada en agentes que usa playbooks procedimentales
- C. Un motor de plantillas JSON exclusivo de AWS
- D. Un reemplazo del control de versiones Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Ansible suele usar playbooks procedimentales y con frecuencia es agentless (SSH/WinRM), enfocado en configurar sistemas.

</details>

---
### Pregunta 3

AWS CloudFormation está limitado a:

- A. Cualquier proveedor de nube mediante plugins
- B. Recursos de AWS usando plantillas JSON o YAML
- C. Únicamente VMware on-premises
- D. Exclusivamente clústeres de Kubernetes

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** CloudFormation es nativo de AWS y usa plantillas JSON/YAML para stacks de AWS.

</details>

---
### Pregunta 4

Pulumi se diferencia de Terraform principalmente porque:

- A. Usa únicamente asistentes gráficos sin código
- B. Permite definir la infraestructura usando lenguajes de programación de propósito general
- C. No puede gestionar recursos en la nube
- D. Requiere la consola de AWS para cada cambio

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Pulumi usa lenguajes como TypeScript, Python y Go en lugar de HCL como experiencia principal de creación.

</details>

---
### Pregunta 5

Una ventaja clave del modelo de providers de Terraform es:

- A. Lo ata a un único proveedor de forma permanente
- B. Permite infraestructura multi-cloud y heterogénea desde un solo flujo de trabajo
- C. Elimina la necesidad de autenticación
- D. Solo soporta nubes construidas por HashiCorp

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los providers permiten a Terraform gestionar muchas plataformas con un flujo de trabajo consistente.

</details>

---
### Pregunta 6

Las configuraciones de Terraform se escriben principalmente en:

- A. Únicamente YAML de CloudFormation
- B. HashiCorp Configuration Language (HCL)
- C. Únicamente INI de inventario de Ansible
- D. Exclusivamente Pulumi Assembly

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El lenguaje nativo de Terraform es HCL, aunque también se admite la sintaxis JSON.

</details>

---
### Pregunta 7

¿Qué herramienta se asocia MÁS con la automatización procedimental, paso a paso, en servidores?

- A. Terraform
- B. Ansible
- C. CloudFormation
- D. Exclusivamente Terraform Cloud

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los playbooks de Ansible describen tareas y pasos; Terraform declara el estado (state) deseado de la infraestructura.

</details>

---
### Pregunta 8

Las plantillas de CloudFormation normalmente se escriben en:

- A. Únicamente HCL
- B. JSON o YAML
- C. Únicamente código fuente en Go
- D. Exclusivamente scripts de shell

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** CloudFormation usa formatos de plantilla JSON o YAML nativos de AWS.

</details>

---
### Pregunta 9

Se dice que Terraform es agnóstico respecto al proveedor (provider-agnostic) porque:

- A. Ignora todas las APIs de los providers
- B. Usa plugins para interactuar con las APIs de muchos proveedores mediante un flujo de trabajo común
- C. No puede configurar AWS
- D. Solo funciona sin conexión

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los plugins de provider abstraen las APIs de los proveedores manteniendo un flujo de trabajo consistente de Terraform.

</details>

---
### Pregunta 10

¿Qué afirmaciones que comparan Terraform con otras herramientas de IaC son VERDADERAS? (Seleccione todas las que correspondan.)

- A. Terraform es declarativo; Ansible suele ser procedimental
- B. CloudFormation es exclusivo de AWS
- C. Pulumi soporta lenguajes de programación reales para la infraestructura
- D. Ansible es principalmente una herramienta de aprovisionamiento de infraestructura como Terraform
- E. Terraform usa HCL como su lenguaje de configuración principal

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** Terraform es aprovisionamiento declarativo con HCL. Ansible se orienta más a la gestión de configuración y es procedimental. CloudFormation es exclusivo de AWS. Pulumi usa lenguajes de propósito general.

</details>

---
### Pregunta 11

Una estrategia multi-cloud con Terraform significa:

- A. Usar una sola herramienta con múltiples providers para gestionar recursos en distintas nubes
- B. Ejecutar únicamente consolas separadas y sin coordinación
- C. Que Terraform elige automáticamente la nube más barata sin configuración
- D. Que los providers no son necesarios para múltiples nubes

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Terraform puede gestionar AWS, Azure, GCP y otros mediante providers en configuraciones unificadas.

</details>

---
### Pregunta 12

¿Por qué un equipo podría elegir Terraform en lugar de CloudFormation?

- A. Necesitan plantillas YAML exclusivas de AWS
- B. Quieren una herramienta agnóstica respecto al proveedor, utilizable en múltiples nubes y servicios
- C. Requieren un modelo de playbooks procedimentales
- D. Quieren evitar cualquier sintaxis declarativa

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El soporte multi-provider de Terraform es adecuado para entornos heterogéneos o multi-cloud.

</details>

---
### Pregunta 13

Ansible suele ser agentless, lo que significa que:

- A. No puede conectarse a hosts remotos
- B. Normalmente usa SSH o WinRM sin instalar un agente permanente en los destinos
- C. Requiere un daemon en cada servidor de forma predeterminada
- D. Solo se ejecuta en el servidor de Terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Ansible normalmente se conecta por SSH/WinRM; esto difiere de muchos sistemas de configuración basados en agentes.

</details>

---
### Pregunta 14

Terraform frente a Pulumi: ambos pueden aprovisionar infraestructura, pero Terraform tradicionalmente usa:

- A. HCL y un flujo de trabajo dedicado de plan/apply
- B. Únicamente cadenas de CloudFormation incrustadas
- C. Hojas de cálculo de Excel para los grafos de recursos
- D. Operaciones manuales en la consola

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Terraform se centra en HCL y en su flujo de trabajo principal; Pulumi se centra en lenguajes de propósito general.

</details>

---
### Pregunta 15

El enfoque en el aprovisionamiento de infraestructura significa que Terraform destaca en:

- A. Crear VPCs, subredes, balanceadores de carga y bases de datos como recursos declarados
- B. Instalar paquetes de aplicaciones en cientos de servidores únicamente mediante listas de tareas
- C. Reemplazar Git para el control de código fuente
- D. Monitorear únicamente trazas de aplicaciones

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El punto fuerte de Terraform son los recursos de infraestructura de nube y de red, no solo las tareas de paquetes a nivel de sistema operativo.

</details>

---
### Pregunta 16

Un error común es creer que Terraform y Ansible no pueden usarse juntos. ¿Qué es correcto?

- A. Abordan capas que se solapan pero son distintas, y con frecuencia son complementarios
- B. HashiCorp prohíbe usar ambos
- C. Ansible reemplaza el state de Terraform
- D. Terraform no puede generar valores de salida para otras herramientas

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los equipos suelen usar Terraform para la infraestructura y Ansible (u otras herramientas) para la configuración cuando es necesario.

</details>

---
### Pregunta 17

Las operaciones de stacks de CloudFormation están ligadas a:

- A. Cualquier nube mediante providers de Terraform
- B. APIs de AWS y tipos de recursos específicos de AWS
- C. Únicamente contenedores Docker locales
- D. Exclusivamente CRDs de Kubernetes

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** CloudFormation gestiona stacks de AWS mediante definiciones de recursos nativas de AWS.

</details>

---
### Pregunta 18

Ser agnóstico respecto al proveedor (provider-agnostic) en Terraform NO significa:

- A. Que todos los providers se comportan de forma idéntica en todas las funcionalidades
- B. Que el mismo flujo de trabajo (init, plan, apply) se aplica en todos los providers
- C. Que puede instalar providers desde un registry
- D. Que puede combinar múltiples providers en una misma configuración

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El flujo de trabajo es consistente, pero las capacidades y los esquemas de los providers difieren según el proveedor.

</details>

---
### Pregunta 19

El uso de lenguajes de programación por parte de Pulumi permite:

- A. Evitar todas las pruebas del código de infraestructura
- B. Usar construcciones de lenguaje conocidas como bucles, clases y paquetes
- C. Eliminar la necesidad de state
- D. Ejecutarse únicamente en la consola de AWS

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los lenguajes de propósito general aportan abstracciones conocidas; el state y las APIs de la nube siguen siendo necesarios.

</details>

---
### Pregunta 20

¿Cuáles son ventajas del enfoque multi-cloud de Terraform? (Seleccione todas las que correspondan.)

- A. Flujo de trabajo consistente entre providers
- B. Capacidad de gestionar entornos heterogéneos en una sola cadena de herramientas
- C. Eliminación automática de todas las caídas de la nube
- D. Prácticas compartidas para plan, revisión y apply
- E. Un único conjunto de habilidades basado en HCL para múltiples plataformas

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D, E**

**Explicación:** Terraform multi-cloud aporta consistencia de flujo de trabajo y prácticas compartidas. No elimina las caídas ni las diferencias entre proveedores.

</details>

---
### Pregunta 21

Terraform es declarativo. Los playbooks de Ansible suelen describirse como:

- A. Puramente declarativos, sin orden de tareas
- B. Secuencias procedimentales de tareas
- C. Únicamente plantillas JSON de CloudFormation
- D. Únicamente constructores de imágenes inmutables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las tareas de Ansible se ejecutan en orden; Terraform declara el estado final y deja que el motor planifique los cambios.

</details>

---
### Pregunta 22

¿Qué comparación es FALSA?

- A. CloudFormation está limitado a AWS
- B. Terraform puede usar providers para muchos proveedores
- C. Ansible es básicamente idéntico a Terraform en su propósito
- D. Pulumi soporta múltiples lenguajes de programación

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: C**

**Explicación:** Ansible y Terraform se solapan en los bordes, pero tienen enfoques principales distintos.

</details>

---
### Pregunta 23

Al evaluar herramientas de IaC, HCL de Terraform está diseñado para ser:

- A. Legible para las personas y adaptado a las estructuras de infraestructura
- B. Idéntico únicamente a las funciones intrínsecas de CloudFormation
- C. Únicamente un lenguaje de aplicación de propósito general
- D. Inutilizable con variables o módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** HCL es un DSL para infraestructura que equilibra la legibilidad con las construcciones propias de IaC.

</details>

---
### Pregunta 24

Un equipo estandarizó exclusivamente en AWS y quiere integración nativa con los servicios y una abstracción mínima. Podría considerar:

- A. CloudFormation o Terraform con el provider de AWS
- B. Terraform solo para software de escritorio
- C. Ansible solo para crear VPCs sin módulos de nube
- D. Git por sí solo, sin IaC

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Tanto CloudFormation como Terraform pueden gestionar AWS; la elección depende del ecosistema y de las necesidades multi-cloud.

</details>

---
### Pregunta 25

El ecosistema de providers de Terraform se distribuye mediante:

- A. El Terraform Registry y los plugins de provider
- B. Únicamente enlaces incrustados de la consola de AWS
- C. Archivos adjuntos de correo electrónico de los proveedores
- D. Módulos de kernel manuales

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los providers se publican y se consumen a través del registry y del mecanismo de plugins.

</details>

---
### Pregunta 26

¿Por qué Terraform NO es un reemplazo de Ansible en todos los casos?

- A. Terraform no puede declarar ningún recurso
- B. Terraform no se enfoca en la configuración detallada a nivel de sistema operativo ni en la orquestación de tareas ad hoc
- C. Ansible no puede tocar servidores Linux
- D. Terraform requiere agentes en cada host

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La configuración de paquetes del sistema operativo, la gestión de usuarios y las tareas ad hoc son más una fortaleza de Ansible que de Terraform.

</details>

---
### Pregunta 27

CloudFormation y Terraform ambos:

- A. Pueden gestionar infraestructura de AWS con plantillas/configuración declarativas
- B. Solo soportan bash imperativo
- C. Requieren Pulumi para funcionar
- D. Están limitados a un único recurso por stack

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Ambos soportan infraestructura de AWS declarativa, aunque la sintaxis y los ecosistemas difieren.

</details>

---
### Pregunta 28

Pulumi también rastrea el state de la infraestructura de forma similar a Terraform porque:

- A. Las APIs de la nube requieren llevar un registro de lo aprovisionado para poder actualizar y destruir
- B. Los lenguajes de programación eliminan las necesidades de persistencia
- C. AWS prohíbe los archivos de state
- D. El state solo es necesario para Ansible

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Cualquier herramienta de IaC que realice gestión del ciclo de vida necesita state o un rastreo equivalente.

</details>

---
### Pregunta 29

Multi-cloud NO significa automáticamente:

- A. Que cada carga de trabajo se ejecute en todas las nubes simultáneamente
- B. Que un equipo puede usar providers de Terraform para distintos proveedores
- C. Que los flujos de trabajo pueden estandarizarse con herramientas compartidas
- D. Que se reduce la dependencia de un proveedor (vendor lock-in) a nivel de herramienta

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La capacidad multi-cloud significa opcionalidad y gestión heterogénea, no una duplicación obligatoria en todas partes.

</details>

---
### Pregunta 30

¿Qué herramientas son exclusivas de AWS o principalmente nativas de AWS? (Seleccione todas las que correspondan.)

- A. AWS CloudFormation
- B. Terraform con el provider hashicorp/aws
- C. AWS CDK (genera CloudFormation)
- D. Terraform con el provider hashicorp/azurerm
- E. Provider de AWS de Pulumi

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, C**

**Explicación:** CloudFormation y CDK (que apunta a CloudFormation) son nativos de AWS. Terraform y Pulumi pueden apuntar a AWS, pero no son plataformas exclusivas de AWS.

</details>

---
### Pregunta 31

El enfoque de Terraform en el aprovisionamiento de infraestructura se demuestra con:

- A. Bloques resource como aws_instance y azurerm_resource_group
- B. Únicamente tareas de permisos de archivos locales
- C. Reemplazar por completo los pipelines de CI/CD
- D. Eliminar las APIs de la nube

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los tipos de recursos de Terraform se corresponden con objetos de infraestructura de nube y de red.

</details>

---
### Pregunta 32

La naturaleza procedimental de Ansible significa que:

- A. El orden de las tareas puede importar para el estado final del sistema
- B. No puede instalar paquetes
- C. Solo declara bloques CIDR de VPC
- D. Nunca usa variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El orden de las tareas y los pasos imperativos son centrales en muchos playbooks de Ansible.

</details>

---
### Pregunta 33

Elegir Pulumi en lugar de Terraform podría deberse a:

- A. El deseo de usar TypeScript/Python con las herramientas de lenguaje existentes
- B. El requisito de usar únicamente CloudFormation en JSON
- C. La necesidad de evitar toda gestión de state
- D. El mandato de usar únicamente ClickOps en la consola

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La familiaridad con el lenguaje y la integración con el ecosistema son razones comunes para adoptar Pulumi.

</details>

---
### Pregunta 34

Los flujos de trabajo agnósticos respecto al proveedor aún requieren:

- A. Ignorar la documentación del provider
- B. Comprender los tipos de recursos y la autenticación de cada provider
- C. Usar un único recurso en todo el proyecto
- D. Deshabilitar terraform init

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Cada provider tiene esquemas, autenticación y comportamientos propios, a pesar de compartir un mismo flujo de trabajo de Terraform.

</details>

---
### Pregunta 35

Terraform comparado con CloudFormation para una empresa multi-cloud:

- A. Terraform se alinea mejor con la gestión de múltiples proveedores desde una sola herramienta
- B. CloudFormation gestiona Azure de forma nativa
- C. Terraform no puede usar sintaxis JSON
- D. CloudFormation es agnóstico respecto al proveedor en todas las nubes

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** CloudFormation es específico de AWS; Terraform soporta muchos providers.

</details>

---
### Pregunta 36

HCL declarativo en Terraform significa que los usuarios escriben:

- A. Bloques resource y data que describen la infraestructura deseada
- B. Únicamente comandos de shell ordenados
- C. Exclusivamente transforms de CloudFormation
- D. Texto plano sin estructura y sin esquema

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los bloques HCL declaran recursos, variables, outputs y configuraciones de providers.

</details>

---
### Pregunta 37

Una trampa común del examen: Terraform y Ansible son solo competidores. Mejor respuesta:

- A. Con frecuencia se complementan entre sí para las capas de infraestructura frente a configuración
- B. No pueden usarse en la misma organización
- C. Ansible almacena el state de Terraform de forma predeterminada
- D. Terraform ejecuta playbooks de Ansible automáticamente sin configuración

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Muchas organizaciones usan ambos para distintas capas de la pila.

</details>

---
### Pregunta 38

Las funciones intrínsecas de CloudFormation y las expresiones de Terraform ambas:

- A. Ayudan a calcular valores dentro de plantillas/configuración declarativas
- B. Reemplazan la necesidad de providers
- C. Eliminan las variables
- D. Tienen una sintaxis idéntica

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Ambas soportan valores dinámicos, pero la sintaxis y las capacidades difieren.

</details>

---
### Pregunta 39

El valor de Terraform en entornos heterogéneos es:

- A. Un único flujo de trabajo plan/apply para diversos providers
- B. La traducción automática de recursos de Azure a recursos de AWS
- C. La eliminación de todos los atributos específicos de cada provider
- D. Un enfoque exclusivo en hardware on-premises

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El beneficio es un flujo de trabajo consistente; los recursos siguen siendo específicos de cada provider.

</details>

---
### Pregunta 40

¿Cuáles describen a Ansible con precisión? (Seleccione todas las que correspondan.)

- A. Enfoque en gestión de configuración
- B. Suele usar playbooks procedimentales
- C. Normalmente agentless sobre SSH/WinRM
- D. Servicio de stacks declarativo exclusivo de AWS
- E. Básicamente lo mismo que el propósito central de Terraform

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** Ansible es de gestión de configuración, procedimental y agentless. No es un servicio de stacks exclusivo de AWS ni tiene el mismo enfoque principal de aprovisionamiento que Terraform.

</details>

---
### Pregunta 41

Pulumi y Terraform ambos soportan:

- A. Infraestructura como código con vistas previas similares a plan (según la configuración) y rastreo de state
- B. Únicamente operaciones manuales en la consola
- C. Exclusivamente la sintaxis de playbooks de Ansible
- D. Gestionar infraestructura sin ningún plugin ni provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Ambas son plataformas de IaC con gestión del ciclo de vida, aunque las interfaces difieren.

</details>

---
### Pregunta 42

¿Por qué se podría preferir Terraform para las bases de infraestructura de red?

- A. Modelado declarativo de VPCs, subredes, enrutamiento y políticas de seguridad
- B. No puede modelar recursos de red
- C. Solo configura archivos /etc/hosts
- D. Reemplaza el DNS a nivel global

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los tipos de recursos de Terraform suelen modelar primitivas de red de la nube.

</details>

---
### Pregunta 43

Los stack sets de CloudFormation son una funcionalidad de AWS para:

- A. Desplegar stacks en múltiples cuentas/regiones
- B. Reemplazar los backends de state de Terraform
- C. Ejecutar playbooks de Ansible
- D. Gestionar suscripciones de Azure

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** StackSets extiende CloudFormation a las cuentas/regiones de una organización de AWS; es específico de AWS.

</details>

---
### Pregunta 44

Los plugins de provider de Terraform son responsables de:

- A. Traducir los cambios de recursos de Terraform en llamadas a la API del proveedor
- B. Formatear únicamente los sistemas de archivos de laptops
- C. Compilar únicamente HCL a bytecode de Python
- D. Almacenar mensajes de commit de Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los providers implementan operaciones CRUD contra APIs externas.

</details>

---
### Pregunta 45

Aprovisionamiento de infraestructura frente a gestión de configuración: ¿qué emparejamiento es el MÁS preciso?

- A. Terraform — aprovisionamiento; Ansible — configuración
- B. Terraform — solo configuración; Ansible — solo aprovisionamiento
- C. Ambos solo hacen análisis de logs
- D. Ninguno interactúa con APIs

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Esta distinción por capas es un punto de comparación central del examen.

</details>

---
### Pregunta 46

Usar lenguajes de programación reales (Pulumi) implica un intercambio:

- A. Toda la necesidad de pruebas
- B. La simplicidad de HCL por la flexibilidad y las abstracciones del lenguaje
- C. Cualquier capacidad de gestionar recursos en la nube
- D. Los requisitos de autenticación del provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los lenguajes añaden flexibilidad; los equipos aún deben gobernar la complejidad y el state.

</details>

---
### Pregunta 47

Que Terraform sea agnóstico respecto a la nube (cloud-agnostic) a nivel de herramienta significa:

- A. Que puede apuntar a múltiples plataformas sin cambiar a productos de IaC completamente distintos
- B. Que todas las nubes comparten nombres de recursos idénticos
- C. Que los precios son idénticos en todas las nubes
- D. Que nunca necesita credenciales

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La consistencia de las herramientas no implica capacidades ni precios idénticos entre nubes.

</details>

---
### Pregunta 48

Una afirmación FALSA sobre CloudFormation es:

- A. Usa plantillas para declarar infraestructura de AWS
- B. Puede gestionar Resource Groups de Azure de forma nativa
- C. Se integra con los servicios de AWS
- D. Las plantillas pueden ser JSON o YAML

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** CloudFormation no gestiona recursos de Azure de forma nativa.

</details>

---
### Pregunta 49

¿Cuáles son razones por las que los equipos adoptan Terraform para multi-cloud? (Seleccione todas las que correspondan.)

- A. Flujo de trabajo unificado (init, plan, apply)
- B. Amplio ecosistema de providers
- C. Esquemas de recursos idénticos en todas las nubes
- D. Patrones de módulos compartidos con variables
- E. Menor necesidad de aprender el DSL de IaC nativo de cada proveedor

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D, E**

**Explicación:** El flujo de trabajo, el ecosistema, los módulos y la reutilización de habilidades son beneficios. Los esquemas de recursos difieren según el provider.

</details>

---
### Pregunta 50

Ansible Galaxy proporciona principalmente:

- A. Roles y colecciones de Ansible reutilizables
- B. Únicamente binarios de providers de Terraform
- C. Stack sets de CloudFormation
- D. Claves de cifrado del state de Pulumi

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Galaxy es el centro de contenido de Ansible; Terraform usa el Terraform Registry para módulos/providers.

</details>

---
### Pregunta 51

HCL de Terraform frente a TypeScript de Pulumi: ambos buscan:

- A. Describir y gestionar la infraestructura de forma programática
- B. Reemplazar los SLAs de los proveedores de nube
- C. Eliminar IAM
- D. Evitar toda revisión de código

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Ambos son enfoques de creación de IaC con distintas opciones de lenguaje.

</details>

---
### Pregunta 52

A veces se malinterpreta agnóstico respecto al proveedor como «sin diferencias entre proveedores». La realidad:

- A. El flujo de trabajo es compartido; los atributos y límites de los recursos siguen siendo específicos de cada proveedor
- B. AWS y Azure usan tipos de recursos idénticos
- C. Terraform ignora los esquemas de los providers
- D. Los providers son opcionales para todos los recursos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Terraform unifica el proceso, no las APIs de nube, que no son idénticas.

</details>

---
### Pregunta 53

Para equipos estrictamente nativos de AWS reacios a las herramientas de terceros, una opción nativa es:

- A. CloudFormation o CDK
- B. Terraform solo para aplicaciones de escritorio
- C. Ansible solo sin módulos de nube
- D. GitOps sin ninguna IaC

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** CloudFormation/CDK son las vías de IaC nativas de AWS.

</details>

---
### Pregunta 54

El modelo declarativo de Terraform contrasta con los comandos ad hoc de Ansible porque:

- A. Los comandos ad hoc son acciones imperativas puntuales sin archivos persistentes de estado deseado
- B. Terraform no puede ejecutarse dos veces
- C. Ansible no puede automatizar nada
- D. Terraform solo funciona en localhost

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los comandos ad hoc de Ansible son imperativos y efímeros en comparación con la configuración declarada de Terraform.

</details>

---
### Pregunta 55

Al comparar herramientas de IaC, el «enfoque en el aprovisionamiento de infraestructura» de Terraform excluye:

- A. Un énfasis principal en el ajuste prolongado de paquetes del sistema operativo como su centro de diseño
- B. Crear balanceadores de carga
- C. Gestionar registros DNS mediante providers
- D. Definir buckets de almacenamiento

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El ajuste a nivel de sistema operativo es más el centro de Ansible; Terraform se centra en los recursos de infraestructura de nube.

</details>

---
### Pregunta 56

Pulumi puede apuntar a múltiples nubes, de forma similar a Terraform, mediante:

- A. Providers/SDKs específicos de cada nube dentro de los programas
- B. La eliminación de todas las credenciales
- C. Únicamente plantillas de CloudFormation
- D. Flujos de trabajo manuales exclusivamente en la consola

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Pulumi usa paquetes de provider para AWS, Azure, GCP y otros.

</details>

---
### Pregunta 57

Terraform frente a CloudFormation: ambos requieren:

- A. Comprender los recursos de nube subyacentes que se están modelando
- B. Lenguajes de plantilla idénticos
- C. Archivos de inventario de Ansible
- D. Ninguna autenticación con las APIs de la nube

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Ambos requieren conocimiento de la nube; los lenguajes y ecosistemas difieren.

</details>

---
### Pregunta 58

¿Qué afirmaciones sobre el propósito de Terraform son correctas? (Seleccione todas las que correspondan.)

- A. Aprovisionamiento declarativo de infraestructura
- B. Soporte multi-cloud basado en providers
- C. Reemplazo principal de la gestión de configuración para todas las tareas del sistema operativo
- D. Usa HCL como lenguaje principal
- E. Compite con CloudFormation en AWS mientras soporta otros proveedores

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D, E**

**Explicación:** Terraform es declarativo, multi-provider, basado en HCL y se solapa con CloudFormation en AWS, pero llega más lejos. No es principalmente una herramienta de gestión de configuración del sistema operativo.

</details>

---
### Pregunta 59

¿Qué herramienta usaría MÁS probablemente para ejecutar tareas ordenadas de instalación de paquetes en VMs existentes?

- A. Terraform solo con bloques resource
- B. Playbooks de Ansible
- C. Políticas de stack de CloudFormation
- D. terraform.tfvars

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Ansible destaca en tareas de configuración ordenadas sobre hosts existentes; Terraform se enfoca en aprovisionar objetos de infraestructura.

</details>

---
### Pregunta 60

Un equipo quiere una sola herramienta de IaC para recursos de AWS, Azure y Kubernetes con el mismo flujo de trabajo. La mejor opción:

- A. Únicamente AWS CloudFormation
- B. Terraform con múltiples providers
- C. ClickOps en la consola de cada nube
- D. Hojas de cálculo para cada recurso

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El modelo de providers de Terraform soporta plataformas heterogéneas bajo un único flujo de trabajo init/plan/apply.

</details>

---
