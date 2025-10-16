---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configuración del acceso a los modelos
description: Como administrador del sistema, puede habilitar el acceso para que los usuarios soliciten la instalación de modelos configurando una cola de solicitudes para almacenar las solicitudes. Aquí tiene una sola ubicación para rastrear y actualizar solicitudes.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 98%

---

# Configurar el acceso a los modelos

Todos los usuarios de [!DNL Adobe Workfront] pueden examinar el catálogo de modelos.

Como administrador del sistema, puede:

* Añadir [!UICONTROL modelos] al menú principal de las plantillas de diseño y asignar la plantilla de diseño a usuarios o grupos. Para obtener más información, consulte [Personalizar el [!UICONTROL menú principal] con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) y [Asignar usuarios a una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Los usuarios que no tengan una plantilla de diseño asignada verán el icono de [!UICONTROL Modelos] en el [!UICONTROL Menú principal].
  >* Cuando crea una nueva plantilla de diseño, el icono de [!UICONTROL Modelos] se incluye en la lista [!UICONTROL Elementos activos] para el [!UICONTROL Menú principal] de forma predeterminada.


* Habilitar el acceso para que los usuarios soliciten la instalación de modelos configurando una cola de solicitudes para almacenar las solicitudes. Aquí tiene una sola ubicación para rastrear y actualizar solicitudes. Para obtener más información, siga el procedimiento que se describe a continuación.
* Instalar modelos. Para obtener más información, consulte [Instalar un modelo](../../administration-and-setup/blueprints/blueprints-install.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Administrador de Workfront </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos {#prerequisites}

* Debe utilizar una cola de solicitudes existente para almacenar las solicitudes de modelo. El proyecto debe guardarse como una cola de solicitudes y debe estar en el estado [!UICONTROL Actual].
* La cola de solicitudes debe ser pública. En los detalles de la cola de solicitudes, &quot;[!UICONTROL ¿Quién puede añadir solicitudes a esta cola?]&quot; debe establecerse en **[!UICONTROL Cualquiera]**.

>[!TIP]
>
>Si desea crear una nueva cola de solicitudes para solicitudes de modelo, debe crearla antes de configurar el acceso a los modelos. Para obtener información sobre la creación de una cola de solicitudes, consulte [Crear una cola de solicitudes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Seleccionar la cola de solicitudes para almacenar solicitudes de modelo

Para que los usuarios puedan solicitar que se instalen modelos para ellos, debe seleccionar una cola de solicitudes para esas solicitudes. Hasta que se defina la cola de solicitudes, los usuarios solo pueden examinar el catálogo de modelos.

{{step1-to-blueprints}}

1. Haga clic en **[!UICONTROL Configurar solicitudes de modelo]** en la parte superior derecha de la pantalla del catálogo.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. En el cuadro de diálogo **[!UICONTROL Configurar modelos]**, empiece a escribir el nombre de una cola de solicitudes activa y selecciónela cuando aparezca en los resultados de búsqueda.

   >[!IMPORTANT]
   >
   >En esta lista solo aparecen colas de solicitudes públicas. Para convertir en pública su cola de solicitudes, consulte la sección [Requisitos previos](#prerequisites) más arriba.

   Se ha establecido la preferencia de la cola de solicitudes y ahora los usuarios pueden solicitar la instalación del modelo.

   ![Configurar cola de solicitudes](assets/Blueprints_access_setup_request_queue.png)

1. (Opcional) Para realizar cambios en la cola de solicitudes real, haga clic en **[!UICONTROL Editar esta cola de solicitudes]**.

   El proyecto de cola de solicitudes se abre en una nueva pestaña del explorador y se puede actualizar según sea necesario.

1. (Opcional) Si la cola de solicitudes contiene grupos de temas o temas de la cola, puede seleccionarlos en la lista.
1. Para volver al catálogo de modelos, haga clic en **[!UICONTROL Cerrar]**.

>[!NOTE]
>
>Al instalar un modelo solicitado, debe cambiar el estado del problema a **[!UICONTROL Cerrado]** o **[!UICONTROL Resuelto]** en la cola de solicitudes para que se notifique al solicitante. Para obtener información sobre la instalación de un modelo, consulte [Instalar un modelo](../../administration-and-setup/blueprints/blueprints-install.md).
