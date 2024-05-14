---
title: Configure las variables [!DNL Workfront] y [!DNL Frame.io] integración
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como un [!DNL Adobe Workfront] administrador, puede integrar [!DNL Workfront] con [!DNL Frame.io] y proporciona a su organización una forma sencilla de revisar y aprobar recursos.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Configure las variables [!DNL Workfront] y [!DNL Frame.io] integración

El administrador de Workfront permite la integración entre Workfront y Frame.io configurando la cuenta predeterminada de Frame.io en el área de Configuración y designando a continuación a los usuarios de Frame.io en Workfront. Esto permite al coordinador del proyecto planificar e iniciar el trabajo con proyectos de Workfront y revisar y aprobar los flujos de trabajo.


## Requisitos de acceso

>[!IMPORTANT]
>
>Esta funcionalidad solo está disponible para las organizaciones que se han incorporado al [!DNL Adobe Admin Console].

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
   <td>Debe ser un [!DNL Workfront] administrador.
   </td>
  </tr>

</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Configuración de un valor predeterminado [!DNL Frame.io] account [!BADGE Muy pronto]{type=Informative}

Una vez predeterminado [!DNL Frame.io] cuenta está configurada, cualquier proyecto creado en [!DNL Workfront] haga que se cree un proyecto de reflejo en Frame.io.

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
1. Clic **Iniciar conexión**.
1. (Condicional) Si es el administrador de más de una cuenta de Frame.io, seleccione la cuenta que desee utilizar.

## Habilitar usuarios de Frame.io

Los usuarios de Workfront que utilicen Frame.io con regularidad deben marcarse como usuarios de Frame.io. Los administradores de Workfront pueden designar a los usuarios de Frame.io en el Perfil de usuario de Workfront.

>[!TIP]
>
>Recomendamos habilitar a los usuarios que trabajan regularmente en herramientas creativas y cargan recursos para su revisión y aprobación como usuarios de Frame.io.

Cuando un usuario está marcado como usuario de Frame.io en Workfront y se añade a un proyecto:

* Se añaden como Collaborator en Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Pueden enviar recursos desde Frame.io a Workfront para su revisión y aprobación formales.
* Pueden ver información en la carpeta de sincronización unidireccional desde Workfront. [!BADGE Muy pronto]{type=Informative}

Para habilitar a los usuarios de Frame.io:

{{step-1-to-users}}

1. Seleccione uno o varios usuarios y haga clic en el botón **Editar** icono ![](assets/edit-icon.png).
1. En la sección Acceso, active la casilla Agregar a proyectos en Frame.io y, a continuación, seleccione **Sí** en el menú desplegable.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Si esta casilla no está marcada, el usuario conserva el acceso a las asignaciones anteriores y se agrega a los proyectos de Frame.io a partir de ahora.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->

