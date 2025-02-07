---
title: Configurar la integración de  [!DNL Workfront] y [!DNL Frame.io] s
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador de [!DNL Adobe Workfront] , integre  [!DNL Workfront]  con  [!DNL Frame.io]  y proporcione a la organización una manera perfecta de revisar y aprobar los recursos.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
hide: true
hidefromtoc: true
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 95%

---

# Configuración de la integración de [!DNL Workfront] y [!DNL Frame.io]

El administrador de Workfront permite la integración entre Workfront y Frame.io configurando la cuenta predeterminada de Frame.io en el área de configuración y, a continuación, designando a los usuarios de Frame.io en Workfront. Esto permite a los coordinadores de proyectos planificar e iniciar el trabajo con proyectos de Workfront y revisar y aprobar los flujos de trabajo.


## Requisitos de acceso

>[!IMPORTANT]
>
>Esta funcionalidad solo está disponible para las organizaciones que se hayan incorporado a [!DNL Adobe Admin Console].

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plan</td>
   <td>Cualquiera</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licencias
   </td>
   <td><p>Actual: [!UICONTROL Plan]</p>
   <p>Nuevo: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>

</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar una cuenta predeterminada de [!DNL Frame.io] [!BADGE Próximamente]{type=Informative}

Una vez configurada la cuenta predeterminada de [!DNL Frame.io], los proyectos creados en [!DNL Workfront] tendrán un proyecto espejo creado en Frame.io.

>[!IMPORTANT]
>
>Esta función estará disponible próximamente. Por ahora, el equipo de Workfront añade manualmente las cuentas de Frame.io. Póngase en contacto con el representante de su cuenta de Adobe para obtener ayuda.

## Configuración de una sola cuenta de Frame.io con un grupo de Workfront

Es posible conectar un solo grupo de Workfront con una sola cuenta de Frame.io diferente de la cuenta predeterminada.

Para configurar una sola cuenta de Frame.io con un grupo de Workfront:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.
1. Elija un grupo existente o haga clic en **Crear grupo**.
1. En el panel izquierdo, haga clic en **Conectar con Frame.io**.
1. Introduzca el token de desarrollador de API.
1. Haga clic en **Iniciar conexión**.
1. (Condicional) Si administra más de una cuenta de Frame.io, seleccione la que quiera utilizar.

## Habilitar usuarios de Frame.io

Los usuarios de Workfront que utilicen Frame.io con regularidad deben marcarse como usuarios de Frame.io. Los administradores de Workfront pueden designar a usuarios de Frame.io en el perfil de usuario de Workfront.

>[!TIP]
>
>Se recomienda habilitar a usuarios que trabajen regularmente en herramientas creativas y carguen recursos para su revisión y aprobación como usuarios de Frame.io.

Cuando se marca a un usuario como usuario de Frame.io en Workfront y se añade a un proyecto:

* Se añaden como colaboradores en Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Podrán enviar recursos desde Frame.io a Workfront para su revisión y aprobación formales.
* Podrán ver información en la carpeta de sincronización unidireccional desde Workfront. [!BADGE Próximamente]{type=Informative}

Para habilitar a usuarios de Frame.io:

{{step-1-to-users}}

1. Seleccione uno o más usuarios y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).
1. En la sección Acceso, active la casilla de verificación Añadir a proyectos en Frame.io y, a continuación, seleccione **Sí** en el menú desplegable.
   ![Agregar a proyecto de marco](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Si esta casilla no estuviera marcada, el usuario conservará el acceso a las asignaciones anteriores y se añadirá a los siguientes proyectos de Frame.io.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
