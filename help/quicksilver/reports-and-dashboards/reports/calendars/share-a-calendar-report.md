---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Compartir un informe de calendario
description: Puede compartir un calendario con otros usuarios y ponerlo a disposición del público, permitiendo que alguien sin una licencia de  [!DNL Adobe Workfront]  lo vea.
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: 0606dab832753543ceef4b5b505413967176aec4
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 82%

---

# Compartir un informe de calendario


Puede compartir un calendario con otros usuarios y ponerlo a disposición del público, permitiendo que alguien sin una licencia de [!DNL Adobe Workfront] lo vea.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: claro</p>
       <p>o</p>
       <p>Actual: Revisar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>[!UICONTROL Ver] o acceso superior a [!UICONTROL Informes], [!UICONTROL Paneles] y [!UICONTROL Calendarios]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>[!UICONTROL View] o permisos superiores para el informe de calendario, con acceso para compartir</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartir un calendario con los usuarios de [!DNL Workfront] {#share-a-calendar-with-workfront-users}

Compartir un calendario es similar a compartir otros objetos. Para obtener más información acerca de cómo compartir objetos en [!DNL Adobe Workfront], consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Los calendarios que se han compartido con usted se muestran con un asterisco (&#42;) junto al nombre del calendario.

Para compartir un calendario dentro de [!DNL Workfront]:

1. Seleccione el calendario que desee compartir.
1. Haga clic en el menú **Más** junto al nombre del calendario y luego haga clic en **Compartir**.
   ![calendario más menú](assets/more-menu-calendar.png)
1. En el campo **[!UICONTROL Give Calendar access to]**, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con los que desea compartir el calendario y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.\
   Para obtener más información acerca de la configuración de permisos, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Opcional) Repita el paso 3 para cada usuario, equipo, función o grupo al que desee conceder acceso al calendario.
1. Especifique los permisos para cada usuario, equipo, función, grupo o compañía que añadió en el paso 3 haciendo clic en el menú desplegable y, a continuación, seleccione el nivel de permiso que desea conceder:

   * **[!UICONTROL Vista]:** los usuarios pueden revisar y compartir el calendario.

     ![Compartir calendario con acceso de visualización](assets/view-calendar.png)

   * **[!UICONTROL Administrar]:** los usuarios tienen acceso completo al calendario, menos derechos administrativos, que se conceden en el nivel de acceso, más todos los permisos de visualización.

     ![Compartir calendario con acceso de administración](assets/manage-calendar.png)

     >[!NOTE]
     >
     >El administrador de [!DNL Workfront] y el creador del calendario tienen la capacidad de quitar permisos de estas entidades.

1. (Opcional) Según la función de un usuario, es posible que pueda hacer clic en **[!UICONTROL Opciones avanzadas]** y, a continuación, hacer clic en **[!UICONTROL Compartir]**&#x200B; para permitir que el usuario comparta el calendario con otros usuarios.

   Para obtener más información acerca de los niveles de permisos, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Opcional) Para que el calendario esté disponible para todos los usuarios de [!DNL Workfront], haga clic en el icono de engranaje y, a continuación, en el menú desplegable, haga clic en **[!UICONTROL Hacer que este sea visible en todo el sistema]** para que el objeto esté disponible para todos los usuarios de [!DNL Workfront].\
   Todos los usuarios pueden ver el objeto en función de los permisos que establezca.

1. Haga clic en **[!UICONTROL Guardar]**.

## Compartir un calendario con un vínculo público

Puede hacer público un calendario y compartir un vínculo con personas que no tengan una licencia de [!DNL Workfront].

1. Seleccione el calendario que desee compartir.
1. Haga clic en **[!UICONTROL Calendar Actions]** y, a continuación, haga clic en **[!UICONTROL Sharing]**.
1. Haga clic en el menú **Más** junto al nombre del calendario.
   ![calendario más menú](assets/more-menu-calendar.png)
Haga clic en **Copiar vínculo público**.
1. Haga clic en **[!UICONTROL Guardar]**.

## Compartir un calendario con un vínculo privado

Puede compartir un vínculo de calendario privado con usuarios de [!DNL Workfront]. Los usuarios deben iniciar sesión para ver el calendario cuando utilicen el vínculo.

1. Seleccione el calendario que desee compartir.
1. Haga clic en el menú **Más** junto al nombre del calendario y luego haga clic en **[!UICONTROL Obtener vínculo compartido]**.
   ![calendario más menú](assets/more-menu-calendar.png)

   >[!NOTE]
   >
   >Los usuarios de [!DNL Workfront] deben tener acceso al calendario para tener acceso a él con el vínculo. Para conceder acceso, consulte [Compartir un calendario con los usuarios de  [!DNL Workfront] ](#share-a-calendar-with-workfront-users).\
   >Si los usuarios no tienen acceso, pueden solicitarlo después de pegar el vínculo en el explorador.
