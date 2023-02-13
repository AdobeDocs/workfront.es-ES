---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configuración del acceso a los modelos
description: Como administrador del sistema, puede habilitar el acceso para que los usuarios soliciten la instalación de modelos configurando una cola de solicitudes para almacenar las solicitudes. Aquí tiene una sola ubicación para realizar el seguimiento y actualizar las solicitudes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Configuración del acceso a los modelos

Todo [!DNL Adobe Workfront] los usuarios pueden examinar el catálogo de modelos.

Como administrador del sistema, puede:

* Agregar [!UICONTROL Planes] en plantillas de diseño y asigne la plantilla de diseño a usuarios o grupos. Para obtener más información, consulte [Personalice el [!UICONTROL Menú principal] uso de una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) y [Asignar usuarios a una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* Los usuarios que no tengan una plantilla de diseño asignada verán la variable [!UICONTROL Planes] en el [!UICONTROL Menú principal].
   >* Al crear una nueva plantilla de diseño, la variable [!UICONTROL Planes] se incluye en la variable [!UICONTROL Elementos activos] para [!UICONTROL Menú principal] de forma predeterminada.



* Habilite el acceso para que los usuarios soliciten la instalación de modelos configurando una cola de solicitudes para almacenar las solicitudes. Aquí tiene una sola ubicación para realizar el seguimiento y actualizar las solicitudes. Para obtener más información, siga el procedimiento a continuación.
* Instale modelos. Para obtener más información, consulte [Instalación de un modelo](../../administration-and-setup/blueprints/blueprints-install.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licencia</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos {#prerequisites}

* Debe utilizar una cola de solicitudes existente para almacenar solicitudes de modelo. El proyecto debe guardarse como cola de solicitud y debe estar en [!UICONTROL Actual] estado.
* La cola de solicitud debe ser pública. En los detalles de la cola de solicitudes, &quot;[!UICONTROL ¿Quién puede añadir solicitudes a esta cola?]&quot; debe estar definido como **[!UICONTROL Cualquiera]**.

>[!TIP]
>
>Si desea crear una nueva cola de solicitudes para solicitudes de modelo, debe crearla antes de configurar el acceso a los modelos. Para obtener información sobre la creación de una cola de solicitudes, consulte [Crear una cola de solicitud](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Seleccione la cola de solicitud para almacenar solicitudes de modelo

Para que los usuarios puedan solicitar que instale modelos, debe seleccionar una cola de solicitudes para dichas solicitudes. Hasta que se defina la cola de solicitud, los usuarios solo podrán examinar el catálogo de modelos.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Planes]**.
1. Haga clic en **[!UICONTROL Configuración de solicitudes de modelo]** en la parte superior derecha de la pantalla del catálogo.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. En el **[!UICONTROL Configuración de modelos]** , empiece a escribir el nombre de una cola de solicitudes activa y selecciónela cuando aparezca en los resultados de búsqueda.

   >[!IMPORTANT]
   >
   >En esta lista solo aparecen las colas de solicitud pública. Para que la cola de solicitudes sea pública, consulte la [Requisitos previos](#prerequisites) sección anterior.

   Se establece la preferencia de cola de solicitud y los usuarios ahora pueden solicitar la instalación del modelo.

   ![Configurar cola de solicitud](assets/Blueprints_access_setup_request_queue.png)

1. (Opcional) Para realizar cambios en la cola de solicitudes real, haga clic en **[!UICONTROL Editar esta cola de solicitudes]**.

   El proyecto de cola de solicitudes se abre en una nueva pestaña del explorador y puede actualizarlo según sea necesario.

1. (Opcional) Si la cola de solicitud contiene grupos de temas o temas de cola, puede seleccionarlos de la lista.
1. Para volver al catálogo de modelos, haga clic en **[!UICONTROL Cerrar]**.

>[!NOTE]
>
>Al instalar un modelo solicitado, debe cambiar el estado del problema a **[!UICONTROL Cerrado]** o **[!UICONTROL Resuelto]** en la cola de solicitudes para que se notifique al solicitante. Para obtener información sobre cómo instalar un modelo, consulte [Instalación de un modelo](../../administration-and-setup/blueprints/blueprints-install.md).
