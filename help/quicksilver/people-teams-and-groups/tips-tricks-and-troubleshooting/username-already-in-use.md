---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: El nombre de usuario ya está en uso
description: Lea estas sugerencias cuando aparezca un error que indica que el nombre de usuario ya se ha utilizado.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

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
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pregunta

Al crear un usuario nuevo, se crea un [!UICONTROL Whoops] se muestra un error que indica que el nombre de usuario ya se ha tomado. No hay otras ocurrencias de este correo electrónico en el sistema. ¿Por qué se muestra esto?

## Solución

Esto puede ocurrir porque el nombre de usuario o la dirección de correo electrónico no son únicos en la [!DNL Adobe Workfront] instancia. Los usuarios pueden tener el mismo nombre de usuario o dirección de correo electrónico en instancias independientes. Por ejemplo, el usuario A podría tener las siguientes direcciones de correo electrónico asociadas a un [!DNL Workfront] cuenta: usera@company1.com y usera@company2.com.

>[!NOTE]
>
>La variable principal [!DNL Workfront] el administrador no puede tener el mismo nombre de usuario o dirección de correo electrónico si está en instancias de Workfront independientes en el mismo clúster.
>
>Si las instancias están en clústeres diferentes, el administrador principal puede tener el mismo nombre de usuario o dirección de correo electrónico. Puede ver el clúster en el que se encuentra la instancia [!UICONTROL Configuración] > [!UICONTROL Sistema] > [!UICONTROL Información del cliente].

### Compruebe si el nombre de usuario es único en su instancia

Asegúrese de que el nombre de usuario y la dirección de correo electrónico sean únicos en la [!DNL Workfront] instancia:

1. Como [!DNL Workfront] administrador, haga clic en el botón **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Usuarios]**.
1. En la lista de personas, busque en la **[!UICONTROL Correo electrónico]** para asegurarse de que no haya correos electrónicos duplicados.
1. Agregue una columna para el nombre de usuario a la vista.

   1. En el **[!UICONTROL Ver]** menú desplegable, haga clic en **[!UICONTROL Personalizar vista]**.
   1. Haga clic en **[!UICONTROL Agregar columna]**.
   1. En el campo de búsqueda, escriba *[!UICONTROL username]*.
   1. Select **[!UICONTROL Usuario]** > **[!UICONTROL Nombre de usuario]**.
   1. Guarde la vista.\
      Esto da como resultado una vista para mostrar los nombres de usuario donde puede buscar el duplicado.

1. En la lista de personas, busque en la **[!UICONTROL Nombre de usuario]** para asegurarse de que no hay nombres de usuario duplicados.
