---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: El nombre de usuario ya está en uso
description: Lea estas sugerencias cuando obtenga un error que indique que el nombre de usuario ya está en uso.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 1%

---

# El nombre de usuario ya está en uso

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL Administrador del sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pregunta

Al crear un usuario nuevo, aparece un error [!UICONTROL Uy] que indica que el nombre de usuario ya está en uso. No hay más incidencias de este correo electrónico en el sistema. ¿Por qué se muestra esto?

## Solución

Esto puede ocurrir porque el nombre de usuario o la dirección de correo electrónico no son únicos en la instancia actual de [!DNL Adobe Workfront]. Los usuarios pueden tener el mismo nombre de usuario o dirección de correo electrónico en instancias independientes. Por ejemplo, el usuario A podría tener las siguientes direcciones de correo electrónico asociadas con una cuenta de [!DNL Workfront]: usera@company1.com y usera@company2.com.

>[!NOTE]
>
>El administrador principal de [!DNL Workfront] no puede tener el mismo nombre de usuario o dirección de correo electrónico si se encuentran en instancias de Workfront independientes en el mismo clúster.
>
>Si las instancias están en clústeres diferentes, el administrador principal puede tener el mismo nombre de usuario o dirección de correo electrónico. Puede ver el clúster en el que se encuentra su instancia en [!UICONTROL Configuración] > [!UICONTROL Sistema] > [!UICONTROL Información del cliente].

### Compruebe si su nombre de usuario es único en su instancia

Asegúrese de que el nombre de usuario y la dirección de correo electrónico sean únicos en la instancia actual de [!DNL Workfront]:

1. Como administrador de [!DNL Workfront], haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Usuarios]**.
1. En la lista de personas, busque en la columna **[!UICONTROL Correo electrónico]** para asegurarse de que no haya correos electrónicos duplicados.
1. Agregue una columna para el nombre de usuario a la vista.

   1. En el menú desplegable **[!UICONTROL Vista]**, haz clic en **[!UICONTROL Personalizar vista]**.
   1. Haga clic en **[!UICONTROL Añadir columna]**.
   1. En el campo de búsqueda, escriba *[!UICONTROL nombre de usuario]*.
   1. Seleccione **[!UICONTROL Usuario]** > **[!UICONTROL Nombre de usuario]**.
   1. Guarde la vista.\
      Esto da como resultado una vista para mostrar los nombres de usuario donde puede buscar el duplicado.

1. En la lista de personas, busque en la columna **[!UICONTROL Nombre de usuario]** para asegurarse de que no haya nombres de usuario duplicados.
