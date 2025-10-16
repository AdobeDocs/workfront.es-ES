---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Ver el registro de actividades de Jira
description: 'Como administrador, puede ver las excepciones y errores que ocurren durante la sincronización o la creación de los vales entre  [!DNL Jira] y [!DNL Adobe Workfront] en un registro de actividad. [!DNL Jira] '
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 23%

---

# Ver el registro de actividad [!UICONTROL [!DNL Jira]]

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la integración de Workfront para Jira no estará disponible después del **28 de febrero de 2026**.
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Jira.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Jira, consulte [Módulos de software de Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Como administrador de [!DNL Jira], puede ver las excepciones y errores que se producen durante la sincronización o la creación de los vales entre [!DNL Adobe Workfront] y [!DNL Jira] en un [!UICONTROL Registro de actividades].

Puede ver hasta 500 elementos en el registro de actividad y se enumeran a partir de los más recientes.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Acceso a Jira</td> 
   <td> <p>Acceso de administrador del sistema</p> <p>Importante: Se recomienda crear cuentas de administrador del sistema independientes en Jira y Workfront para dedicarlas a esta integración, en lugar de utilizar las existentes que podrían adjuntarse a los usuarios.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder vincular elementos entre [!DNL Workfront] y [!DNL Jira], debe

* Instalar [!DNL Workfront for Jira]

  Para obtener instrucciones sobre la instalación de [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Acceder al registro de actividad [!UICONTROL [!DNL Jira] ]:

1. Inicie sesión en Jira como administrador del sistema.
1. Haga clic en **[!UICONTROL Configuración]** en el menú principal de [!DNL Jira].
1. Haga clic en **[!UICONTROL Complementos]** y luego en **[!UICONTROL Administrar complementos]**.

1. Expanda el complemento de **[!DNL Workfront]**.
1. Haga clic en **[!UICONTROL Configurar]**.
1. Inicie sesión en [!DNL Workfront] como administrador del sistema.
1. Seleccione la ficha **[!UICONTROL Registro de actividades]**.

   Ver información sobre excepciones y errores que se produjeron durante la creación de elementos o la sincronización de campos entre las dos aplicaciones.

   El &quot;log&quot; incluye los campos siguientes:

   * Fecha de la incidencia
   * El nombre del usuario en Jira
   * Número de problema de Jira
   * Una breve descripción del error que se produjo.
