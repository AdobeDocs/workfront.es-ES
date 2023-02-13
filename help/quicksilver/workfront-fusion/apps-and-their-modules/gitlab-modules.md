---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de GitLab
description: Adobe Workfront Fusion requiere una licencia de Adobe Workfront Fusion además de una licencia de Adobe Workfront.
author: Becky
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: d55ddd97a69f00a1f42d84dc55a12d2017855776
workflow-type: tm+mt
source-wordcount: '4370'
ht-degree: 0%

---


# [!UICONTROL GitLab] módulos

Adobe Workfront Fusion requiere una licencia de Adobe Workfront Fusion además de una licencia de Adobe Workfront.

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!UICONTROL GitLab], así como conectarlo a varias aplicaciones y servicios de terceros.

>[!NOTE]
>
>Este artículo espera cierta familiaridad con la documentación de API y con la [!DNL GitLab] en general.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Connect [!DNL GitLab] a [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. En cualquier [!DNL Workfront Fusion] [!DNL Gitlab] módulo, haga clic en **[!UICONTROL Agregar]** junto al campo de conexión.
1. Configure los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td> <p>Introduzca un nombre para la conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Introduzca la dirección URL de su [!DNL GitLab] instancia.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access Token]</td> 
      <td><p>Introduzca su [!UICONTROL Private Token] o [!UICONTROL Personal Access Token].</p><p>Para obtener información sobre cómo localizar o crear un token de acceso personal en [!DNL GitLab], consulte "Crear un token de acceso personal" en <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Tokens de acceso personal</a> en el [!DNL GitLab] documentación.</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Haga clic en **[!UICONTROL Continuar]**.
1. Haga clic en **[!UICONTROL Autorizar]** para crear la conexión y volver al módulo.

## [!DNL GitLab] módulos y sus campos

Al configurar [!DNL GitLab] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL GitLab] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheur

+++**[!UICONTROL Estado de la compilación de Watch]**

Este módulo de déclencheur instantáneo inicia un escenario cuando cambia el estado de una compilación.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el vínculo web observe los cambios de estado de compilación</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver comentarios de confirmación/MR/número/fragmento]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se realiza un comentario en una confirmación, una solicitud de combinación, un problema o un fragmento de código.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web vea para comentarios</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Commits (empuches)]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se envía una confirmación a un repositorio. Este módulo no inicia un escenario cuando se inserta una etiqueta.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web vea para confirmaciones</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
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
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web mire los comentarios del problema</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Problemas de observación]**

Esta [!UICONTROL déclencheur instantáneo] inicia un escenario cuando se crea un problema o cuando se actualiza, cierra o vuelve a abrir un problema existente.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el vínculo web observe si hay problemas</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver solicitudes de combinación]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se produce uno de los siguientes:

* Se crea una nueva solicitud de combinación
* Se actualiza, combina o cierra una solicitud de combinación existente
* Se agrega una confirmación en la rama de origen


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web observe para las solicitudes de combinación</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
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
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web observe para los comentarios de solicitud de combinación</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Estado de la canalización de inspección]**

Este módulo de déclencheur instantáneo inicia un escenario cuando cambia el estado de una canalización.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web observe los cambios de estado de la canalización</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL GitLab] cuenta para [!DNL Workfront] Fusion, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] a [!DNL Workfront] Fusión</a> en este artículo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Resultados máximos</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo vea durante cada ciclo de ejecución del escenario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver ramas de repositorios]**

Este módulo de déclencheur programado inicia un escenario cuando se agrega una nueva rama a un repositorio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL GitLab] cuenta para [!DNL Workfront] Fusion, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] a [!DNL Workfront] Fusión</a> en este artículo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Resultados máximos</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo vea durante cada ciclo de ejecución del escenario.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Etiquetas del repositorio de Watch]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se crea o elimina una etiqueta en un repositorio.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el vínculo web busque etiquetas</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver comentarios de fragmento]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se realiza un nuevo comentario en un fragmento.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web vea para comentarios</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Ver todos]**

Este módulo de déclencheur programado inicia un escenario cuando se agrega una nueva tarea. Cuando no se aplica ningún filtro, el déclencheur se ejecuta cuando se agrega una nueva tarea pendiente.

Para obtener información sobre los campos, consulte [Obtener una lista de tareas pendientes](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Ver página wiki]**

Este módulo de déclencheur instantáneo inicia un escenario cuando se crea o edita una página wiki.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td><p>Seleccione el enlace web que desee usar para este déclencheur o agregue un nuevo vínculo web. </p><p>Para añadir un nuevo enlace web, <ol><li>Haga clic en <b>[!UICONTROL Agregar]</b> junto al campo [!UICONTROL weblock].</li><li>Introduzca lo siguiente: <ul><li>Un nombre para el enlace web</li><li>La conexión que desea utilizar para este enlace web</li><li>El proyecto que desea que el enlace web vea para páginas wiki</li></ul></li><li>Haga clic en <b>[!UICONTROL Guardar]</b> para guardar el enlace web y volver al módulo. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Acciones

+++**[!UICONTROL Aceptar solicitud de combinación]**

Este módulo de acción combina los cambios enviados con la solicitud de combinación dada.

Para obtener información sobre los campos, consulte [Aceptar solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Cancelar una compilación]**

Este módulo de acción cancela una sola compilación de un proyecto.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL GitLab] cuenta para [!DNL Workfront] Fusion, consulte <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Connect [!DNL GitLab] a [!DNL Workfront] Fusión</a> en este artículo.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID del proyecto]</td> 
   <td> <p>Seleccione o asigne el proyecto que contiene la compilación que desea cancelar.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID de compilación]</td> 
   <td>Seleccione o asigne la compilación que desee cancelar.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Merge commit message]</td> 
   <td> Introduzca o asigne un mensaje de confirmación para la combinación.
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

Para obtener información sobre los campos, consulte [Cancelar los trabajos de una canalización](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Cancelar combinación cuando la canalización se realice correctamente]**

Si una solicitud de combinación está configurada para combinarse cuando una canalización se realiza correctamente, este módulo de acción cancela esa acción.

Para obtener información sobre los campos, consulte [Cancelar combinación cuando la canalización se realice correctamente](https://docs.gitlab.com/ee/api/merge_requests.html) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Cherry elige un compromiso]**

Este módulo de acción cereza selecciona una confirmación en una rama determinada.

Para obtener información sobre los campos, consulte [Cherry elige un compromiso](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear una etiqueta nueva]**

Este módulo de acción crea una etiqueta nueva para el repositorio dado.

Para obtener información sobre los campos, consulte [Crear una etiqueta nueva](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Creación de una nueva canalización]**

Este módulo de acción crea una nueva canalización para el proyecto dado.

Para obtener información sobre los campos, consulte [Creación de una nueva canalización](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear una nueva versión]**

Este módulo de acción agrega notas de la versión a la etiqueta git existente.

Para obtener información sobre los campos, consulte [Crear una versión](https://docs.gitlab.com/ee/api/releases/#create-a-release) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear una etiqueta nueva]**

Este módulo de acción crea una nueva etiqueta en el repositorio que apunta a la referencia suministrada.

Para obtener información sobre los campos, consulte [Crear una etiqueta nueva](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear un todo]**

Este módulo de acción crea una acción para el usuario actual en el problema seleccionado. El usuario actual es el usuario identificado por las credenciales de la conexión utilizada para este módulo.

Para obtener información sobre los campos, consulte [Cree un](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Creación de una tarea en una solicitud de combinación]**

Este módulo de acción crea una tarea para el usuario actual en la solicitud de combinación seleccionada. El usuario actual es el usuario identificado por las credenciales de la conexión utilizada para este módulo.

Para obtener información sobre los campos, consulte [Crear una tarea pendiente](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear solicitud de combinación]**

Este módulo de acción crea una nueva solicitud de combinación en un proyecto.

Para obtener información sobre los campos, consulte [Crear solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear nuevo archivo en el repositorio]**

Este módulo de acción crea un nuevo archivo en el repositorio seleccionado.

Para obtener información sobre los campos, consulte [Crear nuevo archivo en el repositorio](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear nueva nota del problema]**

Este módulo de acción crea una nota de problema para un solo problema de proyecto.

Para obtener información sobre los campos, consulte [Crear nueva nota del problema](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear nueva nota de solicitud de combinación]**

Este módulo de acción crea una nota para una única solicitud de combinación.

Para obtener información sobre los campos, consulte [Crear nueva nota de solicitud de combinación](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear un nuevo hito]**

Este módulo de acción crea un nuevo hito para un proyecto.

Para obtener información sobre los campos, consulte [Crear nuevo hito](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear nueva nota de fragmento]**

Este módulo de acción crea una nota nueva para un solo fragmento. Las notas de fragmento son comentarios que los usuarios pueden publicar en un fragmento.

Para obtener información sobre los campos, consulte [Crear nueva nota de fragmento](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear rama de repositorio]**

Este módulo de acción crea una sola rama de repositorio.

Para obtener información sobre los campos, consulte [Crear rama de repositorio](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Crear variable de compilación]**

Este módulo de acción crea una nueva variable de compilación.

Para obtener información sobre los campos, consulte [Crear variable](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Eliminar una solicitud de combinación]**

Este módulo de acción solo es para administradores y propietarios de proyectos. Elimina la solicitud de combinación en cuestión

Para obtener información sobre los campos, consulte [Eliminar una solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Eliminar archivo existente en el repositorio]**

Este módulo de acción elimina un archivo existente del repositorio.

Para obtener información sobre los campos, consulte [Eliminar archivo existente en el repositorio](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Eliminar rama del repositorio]**

Este módulo de acción elimina una rama del repositorio.

Para obtener información sobre los campos, consulte [Eliminar rama del repositorio](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Editar problema]**

Este módulo de acción actualiza un problema de proyecto existente. Esta llamada también se utiliza para marcar un problema como cerrado.

Para obtener información sobre los campos, consulte [Editar problema](https://docs.gitlab.com/ee/api/issues.html#edit-issue) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Editar Milestone]**
Este módulo de acción actualiza un hito de proyecto existente.

Para obtener información sobre los campos, consulte [Editar hito](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Borrar una compilación]**

Este módulo de acción borra una compilación de un proyecto (elimina los artefactos del trabajo y el registro de trabajos).

Para obtener información sobre los campos, consulte [Borrar un trabajo](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener una lista de todos]**

Este módulo de búsqueda recupera una lista de elementos pendientes.

Para obtener información sobre los campos, consulte [Obtener una lista de tareas pendientes](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener una sola compilación]**

Este módulo de acción recupera un solo trabajo de un proyecto.

Para obtener información sobre los campos, consulte [Obtener un solo trabajo](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener una sola etiqueta de repositorio]**

Este módulo de acción recupera una etiqueta de repositorio específica determinada por su nombre.

Para obtener información sobre los campos, consulte [Obtener una sola etiqueta de repositorio](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener una implementación específica]**

Este módulo de acción recupera una implementación específica.

Para obtener información sobre los campos, consulte [Obtener una implementación específica](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener todos los problemas asignados a un solo hito]**

Este módulo de búsqueda recupera todos los problemas asignados a un solo hito del proyecto.

Para obtener información sobre los campos, consulte [Obtener todos los problemas asignados a un solo hito](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener archivo del repositorio]**

Este módulo de acción recupera información sobre un archivo del repositorio como nombre, tamaño o contenido.

Para obtener información sobre los campos, consulte [Obtener archivo del repositorio](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener usuarios del proyecto]**

Este módulo de búsqueda recupera a los usuarios del proyecto.

Para obtener información sobre los campos, consulte [Obtener usuarios del proyecto](https://docs.gitlab.com/ee/api/projects.html#get-project-users) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener un solo problema]**

Este módulo de acción recupera los detalles del problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para crear una nueva conexión, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td> <p>Seleccione el proyecto que contiene el problema sobre el que desea recuperar detalles.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Problema ID]</td> 
   <td> <p>Introduzca o asigne el nombre del problema del que desea recuperar detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Obtener una sola nota del número]**

Este módulo de acción recupera una sola nota para un problema específico del proyecto.

Para obtener información sobre los campos, consulte [Obtener una sola nota del número](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener solicitud de combinación única]**

Este módulo de acción recupera información sobre una única solicitud de combinación.

Para obtener información sobre los campos, consulte [Obtener solicitud de combinación única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener cambios de solicitud de combinación única]**

Este módulo de búsqueda recupera información sobre la solicitud de combinación, incluidos sus archivos y cambios.

Para obtener información sobre los campos, consulte [Obtener cambios de solicitud de combinación única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener confirmaciones de solicitud de combinación única]**

Este módulo de acción recupera una lista de confirmaciones de solicitud de combinación.

Para obtener información sobre los campos, consulte [Obtener confirmaciones de solicitud de combinación única](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener nota de solicitud de combinación única]**

Este módulo de acción devuelve una sola nota para una solicitud de combinación determinada.

Para obtener información sobre los campos, consulte [Obtener nota de solicitud de combinación única](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener un hito]**

Este módulo de acción recupera los detalles de hitos.

Para obtener información sobre los campos, consulte [Obtener un solo hito](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener un solo proyecto]**

Este módulo de acción recupera los detalles del proyecto.

Para obtener información sobre los campos, consulte [Obtener un solo proyecto](https://docs.gitlab.com/ee/api/projects.html#get-single-project) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener una sola rama del repositorio]**

Este módulo de acción recupera los detalles de las ramas del repositorio.

Para obtener información sobre los campos, consulte [Obtener una sola rama del repositorio](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener nota de fragmento]**

Este módulo recupera una sola nota de un fragmento determinado.

Para obtener información sobre los campos, consulte [Obtener una sola nota de fragmento](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener los comentarios de un compromiso]**

Este módulo de búsqueda recupera los comentarios de una confirmación en un proyecto.

Para obtener información sobre los campos, consulte [Obtener los comentarios de un compromiso](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener la diferencia de una confirmación]**

Este módulo de acción obtiene la diferencia de una confirmación en un proyecto.

Para obtener información sobre los campos, consulte [Obtener la diferencia de una confirmación](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Conservar artefactos]**

Evita que se eliminen artefactos cuando se establece la caducidad.

Para obtener información sobre los campos, consulte [Conservar artefactos](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar todas las notas de solicitud de combinación]**

Este módulo de búsqueda recupera una lista de todas las notas de una única solicitud de combinación.

Para obtener información sobre los campos, consulte [Enumerar todas las notas de solicitud de combinación](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar todas las notas de fragmento]**

Este módulo obtiene una lista de todas las notas de un solo fragmento. Las notas de fragmento son comentarios que los usuarios pueden publicar en un fragmento.

Para obtener información sobre los campos, consulte [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar compilaciones de confirmación]**

Este módulo de búsqueda devuelve una lista de compilaciones para una confirmación específica en un proyecto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para crear una nueva conexión, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID del proyecto]</td> 
   <td> <p>Seleccione el proyecto que contiene la confirmación para la que desea enumerar las compilaciones.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ámbito]</td> 
   <td> Para limitar la búsqueda a generar con un estado específico, seleccione el estado . Dejar este campo en blanco devuelve todas las compilaciones de la confirmación.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Enumerar problemas]**

Este módulo de búsqueda devuelve todos los problemas según la configuración de filtro especificada.

Para obtener información sobre los campos, consulte [Enumerar problemas](https://docs.gitlab.com/ee/api/issues.html#list-issues) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar problemas que se cierran al combinar]**

Este módulo de búsqueda recupera todos los problemas que se cerrarían al combinar la solicitud de combinación proporcionada.

Para obtener información sobre los campos, consulte [Enumerar problemas que se cerrarán al combinar](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Etiquetas de lista]**

Este módulo de búsqueda recupera todas las etiquetas del proyecto.

Para obtener información sobre los campos, consulte [Enumerar etiquetas](https://docs.gitlab.com/ee/api/labels.html#list-labels) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar solicitudes de combinación]**

Este módulo de búsqueda recupera todas las solicitudes de combinación según la configuración del filtro.

Para obtener información sobre los campos, consulte [Enumerar solicitudes de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar proyectos en propiedad]**

Este módulo de búsqueda recupera proyectos en los que el usuario autenticado está establecido como propietario.

Para obtener información sobre los campos, consulte [Enumerar proyectos de usuario](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar compilaciones de proyectos]**

Este módulo de búsqueda recupera una lista de compilaciones en un proyecto.

Para obtener información sobre los campos, consulte [Enumerar trabajos de proyecto](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar implementaciones de proyectos]**

Este módulo de búsqueda recupera una lista de implementaciones en un proyecto.

Para obtener información sobre los campos, consulte [Enumerar implementaciones de proyectos](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar notas de problemas del proyecto]**

Este módulo de búsqueda recupera una lista de todas las notas de un solo problema.

Para obtener información sobre los campos, consulte [Enumerar notas de problemas del proyecto](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar problemas de proyecto]**

Este módulo de búsqueda devuelve todos los problemas de un proyecto especificado.

Para obtener información sobre los campos, consulte [Enumerar problemas de proyecto](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar hitos del proyecto]**

Este módulo de búsqueda recupera todos los hitos del proyecto.

Para obtener información sobre los campos, consulte [Enumerar hitos del proyecto](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar canalizaciones de proyectos]**

Este módulo de búsqueda recupera todas las canalizaciones del proyecto.

Para obtener información sobre los campos, consulte [Enumerar canalizaciones de proyectos](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar etiquetas del repositorio del proyecto]**

Este módulo de búsqueda recupera una lista de etiquetas de repositorio de un proyecto, ordenadas por nombre en orden alfabético inverso.

Para obtener información sobre los campos, consulte [Enumerar etiquetas del repositorio del proyecto](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar variables de proyecto]**

Este módulo de búsqueda recupera una lista de las variables de un proyecto.

Para obtener información sobre los campos, consulte [Enumerar variables de proyecto](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar proyectos]**

Este módulo de búsqueda recupera todos los proyectos de los que es miembro el usuario autenticado.

Para obtener información sobre los campos, consulte [Enumerar todos los proyectos](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar ramas de repositorios]**

Este módulo busca ramas del repositorio según el término de búsqueda.

Para obtener información sobre los campos, consulte [Enumerar ramas de repositorios](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Listar confirmaciones de repositorios]**

Este módulo de búsqueda recupera una lista de confirmaciones de repositorios en un proyecto.

Para obtener información sobre los campos, consulte [Listar confirmaciones de repositorios](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Enumerar colaboradores del repositorio]**

Este módulo de búsqueda recupera una lista de colaboradores del repositorio.

Para obtener información sobre los campos, consulte [Colaboradores](https://docs.gitlab.com/ee/api/repositories.html#contributors) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Árbol de repositorios de listas]**

Este módulo de búsqueda recupera una lista de archivos y directorios de repositorios en un proyecto.

Para obtener información sobre los campos, consulte [Árbol de repositorios de listas](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Marcar una tarea como completada]**

Este módulo de acción marca un solo elemento pendiente de hacer dado por su ID para el usuario actual tal como lo ha hecho.

Para obtener información sobre los campos, consulte [Marcar como hecho un elemento para hacer como hecho](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Modificar nota de problema existente]**

Modifica una nota existente de un problema.

Para obtener información sobre los campos, consulte [Modificar nota de problema existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Modificar nota de solicitud de combinación existente]**

Modifica la nota existente de una solicitud de combinación.

Para obtener información sobre los campos, consulte [Modificar nota de solicitud de combinación existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Modificar nota de fragmento existente]**

Este módulo de acción modifica una nota existente de un fragmento.

Para obtener información sobre los campos, consulte [Modificar nota de fragmento existente](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Nuevo problema]**

Este módulo de acción crea un nuevo problema de proyecto.

Para obtener información sobre los campos, consulte [Nuevo problema](https://www.integromat.com/en/help/app/gitlab) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Reproducción de una compilación]**

Este módulo de acción déclencheur una acción manual para iniciar un trabajo.

Para obtener información sobre los campos, consulte [Reproducir un trabajo](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Publicar comentario para confirmar]**

Este módulo de acción agrega un comentario a una confirmación.

Para obtener información sobre los campos, consulte [Publicar comentario para confirmar](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Eliminar variable]**

Este módulo de acción elimina la variable de un proyecto.

Para obtener información sobre los campos, consulte [Eliminar variable](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Reintentar una compilación]**

Este módulo de acción reintenta una sola compilación en una confirmación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para crear una nueva conexión, consulte <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] a Workfront Fusion]</a> en este artículo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID del proyecto]</td> 
   <td> <p>Seleccione el proyecto que contiene la compilación que desea reintentar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de compilación]</td> 
   <td> Seleccione la compilación que desee reintentar. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Reintentar trabajos fallidos en una canalización]**

Este módulo de acción reintenta compilaciones fallidas en una canalización.

Para obtener información sobre los campos, consulte [Reintentar trabajos en una canalización](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Obtener una variable]**

Este módulo recupera los detalles de la variable específica de un proyecto.

Para obtener información sobre los campos, consulte [Mostrar detalles de variables](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Actualizar una versión]**

Este módulo de acción actualiza una versión.

Para obtener información sobre los campos, consulte [Actualizar una versión](https://docs.gitlab.com/ee/api/releases/#update-a-release) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Actualizar solicitud de combinación]**

Este módulo de acción actualiza una solicitud de combinación existente. Puede cambiar la rama de destino, el título o incluso cerrar el MR.

Para obtener información sobre los campos, consulte [Actualizar solicitud de combinación](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) en el [!DNL GitLab] documentación.

+++

+++**[!UICONTROL Actualizar una variable]**

Este módulo de acción actualiza la variable de un proyecto.

Para obtener información sobre los campos, consulte [Actualizar variable](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) en el [!DNL GitLab] documentación.

+++
