---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Ver el registro de actividades de Jira
description: Como [!DNL Jira] administrador, puede ver las excepciones y los errores que se producen durante la sincronización o la creación de los tickets entre [!DNL Adobe Workfront] y [!DNL Jira] en un registro de actividades.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Consulte la [!UICONTROL [!DNL Jira] Registro de actividades]

Como [!DNL Jira] administrador, puede ver las excepciones y los errores que se producen durante la sincronización o la creación de los tickets entre [!DNL Adobe Workfront] y [!DNL Jira] en un [!UICONTROL Registro de actividades].

Puede ver hasta 500 elementos en el registro de actividades, que se enumeran a partir de los más recientes.

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
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] información general sobre licencias</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en [!DNL Jira] y [!DNL Workfront] para dedicarse a esta integración, en lugar de usar las existentes que se podrían adjuntar a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Antes de poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe

* Instalar [!DNL Workfront for Jira]

   Para obtener instrucciones sobre la instalación [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Acceda a la [!UICONTROL [!DNL Jira] Registro de actividades]:

1. Inicie sesión en Jira como administrador del sistema.
1. Haga clic en **[!UICONTROL Configuración]** en el [!DNL Jira] para abrir el Navegador.
1. Haga clic en **[!UICONTROL Complementos]**, luego **[!UICONTROL Administrar complementos]**.

1. Expanda el **[!DNL Workfront]** complemento.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Iniciar sesión en [!DNL Workfront] como administrador del sistema.
1. Seleccione el **[!UICONTROL Registro de actividades]** pestaña .

   Vea información sobre excepciones y errores que se produjeron durante la creación de elementos o la sincronización de campos entre las dos aplicaciones.

   El registro incluye los siguientes campos:

   * Fecha de la incidencia
   * El nombre del usuario en Jira
   * Número de problema de Jira
   * Una breve descripción del error que se produjo.
