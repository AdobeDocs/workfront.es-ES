---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos GitLab
description: Adobe Workfront Fusion requiere una licencia Adobe Workfront Fusion además de una licencia Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '4070'
ht-degree: 0%

---


# Módulos [!UICONTROL GitLab]

Adobe Workfront Fusion requiere una licencia Adobe Workfront Fusion además de una licencia Adobe Workfront.

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que usan [!UICONTROL GitLab], así como conectarlo a varias aplicaciones y servicios de terceros.

>[!NOTE]
>
>Este artículo espera estar familiarizado con la documentación de la API y con la funcionalidad de [!DNL GitLab] en general.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Conectar [!DNL GitLab] a [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. En cualquier módulo de [!DNL Workfront Fusion] [!DNL Gitlab], haga clic en **[!UICONTROL Agregar]** junto al campo de conexión.
1. Configure los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de conexión]</td> 
      <td> <p>Introduzca un nombre para la conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Escriba la dirección URL de su instancia de [!DNL GitLab].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token de acceso]</td> 
      <td><p>Introduzca su [!UICONTROL Private Token] o [!UICONTROL Personal Access Token].</p><p>Para obtener información sobre cómo buscar o crear un token de acceso personal en [!DNL GitLab], consulte "Crear un token de acceso personal" en <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Tokens de acceso personal</a> en la documentación de [!DNL GitLab].</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Haga clic en **[!UICONTROL Continuar]**.
1. Haga clic en **[!UICONTROL Autorizar]** para crear la conexión y volver al módulo.

## [!DNL GitLab] módulos y sus campos

Al configurar [!DNL GitLab] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL GitLab] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheur

+++**[!UICONTROL Ver estado de compilación]**

Este módulo de déclencheur instantáneo inicia un escenario cuando cambia el estado de una compilación.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook inspeccione en busca de cambios de estado de compilación</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Observar comentarios de confirmación/MR/problema/fragmento]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se realiza un comentario en una confirmación, solicitud de combinación, problema o fragmento de código.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea para comentarios</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver confirmaciones (inserciones)]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se inserta una confirmación en un repositorio. Este módulo no inicia un escenario cuando se inserta una etiqueta.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea para confirmar</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver comentario del problema]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se realiza un comentario sobre un problema.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea para comentarios sobre problemas</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Problemas de observación]**

Este módulo de [!UICONTROL déclencheur instantáneo] inicia un escenario cuando se crea un problema o cuando se actualiza, cierra o reabre uno existente.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea por problemas</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver solicitudes de combinación]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se produce una de las siguientes situaciones:

* Se crea una nueva solicitud de combinación
* Se actualiza, fusiona o cierra una solicitud de combinación existente
* Se agrega una confirmación en la rama de origen


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea para solicitudes de combinación</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver comentarios de solicitud de combinación]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se realiza un comentario en una solicitud de combinación.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea para los comentarios de las solicitudes de combinación</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver estado de la canalización]**

Este módulo de déclencheur instantáneo inicia un escenario cuando cambia el estado de una canalización.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el gancho web observe si cambia el estado de la canalización</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver proyectos]**

Este módulo de déclencheur programado inicia un escenario cuando se agrega un nuevo proyecto del que es miembro el usuario autenticado.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL GitLab] a [!DNL Workfront] Fusion, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Conectar [!DNL GitLab] a [!DNL Workfront] Fusion</a> en este artículo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Resultados máximos</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo vea durante cada ciclo de ejecución de escenario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Observar ramas del repositorio]**

Este módulo de déclencheur programado inicia un escenario cuando se agrega una nueva rama a un repositorio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL GitLab] a [!DNL Workfront] Fusion, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Conectar [!DNL GitLab] a [!DNL Workfront] Fusion</a> en este artículo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Resultados máximos</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo vea durante cada ciclo de ejecución de escenario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver etiquetas de repositorio]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se crea o elimina una etiqueta en un repositorio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook inspeccione en busca de etiquetas</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Observar comentarios de fragmentos]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se realiza un nuevo comentario en un fragmento.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea para comentarios</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver todos]**

Este módulo de déclencheur programado inicia un escenario cuando se agrega una tarea pendiente nueva. Cuando no se aplica ningún filtro, el déclencheur se ejecuta cuando se agrega una nueva tarea pendiente.

Para obtener información sobre los campos, consulte [Obtener una lista de tareas pendientes](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Ver página wiki]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se crea o edita una página wiki.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Seleccione el webhook que desee utilizar para este déclencheur o agregue uno nuevo. </p><p>Para agregar un nuevo webhook, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL webhook].</li><li>Introduzca lo siguiente: <ul><li>Nombre del webhook</li><li>La conexión que desea utilizar para este webhook</li><li>El proyecto que desea que el webhook vea en busca de páginas wiki</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el webhook y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Acciones

+++**[!UICONTROL Aceptar solicitud de combinación]**

Este módulo de acción combina los cambios enviados con la solicitud de combinación determinada.

Para obtener información sobre los campos, consulte [Aceptar solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Cancelar una compilación]**

Este módulo de acción cancela una sola compilación de un proyecto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL GitLab] a [!DNL Workfront] Fusion, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Conectar [!DNL GitLab] a [!DNL Workfront] Fusion</a> en este artículo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto]</td> 
   <td> <p>Seleccione o asigne el proyecto que contiene la compilación que desea cancelar.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Id. de compilación]</td> 
   <td>Seleccione o asigne la compilación que desea cancelar.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Mensaje de confirmación de combinación]</td> 
   <td> Introduzca o asigne un mensaje de compromiso para la combinación.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Debe quitar la rama de origen]</td> 
   <td>Seleccione si desea quitar la rama de origen cuando se complete la combinación.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Combinar cuando la compilación se realiza correctamente]</td> 
   <td>Seleccione si desea combinar la solicitud de combinación en cuanto se complete la compilación.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>Si está presente, este SHA debe coincidir con el HEAD de la rama de origen. Si no coincide, la combinación falla.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Cancelar las compilaciones de una canalización]**

Este módulo de acción cancela las compilaciones de una sola canalización.

Para obtener información sobre los campos, consulte [Cancelar los trabajos de una canalización](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Cancelar combinación cuando la canalización se realice correctamente]**

Si una solicitud de combinación está configurada para combinarse cuando una canalización se realiza correctamente, este módulo de acción cancela esa acción.

Para obtener información sobre los campos, consulte [Cancelar la combinación cuando la canalización se realice correctamente](https://docs.gitlab.com/ee/api/merge_requests.html) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Cherry elige un compromiso]**

Este módulo de acción selecciona una confirmación para una rama determinada.

Para obtener información sobre los campos, consulte [Cherry elige un compromiso](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear una etiqueta nueva]**

Este módulo de acción crea una nueva etiqueta para el repositorio determinado.

Para obtener información sobre los campos, consulte [Crear una etiqueta nueva](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear una nueva canalización]**

Este módulo de acción crea una nueva canalización para el proyecto determinado.

Para obtener información sobre los campos, consulte [Crear una nueva canalización](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear nueva versión]**

Este módulo de acción añade notas de la versión a la etiqueta de Git existente.

Para obtener información sobre los campos, consulte [Crear una versión](https://docs.gitlab.com/ee/api/releases/#create-a-release) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear una etiqueta nueva]**

Este módulo de acción crea una nueva etiqueta en el repositorio que apunta a la referencia proporcionada.

Para obtener información sobre los campos, consulte [Crear una etiqueta nueva](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear un todo]**

Este módulo de acción crea una tarea para el usuario actual en el problema seleccionado. El usuario actual es el usuario identificado por las credenciales de la conexión utilizada para este módulo.

Para obtener información sobre los campos, consulte [Crear una tarea pendiente](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear una tarea en una solicitud de combinación]**

Este módulo de acción crea una tarea para el usuario actual en la solicitud de combinación seleccionada. El usuario actual es el usuario identificado por las credenciales de la conexión utilizada para este módulo.

Para obtener información sobre los campos, consulte [Crear una tarea pendiente](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear solicitud de combinación]**

Este módulo de acción crea una nueva solicitud de combinación en un proyecto.

Para obtener información sobre los campos, consulte [Crear solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear nuevo archivo en el repositorio]**

Este módulo de acción crea un nuevo archivo en el repositorio seleccionado.

Para obtener información sobre los campos, consulte [Crear nuevo archivo en el repositorio](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear nueva nota de problema]**

Este módulo de acción crea una nota de problema para un solo problema de proyecto.

Para obtener información sobre los campos, consulte [Crear nueva nota de problema](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear nueva nota de solicitud de combinación]**

Este módulo de acción crea una nota para una sola solicitud de combinación.

Para obtener información sobre los campos, consulte [Crear nueva nota de solicitud de combinación](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear un nuevo hito]**

Este módulo de acción crea un nuevo hito para un proyecto.

Para obtener información sobre los campos, consulte [Crear nuevo hito](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear nueva nota de fragmento]**

Este módulo de acción crea una nota nueva para un solo fragmento de código. Las notas de fragmento son comentarios que los usuarios pueden publicar en un fragmento.

Para obtener información sobre los campos, consulte [Crear nueva nota de fragmento](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear rama de repositorio]**

Este módulo de acción crea una sola rama del repositorio.

Para obtener información sobre los campos, consulte [Crear rama de repositorio](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Crear variable de compilación]**

Este módulo de acción crea una nueva variable de compilación.

Para obtener información sobre los campos, consulte [Crear variable](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Eliminar una solicitud de combinación]**

Este módulo de acción es solo para administradores y propietarios de proyectos. Elimina la solicitud de combinación en cuestión

Para obtener información sobre los campos, consulte [Eliminar una solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Eliminar archivo existente en el repositorio]**

Este módulo de acción elimina un archivo existente del repositorio.

Para obtener información sobre los campos, consulte [Eliminar archivo existente en el repositorio](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Eliminar rama del repositorio]**

Este módulo de acción elimina una rama del repositorio.

Para obtener información sobre los campos, consulte [Eliminar la rama del repositorio](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Editar problema]**

Este módulo de acción actualiza un problema existente del proyecto. Esta llamada también se utiliza para marcar un problema como cerrado.

Para obtener información sobre los campos, consulte [Editar problema](https://docs.gitlab.com/ee/api/issues.html#edit-issue) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Editar hito]**
Este módulo de acción actualiza un hito de proyecto existente.

Para obtener información sobre los campos, consulte [Editar hito](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Borrar una compilación]**

Este módulo de acción borra una compilación de un proyecto (elimina los artefactos de trabajo y el registro de trabajos).

Para obtener información sobre los campos, consulte [Borrar un trabajo](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener una lista de todos]**

Este módulo de búsqueda recupera una lista de elementos pendientes.

Para obtener información sobre los campos, consulte [Obtener una lista de tareas pendientes](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener una sola compilación]**

Este módulo de acción recupera un solo trabajo de un proyecto.

Para obtener información sobre los campos, consulte [Obtener un solo trabajo](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener una sola etiqueta de repositorio]**

Este módulo de acción recupera una etiqueta de repositorio específica determinada por su nombre.

Para obtener información sobre los campos, consulte [Obtener una sola etiqueta de repositorio](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener una implementación específica]**

Este módulo de acción recupera una implementación específica.

Para obtener información sobre los campos, consulte [Obtener una implementación específica](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener todos los problemas asignados a un solo hito]**

Este módulo de búsqueda recupera todos los problemas asignados a un solo hito de proyecto.

Para obtener información sobre los campos, consulte [Obtener todos los problemas asignados a un solo hito](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener archivo del repositorio]**

Este módulo de acción recupera información sobre un archivo del repositorio, como nombre, tamaño o contenido.

Para obtener información sobre los campos, consulte [Obtener archivo del repositorio](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener usuarios del proyecto]**

Este módulo de búsqueda recupera los usuarios del proyecto.

Para obtener información sobre los campos, consulte [Obtener usuarios del proyecto](https://docs.gitlab.com/ee/api/projects.html#get-project-users) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener un solo problema]**

Este módulo de acción recupera los detalles del problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para crear una nueva conexión, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Conectar [!DNL GitLab] a Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proyecto]</td> 
   <td> <p>Seleccione el proyecto que contiene el problema del que desea obtener detalles.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de problema]</td> 
   <td> <p>Escriba o asigne el nombre del problema del que desea obtener detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Obtener nota de un solo problema]**

Este módulo de acción recupera una sola nota para un problema específico del proyecto.

Para obtener información sobre los campos, consulte [Obtener nota sobre un solo problema](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener solicitud de combinación única]**

Este módulo de acción recupera información sobre una única solicitud de combinación.

Para obtener información sobre los campos, consulte [Obtener solicitud de combinación única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener cambios de solicitud de combinación única]**

Este módulo de búsqueda recupera información sobre la solicitud de combinación, incluidos sus archivos y cambios.

Para obtener información sobre los campos, consulte [Obtener cambios en una solicitud de combinación única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener confirmaciones de solicitud de combinación única]**

Este módulo de acción recupera una lista de confirmaciones de solicitudes de combinación.

Para obtener información sobre los campos, consulte [Obtener confirmaciones de solicitud de combinación única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener nota de solicitud de combinación única]**

Este módulo de acción devuelve una sola nota para una solicitud de combinación determinada.

Para obtener información sobre los campos, consulte [Obtener nota de solicitud de combinación única](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener un hito]**

Este módulo de acción recupera detalles del hito.

Para obtener información sobre los campos, consulte [Obtener un solo hito](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener un solo proyecto]**

Este módulo de acción recupera los detalles del proyecto.

Para obtener información sobre los campos, consulte [Obtener un solo proyecto](https://docs.gitlab.com/ee/api/projects.html#get-single-project) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener una sola rama del repositorio]**

Este módulo de acción recupera los detalles de la rama del repositorio.

Para obtener información sobre los campos, consulte [Obtener una sola rama del repositorio](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener nota de fragmento]**

Este módulo recupera una sola nota para un fragmento determinado.

Para obtener información sobre los campos, consulte [Obtener una sola nota de fragmento](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener los comentarios de una confirmación]**

Este módulo de búsqueda recupera los comentarios de una confirmación en un proyecto.

Para obtener información sobre los campos, consulte [Obtener los comentarios de una confirmación](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener la diferencia de una confirmación]**

Este módulo de acción obtiene la diferencia de una confirmación en un proyecto.

Para obtener información sobre los campos, consulte [Obtener la diferencia de una confirmación](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Conservar artefactos]**

Evita que se eliminen artefactos cuando se establece la caducidad.

Para obtener información sobre los campos, consulte [Conservar artefactos](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar todas las notas de solicitud de combinación]**

Este módulo de búsqueda recupera una lista de todas las notas de una única solicitud de combinación.

Para obtener información sobre los campos, consulte [Enumerar todas las notas de solicitudes de combinación](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar todas las notas de fragmentos]**

Este módulo obtiene una lista de todas las notas de un solo fragmento. Las notas de fragmento son comentarios que los usuarios pueden publicar en un fragmento.

Para obtener información sobre los campos, consulte [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar compilaciones de confirmación]**

Este módulo de búsqueda devuelve una lista de compilaciones para una confirmación específica en un proyecto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para crear una nueva conexión, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Conectar [!DNL GitLab] a Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto]</td> 
   <td> <p>Seleccione el proyecto que contiene la confirmación para la que desea enumerar las compilaciones.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ámbito]</td> 
   <td> Para limitar la búsqueda a fin de que se genere con un estado específico, seleccione el estado. Si se deja este campo en blanco, se devuelven todas las compilaciones de la confirmación.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Enumerar problemas]**

Este módulo de búsqueda devuelve todos los problemas según la configuración de filtro especificada.

Para obtener información sobre los campos, consulte [Enumerar problemas](https://docs.gitlab.com/ee/api/issues.html#list-issues) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar problemas que se cierran al combinar]**

Este módulo de búsqueda recupera todos los problemas que se cerrarían combinando la solicitud de combinación proporcionada.

Para obtener información sobre los campos, consulte [Problemas de lista que se cerrarán al combinar](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Etiquetas de lista]**

Este módulo de búsqueda recupera todas las etiquetas del proyecto.

Para obtener información sobre los campos, consulte [Etiquetas de lista](https://docs.gitlab.com/ee/api/labels.html#list-labels) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Solicitudes de combinación de lista]**

Este módulo de búsqueda recupera todas las solicitudes de combinación mediante la configuración del filtro.

Para obtener información sobre los campos, consulte [Solicitudes de combinación de listas](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Lista de proyectos en propiedad]**

Este módulo de búsqueda recupera proyectos en los que el usuario autenticado está establecido como propietario.

Para obtener información sobre los campos, consulte [Enumerar proyectos de usuarios](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar compilaciones de proyecto]**

Este módulo de búsqueda recupera una lista de compilaciones de un proyecto.

Para obtener información sobre los campos, consulte [Enumerar trabajos de proyecto](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar implementaciones de proyectos]**

Este módulo de búsqueda recupera una lista de implementaciones en un proyecto.

Para obtener información sobre los campos, consulte [Enumerar implementaciones de proyectos](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar notas de problemas de proyectos]**

Este módulo de búsqueda recupera una lista de todas las notas de un solo problema.

Para obtener información sobre los campos, consulte [Enumerar notas de problemas de proyectos](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar problemas de proyecto]**

Este módulo de búsqueda devuelve todos los problemas de un proyecto especificado.

Para obtener información sobre los campos, consulte [Enumerar problemas del proyecto](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar hitos de proyecto]**

Este módulo de búsqueda recupera todos los hitos del proyecto.

Para obtener información sobre los campos, consulte [Enumerar hitos de proyecto](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar canalizaciones de proyecto]**

Este módulo de búsqueda recupera todas las canalizaciones del proyecto.

Para obtener información sobre los campos, consulte [Enumerar canalizaciones de proyecto](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar etiquetas de repositorio de proyectos]**

Este módulo de búsqueda recupera una lista de etiquetas de repositorio de un proyecto, ordenadas por nombre en orden alfabético inverso.

Para obtener información sobre los campos, consulte [Enumerar etiquetas de repositorio de proyectos](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar variables de proyecto]**

Este módulo de búsqueda recupera una lista de variables de un proyecto.

Para obtener información sobre los campos, consulte [Enumerar variables de proyecto](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar proyectos]**

Este módulo de búsqueda recupera todos los proyectos de los que es miembro el usuario autenticado.

Para obtener información sobre los campos, consulte [Enumerar todos los proyectos](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar ramas del repositorio]**

Este módulo busca ramas de repositorio por término de búsqueda.

Para obtener información sobre los campos, consulte [Enumerar las ramas del repositorio](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar confirmaciones de repositorio]**

Este módulo de búsqueda recupera una lista de confirmaciones de repositorio en un proyecto.

Para obtener información sobre los campos, consulte [Enumerar confirmaciones de repositorio](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Enumerar colaboradores de repositorio]**

Este módulo de búsqueda recupera una lista de colaboradores del repositorio.

Para obtener información sobre los campos, consulte [Colaboradores](https://docs.gitlab.com/ee/api/repositories.html#contributors) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Árbol de repositorios de listas]**

Este módulo de búsqueda recupera una lista de archivos y directorios del repositorio en un proyecto.

Para obtener información sobre los campos, consulte [Árbol del repositorio de listas](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Marcar un todo como listo]**

Este módulo de acción marca un solo elemento pendiente dado por su ID para el usuario actual como listo.

Para obtener información sobre los campos, consulte [Marcar un elemento para hacer como hecho](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Modificar nota de problema existente]**

Modifica una nota existente de un problema.

Para obtener información sobre los campos, consulte [Modificar nota de problema existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Modificar nota de solicitud de combinación existente]**

Modifica la nota existente de una solicitud de combinación.

Para obtener información sobre los campos, consulte [Modificar la nota de solicitud de combinación existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Modificar nota de fragmento existente]**

Este módulo de acción modifica una nota existente de un fragmento.

Para obtener información sobre los campos, consulte [Modificar nota de fragmento existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Nuevo problema]**

Este módulo de acción crea un nuevo problema de proyecto.

Para obtener información sobre los campos, consulte [Nuevo problema](https://www.integromat.com/en/help/app/gitlab) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Reproducir una compilación]**

Este módulo de acción déclencheur una acción manual para iniciar un trabajo.

Para obtener información sobre los campos, consulte [Reproducir un trabajo](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Comentario de Post para confirmar]**

Este módulo de acción añade un comentario a una confirmación.

Para obtener información sobre los campos, consulte [Comentario de Post para confirmar](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Quitar variable]**

Este módulo de acción elimina la variable de un proyecto.

Para obtener información sobre los campos, consulte [Quitar variable](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Reintentar una compilación]**

Este módulo de acción reintenta una sola compilación en una confirmación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para crear una nueva conexión, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Conectar [!DNL GitLab] a Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de proyecto]</td> 
   <td> <p>Seleccione el proyecto que contiene la compilación que desea volver a intentar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de compilación]</td> 
   <td> Seleccione la compilación que desea volver a intentar. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Reintentar trabajos con errores en una canalización]**

Este módulo de acción reintenta las compilaciones con errores en una canalización.

Para obtener información sobre los campos, consulte [Reintentar trabajos en una canalización](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Obtener una variable]**

Este módulo recupera detalles de la variable específica de un proyecto.

Para obtener información sobre los campos, consulte [Mostrar detalles de la variable](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Actualizar una versión]**

Este módulo de acción actualiza una versión.

Para obtener información sobre los campos, consulte [Actualizar una versión](https://docs.gitlab.com/ee/api/releases/#update-a-release) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Actualizar solicitud de combinación]**

Este módulo de acción actualiza una solicitud de combinación existente. Puede cambiar la rama de destino, el título o incluso cerrar el MR.

Para obtener información sobre los campos, consulte [Actualizar solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) en la documentación de [!DNL GitLab].

+++

+++**[!UICONTROL Actualizar una variable]**

Este módulo de acción actualiza la variable de un proyecto.

Para obtener información sobre los campos, consulte [Actualizar variable](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) en la documentación de [!DNL GitLab].

+++
