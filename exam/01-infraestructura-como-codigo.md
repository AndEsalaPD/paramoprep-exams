# Comprender la Infraestructura como Código (IaC)

> **Dominio del examen:** Comprender la Infraestructura como Código (IaC) | **Peso:** 5-7%
> **Preguntas:** 60 | **Formato:** Opción múltiple y selección múltiple (como Terraform Associate 004)

Abarca los conceptos de IaC, los enfoques declarativo vs. imperativo, los beneficios de la automatización y cómo encaja Terraform en el panorama de IaC.

**Instrucciones:** Responda cada pregunta y luego expanda el desplegable para verificar su respuesta y la explicación.

---

### Pregunta 1

¿Qué es la Infraestructura como Código (IaC)?

- A. Administrar la infraestructura exclusivamente a través de la consola web de un proveedor de nube
- B. Definir y administrar la infraestructura mediante archivos de configuración legibles por máquina
- C. Escribir scripts de shell que se conectan por SSH a los servidores para instalar paquetes
- D. Almacenar diagramas de infraestructura en una wiki para los equipos de operaciones

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** IaC define la infraestructura en archivos de configuración bajo control de versiones, en lugar de pasos manuales o scripts ad hoc.

</details>

---
### Pregunta 2

¿Qué práctica es un beneficio principal de la Infraestructura como Código?

- A. Eliminar la necesidad de las APIs del proveedor de nube
- B. Almacenar las definiciones de infraestructura en control de versiones para tener historial y colaboración
- C. Garantizar cero tiempo de inactividad en cada despliegue
- D. Eliminar la necesidad de probar los cambios antes de producción

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El control de versiones permite tener historial de cambios, revisiones, reversiones y colaboración del equipo sobre las definiciones de infraestructura.

</details>

---
### Pregunta 3

En un enfoque de IaC declarativo, ¿qué especifica principalmente el profesional?

- A. La secuencia exacta de llamadas a la API para alcanzar el estado deseado
- B. El estado final deseado de la infraestructura
- C. El orden de los comandos de shell en cada host
- D. Únicamente las direcciones IP de los servidores existentes

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El IaC declarativo describe cómo debe verse la infraestructura; la herramienta determina cómo lograr ese estado.

</details>

---
### Pregunta 4

¿Qué afirmación describe mejor un enfoque imperativo para la administración de infraestructura?

- A. Se declara el estado objetivo y la herramienta concilia las diferencias
- B. Se especifican los comandos paso a paso que se deben ejecutar
- C. Solo se almacena la infraestructura en plantillas JSON
- D. Nunca se modifica la infraestructura después de su creación inicial

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los enfoques imperativos se centran en cómo ejecutar los cambios (comandos/pasos), no solo en el resultado deseado.

</details>

---
### Pregunta 5

Terraform se clasifica mejor como qué tipo de herramienta de IaC?

- A. Administración de configuración imperativa
- B. Aprovisionamiento de infraestructura declarativo
- C. Sistema de aplicación de parches a hosts basado en agentes
- D. Solo automatización de runbooks manuales

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform usa HCL declarativo para describir la infraestructura deseada y la aprovisiona mediante providers.

</details>

---
### Pregunta 6

¿Qué significa idempotencia en el contexto de IaC?

- A. Cada apply debe destruir primero todos los recursos
- B. Aplicar repetidamente la misma configuración produce el mismo resultado sin efectos secundarios no deseados
- C. Solo una persona puede ejecutar apply a la vez
- D. Los recursos nunca pueden actualizarse después de su creación

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las operaciones idempotentes producen resultados consistentes cuando se repiten; Terraform busca lograr esto durante plan/apply.

</details>

---
### Pregunta 7

¿Qué escenario ilustra mejor la infraestructura inmutable?

- A. Conectarse por SSH a un servidor y aplicar parches a los paquetes directamente
- B. Reemplazar una instancia fallida por una nueva construida a partir de la misma imagen/configuración
- C. Editar manualmente las reglas de los grupos de seguridad en la consola
- D. Almacenar el estado del servidor solo en discos locales sin copias de seguridad

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La infraestructura inmutable favorece reemplazar los componentes con instancias nuevas en lugar de modificar directamente las que están en ejecución.

</details>

---
### Pregunta 8

¿Qué empresa desarrolla Terraform y en qué lenguaje está escrito?

- A. Amazon; Python
- B. HashiCorp; Go
- C. Microsoft; C#
- D. Google; Java

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform es un proyecto de código abierto de HashiCorp implementado principalmente en Go.

</details>

---
### Pregunta 9

¿Qué es el configuration drift (deriva de configuración)?

- A. Cuando el archivo de state de Terraform se elimina accidentalmente
- B. Cuando la infraestructura real se desvía de la configuración de IaC definida
- C. Cuando los plugins de provider no se descargan durante init
- D. Cuando los errores de sintaxis de HCL impiden la validación

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El drift ocurre cuando cambios manuales o externos hacen que la infraestructura real difiera del código y del state.

</details>

---
### Pregunta 10

¿Cuáles son beneficios comunes de la Infraestructura como Código? (Seleccione todas las que correspondan.)

- A. Consistencia entre entornos
- B. Eliminación de todo el trabajo operativo humano
- C. Reutilización de patrones de configuración
- D. Mejor capacidad de auditoría gracias al historial de versiones
- E. Automatización del aprovisionamiento

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, C, D, E**

**Explicación:** IaC mejora la consistencia, la reutilización, los registros de auditoría y la automatización. Reduce el trabajo manual, pero no elimina todo el criterio humano ni todas las operaciones.

</details>

---
### Pregunta 11

¿Qué es el antipatrón ClickOps?

- A. Usar herramientas de CLI en lugar de una GUI
- B. Realizar cambios de infraestructura únicamente mediante clics en la consola de la nube, sin definiciones codificadas
- C. Automatizar despliegues con pipelines de CI
- D. Almacenar el código de Terraform en Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** ClickOps se refiere a administrar la infraestructura mediante clics en la interfaz de la consola, lo cual es difícil de revisar, reproducir y auditar.

</details>

---
### Pregunta 12

En la metáfora del ganado vs. las mascotas (cattle vs. pets), los servidores tipo ganado se caracterizan por:

- A. Ajustes manuales únicos y nombres sentimentales
- B. Ser desechables y reemplazarse en lugar de recuperarse individualmente con cuidados
- C. Nunca escalar horizontalmente
- D. Ejecutarse siempre sin automatización

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El ganado es intercambiable y reemplazable; las mascotas se tratan como sistemas únicos y de larga vida.

</details>

---
### Pregunta 13

¿Cómo mejora IaC la reproducibilidad?

- A. Impidiendo para siempre todos los cambios de configuración
- B. Codificando las definiciones de los entornos para poder recrearlos de manera consistente
- C. Ocultando los detalles de la infraestructura a los desarrolladores
- D. Exigiendo que cada recurso se cree manualmente primero

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las definiciones codificadas permiten reconstruir los entornos de la misma manera entre equipos, regiones y en distintos momentos.

</details>

---
### Pregunta 14

¿Qué capacidad respalda la capacidad de auditoría en los flujos de trabajo de IaC?

- A. Eliminar commits antiguos de Git después del merge
- B. Historial de cambios bajo control de versiones con autoría y marcas de tiempo
- C. Deshabilitar los registros en las APIs de la nube
- D. Almacenar secretos en texto plano en el código

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El historial del VCS muestra quién cambió qué y cuándo, lo que respalda las auditorías y las revisiones de cumplimiento.

</details>

---
### Pregunta 15

GitOps en la administración de infraestructura normalmente significa:

- A. Usar Git como fuente de verdad y ejecutar los despliegues a partir de cambios aprobados
- B. Evitar cualquier automatización en los pipelines de despliegue
- C. Almacenar solo imágenes binarias en Git sin configuración
- D. Prohibir los pull requests para el código de infraestructura

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** GitOps usa los flujos de trabajo de Git (PRs, merges) como plano de control del estado deseado del sistema, a menudo con conciliación automatizada.

</details>

---
### Pregunta 16

¿Qué afirmación sobre el IaC declarativo es VERDADERA?

- A. Se debe programar cada llamada a la API en orden
- B. La herramienta compara el estado deseado con el estado real y planifica los cambios
- C. Las herramientas declarativas no pueden destruir recursos
- D. Las configuraciones declarativas no pueden usar variables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las herramientas declarativas concilian el estado deseado con el real; el plan de Terraform muestra la diferencia propuesta.

</details>

---
### Pregunta 17

Un equipo aplica dos veces la misma configuración de Terraform sin cambios de código ni externos. ¿Cuál es el resultado esperado?

- A. Todos los recursos se destruyen en la segunda ejecución
- B. No se requieren cambios en la segunda ejecución
- C. Se crea un nuevo archivo de state cada vez con IDs de recursos diferentes
- D. Terraform se niega a ejecutarse una segunda vez

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El comportamiento idempotente significa que un segundo apply sin drift no debe producir cambios.

</details>

---
### Pregunta 18

¿Por qué un cambio manual en la consola es un riesgo para los entornos administrados con IaC?

- A. Actualiza automáticamente las versiones de Terraform
- B. Puede introducir drift que el siguiente plan/apply podría sobrescribir o con el que podría entrar en conflicto
- C. Impide que se carguen los plugins de provider
- D. Fuerza la eliminación inmediata de todos los recursos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los cambios manuales causan drift; la siguiente ejecución de Terraform puede revertir esos cambios o entrar en conflicto con ellos, según las reglas de lifecycle.

</details>

---
### Pregunta 19

¿Cuál NO es un beneficio típico de IaC?

- A. Aprovisionamiento de entornos más rápido y repetible
- B. Revisión por pares de los cambios de infraestructura
- C. Inmunidad garantizada contra errores de configuración
- D. Documentación que se mantiene cercana a la configuración real

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: C**

**Explicación:** IaC reduce los errores pero no garantiza configuraciones perfectas; las revisiones y las pruebas siguen siendo necesarias.

</details>

---
### Pregunta 20

¿Qué afirmaciones sobre los enfoques declarativo vs. imperativo son correctas? (Seleccione todas las que correspondan.)

- A. Las configuraciones declarativas describen el estado final deseado
- B. Los scripts imperativos se centran en la secuencia de acciones
- C. El modelo principal de Terraform es imperativo
- D. Las herramientas declarativas aún pueden realizar operaciones ordenadas internamente
- E. Las herramientas imperativas no pueden usar bucles

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Lo declarativo describe resultados; lo imperativo describe pasos. Terraform es declarativo, aunque internamente ejecuta operaciones ordenadas. Las herramientas imperativas sí pueden usar bucles.

</details>

---
### Pregunta 21

Que Terraform sea de código abierto significa que:

- A. Todos los recursos de nube que crea son gratuitos
- B. Su código fuente está disponible públicamente bajo una licencia de código abierto
- C. Solo puede administrar pilas de software de código abierto
- D. No requiere plugins de provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El código abierto se refiere a la disponibilidad del código del proyecto Terraform, no a la facturación de la nube ni a los requisitos de los providers.

</details>

---
### Pregunta 22

¿Qué práctica ayuda a reducir el configuration drift?

- A. Hacer cambios en producción solo desde la consola por rapidez
- B. Tratar el repositorio de IaC como la fuente de verdad y evitar ediciones no administradas
- C. Deshabilitar terraform plan en CI
- D. Almacenar el state solo en laptops individuales

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Establecer el código como fuente de verdad y revisar los cambios limita el drift no administrado.

</details>

---
### Pregunta 23

La infraestructura inmutable se combina bien con IaC porque:

- A. Los servidores nunca necesitan reemplazo
- B. Se pueden aprovisionar nuevas instancias a partir de la misma definición en lugar de aplicar parches directamente
- C. Elimina la necesidad de state
- D. No requiere probar las imágenes

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** IaC define cómo se construyen las nuevas instancias; la inmutabilidad reemplaza las instancias existentes en lugar de mutarlas.

</details>

---
### Pregunta 24

¿Qué papel desempeña la automatización en IaC?

- A. Elimina la necesidad de archivos de configuración
- B. Ejecuta los cambios de infraestructura definidos de manera consistente y sin pasos manuales
- C. Evita todo el tiempo de inactividad durante las actualizaciones
- D. Reemplaza los sistemas de control de versiones

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La automatización aplica los cambios codificados de manera confiable; el VCS y los procesos de revisión siguen siendo importantes.

</details>

---
### Pregunta 25

¿Qué ejemplo muestra mejor la reutilización en IaC?

- A. Copiar y pegar capturas de pantalla de la consola en tickets
- B. Usar el mismo module o patrón para dev, staging y prod con distintas variables
- C. Crear cada entorno desde cero sin código compartido
- D. Documentar los servidores solo en hojas de cálculo

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los modules parametrizados y los patrones compartidos permiten la reutilización entre entornos.

</details>

---
### Pregunta 26

¿Por qué los auditores podrían preferir IaC sobre ClickOps?

- A. IaC oculta todo el historial de cambios
- B. Los cambios de IaC son rastreables en el control de versiones y en los pipelines
- C. IaC elimina la necesidad de controles de acceso
- D. IaC impide cualquier cambio en producción

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los commits rastreables y los registros de los pipelines sirven como evidencia de auditoría; ClickOps carece de registros de cambios estructurados.

</details>

---
### Pregunta 27

El modelo declarativo de Terraform implica que los profesionales se centran en:

- A. Escribir bucles de bash para cada endpoint de API
- B. Bloques de recursos que describen los atributos deseados
- C. Instalar agentes en cada VM antes de aprovisionar
- D. Compilar HCL únicamente en plantillas ARM

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los profesionales declaran recursos y atributos en HCL; Terraform se encarga de las interacciones con los providers.

</details>

---
### Pregunta 28

La idempotencia ayuda a los equipos de operaciones porque:

- A. Los apply fallidos nunca requieren investigación
- B. Volver a ejecutar la configuración tras un fallo parcial puede converger de forma segura al estado deseado
- C. Garantiza que los recursos no cuesten nada
- D. Elimina el orden de dependencias

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las herramientas idempotentes pueden reintentar o volver a aplicar con seguridad para alcanzar el estado final definido.

</details>

---
### Pregunta 29

El configuration drift se detecta con MAYOR probabilidad cuando:

- A. terraform validate falla por sintaxis
- B. terraform plan muestra cambios inesperados con un código sin modificaciones
- C. terraform fmt reformatea archivos
- D. terraform version imprime la versión de la CLI

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Plan compara el estado deseado (código + state) con la infraestructura real; el drift aparece como diferencias inesperadas.

</details>

---
### Pregunta 30

¿Cuáles son características del modelo de mascotas (pets) de la infraestructura? (Seleccione todas las que correspondan.)

- A. Los servidores se tratan como únicos e irremplazables
- B. La intervención manual es común para la recuperación
- C. Los servidores se numeran y se descartan como el ganado
- D. Fuerte apego emocional u operativo a los hosts individuales
- E. Escalado horizontal con instancias idénticas y desechables

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** Las mascotas son únicas, se cuidan manualmente y son difíciles de reemplazar. El modelo de ganado implica instancias desechables, numeradas y escaladas.

</details>

---
### Pregunta 31

GitOps complementa a IaC al:

- A. Reemplazar la necesidad de cualquier lenguaje de IaC
- B. Usar flujos de trabajo de Git para proponer, revisar y fusionar cambios de infraestructura
- C. Prohibir los apply automatizados
- D. Almacenar credenciales de la nube en commits de Git

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** GitOps aplica las prácticas de entrega de software (PRs, merges) a las definiciones de infraestructura.

</details>

---
### Pregunta 32

¿Qué afirmación sobre la consistencia entre entornos es VERDADERA para IaC?

- A. Código idéntico con distintos valores de variables aún puede producir entornos apropiadamente diferentes
- B. Todos los entornos deben usar exactamente los mismos valores de variables
- C. IaC no puede admitir múltiples entornos
- D. Consistencia significa que cada recurso debe tener el mismo nombre en prod y en dev

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El código compartido con variables específicas de cada entorno permite tener patrones consistentes con diferencias intencionales.

</details>

---
### Pregunta 33

Un error común es creer que IaC elimina por completo el trabajo de operaciones. ¿Qué es más preciso?

- A. IaC desplaza el trabajo hacia definir, revisar y gobernar la infraestructura como código
- B. IaC significa que nadie monitorea producción
- C. IaC elimina la necesidad de prácticas de seguridad
- D. IaC solo funciona en centros de datos locales (on-premises)

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** IaC automatiza el aprovisionamiento, pero aún requiere diseño, pruebas, monitoreo y gobernanza.

</details>

---
### Pregunta 34

HashiCorp Terraform se utiliza principalmente para:

- A. Solo pruebas unitarias a nivel de aplicación
- B. Aprovisionamiento y administración del ciclo de vida de la infraestructura
- C. Empaquetado de software de escritorio
- D. Solo optimización de consultas de bases de datos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform aprovisiona y administra recursos de infraestructura mediante providers.

</details>

---
### Pregunta 35

¿Por qué se considera que el control de versiones es fundamental para IaC?

- A. Cifra el tráfico de la API de la nube
- B. Rastrea los cambios, permite la colaboración y respalda la reversión
- C. Descarga los plugins de provider automáticamente
- D. Reemplaza a terraform init

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El VCS es esencial para la administración colaborativa y auditable del código de infraestructura.

</details>

---
### Pregunta 36

La configuración declarativa suele ser más fácil de razonar porque:

- A. Oculta todas las dependencias entre recursos
- B. Establece los resultados en lugar de cada paso de bajo nivel
- C. No puede expresar actualizaciones de recursos existentes
- D. No requiere seguimiento del state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Describir el estado deseado suele ser más claro que mantener secuencias de comandos imperativos.

</details>

---
### Pregunta 37

Cuando la infraestructura es inmutable, la aplicación de parches de seguridad en un servidor a menudo significa:

- A. Editar paquetes directamente solo en la instancia en ejecución
- B. Construir una nueva imagen/instancia y reemplazar la anterior
- C. Deshabilitar todas las actualizaciones para evitar cambios
- D. Quitar el servidor únicamente del state de Terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los patrones inmutables despliegan nuevas versiones en lugar de mutar directamente los sistemas en ejecución.

</details>

---
### Pregunta 38

ClickOps se considera un antipatrón principalmente porque:

- A. Usa demasiada automatización
- B. Carece de la reproducibilidad y la revisión por pares propias de los flujos de trabajo codificados
- C. Requiere conocimientos de HCL
- D. Obliga a realizar despliegues multinube

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los cambios realizados solo desde la consola son difíciles de reproducir, revisar y auditar en comparación con los flujos de trabajo basados en código.

</details>

---
### Pregunta 39

La reproducibilidad en la recuperación ante desastres se ve favorecida por IaC porque:

- A. Nunca se necesitan copias de seguridad
- B. La infraestructura puede recrearse a partir de las definiciones almacenadas
- C. Los proveedores de nube deshabilitan la recuperación manual
- D. Los archivos de state siempre son públicos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las definiciones codificadas junto con el state permiten reconstruir la infraestructura después de incidentes.

</details>

---
### Pregunta 40

¿Qué actividad del equipo se alinea con los requisitos de auditabilidad de IaC?

- A. Fusionar cambios de infraestructura sin revisión
- B. Exigir la aprobación de pull requests para los modules de producción
- C. Eliminar el state de Terraform después de cada apply
- D. Compartir las claves raíz de la nube en el chat

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las aprobaciones de PR crean un rastro auditable de los cambios de infraestructura revisados.

</details>

---
### Pregunta 41

¿Qué elementos son ejemplos de configuration drift? (Seleccione todas las que correspondan.)

- A. Una regla de grupo de seguridad agregada manualmente en la consola
- B. Una etiqueta (tag) modificada fuera de Terraform después del último apply
- C. Ejecutar terraform fmt en archivos sin formato
- D. Un tipo de instancia modificado directamente en la interfaz de la nube
- E. Actualizar HCL y ejecutar terraform plan

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** El drift es cuando la infraestructura real difiere del código/state. fmt y planificar cambios de código son pasos normales del flujo de trabajo, no drift.

</details>

---
### Pregunta 42

La 'automatización' de IaC reduce más directamente:

- A. La necesidad de tomar decisiones de arquitectura
- B. Los pasos repetitivos de aprovisionamiento manual
- C. El costo de todos los servicios de la nube a cero
- D. El requisito de autenticación del provider

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La automatización se encarga del aprovisionamiento repetitivo; la arquitectura y las credenciales siguen siendo necesarias.

</details>

---
### Pregunta 43

Que Terraform sea de código abierto permite a las organizaciones:

- A. Evitar el uso de cualquier soporte o producto comercial
- B. Inspeccionar, contribuir y adoptar la herramienta sin dependencia propietaria (lock-in) a nivel de la herramienta
- C. Omitir las restricciones de versión de los providers
- D. Ejecutar Terraform sin un backend de state

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El código abierto permite transparencia y contribución de la comunidad; las organizaciones aún pueden usar las ofertas empresariales.

</details>

---
### Pregunta 44

En la automatización imperativa, la idempotencia suele ser:

- A. Automática para cada script
- B. Más difícil de garantizar sin verificaciones explícitas en cada paso
- C. Imposible por definición
- D. Solo disponible en herramientas declarativas

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los scripts imperativos a menudo deben incluir lógica condicional para evitar efectos secundarios duplicados.

</details>

---
### Pregunta 45

El modelo de ganado (cattle) fomenta:

- A. Servidores snowflake con configuraciones manuales únicas
- B. Tratar las instancias como intercambiables y reemplazarlas ante una falla
- C. Nunca usar grupos de autoescalado
- D. Evitar las definiciones de infraestructura en código

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La infraestructura tipo ganado es desechable y uniforme, lo que permite escalar y recuperarse fácilmente.

</details>

---
### Pregunta 46

Los flujos de trabajo de Terraform basados en GitOps suelen activar los apply desde:

- A. Laptops locales aleatorias sin revisión
- B. Pipelines de CI/CD tras cambios fusionados en ramas rastreadas
- C. Tickets de cambio realizados solo desde la consola
- D. Adjuntos de correo electrónico sin control de versiones

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El código revisado y fusionado en Git suele activar pipelines automatizados de plan/apply.

</details>

---
### Pregunta 47

¿Qué define mejor la Infraestructura como Código?

- A. Documentar los servidores en una hoja de cálculo después de crearlos
- B. Administrar la infraestructura mediante configuración versionada y legible por máquina
- C. Usar únicamente diagramas de red gráficos
- D. Ejecutar comandos de CLI ad hoc sin guardarlos

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** IaC trata de definiciones de infraestructura codificadas y versionadas, no de documentación posterior a los hechos.

</details>

---
### Pregunta 48

Un beneficio de la consistencia en IaC es:

- A. Dev y prod pueden seguir los mismos patrones, lo que reduce las sorpresas de "en mi máquina funciona"
- B. Todos los entornos deben compartir un único archivo de state
- C. No se permiten variables
- D. Los providers no pueden configurarse por entorno

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** Los patrones compartidos con entradas específicas de cada entorno mejoran la consistencia sin ser idénticos en cada detalle.

</details>

---
### Pregunta 49

¿Por qué se favorece la inmutabilidad en las operaciones cloud-native?

- A. Fomenta la edición de servidores de producción en ejecución
- B. Reduce el estado impredecible acumulado por los cambios realizados directamente en los servidores
- C. Elimina la necesidad de despliegues
- D. Impide el escalado horizontal

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Reemplazar instancias evita mutaciones difíciles de rastrear en servidores de larga vida.

</details>

---
### Pregunta 50

Los registros de auditoría de la infraestructura son más débiles cuando los equipos dependen de:

- A. Modules de Terraform respaldados por Git con registros de CI
- B. Cambios en la consola sin documentar realizados por varios administradores
- C. Versiones etiquetadas del código de infraestructura
- D. Solicitudes de cambio aprobadas vinculadas a commits

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** El trabajo no documentado en la consola carece de un historial de cambios centralizado y con capacidad de búsqueda.

</details>

---
### Pregunta 51

¿Qué prácticas se alinean con los principios de GitOps para la infraestructura? (Seleccione todas las que correspondan.)

- A. El repositorio de Git como fuente de verdad del estado deseado
- B. Pull requests para los cambios de infraestructura
- C. Ediciones directas en la consola de producción como flujo de trabajo principal
- D. Conciliación o despliegue automatizado a partir de merges aprobados
- E. Almacenar terraform.tfstate en un repositorio público de Git sin protección

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D**

**Explicación:** GitOps usa Git como fuente de verdad, revisiones mediante PR y despliegue automatizado. Las ediciones priorizando la consola y subir el state sin protección a un commit violan las mejores prácticas.

</details>

---
### Pregunta 52

La relación de Terraform con HashiCorp significa que:

- A. Terraform solo funciona con HashiCorp Cloud Platform
- B. Terraform es un producto de HashiCorp con un ecosistema de providers y ofertas empresariales
- C. Terraform no puede usarse sin una licencia de HashiCorp en todos los casos
- D. Terraform no tiene relación con los productos comerciales de HashiCorp

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Terraform es desarrollado por HashiCorp; la CLI principal es de código abierto, con plataformas comerciales opcionales.

</details>

---
### Pregunta 53

La idempotencia NO significa que:

- A. Las ejecuciones repetidas son seguras cuando la configuración no cambia
- B. La herramienta nunca devolverá errores
- C. El estado final coincide con la configuración declarada
- D. Se evitan los cambios innecesarios cuando ya se alcanzó la convergencia

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** La idempotencia se refiere a la consistencia del resultado, no a una ejecución libre de errores en todos los escenarios de falla.

</details>

---
### Pregunta 54

Al comparar IaC con las operaciones manuales, reutilización significa que:

- A. Cada proyecto debe duplicar todo el código sin compartir nada
- B. Los modules y patrones pueden compartirse entre equipos y proyectos
- C. Solo puede usarse una región de nube
- D. Los asistentes de la consola almacenan automáticamente plantillas reutilizables

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Los modules y patrones reutilizables son una ventaja central de IaC frente a las configuraciones manuales de un solo uso.

</details>

---
### Pregunta 55

El configuration drift puede hacer que terraform plan muestre:

- A. Ninguna salida jamás
- B. Actualizaciones o reemplazos para realinear la infraestructura con el código
- C. Solo mensajes de descarga de providers
- D. Cambios automáticos de terraform fmt

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Plan propone cambios para corregir las diferencias entre la infraestructura real y la configuración deseada.

</details>

---
### Pregunta 56

Las herramientas de IaC declarativas aún exigen que los profesionales comprendan:

- A. Nada sobre los servicios de nube
- B. Las dependencias entre recursos, el comportamiento de los providers y las implicaciones del ciclo de vida
- C. Solo herramientas de diseño gráfico
- D. Cómo conectarse manualmente por SSH a cada recurso

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Declarativo no significa magia; el modelado correcto y las dependencias siguen importando.

</details>

---
### Pregunta 57

La naturaleza de código abierto de Terraform afecta principalmente a:

- A. La disponibilidad y el desarrollo comunitario de la CLI principal
- B. Si AWS cobra por EC2
- C. El uso obligatorio de un proveedor específico de backend de state
- D. La eliminación de toda autenticación de providers

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** El código abierto rige el proyecto principal de Terraform; la facturación de la nube y la autenticación son aspectos independientes.

</details>

---
### Pregunta 58

ClickOps se opone MÁS directamente a:

- A. Cambios de infraestructura revisados por pares y bajo control de versiones
- B. Usar providers para múltiples nubes
- C. Almacenar salidas en terraform outputs
- D. Ejecutar terraform validate localmente

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: A**

**Explicación:** ClickOps omite los flujos de trabajo codificados y revisables que promueve IaC.

</details>

---
### Pregunta 59

La infraestructura inmutable e IaC en conjunto respaldan:

- A. Servidores de producción snowflake
- B. Compilaciones repetibles y despliegues controlados mediante nuevas instancias
- C. Evitar toda la gestión de cambios
- D. Eliminar el state de Terraform

<details>
<summary>Ver respuesta</summary>

**Respuesta correcta: B**

**Explicación:** Las compilaciones codificadas junto con las actualizaciones basadas en reemplazo permiten despliegues controlados y repetibles.

</details>

---
### Pregunta 60

¿Cuáles son beneficios válidos de IaC que se destacan en el examen Terraform Associate? (Seleccione todas las que correspondan.)

- A. Integración con control de versiones
- B. Automatización del aprovisionamiento
- C. Cero incidentes de seguridad garantizados
- D. Consistencia entre entornos
- E. Reutilización mediante modules y patrones

<details>
<summary>Ver respuesta</summary>

**Respuestas correctas: A, B, D, E**

**Explicación:** El control de versiones, la automatización, la consistencia y la reutilización son beneficios centrales de IaC. Ninguna herramienta garantiza cero incidentes de seguridad.

</details>

---
