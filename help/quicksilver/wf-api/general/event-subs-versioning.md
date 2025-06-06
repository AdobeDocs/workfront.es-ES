---
content-type: api
navigation-topic: general-api
title: Versiones de suscripción de evento
description: API de suscripción a eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: f34f48d974db200d9ce1815c805885707ab27f6d
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 1%

---

# Versiones de suscripción de evento

Workfront tiene dos versiones de suscripciones a eventos. Este artículo describe las diferencias entre ellos.

La nueva versión no es un cambio en la API de Workfront, sino un cambio en la funcionalidad de suscripción de evento.

La capacidad de actualizar o reducir las suscripciones a eventos garantiza que, cuando se realicen cambios en la estructura de los eventos, las suscripciones existentes no se rompan, lo que le permite probar y actualizar a la nueva versión sin interrupciones en la suscripción de evento.


Al actualizar o reducir la suscripción de evento a otra versión, se reciben eventos duplicados para cada entrega de evento durante un periodo de cinco minutos después del cambio de versión. Los duplicados incluyen una de cada versión de suscripción de evento 1 y una versión 2. Esto garantiza que no se pierda ningún evento debido al cambio de la versión de suscripción del evento.

Para obtener información sobre los extremos utilizados para actualizar o degradar suscripciones de evento, consulte [Control de versiones de suscripciones de evento](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) en el artículo API de suscripción de evento.

>[!IMPORTANT]
>
>Las siguientes versiones afectarán al control de versiones de suscripciones a eventos:
>
>* **Versión 25.2** (10 de abril de 2025): todas las suscripciones nuevas creadas después de la versión 25.2 se crean como Versión 2.
>* **15 de enero de 2026**: todas las suscripciones de la versión 1 restantes se migran a la versión 2.

## Cambios entre las versiones 1 y 2

Se han realizado los siguientes cambios para las suscripciones de evento Versión 2:


### Cambios generales


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Campos afectados</b></p> </th> 
   <th> <p><b>Versión 1 (comportamiento anterior)</b></p> </th> 
   <th> <p><b>Versión 2 (Cambiar)</b></p> </th> 
   <th> <p><b>Acción de corrección</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Valores de parámetro calculados</p> </td> 
   <td> <p>Cualquier objeto creado a partir de una plantilla que incluya un formulario personalizado con valores de parámetros calculados, se enviará un evento <code>CREATE</code> y, a continuación, se enviará un <code>UPDATE</code> con los valores de los parámetros (incluidos los campos calculados y sus valores). </p> </td> 
   <td> <p>Cuando se crea un objeto a partir de una plantilla que incluye un formulario personalizado con valores de parámetros calculados, solo se envía un evento <code>CREATE</code> que contiene valores de parámetro, incluidos campos calculados.</p> </td> 
   <td> <p>Si tiene una suscripción para <code>UPDATE</code> eventos y espera recibir un evento <code>UPDATE</code> después de crear un objeto con valores de parámetros calculados, ya no recibirá ese evento <code>UPDATE</code>. Si desea ver los valores de parámetros calculados al crear el objeto, debe crear una suscripción adicional de <code>CREATE</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Campos de tipo de selección múltiple</p> </td> 
   <td> <p>Para cualquier tipo de evento que contenga un cambio en un campo de tipo de selección múltiple, si el campo solo contuviera un valor, se convertiría en y se enviaría como una cadena. De lo contrario, se enviaría como una matriz. </p><p>Ejemplos:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> se convierte y se envía como <code>myMultiSelectField: "oneValue"</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> se envía como <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Independientemente de cuántos valores haya en la matriz, se envía como una matriz. </p><p>Ejemplos:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> se envía como <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> se envía como <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Si tiene una suscripción con un filtro en un campo de selección múltiple y el valor como cadena, debe crear una nueva suscripción con el mismo filtro que tenga el valor como matriz. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Cambios específicos de objeto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>Código de objeto</b> </th> 
   <th> <b>Campos afectados</b> </th> 
   <th> <b>Versión 1 (comportamiento anterior)</b></th> 
   <th> <b>Versión 2 (Cambiar)</b> </th> 
   <th> <b>Acción de corrección</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizó este objeto, el evento <code>UPDATE</code> a veces mostraba incorrectamente el cambio de los campos afectados de <code>null</code> a <code>ID value</code>.</td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para los campos afectados.</td> 
   <td>Ninguno. Si tiene un filtro en los campos afectados, recibirá un evento <code>UPDATE</code> solo si estos campos han cambiado realmente, no si ha cambiado algún otro valor.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizaba cualquier valor de parámetro en este objeto, el evento <code>UPDATE</code> mostraba incorrectamente el cambio de campo afectado de <code>null</code> a <code>object id</code>. </td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para los campos afectados.</td> 
   <td>Ninguno. Si tiene un filtro en los campos afectados, recibirá un evento <code>UPDATE</code> solo si estos campos han cambiado realmente, no si ha cambiado algún otro valor.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>Cuando se eliminaba un documento, el evento <code>DELETE</code> mostraba incorrectamente el campo afectado como una matriz vacía en el estado antes.    </td> 
   <td>El evento <code>DELETE</code> muestra correctamente el campo afectado en el estado antes.</td> 
   <td>Ninguno. El evento <code>DELETE</code> se enviará, pero ahora mostrará los datos correctos para el campo afectado. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizara este objeto, se enviarían dos eventos <code>UPDATE</code>. El primero no incluyó los campos afectados, mientras que el segundo sí lo hizo.</td> 
   <td>Todas las actualizaciones de campo, incluidos los campos afectados, están presentes en un único evento <code>UPDATE</code> y no se envía un segundo evento innecesario.     </td> 
   <td>Ninguno. Si tiene un filtro en los campos afectados, los eventos se entregan en el primer evento. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizaba cualquier valor de parámetro en un Expense, el evento <code>UPDATE</code> mostraba incorrectamente el cambio topReferenceObjCode de <code>EXPNS</code> a <code>PROJ</code> y el cambio de <code>referenceObjectName</code> de <code>null</code> a <code>string value of project name</code>.      </td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para los campos afectados.</td> 
   <td>Ninguno. Si tiene un filtro en los campos afectados, recibirá un evento <code>UPDATE</code> solo si estos campos han cambiado realmente, no si ha cambiado algún otro valor.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Cuando se eliminó un objeto Expense, se envió un evento <code>UPDATE</code> cambiando los campos afectados a null antes de que se enviara el evento <code>DELETE</code>.    </td> 
   <td>No se envió el evento <code>UPDATE</code> adicional. El evento <code>DELETE</code> tiene valores correctos para los campos afectados en el estado antes. </td> 
   <td>Si tiene un filtro para los campos afectados en <code>UPDATE</code> eventos y espera recibirlo cuando se elimine el objeto, ya no recibirá ese evento <code>UPDATE</code>. Si desea ver estos campos cuando se elimine el objeto, debe crear una suscripción adicional de <code>DELETE</code>.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HOUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>Cuando se eliminó este objeto, el evento <code>DELETE</code> mostró incorrectamente los campos afectados como <code>null</code> en el estado antes. </td> 
   <td>El evento <code>DELETE</code> muestra correctamente los campos afectados en el estado antes.</td> 
   <td>Ninguno. El evento <code>DELETE</code> se sigue enviando, pero ahora muestra los datos correctos para los campos afectados. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizaba cualquier valor de parámetro en este objeto, el evento <code>UPDATE</code> mostraba incorrectamente el cambio de campo afectado de <code>null</code> a <code>ID value</code>. </td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para el campo afectado.</td> 
   <td>Ninguno. Si tiene un filtro en el campo afectado, recibirá un evento <code>UPDATE</code> solo si ese campo ha cambiado realmente, no si ha cambiado algún otro valor de parámetro.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizó este objeto, el evento <code>UPDATE</code> a veces mostraba incorrectamente el cambio de los campos afectados de <code>null</code> a <code>ID value</code>.</td> 
   <td>Todos los <code>UPDATE</code> eventos mostrarán el valor correcto para los campos afectados.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>Cuando se actualizaba cualquier valor de parámetro en este objeto, el evento <code>UPDATE</code> mostraba incorrectamente el cambio de campo afectado de <code>null</code> a <code>ID value</code>. </td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para el campo afectado.</td> 
   <td>Ninguno. Si tiene un filtro en el campo afectado, recibirá un evento <code>UPDATE</code> solo si ese campo ha cambiado realmente, no si ha cambiado algún otro valor de parámetro.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizó este objeto, el evento <code>UPDATE</code> a veces mostraba incorrectamente el cambio de los campos afectados de <code>null</code> a <code>ID value</code>.</td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para el campo afectado.</td> 
   <td>Ninguno. Si tiene un filtro en el campo afectado, recibirá un evento <code>UPDATE</code> solo si ese campo ha cambiado realmente, no si ha cambiado algún otro valor de parámetro.
  </tr> 
  <tr> 
   <th rowspan="2">TASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizaba cualquier valor de parámetro en este objeto, el evento <code>UPDATE</code> mostraba incorrectamente el cambio de campo afectado de <code>null</code> a <code>ID value</code>. </td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para el campo afectado.</td> 
   <td>Ninguno. Si tiene un filtro en el campo afectado, recibirá un evento <code>UPDATE</code> solo si ese campo ha cambiado realmente, no si ha cambiado algún otro valor de parámetro.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Cuando se actualizó este objeto, el evento <code>UPDATE</code> a veces mostraba incorrectamente el cambio de los campos afectados de <code>null</code> a <code>ID value</code>.</td> 
   <td>Todos los eventos <code>UPDATE</code> muestran el valor correcto para el campo afectado.</td> 
   <td>Ninguno. Si tiene un filtro en el campo afectado, recibirá un evento <code>UPDATE</code> solo si ese campo ha cambiado realmente, no si ha cambiado algún otro valor de parámetro.
 </tbody> 
</table>


## Actualización de la versión de suscripción del evento en un escenario de Workfront Fusion

Workfront Fusion utiliza suscripciones de eventos para inspeccionar los cambios en Workfront en los escenarios de déclencheur. Puede actualizar la versión de suscripción de evento que Fusion utiliza directamente en un escenario mediante el módulo Workfront > Actualizar versión de carga útil de eventos.

Para obtener instrucciones sobre el uso de este módulo, consulte [Módulos de Workfront](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules) en la documentación de Workfront Fusion.

Para obtener recursos sobre cómo preservar los escenarios de Workfront Fusion durante la actualización de la suscripción al evento, incluida una grabación del seminario web, consulte [Conservación de los escenarios de Fusion durante la actualización de las suscripciones a eventos V2](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/td-p/754182?profile.language=es).
