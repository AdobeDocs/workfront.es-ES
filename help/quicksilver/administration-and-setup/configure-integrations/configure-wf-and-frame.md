---
title: Configurar la integración de  [!DNL Workfront] y [!DNL Frame.io] s
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador de  [!DNL Adobe Workfront] puedes integrar [!DNL Workfront] con [!DNL Frame.io] y proporcionar a tu organización una manera perfecta de revisar y aprobar los recursos.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: 0d737bc410f3db4eeff52fa8954acdb8a0eb1a6e
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Configurar la integración de [!DNL Workfront] y [!DNL Frame.io]

El administrador de Workfront permite la integración entre Workfront y Frame.io configurando la cuenta predeterminada de Frame.io en el área de Configuración y designando a continuación a los usuarios de Frame.io en Workfront. Esto permite al coordinador del proyecto planificar e iniciar el trabajo con proyectos de Workfront y revisar y aprobar los flujos de trabajo.


## Requisitos de acceso

>[!IMPORTANT]
>
>Esta funcionalidad solo está disponible para las organizaciones que se han incorporado a [!DNL Adobe Admin Console].

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licencias</strong>
   </td>
   <td>Actual: [!UICONTROL plan] <br>
   Nuevo: [!UICONTROL Standard]
   </td>
  </tr>

<tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>

</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Configurar una cuenta predeterminada [!DNL Frame.io] [!BADGE Próximamente]{type=Informative}

Una vez configurada la cuenta predeterminada [!DNL Frame.io], los proyectos creados en [!DNL Workfront] tendrán un proyecto de reflejo creado en Frame.io.

>[!IMPORTANT]
>
>Esta función estará disponible próximamente. Por ahora, el equipo de Workfront agrega manualmente las cuentas de Frame.io. Póngase en contacto con el representante de su cuenta de Adobe para obtener ayuda.

## Configuración de una sola cuenta de Frame.io con un grupo de Workfront

Puede conectar un solo grupo de Workfront con una sola cuenta de Frame.io diferente de la cuenta predeterminada.

Para configurar una sola cuenta de Frame.io con un grupo de Workfront:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.
1. Elija un grupo existente o haga clic en **Crear grupo**.
1. En el panel izquierdo, haga clic en **Conectar con Frame.io**.
1. Introduzca el token de desarrollador de API.
1. Haga clic en **Iniciar conexión**.
1. (Condicional) Si es el administrador de más de una cuenta de Frame.io, seleccione la cuenta que desee utilizar.

## Habilitar usuarios de Frame.io

Los usuarios de Workfront que utilicen Frame.io con regularidad deben marcarse como usuarios de Frame.io. Los administradores de Workfront pueden designar a los usuarios de Frame.io en el Perfil de usuario de Workfront.

>[!TIP]
>
>Recomendamos habilitar a los usuarios que trabajan regularmente en herramientas creativas y cargan recursos para su revisión y aprobación como usuarios de Frame.io.

Cuando un usuario está marcado como usuario de Frame.io en Workfront y se añade a un proyecto:

* Se añaden como Collaborator en Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Pueden enviar recursos desde Frame.io a Workfront para su revisión y aprobación formales.
* Pueden ver información en la carpeta de sincronización unidireccional desde Workfront. [!BADGE Próximamente]{type=Informative}

Para habilitar a los usuarios de Frame.io:

{{step-1-to-users}}

1. Seleccione uno o más usuarios y luego haga clic en el icono **Editar** ![](assets/edit-icon.png).
1. En la sección Acceso, active la casilla de verificación Agregar a proyectos en Frame.io y, a continuación, seleccione **Sí** en el menú desplegable.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Si esta casilla no está marcada, el usuario conserva el acceso a las asignaciones anteriores y se agrega a los proyectos de Frame.io en adelante.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
