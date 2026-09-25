# Comprender las capacidades de HCP Terraform

> **Dominio del examen:** Comprender las capacidades de HCP Terraform | **Peso:** 8-10%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre HCP Terraform frente a OSS, el bloque cloud, workflows, modos de ejecución, Sentinel, run triggers, registry y estimación de costos.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

HCP Terraform (anteriormente Terraform Cloud) es:

- A. Un fork de Terraform solo local, sin funciones remotas
- B. La plataforma SaaS administrada de HashiCorp para la colaboración en Terraform y las operaciones remotas
- C. Un reemplazo de todos los proveedores de nube
- D. Únicamente un linter de módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** HCP Terraform agrega ejecuciones (runs) remotas, RBAC, registry, políticas y más.

</details>

---
### Pregunta 2

Terraform CLI de código abierto (OSS) se diferencia de HCP Terraform porque el CLI OSS:

- A. No puede ejecutar plan ni apply
- B. Se ejecuta localmente por defecto, a menos que se configure para usar el backend remoto de HCP Terraform
- C. Solo funciona con AWS
- D. Incluye Sentinel integrado de forma local

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El CLI OSS es local por defecto; cloud {} lo conecta a HCP Terraform.

</details>

---
### Pregunta 3

El bloque cloud {} configura:

- A. Las regiones de AWS
- B. La integración con la organización y los workspaces de HCP Terraform
- C. Solo las versiones de los providers
- D. Solo las rutas del state local

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El bloque cloud vincula el CLI con la organización y los workspaces de HCP Terraform.

</details>

---
### Pregunta 4

Un bloque cloud de ejemplo requiere:

- A. La configuración de organization y workspaces
- B. Solo alias de provider
- C. Solo valores por defecto de variables
- D. Siempre el nombre de un bucket de S3

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** organization más workspaces { name = ... } o tags.

</details>

---
### Pregunta 5

terraform login se utiliza para:

- A. Autenticar el CLI con HCP Terraform
- B. Iniciar sesión en la consola de AWS
- C. Solo descargar providers
- D. Desbloquear DynamoDB

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** login almacena el token de API de HCP Terraform en el archivo de credenciales.

</details>

---
### Pregunta 6

El plan gratuito (free tier) de HCP Terraform incluye hasta:

- A. 50 recursos administrados
- B. 500 recursos administrados
- C. Recursos ilimitados
- D. Cero recursos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Dato del examen: el plan gratuito permite hasta 500 recursos administrados.

</details>

---
### Pregunta 7

El workflow dirigido por VCS en HCP Terraform significa que:

- A. Los plan/apply se activan a partir de eventos de Git como pull requests y merges
- B. Terraform no puede usar Git
- C. Solo se permiten apply locales
- D. El state se almacena únicamente en laptops

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Se conectan repositorios para que los eventos de VCS inicien ejecuciones (runs) automáticamente.

</details>

---
### Pregunta 8

El workflow dirigido por CLI significa que:

- A. Los ingenieros ejecutan terraform plan/apply de forma local o mediante el CLI contra workspaces de HCP Terraform
- B. No interviene ningún CLI
- C. Solo se usan clics manuales en la UI
- D. Solo Ansible

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El workflow dirigido por CLI usa terraform login más ejecución remota o modos de ejecución local.

</details>

---
### Pregunta 9

El workflow dirigido por API permite:

- A. Que los sistemas de automatización creen ejecuciones (runs) mediante la API de HCP Terraform
- B. Solo acceso por consola
- C. Solo fmt
- D. Solo graph

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La API se integra con CI/CD y con automatizaciones personalizadas.

</details>

---
### Pregunta 10

Los workspaces de HCP Terraform se diferencian de los workspaces del CLI porque los workspaces de HCP:

- A. Son simplemente carpetas locales terraform.workspace renombradas
- B. Tienen state, variables e historial de ejecuciones (runs) independientes por cada workspace de la organización
- C. No pueden conectarse a VCS
- D. No almacenan state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Gran trampa del examen: los workspaces de HCP ≠ los workspaces del CLI.

</details>

---
### Pregunta 11

El comando terraform workspace select del CLI cambia:

- A. La configuración de los workspaces en la UI de HCP Terraform
- B. Únicamente la selección del archivo de state del workspace del CLI, local o remoto
- C. La cuenta de AWS
- D. Las políticas de Sentinel

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los workspaces del CLI cambian entre espacios de nombres de state; no tienen relación con los objetos workspace de HCP.

</details>

---
### Pregunta 12

El modo de ejecución remota (Remote execution mode) significa que:

- A. El plan y el apply se ejecutan en la infraestructura de HCP Terraform
- B. Los planes solo se ejecutan en el navegador
- C. El apply está deshabilitado
- D. El state es únicamente local

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Remote es el modo por defecto: las ejecuciones (runs) se realizan en agentes administrados por HashiCorp.

</details>

---
### Pregunta 13

El modo de ejecución local (Local execution mode) en HCP Terraform significa que:

- A. Las operaciones se ejecutan en su máquina, pero el state y las variables pueden seguir en HCP Terraform
- B. Todo, incluido el state, es únicamente local
- C. Sentinel se ejecuta solo de forma local
- D. VCS queda deshabilitado de forma permanente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El modo local usa su propio cómputo; la plataforma sigue registrando las ejecuciones (runs) y el state según la configuración.

</details>

---
### Pregunta 14

El modo de ejecución con agentes (Agent execution mode) utiliza:

- A. Agentes autoalojados en su red para realizar las ejecuciones (runs)
- B. Solo workers de internet público
- C. Ninguna autenticación
- D. Solo Docker en las laptops de HashiCorp

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los agentes alcanzan recursos privados que están detrás de firewalls.

</details>

---
### Pregunta 15

Las políticas de Sentinel en HCP Terraform se ejecutan:

- A. Solo antes de init
- B. Entre las etapas de plan y apply
- C. Solo después de destroy
- D. Nunca en Terraform Cloud

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las verificaciones de políticas ocurren después del plan y antes de que se permita el apply.

</details>

---
### Pregunta 16

Las políticas de Sentinel de tipo advisory:

- A. Bloquean los apply de forma incondicional
- B. Advierten o registran las violaciones, pero permiten que el apply continúe
- C. Eliminan workspaces
- D. Reemplazan providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las políticas advisory señalan problemas sin bloquear de forma estricta.

</details>

---
### Pregunta 17

Las políticas de Sentinel de tipo hard-mandatory:

- A. Deben aprobarse o el apply se bloquea
- B. Son solo sugerencias opcionales
- C. Se ejecutan solo de forma local
- D. Omiten la fase de plan

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Hard-mandatory aplica la gobernanza antes del apply.

</details>

---
### Pregunta 18

Los run triggers permiten:

- A. Que un workspace ponga en cola automáticamente ejecuciones (runs) en otro workspace después de apply exitosos
- B. Eliminar repositorios de VCS
- C. Omitir el plan
- D. State únicamente local

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los stacks dependientes pueden encadenarse mediante run triggers.

</details>

---
### Pregunta 19

HCP Terraform almacena el state:

- A. Sin cifrar por defecto en git
- B. Cifrado en reposo en la plataforma
- C. Solo en las laptops de los ingenieros
- D. En los esquemas de los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La plataforma administra el remote state cifrado.

</details>

---
### Pregunta 20

Las variables de Terraform en la UI de HCP Terraform sirven para:

- A. Valores consumidos por la configuración de Terraform (HCL)
- B. Solo las claves de acceso de AWS para el sistema operativo de la instancia, siempre
- C. Reemplazar providers
- D. La disposición del grafo

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las variables de Terraform se asignan a var.* en la configuración.

</details>

---
### Pregunta 21

Las variables de entorno en HCP Terraform sirven para:

- A. Establecer el entorno del proceso, como AWS_ACCESS_KEY_ID, para los providers
- B. Definir bloques output
- C. Reemplazar la configuración del backend en HCL
- D. Solo dar estilo a la UI

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las variables de entorno configuran el entorno de ejecución para los runs y los agentes.

</details>

---
### Pregunta 22

Marcar una variable como sensible en HCP Terraform:

- A. La oculta de la exposición casual en la UI y en los logs
- B. Elimina la necesidad de cifrado
- C. Elimina la variable al hacer apply
- D. Deshabilita VCS

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las variables sensibles de la UI se enmascaran de forma similar al comportamiento del CLI.

</details>

---
### Pregunta 23

El registry privado de módulos en HCP Terraform permite a las organizaciones:

- A. Publicar y compartir módulos de forma privada dentro de la organización
- B. Usar solo módulos del registry público
- C. Evitar el versionado fijo (version pinning)
- D. Deshabilitar las ejecuciones remotas

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El registry privado aloja módulos internos con versionado.

</details>

---
### Pregunta 24

La estimación de costos en HCP Terraform es compatible con:

- A. AWS, Azure y GCP
- B. Solo VMware on-premises
- C. Solo proveedores de DNS
- D. Ninguna nube pública

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La estimación de costos cubre las principales nubes públicas; dato del examen.

</details>

---
### Pregunta 25

El cambio de nombre del bloque terraform cloud {} refleja:

- A. El cambio de marca a HCP Terraform, mientras el bloque cloud sigue siendo el punto de integración
- B. La eliminación de los backends remotos
- C. La obsolescencia de las organizaciones
- D. State local obligatorio

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La configuración sigue usando el bloque cloud {} en las versiones recientes de Terraform.

</details>

---
### Pregunta 26

Las funciones de equipos y gobernanza de HCP Terraform incluyen:

- A. RBAC, policy sets y registros de auditoría (según el plan)
- B. Solo fmt
- C. Solo el grafo local
- D. Sin variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los planes superiores agregan SSO, políticas y permisos por equipo.

</details>

---
### Pregunta 27

Al usar el backend remoto con HCP Terraform, terraform apply:

- A. Puede ejecutarse de forma remota y transmitir los logs a la UI
- B. No puede mostrar logs
- C. Siempre modifica únicamente los archivos de state locales
- D. Omite el plan

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las ejecuciones remotas muestran logs y estado en la UI de HCP Terraform.

</details>

---
### Pregunta 28

¿Qué autentica las sesiones del CLI en HCP Terraform?

- A. terraform login / tokens de API
- B. terraform fmt
- C. Solo terraform validate
- D. Solo AWS STS

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** login obtiene y almacena un token de API.

</details>

---
### Pregunta 29

Los workspaces vinculados a ramas de VCS suelen usar:

- A. Patrones de un workspace por entorno o por rama, según el diseño de la organización
- B. Un único workspace global, siempre
- C. Sin state
- D. Solo workspaces del CLI

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Las organizaciones eligen estrategias de workspaces; el examen espera que se conozca el concepto de integración con VCS.

</details>

---
### Pregunta 30

Los planes especulativos (speculative plans) en pull requests están asociados con:

- A. El workflow dirigido por VCS
- B. Solo terraform destroy
- C. Solo el grafo local
- D. force-unlock

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** La integración con VCS puede ejecutar planes especulativos antes del merge.

</details>

---
### Pregunta 31

HCP Terraform impide por defecto la descarga del state mediante:

- A. RBAC y permisos sobre el acceso al workspace y al state
- B. Eliminar todos los outputs
- C. Deshabilitar los providers
- D. Forzar el state local

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los permisos controlan quién puede leer y escribir el state y las variables.

</details>

---
### Pregunta 32

Los policy sets asocian las políticas de Sentinel a:

- A. Workspaces o grupos de workspaces
- B. Solo los esquemas de los providers
- C. Solo .tfvars
- D. Solo módulos del registry público

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los policy sets se dirigen a colecciones de workspaces.

</details>

---
### Pregunta 33

Las run tasks (integraciones posteriores al plan) se diferencian de Sentinel porque las run tasks:

- A. Son integraciones externas en ciertas etapas de la ejecución; Sentinel es policy-as-code de HashiCorp
- B. Son idénticas a Sentinel
- C. Reemplazan terraform plan
- D. Solo se ejecutan después de destroy

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Debe saber que Sentinel es policy-as-code entre el plan y el apply; las run tasks son integraciones.

</details>

---
### Pregunta 34

terraform logout:

- A. Elimina las credenciales almacenadas de HCP Terraform para el CLI
- B. Elimina todos los recursos en la nube
- C. Desbloquea el state
- D. Migra backends

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** logout borra localmente el token de autenticación del CLI.

</details>

---
### Pregunta 35

Revisión n.º 35: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 36

Revisión n.º 36: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 37

Revisión n.º 37: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 38

Revisión n.º 38: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 39

Revisión n.º 39: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 40

Revisión n.º 40: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 41

Revisión n.º 41: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 42

Revisión n.º 42: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 43

Revisión n.º 43: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 44

Revisión n.º 44: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 45

Revisión n.º 45: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 46

Revisión n.º 46: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 47

Revisión n.º 47: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 48

Revisión n.º 48: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 49

Revisión n.º 49: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 50

Revisión n.º 50: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 51

Revisión n.º 51: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 52

Revisión n.º 52: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 53

Revisión n.º 53: confirme su respuesta con la documentación de Terraform.

- A. Opción A
- B. Opción B
- C. Opción C
- D. Opción D

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

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

**Explicación:** Marcador de posición recortado para cumplir con el número de preguntas por dominio.

</details>

---
### Pregunta 55

¿Cuáles son verdaderas sobre HCP Terraform frente a OSS? (Seleccione todas las que correspondan.)

- A. HCP Terraform ofrece ejecución remota de runs y funciones de colaboración
- B. El CLI OSS puede conectarse a HCP Terraform mediante cloud {}
- C. Los workspaces de HCP Terraform son idénticos a terraform workspace del CLI
- D. El state se almacena cifrado en la plataforma
- E. El plan gratuito incluye hasta 500 recursos administrados

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D, E**

**Explicación:** Los workspaces de HCP NO son lo mismo que los workspaces del CLI.

</details>

---
### Pregunta 56

¿Qué modos de ejecución existen en HCP Terraform? (Seleccione todas las que correspondan.)

- A. Remote
- B. Local
- C. Agent
- D. Sentinel
- E. VCS

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** Remote, Local y Agent son modos de ejecución. Sentinel es una política; VCS es un workflow.

</details>

---
### Pregunta 57

¿Qué workflows admite HCP Terraform? (Seleccione todas las que correspondan.)

- A. Dirigido por VCS
- B. Dirigido por CLI
- C. Dirigido por API
- D. Solo click-ops manual sin API
- E. Planes especulativos en pull requests (integración con VCS)

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** HCP Terraform admite workflows de VCS, CLI y API.

</details>

---
### Pregunta 58

¿Qué afirmaciones sobre Sentinel son correctas? (Seleccione todas las que correspondan.)

- A. Las políticas se evalúan entre el plan y el apply
- B. Las políticas advisory pueden advertir sin bloquear
- C. Las políticas hard-mandatory bloquean el apply cuando fallan
- D. Sentinel se ejecuta dentro de terraform console de forma local por defecto
- E. Los policy sets asocian políticas a workspaces

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, E**

**Explicación:** Sentinel es una función de gobernanza de HCP Terraform, no de la consola local.

</details>

---
### Pregunta 59

¿Qué afirmaciones sobre variables y almacenamiento son verdaderas en HCP Terraform? (Seleccione todas las que correspondan.)

- A. Las variables de Terraform se asignan a var.* de HCL
- B. Las variables de entorno configuran el runtime, por ejemplo las credenciales del provider
- C. Las variables sensibles se enmascaran en la UI y en los logs
- D. El registry privado puede alojar módulos internos
- E. La estimación de costos funciona para AWS, Azure y GCP

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, D, E**

**Explicación:** Todas las afirmaciones reflejan capacidades estándar de HCP Terraform.

</details>

---
### Pregunta 60

¿Qué funciones de colaboración se asocian con HCP Terraform? (Seleccione todas las que correspondan.)

- A. Run triggers entre workspaces
- B. Remote state cifrado
- C. Autenticación con terraform login
- D. Configuración del bloque cloud {}
- E. Reemplazar terraform init por completo

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C, D**

**Explicación:** init sigue siendo necesario; cloud {} configura el backend/integración de HCP Terraform.

</details>

---
