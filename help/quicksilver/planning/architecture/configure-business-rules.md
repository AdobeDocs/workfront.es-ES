---
title: Configurar reglas de negocio de tipo de registro
description: Puede configurar reglas empresariales de tipo de registro que definan cómo se administran los registros de ese tipo en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 31db7a4ef190793558bcb2fa10beb2585e1068e4
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 2%

---


# Configurar reglas empresariales de tipo de registro

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Puede configurar reglas empresariales de tipo de registro que definan cómo se administran los registros de ese tipo en Adobe Workfront Planning.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para realizar los pasos de este artículo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p></li>
O
<li><p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar de planificación</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo y en un tipo de registro</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al configurar reglas empresariales

* Puede configurar reglas para cuándo se pueden editar o eliminar los registros, según las condiciones que defina.

  Por ejemplo, puede crear condiciones para requerir que ciertos campos tengan un valor. Si falta el valor en esos campos, los usuarios no pueden editar ni eliminar ese registro.
* No se pueden agregar reglas de negocio a los tipos de registro global en sus espacios de trabajo primarios o secundarios.
* No se pueden configurar reglas para cuándo se crean los registros. Todas las personas con permisos de administración en el tipo de registro pueden crear registros.
* Puede crear una condición para la regla de negocio que haga referencia a todos los tipos de campo excepto a los siguientes:
  * Campos de fórmula
  * Campos de búsqueda
  * Campos de referencia

## Configurar reglas empresariales

1. Vaya a un tipo de registro.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro y, a continuación, haga clic en Reglas de negocio.


**&#x200B;**&#x200B;**&#x200B;**&#x200B;*** DE CLAUDE - MÁS ABAJO - DEBE EDITAR &#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;***

## Configuración de reglas de negocio en Workfront Planning: Guía paso a paso

¿Ha cambiado un registro a &quot;Listo para la ejecución&quot; solo para averiguar más tarde que la mitad de los campos obligatorios (marca, indicación, fechas de lanzamiento) nunca se rellenaron? Para cuando alguien se da cuenta, ya hay un proyecto descendente con datos que faltan, y alguien tiene que rastrear los detalles y rellenarlos a mano.

Las reglas empresariales lo arreglan. Permiten configurar un punto de comprobación simple: **antes de que un registro pueda pasar a un estado específico, se deben rellenar ciertos campos.** Si no lo están, la persona que realiza el cambio ve exactamente lo que falta y no puede continuar hasta que se corrija.

Esta guía explica qué hacen las reglas empresariales, cómo configurarlas y qué experimentará su equipo una vez que se publique.

### Qué hacen realmente las reglas empresariales

Las reglas de negocio adjuntan una condición a un **cambio de estado**. En lugar de aplicar datos completos en el momento en que alguien crea un registro (lo que ralentizaría a todos), la regla solo se activa en un momento específico y deliberado: cuando un estado está a punto de cambiar a un estado que usted ha configurado.

Una regla tiene este aspecto en lenguaje sencillo:

> &quot;Antes de que un registro pueda pasar a **Listo para la ejecución**, el campo **Marca** debe tener un valor.&quot;

Si el campo está vacío, el cambio de estado se bloquea y la persona recibe un mensaje claro que le indica qué corregir. Una vez que lo rellenan e intentan de nuevo, el cambio se realiza.

Algunas cosas importantes: *no*:

* **No bloquea la creación de registros.** Las personas pueden crear un nuevo registro al instante y rellenarlo con el tiempo, exactamente como hoy.
* **No se rellena automáticamente nada ni cambia los estados automáticamente.** Una persona siempre tiene que hacer el cambio de estado ellos mismos.
* **No marca de forma retroactiva los registros antiguos.** Los registros que ya se encuentran en el estado de destino no se ven afectados; la comprobación solo se ejecuta la próxima vez que alguien intente mover un registro *a* ese estado.



### Antes de comenzar

Para poder configurar las reglas, hay que cumplir un par de cosas:

1. **Debe activarse la característica para su organización.** Esto se realiza del lado de Adobe (a través de un indicador de funcionalidad), no de algo que se haya habilitado a sí mismo. Si no ve la sección de reglas empresariales que se describe a continuación, póngase en contacto con su contacto de Adobe para confirmar que se ha habilitado para su inquilino.
2. **Necesita permisos de administrador o configurador de área de trabajo.** Los planificadores habituales no pueden crear ni editar reglas; sólo las personas que gestionan la configuración del espacio de trabajo pueden hacerlo.

### Paso 1: Abrir el área de configuración de reglas empresariales

Las reglas empresariales se aplican junto con la configuración del otro administrador; no es necesario que busque un panel &quot;Planificación&quot; independiente. Desde el área de configuración del flujo de trabajo:

1. Vaya al área principal **configuración del flujo de trabajo / configuración de administración** para su área de trabajo.
2. Busque la sección **reglas de negocio** para el tipo de registro que desea configurar (por ejemplo, &quot;Materiales&quot; o &quot;Campañas&quot;).


### Paso 2: Elija el tipo de registro

Las reglas se configuran por tipo de registro, por lo que debe elegir el tipo al que desee agregar una regla. Por ejemplo, si desea asegurarse de que todos los registros de materiales tienen campos clave rellenados antes de la ejecución, seleccione **Materiales**.



### Paso 3: Crear una regla nueva

Para cada regla, debe especificar tres cosas:

| Lo que ha configurado | Ejemplo |
|---|---|
| **Tipo de registro** | Materiales |
| **Estado de destino** | Listo para la ejecución |
| **Campo obligatorio** | Marca |

En otras palabras: &quot;Cuando el estado de un registro de materiales se cambia a **Listo para ejecución**, el campo **Marca** debe tener un valor&quot;.

Puede agregar más de una regla para el mismo estado. Por ejemplo, es posible que necesite que la marca, el área terapéutica, la indicación y la fecha estimada de inicio se rellenen antes de que un registro pueda pasar a &quot;Listo para la ejecución&quot;; cada uno es su propia regla y todos se comprueban juntos.

**¿Qué campos puede requerir?**
&#x200B;- Campos de registro conectados (por ejemplo, un registro vinculado de marca o indicación): la regla se aprueba en cuanto se vincula al menos un registro.
&#x200B;- Campos de texto estándar (una sola línea o párrafo): la regla se pasa una vez que haya algún valor.
&#x200B;- Campos de fecha: la regla se pasa una vez que se ha establecido una fecha.

**Lo que aún no puede usar:** los campos de fórmula y los campos de búsqueda no se admiten como destinos de regla en esta versión, ya que se calculan en segundo plano en lugar de ser rellenados directamente por una persona.

### Paso 4: Escriba el mensaje que verán los usuarios

Al crear una regla, también debe proporcionar el mensaje que se muestra si alguien intenta realizar el cambio sin haber rellenado el campo. Manténgalo específico y procesable, algo así como:

> &quot;Se requiere una marca&quot;.

No es necesario preocuparse por formatear un banner de error completo: el sistema gestiona los mensajes combinados si se infringen varias reglas a la vez (consulte a continuación).

### Paso 5: Guardar la regla

Una vez guardada, la regla se aplicará **inmediatamente** a todos los usuarios del área de trabajo, sin necesidad de cerrar la sesión, actualizar o esperar a una implementación. La próxima vez que alguien intente mover un registro a ese estado, se comprueba la regla.

### Lo que realmente experimentará su equipo

Esto es lo que cambia para las personas que utilizan Planning día a día, una vez que una regla está activa.

#### Si un campo obligatorio está vacío

1. Un planificador abre un registro y cambia el estado al estado cerrado (por ejemplo, &quot;Listo para ejecución&quot;).
2. El sistema comprueba todas las reglas vinculadas a ese estado.
3. Si un campo obligatorio está vacío, el cambio es **rechazado** — el estado vuelve a ser el que era.
4. Aparece un mensaje de mensaje emergente que indica exactamente los campos que faltan:
   > *&quot;Cambio de estado bloqueado: &#39;Marca&#39; y &#39;Fecha de inicio estimada&#39; deben rellenarse antes de pasar a &#39;Listo para ejecución&#39;&quot;*
5. El planificador rellena los campos que faltan e intenta el cambio de estado de nuevo.
6. Esta vez, la regla se aprueba y el estado se actualiza normalmente.

#### Si todo está ya rellenado

Nada cambia. El estado se actualiza instantáneamente sin pasos ni ventanas emergentes adicionales. Las reglas empresariales son invisibles hasta que realmente se necesitan.

#### Si faltan varios campos a la vez

Todas las reglas infringidas se comprueban juntas y el mensaje enumera todos los campos que faltan de una sola vez: los planificadores no tienen que corregir un campo, intentarlo de nuevo, recibir información sobre el siguiente y repetir.

### Paso 6: Editar o eliminar una regla más adelante

Las reglas no se establecen en piedra. Para realizar cambios:

1. Vuelva al área de configuración de reglas empresariales para el tipo de registro.
2. Busque la regla que desee cambiar.
3. Edite el campo, el estado de destino o el mensaje necesarios, o bien elimine la regla por completo.
4. Guardar. El cambio se aplica inmediatamente a los cambios de estado futuros.

Tenga en cuenta: editar o eliminar una regla **solo afecta a las transiciones a partir de ahora.** Los registros que ya pasaron al estado de destino antes del cambio no se vuelven a evaluar.
3## Algunas cosas que vale la pena conocer

* **Esto es independiente del bloqueo de registros después de un cambio de estado.** Las reglas de negocio (como se describe aquí) solo comprueban la integridad del campo *antes de* que se realice un cambio de estado. Una función relacionada diferente rige si un registro queda totalmente bloqueado frente a ediciones/eliminación una vez que alcanza un estado determinado; eso no es lo que se trata aquí.
* **Los cambios de estado masivos** (que cambian el estado de muchos registros a la vez) aún no están completamente definidos para la forma en que interactúan con las reglas de negocio; si su equipo depende en gran medida de las acciones masivas, consulte con su contacto de Adobe el comportamiento actual.
* **Si una regla no se puede evaluar** debido a un error del sistema, la transición se bloqueará en lugar de permitirse sin aviso; nunca terminará con un registro incompleto que se deslice más allá de una regla debido a un problema con el servidor.
* **Al desactivar la característica**, no se eliminan las reglas configuradas, simplemente se ponen en pausa. Si se vuelve a activar, se restauran exactamente como estaban, no es necesario realizar ninguna reconfiguración.

### Referencia rápida: configuración de la primera regla

1. Confirme que la función esté habilitada para su inquilino.
2. Vaya a la configuración del flujo de trabajo → las reglas empresariales del tipo de registro.
3. Elija el tipo de registro (por ejemplo, Materiales).
4. Crear una regla: estado de destinatario + campo obligatorio.
5. Escriba un mensaje de error claro y específico.
6. Guardar... está activo inmediatamente.
7. Repita el proceso para cada campo que desee requerir.
8. Pruébelo usted mismo: intente cambiar el estado de un registro con el campo vacío, confirme que ve el mensaje esperado, rellene el campo y confirme que el cambio de estado se produce.

Eso es todo. A partir de ahora, cualquiera que convierta un registro hacia adelante recibirá un claro empujón si falta algo, en lugar de un proyecto que siga apareciendo silenciosamente incompleto.