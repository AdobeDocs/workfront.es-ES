---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Este nombre de usuario ya se está utilizando
description: Lea estas sugerencias cuando obtenga un error que indique que el nombre de usuario ya está en uso.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 722295463c1338a70ff42c26acf69b09cf33f725
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 97%

---

# El nombre de usuario ya está en uso

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Administrador del sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pregunta

Al crear un usuario nuevo, aparece el error [!UICONTROL Uy] que indica que el nombre de usuario ya está en uso. No hay más incidencias de este correo electrónico en el sistema. ¿Por qué se muestra esto?

## Solución

Esto puede ocurrir porque el nombre de usuario o la dirección de correo electrónico no son únicos en la instancia actual de [!DNL Adobe Workfront]. Los usuarios pueden tener el mismo nombre de usuario o dirección de correo electrónico en instancias independientes. Por ejemplo, el usuario A podría tener las siguientes direcciones de correo electrónico asociadas con una cuenta de [!DNL Workfront]: usera@company1.com y usera@company2.com.

>[!NOTE]
>
>El administrador principal de [!DNL Workfront] no puede tener el mismo nombre de usuario o dirección de correo electrónico si se encuentran en instancias de Workfront independientes en el mismo clúster.
>
>Si las instancias están en clústeres diferentes, el administrador principal puede tener el mismo nombre de usuario o dirección de correo electrónico. Puede ver el clúster en el que se encuentra su instancia en [!UICONTROL Setup] > [!UICONTROL System] > [!UICONTROL Customer Info].

### Comprobar si su nombre de usuario es único en su instancia

Asegúrese de que el nombre de usuario y la dirección de correo electrónico sean únicos en la instancia actual de [!DNL Workfront]:

{{step-1-to-users}}

1. En la lista de personas, busque en la columna **[!UICONTROL Email]** para asegurarse de que no haya correos electrónicos duplicados.
1. Añada una columna para el nombre de usuario a la vista.

   1. En el menú desplegable **[!UICONTROL View]**, haga clic en **[!UICONTROL Customize View]**.
   1. Haga clic en **[!UICONTROL Añadir columna]**.
   1. En el campo de búsqueda, escriba *[!UICONTROL username]*.
   1. Seleccione **[!UICONTROL User]** > **[!UICONTROL Username]**.
   1. Guarde la vista.\
      Esto da como resultado una vista para mostrar los nombres de usuario donde puede buscar el duplicado.

1. En la lista de personas, busque en la columna **[!UICONTROL Username]** para asegurarse de que no haya nombres de usuario duplicados.
