---
title: Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning
description: Puede agregar un proceso de aprobación a un formulario de solicitud de Adobe Workfront Planning para iniciar una aprobación para cada solicitud enviada antes de crear un registro.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 4%

---

# Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede agregar un proceso de aprobación a un formulario de solicitud de Adobe Workfront Planning para iniciar una aprobación para cada solicitud enviada antes de crear un registro.

Este artículo describe cómo un administrador del espacio de trabajo puede agregar una aprobación a un formulario de solicitud asociado a un tipo de registro.

Para obtener información acerca de cómo crear un formulario de solicitud en Workfront Planning, vea [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Para obtener información sobre cómo enviar una solicitud a un tipo de registro para crear un registro, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete Workfront y cualquier paquete Planning</p>
O
<p>Cualquier paquete de flujo de trabajo y cualquier paquete de Planning</p>

<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos a un espacio de trabajo y tipo de registro</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la adición de aprobaciones a un formulario de solicitud

* Puede agregar uno o varios aprobadores a un formulario de solicitud. Solo puede agregar usuarios como aprobadores.
* Puede mostrar la información de aprobación de un registro creado enviando un formulario de solicitud en los campos Aprobado por y Fecha de aprobación. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).
* Cuando se agregan varios aprobadores a un formulario de solicitud, todos los aprobadores deben aceptar la solicitud antes de crear un registro en Workfront Planning.
* Si todos los aprobadores aprueban la solicitud, se crea un registro para el tipo de registro asociado al formulario de solicitud.
* Si al menos un aprobador rechaza la solicitud y todos los demás la aprueban, se crea una solicitud para el área de Solicitudes en Workfront, pero no se crea ningún registro para el tipo de registro asociado al formulario de solicitud.
* Añadir aprobaciones a un formulario de solicitud es opcional. Workfront Planning crea inmediatamente un registro cuando se envía una solicitud, si el formulario de solicitud no está asociado a una aprobación.

## Agregar una aprobación a un formulario de solicitud en el entorno de producción

1. Comience a crear un formulario de solicitud para un tipo de registro, como se describe en [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Haga clic en **Configuración**.

   Se muestra el área **Configuración**.

   ![Ficha de configuración](assets/configuration-tab.png)
1. En el campo **Aprobadores**, empiece a escribir el nombre de un usuario o equipo que desee establecer como aprobador y, a continuación, selecciónelo cuando se muestre en la lista.
1. (Opcional y condicional) Si ha establecido más de un aprobador y solo necesita un aprobador para tomar una decisión, habilite la opción **Solo se requiere una decisión**.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Puede agregar uno o varios aprobadores a un formulario de solicitud.
   >
   >* Si agrega más de un aprobador y la opción Only one decision is required no está habilitada, todos los aprobadores deben aprobar la solicitud antes de que Workfront Planning cree un registro.
   >
   >* Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro. La solicitud permanece en el área de solicitudes de Workfront.
   >
   >* Si añade más de un aprobador y la opción Only one decision is required no está activada, todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.
   >
   >* Si un equipo se establece como aprobador, solo se requiere una decisión del equipo.


1. (Opcional) Haga clic en **Publicar** si nunca antes había compartido el formulario de solicitud.

   O

   Haga clic en **Compartir** para compartir el formulario y luego en **Copiar vínculo**.
1. (Opcional) Una vez que un usuario utiliza el vínculo que comparte y envía una solicitud, Workfront Planning envía una notificación de aprobación en la aplicación y un correo electrónico a los aprobadores.

   >[!NOTE]
   >
   >   La instancia de Workfront de su organización debe incorporarse a la experiencia unificada de Adobe para que los usuarios puedan recibir notificaciones por correo electrónico y en la aplicación.


   Para obtener información acerca de cómo aprobar solicitudes, vea [Aprobar una solicitud](/help/quicksilver/planning/requests/approve-request.md).

<div class="preview">

## Adición de reglas de aprobación a un formulario de solicitud

>[!NOTE]
>
>Esta funcionalidad solo está disponible en el entorno de vista previa.

Las reglas de aprobación definen el proceso de aprobación en función de los valores de campo en las solicitudes enviadas.

Por ejemplo, si un formulario de solicitud tiene el campo &quot;Tipo de campaña&quot;, se puede crear una regla que envíe la solicitud a una persona cuando el campo tenga el valor &quot;Digital&quot; y a una persona diferente cuando tenga el valor &quot;Imprimir&quot;.

Tenga en cuenta lo siguiente al añadir reglas de aprobación:

* Puede añadir uno o varios aprobadores a una regla de aprobación.
* Si al menos un aprobador rechaza la solicitud, esta se rechaza y no se crea el registro. La solicitud permanece en el área de solicitudes de Workfront.
* Si añade más de un aprobador y la opción Only one decision is required no está activada, todos los aprobadores deben tomar una decisión antes de aprobar o rechazar una solicitud.
* Si un equipo se establece como aprobador, solo se requiere una decisión del equipo.

Para obtener más información sobre cómo agregar aprobaciones, consulte [Agregar aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

Para definir reglas de aprobación para un formulario de solicitud:

1. Comience a crear un formulario de solicitud para un tipo de registro, como se describe en [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Haga clic en **Configuración**.

   Se muestra la pestaña Configuración.

1. Para comenzar a configurar las reglas de aprobación, haga clic en el icono ![Aprobaciones](assets/approvals-icon-on-form.png) de aprobaciones en el panel de navegación izquierdo.

1. (Opcional) Si desea establecer un proceso de aprobación predeterminado, agregue al menos un usuario o equipo al campo **Aprobadores** del área Regla de aprobación predeterminada y, a continuación, haga clic en la casilla de verificación **Solo se requiere una decisión** si desea que el registro se cree después de que cualquiera de los aprobadores predeterminados lo haya aprobado.

   ![Área de regla de aprobación predeterminada](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Opcional) Para cada regla de aprobación adicional, haga lo siguiente:

   1. Haga clic en **Agregar regla de aprobación**
   1. Haga clic en el título del marcador de posición &quot;Regla de aprobación sin título&quot; e introduzca un nombre para la regla de aprobación.
   1. Haga clic en **Seleccionar un campo** y seleccione el campo que activa la regla.
   1. Seleccione el operador de la regla. Los operadores varían según el tipo de campo.
   1. Si el operador seleccionado requiere un valor, haga clic en el icono de signo más y añada uno o más valores.
   1. (Opcional) Agregue más condiciones utilizando AND u OR haciendo clic en Agregar condición y configurando la condición adicional como en los pasos C-E.
   1. En el área Acciones de la regla de aprobación, en el campo **Aprobadores**, agregue al menos un usuario o equipo que se establecerá en el aprobador cuando se cumpla la condición.
   1. 
      1. (Condicional) Si desea que el registro se cree después de que cualquiera de los aprobadores lo haya aprobado, marque la casilla **Solo se requiere una decisión**.

1. Haga clic en **Guardar** para guardar las reglas de aprobación.
1. (Opcional) Haga clic en **Publicar** si nunca antes había compartido el formulario de solicitud.

</div>
