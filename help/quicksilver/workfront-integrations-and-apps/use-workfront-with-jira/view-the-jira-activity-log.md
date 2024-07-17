---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Ver el registro de actividades de Jira
description: Como administrador, puede ver las excepciones y errores que ocurren durante la sincronización o la creación de los vales entre  [!DNL Adobe Workfront] y [!DNL Jira] en un registro de actividad. [!DNL Jira]
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Ver el registro de actividad [!UICONTROL [!DNL Jira]]

Como administrador de [!DNL Jira], puede ver las excepciones y errores que se producen durante la sincronización o la creación de los vales entre [!DNL Adobe Workfront] y [!DNL Jira] en un [!UICONTROL Registro de actividades].

Puede ver hasta 500 elementos en el registro de actividad y se enumeran a partir de los más recientes.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe [!DNL Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarlas a esta integración, en lugar de usar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre los administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

Para poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe

* Instalar [!DNL Workfront for Jira]

  Para obtener instrucciones sobre la instalación de [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Acceder al registro de actividad [!UICONTROL [!DNL Jira] ]:

1. Inicie sesión en Jira como administrador del sistema.
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haz clic en **[!UICONTROL Complementos]** y luego en **[!UICONTROL Administrar complementos]**.

1. Expanda el complemento **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Inicie sesión en [!DNL Workfront] como administrador del sistema.
1. Seleccione la ficha **[!UICONTROL Registro de actividades]**.

   Ver información sobre excepciones y errores que se produjeron durante la creación de elementos o la sincronización de campos entre las dos aplicaciones.

   El &quot;log&quot; incluye los campos siguientes:

   * Fecha de la incidencia
   * El nombre del usuario en Jira
   * Número de problema de Jira
   * Una breve descripción del error que se produjo.
