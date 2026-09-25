# Usar el flujo de trabajo principal de Terraform

> **Dominio del examen:** Usar el flujo de trabajo principal de Terraform | **Peso:** 8-10%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Cubre init, validate, fmt, plan, apply, destroy, el uso de targeting y el ciclo de vida estándar escribir-planificar-aplicar (write-plan-apply).

**Instrucciones:** Responda cada pregunta y luego despliegue el menú para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Cuál es el primer comando que debe ejecutar en un nuevo directorio de trabajo de Terraform?

- A. terraform plan
- B. terraform init
- C. terraform apply
- D. terraform validate

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Init descarga los providers y módulos (modules) y configura el backend. Plan y apply requieren que la inicialización se haya realizado antes.

</details>

---
### Pregunta 2

¿Qué logra principalmente `terraform init`?

- A. Aplica los cambios de configuración en la nube
- B. Inicializa el backend, instala los providers y descarga los módulos
- C. Da formato a los archivos .tf según el estilo canónico
- D. Destruye todos los recursos administrados

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Init prepara el directorio de trabajo. No modifica la infraestructura real.

</details>

---
### Pregunta 3

¿Cuándo debe usar `terraform init -upgrade`?

- A. Para migrar el state a un nuevo backend
- B. Para actualizar los providers/módulos a las versiones más recientes permitidas por las restricciones
- C. Para validar únicamente la sintaxis
- D. Para destruir recursos específicos (targeted)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-upgrade` vuelve a consultar el registry en busca de versiones más recientes de providers/módulos permitidas por sus restricciones de versión.

</details>

---
### Pregunta 4

¿Qué hace `terraform init -migrate-state`?

- A. Copia los archivos .tf a un nuevo directorio
- B. Reconfigura el backend y migra el state existente al nuevo backend
- C. Actualiza la versión de la CLI de Terraform
- D. Importa automáticamente todos los recursos de la nube

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Use `-migrate-state` cuando cambie la configuración del backend para que Terraform mueva el state a la nueva ubicación de almacenamiento.

</details>

---
### Pregunta 5

¿Qué verifica `terraform validate`?

- A. Si las credenciales de la nube son válidas
- B. La sintaxis y la consistencia interna de la configuración sin acceder a servicios remotos
- C. Si los archivos .tf cumplen con el formato canónico
- D. Si el plan guardado coincide con el state actual

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Validate verifica la sintaxis HCL y la consistencia lógica. No verifica las credenciales ni la conectividad con las API.

</details>

---
### Pregunta 6

¿Cuál es el propósito de `terraform fmt`?

- A. Validar los esquemas de los providers
- B. Reescribir los archivos .tf al estilo de formato canónico
- C. Generar un plan de ejecución
- D. Bloquear el state para ejecuciones concurrentes

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `fmt` estandariza el formato (sangría, espaciado). No cambia la lógica de los recursos.

</details>

---
### Pregunta 7

¿Qué hace `terraform fmt -check`?

- A. Verifica únicamente errores de sintaxis
- B. Informa si los archivos necesitan formato sin modificarlos (código de salida distinto de cero si se necesitan cambios)
- C. Verifica la conectividad con la API remota
- D. Valida los tipos de las variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-check` es apto para CI: devuelve 0 si el formato es correcto y un valor distinto de cero si sería necesario reformatear.

</details>

---
### Pregunta 8

¿Por qué usar `terraform fmt -recursive`?

- A. Para dar formato a los archivos .tf de los subdirectorios además del directorio actual
- B. Para destruir recursivamente los módulos anidados
- C. Para volver a ejecutar init en todas las carpetas hijas
- D. Para validar todos los módulos del registry

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** `-recursive` recorre los subdirectorios aplicando el formato; es útil en monorepos con configuración anidada.

</details>

---
### Pregunta 9

¿Qué afirmaciones distinguen a validate de fmt? Seleccione todas las que correspondan.

- A. validate verifica la sintaxis y la consistencia
- B. fmt cambia el formato de los archivos
- C. validate requiere acceso a la API de la nube
- D. fmt -check es útil en los pipelines de CI

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Validate no necesita acceso a la nube. fmt da formato a los archivos; `-check` verifica el formato sin escribir cambios.

</details>

---
### Pregunta 10

¿`terraform plan` modifica la infraestructura real?

- A. Sí, crea un despliegue parcial
- B. No, solo muestra un plan de ejecución propuesto
- C. Solo cuando se usa -auto-approve
- D. Solo para los data sources

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Plan es de solo lectura respecto a la infraestructura. Los cambios ocurren únicamente en apply.

</details>

---
### Pregunta 11

¿Cómo se guarda un plan en un archivo para aplicarlo después?

- A. terraform plan -save=plan.tfplan
- B. terraform plan -out=plan.tfplan
- C. terraform apply -out=plan.tfplan
- D. terraform plan > plan.tfplan

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Use `terraform plan -out=<file>` para guardar un plan binario. Aplíquelo con `terraform apply <file>`.

</details>

---
### Pregunta 12

¿Qué muestra `terraform plan -destroy`?

- A. Un plan para crear todos los recursos
- B. Un plan que muestra los recursos que serían destruidos
- C. Un plan para importar recursos existentes
- D. Un plan para dar formato a los archivos de configuración

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-destroy` muestra una vista previa de la destrucción de todos los recursos administrados (objetivo similar al del comando destroy).

</details>

---
### Pregunta 13

¿Cómo se aplica un archivo de plan guardado previamente?

- A. terraform apply -plan=plan.tfplan
- B. terraform apply plan.tfplan
- C. terraform plan -apply plan.tfplan
- D. terraform init plan.tfplan

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Ejecute `terraform apply plan.tfplan`. El plan guardado fija los cambios exactos; no hay aprobación interactiva para el contenido del plan.

</details>

---
### Pregunta 14

¿Qué hace `terraform apply -auto-approve`?

- A. Omite el aviso de aprobación interactiva
- B. Ejecuta automáticamente terraform init primero
- C. Aprueba únicamente las operaciones de destrucción
- D. Deshabilita el bloqueo del state (state locking)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** `-auto-approve` aplica sin pedir `yes`. Es peligroso en producción, ya que los cambios se ejecutan de inmediato.

</details>

---
### Pregunta 15

¿Cuándo es apropiado usar `terraform apply -target`?

- A. Como opción predeterminada en cada apply
- B. Solo en casos excepcionales; puede dejar la infraestructura en un estado parcial
- C. Nunca, fue eliminado en Terraform 1.0
- D. Solo durante terraform destroy

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El targeting limita el alcance del apply. El examen espera que sepa que existe, pero que conlleva riesgos de inconsistencias en las dependencias.

</details>

---
### Pregunta 16

¿Cómo se pasa una variable por la línea de comandos durante apply?

- A. terraform apply -var name=value
- B. terraform apply -var="name=value"
- C. terraform apply --variable name:value
- D. terraform apply -Dname=value

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Use `-var="name=value"` o `-var-file=filename` en los comandos plan/apply/destroy.

</details>

---
### Pregunta 17

¿Qué hace `terraform apply -var-file=prod.tfvars`?

- A. Crea un nuevo archivo tfvars
- B. Carga los valores de las variables desde el archivo especificado para esta ejecución
- C. Exporta los outputs a prod.tfvars
- D. Valida únicamente la sintaxis de prod.tfvars

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-var-file` proporciona valores de variables. Se pueden usar varias opciones `-var-file`; los archivos posteriores sobrescriben a los anteriores.

</details>

---
### Pregunta 18

¿Qué símbolos de la salida del plan son correctos? Seleccione todas las que correspondan.

- A. + significa crear
- B. - significa destruir
- C. ~ significa reemplazar
- D. <= significa leer (data source)

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** `~` significa actualización in situ (in-place). `-/+` significa reemplazar (destruir y luego crear). `<=` indica la lectura de un data source.

</details>

---
### Pregunta 19

¿Qué indica el símbolo `-/+` en la salida del plan?

- A. El recurso se actualizará in situ (in-place)
- B. El recurso será destruido y vuelto a crear
- C. El recurso será importado
- D. El data source solo será actualizado (refresh)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-/+` señala un reemplazo forzado: se destruye el recurso existente y se crea uno nuevo.

</details>

---
### Pregunta 20

¿Qué hace `terraform destroy`?

- A. Elimina únicamente el directorio .terraform
- B. Crea un plan de destrucción y elimina toda la infraestructura administrada tras la confirmación
- C. Elimina recursos del state sin realizar cambios en la nube
- D. Da formato y valida la configuración

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `destroy` es un comando de conveniencia que planifica y aplica la destrucción de todos los recursos de la configuración.

</details>

---
### Pregunta 21

¿En qué se diferencia `terraform apply -destroy` de `terraform destroy`?

- A. Son comandos sin relación
- B. Ambos producen planes de destrucción; destroy es un atajo, mientras que apply -destroy usa la ruta de código de apply
- C. apply -destroy solo destruye los recursos específicos (targeted)
- D. destroy requiere un archivo de plan guardado

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Ambos inician la destrucción. `terraform destroy` es esencialmente `apply` con semántica de destrucción. Conozca ambos para el examen.

</details>

---
### Pregunta 22

¿Se puede usar `-target` con `terraform destroy`?

- A. No
- B. Sí, para destruir recursos específicos
- C. Solo con el backend local
- D. Solo en HCP Terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform destroy -target=<address>` destruye únicamente el recurso especificado y sus dependencias.

</details>

---
### Pregunta 23

¿Cuál es el orden correcto del flujo de trabajo principal?

- A. apply → init → plan → write
- B. write → init → plan → apply
- C. init → write → destroy → plan
- D. validate → apply → init → plan

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Flujo estándar: redactar la configuración, inicializar, obtener una vista previa con plan y luego aplicar los cambios.

</details>

---
### Pregunta 24

¿Debe volver a ejecutar `terraform init` después de cambiar únicamente argumentos de recursos (sin nuevos providers/módulos/backend)?

- A. Sí, siempre antes de cada plan
- B. No necesariamente; init es necesario cuando cambian los providers, los módulos o el backend
- C. Nunca después del primer init
- D. Solo en destroy

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los cambios de configuración en recursos existentes no requieren volver a ejecutar init, a menos que cambien las dependencias o el backend.

</details>

---
### Pregunta 25

¿Qué opciones (flags) de init cumplen estos propósitos? Seleccione todas las que correspondan.

- A. -upgrade actualiza las versiones de providers/módulos dentro de las restricciones
- B. -migrate-state mueve el state cuando cambia el backend
- C. -auto-approve omite los avisos de apply
- D. init es necesario antes del primer plan

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** `-auto-approve` pertenece a apply, no a init. Init debe ejecutarse antes de planificar en un directorio nuevo.

</details>

---
### Pregunta 26

Si `terraform validate` tiene éxito, ¿se garantiza que la configuración se desplegará correctamente?

- A. Sí, validate cubre todos los errores en tiempo de ejecución
- B. No, validate no verifica errores reales de las API ni los permisos
- C. Solo con un backend remoto
- D. Solo para los módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Validate detecta errores de sintaxis y de referencias, pero no los límites de cuota de la nube, las denegaciones de IAM ni los problemas de red que se descubren durante apply.

</details>

---
### Pregunta 27

¿`terraform fmt` modifica la lógica de los recursos o los valores de los atributos?

- A. Sí, optimiza las expresiones
- B. No, solo cambia los espacios en blanco y el formato
- C. Elimina los recursos sin usar
- D. Actualiza las versiones de los providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** fmt es cosmético. No altera la infraestructura que se creará.

</details>

---
### Pregunta 28

¿Qué código de salida devuelve `terraform fmt -check` cuando los archivos necesitan formato?

- A. 0
- B. Distinto de cero (3 en las versiones recientes de Terraform)
- C. 1 solo para errores de sintaxis
- D. Nunca devuelve un valor distinto de cero

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-check` devuelve un valor distinto de cero cuando el formato difiere; se usa en CI para hacer cumplir el estilo.

</details>

---
### Pregunta 29

¿Puede ejecutarse `terraform plan` sin `terraform init`?

- A. Sí, siempre
- B. No, init debe haberse ejecutado correctamente antes
- C. Solo con -refresh-only
- D. Solo para los planes de destrucción

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Plan requiere providers y backend inicializados. Los directorios sin inicializar generan un error en plan.

</details>

---
### Pregunta 30

Al aplicar un archivo de plan guardado, ¿puede agregar nuevas opciones `-var`?

- A. Sí, para sobrescribir el plan
- B. No, el plan guardado es fijo; las variables se resolvieron cuando se creó el plan
- C. Solo con -auto-approve
- D. Solo para los planes de destrucción

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los planes guardados encapsulan las decisiones tomadas en el momento del plan. Aplique el archivo de plan tal cual, sin alterar las variables.

</details>

---
### Pregunta 31

¿Qué opciones (flags) de apply son válidas? Seleccione todas las que correspondan.

- A. -auto-approve
- B. -target=aws_instance.web
- C. -var="env=prod"
- D. -generate-config-out

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** `-generate-config-out` es una opción de plan para los flujos de importación, no una opción de apply.

</details>

---
### Pregunta 32

¿Qué significa el símbolo `+` en la salida del plan?

- A. Destruir
- B. Crear
- C. Leer
- D. Sin operación (no-op)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `+` indica que se creará un recurso.

</details>

---
### Pregunta 33

¿Qué significa el símbolo `-` en la salida del plan?

- A. Crear
- B. Destruir
- C. Actualización in situ (in-place)
- D. Importar

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-` significa que el recurso será destruido.

</details>

---
### Pregunta 34

¿Qué significa `~` en la salida del plan?

- A. Actualización in situ (in-place)
- B. Reemplazar
- C. Crear
- D. Ignorar

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** `~` en los atributos muestra una modificación in situ. El símbolo `-/+` a nivel de recurso indica un reemplazo.

</details>

---
### Pregunta 35

¿Qué indica `<=` en la salida del plan?

- A. Descarga de módulos
- B. Lectura de un data source durante el plan
- C. Migración del state
- D. Actualización de un provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `<=` aparece en los data sources que se leerán durante el ciclo de plan/apply.

</details>

---
### Pregunta 36

¿Es `terraform destroy` interactivo de forma predeterminada?

- A. No, siempre se aprueba automáticamente
- B. Sí, solicita confirmación a menos que se use -auto-approve
- C. Nunca solicita confirmación
- D. Solo con un backend remoto

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Al igual que apply, destroy solicita confirmación a menos que se pase `-auto-approve`.

</details>

---
### Pregunta 37

¿Puede `terraform plan` aceptar `-var-file`?

- A. No, solo apply
- B. Sí, plan y apply aceptan tanto -var como -var-file
- C. Solo destroy acepta archivos de variables
- D. Solo init acepta archivos de variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las opciones de variables funcionan en plan, apply y destroy para que el plan refleje los valores elegidos.

</details>

---
### Pregunta 38

¿Qué comandos forman parte del flujo de trabajo principal Escribir → Init → Plan → Apply? Seleccione todas las que correspondan.

- A. terraform init
- B. terraform plan
- C. terraform graph
- D. terraform apply

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** graph es una herramienta de inspección de la CLI (dominio 4), no forma parte del flujo de trabajo principal de aprovisionamiento.

</details>

---
### Pregunta 39

¿Qué sucede si ejecuta `terraform apply` sin un plan guardado?

- A. Falla de inmediato
- B. Terraform genera un nuevo plan y solicita aprobación antes de aplicar
- C. Aplica sin ninguna vista previa
- D. Solo ejecuta validate

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El apply predeterminado muestra el plan y pide confirmación, salvo que se use `-auto-approve` o se aplique un archivo de plan guardado.

</details>

---
### Pregunta 40

¿Por qué guardar un plan con `-out` antes de apply en CI/CD?

- A. Para omitir terraform init
- B. Para asegurar que se aplique exactamente el plan revisado
- C. Para no necesitar providers
- D. Para deshabilitar el bloqueo del state (state locking)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los planes guardados evitan el drift entre la revisión y el apply: lo que se aprobó es exactamente lo que se ejecuta.

</details>

---
### Pregunta 41

¿Ejecuta `terraform destroy` un plan primero?

- A. No, elimina de inmediato sin vista previa
- B. Sí, muestra qué será destruido antes de la confirmación
- C. Solo con -target
- D. Solo para los módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Destroy presenta un plan de destrucción y espera la confirmación (a menos que se apruebe automáticamente).

</details>

---
### Pregunta 42

¿Puede ejecutar `terraform validate` antes de `terraform init`?

- A. A veces, pero se recomienda ejecutar init primero para una validación completa con los providers
- B. Nunca, bajo ninguna circunstancia
- C. Solo después de apply
- D. Validate siempre requiere un remote state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Una validación básica puede funcionar, pero los esquemas de los providers a menudo requieren init. Mejor práctica: ejecutar init y luego validate.

</details>

---
### Pregunta 43

¿Qué problema tiene usar `-auto-approve` en un CI de producción sin revisión?

- A. Deshabilita los providers
- B. Los cambios de infraestructura se aplican sin revisión humana del plan
- C. Impide el bloqueo del state
- D. Elimina el archivo de state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El examen enfatiza que `-auto-approve` omite el aviso de seguridad, lo cual es peligroso sin controles de revisión del plan independientes.

</details>

---
### Pregunta 44

Si cambia la configuración del backend, ¿qué combinación de comandos se requiere?

- A. terraform apply -migrate-state
- B. terraform init -migrate-state
- C. terraform plan -migrate-state
- D. terraform fmt -migrate-state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los cambios de backend requieren volver a ejecutar init con `-migrate-state` para mover el state existente al nuevo backend.

</details>

---
### Pregunta 45

¿Qué comando muestra una vista previa de los cambios sin aplicarlos?

- A. terraform apply
- B. terraform plan
- C. terraform init
- D. terraform fmt

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Plan es el paso de vista previa. Apply ejecuta los cambios.

</details>

---
### Pregunta 46

¿Qué requiere `terraform apply -destroy` antes de ejecutarse?

- A. Únicamente un archivo de plan de destrucción guardado
- B. Un init exitoso; luego planifica la destrucción como otras operaciones de apply
- C. Ejecutar terraform import primero
- D. Eliminar todos los bloques output

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Apply -destroy necesita un directorio inicializado y sigue el flujo normal de apply con semántica de destrucción.

</details>

---
### Pregunta 47

¿Están disponibles las opciones `-var` en `terraform plan`?

- A. No
- B. Sí
- C. Solo en destroy
- D. Solo en HCP Terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Pase las variables en el momento del plan para que la vista previa coincida con los valores usados en apply.

</details>

---
### Pregunta 48

¿Cuál es la relación entre `terraform plan -destroy` y `terraform destroy`?

- A. No tienen relación
- B. Ambos muestran una vista previa de la destrucción; destroy engloba la planificación y la aplicación de la destrucción
- C. plan -destroy aplica los cambios
- D. destroy no puede apuntar a recursos específicos (target)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-destroy` en plan muestra una vista previa de las eliminaciones. `terraform destroy` automatiza el flujo completo de destrucción.

</details>

---
### Pregunta 49

¿Qué afirmaciones sobre las operaciones de destrucción son verdaderas? Seleccione todas las que correspondan.

- A. terraform destroy elimina la infraestructura administrada
- B. terraform apply -destroy también planifica la destrucción
- C. destroy -target limita el alcance
- D. destroy omite la planificación por completo

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, C**

**Explicación:** Destroy muestra un plan antes de continuar, a menos que se apruebe automáticamente. No omite la planificación.

</details>

---
### Pregunta 50

Después de `terraform init -upgrade`, ¿qué debe ejecutar para obtener una vista previa de los cambios resultantes?

- A. Solo terraform fmt
- B. terraform plan
- C. terraform force-unlock
- D. Solo terraform console

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Tras actualizar los providers/módulos, ejecute plan para ver cómo afectan a la infraestructura las actualizaciones de dependencias.

</details>

---
### Pregunta 51

¿Qué paso del flujo de trabajo detecta HCL sin formato en CI?

- A. terraform validate
- B. terraform fmt -check
- C. terraform plan
- D. terraform init

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Use `fmt -check` en CI para hacer cumplir el formato. validate no verifica el estilo.

</details>

---
### Pregunta 52

¿Puede `terraform apply` usar varios argumentos `-var-file`?

- A. No, solo un archivo
- B. Sí, los archivos posteriores sobrescriben a los anteriores en las claves duplicadas
- C. Solo con variables JSON
- D. Solo en init

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Varias opciones `-var-file` se combinan, y los archivos posteriores tienen prioridad para los nombres de variables duplicados.

</details>

---
### Pregunta 53

¿Cuál es el riesgo principal de depender de `-target` para los despliegues rutinarios?

- A. Elimina el archivo de state
- B. Las dependencias pueden ignorarse, dejando la infraestructura inconsistente
- C. Impide la descarga de providers
- D. Deshabilita los outputs

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las operaciones con targeting omiten el orden completo del grafo; es aceptable para emergencias, pero no para el flujo de trabajo estándar.

</details>

---
### Pregunta 54

¿`terraform plan -out` fija los valores de las variables usados en el momento del plan?

- A. No, las variables se resuelven de nuevo en apply
- B. Sí, el plan guardado captura los cambios planificados con los valores resueltos
- C. Solo para los módulos
- D. Solo con el backend local

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El archivo de plan guardado conserva el conjunto de acciones planificadas; apply usa ese plan congelado.

</details>

---
### Pregunta 55

¿Qué comando debe ejecutarse después de editar archivos .tf para corregir la sangría antes de hacer commit?

- A. terraform validate
- B. terraform fmt
- C. terraform apply
- D. terraform destroy

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `terraform fmt` (a menudo con `-recursive`) estandariza el formato antes del control de versiones.

</details>

---
### Pregunta 56

¿Pueden `terraform plan` y `terraform apply` usar `-input=false`?

- A. No, las opciones de entrada no existen
- B. Sí, para deshabilitar los avisos interactivos de variables
- C. Solo apply lo admite
- D. Solo con HCP Terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** `-input=false` evita que la CLI solicite valores de variables no definidas; es útil en la automatización cuando todos los valores se proporcionan mediante archivos u opciones.

</details>

---
### Pregunta 57

¿Qué hace ejecutar `terraform apply` sin argumentos después de rechazar el aviso de confirmación?

- A. Aplica cambios parciales
- B. Cancela el apply; no se realiza ningún cambio
- C. Guarda el plan automáticamente
- D. Ejecuta destroy en su lugar

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Responder `no` cancela el apply. No se producen cambios en la infraestructura.

</details>

---
### Pregunta 58

¿Es necesario `terraform destroy` para eliminar un solo recurso conservando los demás?

- A. Sí, destroy siempre elimina todo
- B. No, puede usar destroy -target o eliminar el recurso de la configuración y ejecutar apply
- C. Solo funciona terraform state rm
- D. Solo HCP Terraform admite la eliminación selectiva

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Eliminación selectiva: elimine el bloque del recurso y ejecute apply, o use `destroy -target`. No es necesario un destroy completo.

</details>

---
### Pregunta 59

¿Qué comando verifica la configuración sin contactar las API del proveedor de nube?

- A. terraform plan
- B. terraform validate
- C. terraform apply
- D. terraform refresh

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Validate es local. Plan puede contactar a los providers para actualizar el state (refresh), a menos que se use `-refresh=false`.

</details>

---
### Pregunta 60

Después de cambiar únicamente `terraform.tfvars`, ¿debe ejecutar init de nuevo antes de plan?

- A. Sí, siempre
- B. No, los cambios en los valores de las variables no requieren volver a ejecutar init
- C. Solo con un backend remoto
- D. Solo si se usan módulos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los valores de las variables se evalúan en plan/apply. Init no es necesario solo por cambios en tfvars.

</details>

---
