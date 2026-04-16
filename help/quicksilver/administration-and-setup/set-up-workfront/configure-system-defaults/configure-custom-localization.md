---
user-type: administrator
product-area: system-administration;setup
title: Configurar la localización personalizada
description: La localización personalizada le permite definir términos y frases personalizados en diferentes idiomas. A continuación, Workfront muestra estos términos en el idioma establecido en la configuración del explorador.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
source-git-commit: 28178c3794832e14552d988259c1792a6fed1da1
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 19%

---

# Configuración de la localización personalizada

La localización personalizada le permite definir términos y frases personalizados en diferentes idiomas. A continuación, Workfront muestra estos términos en el idioma establecido en la configuración de Adobe Identity Management (IMS) del usuario. Si el usuario no está en Adobe IMS, los términos se muestran en el idioma establecido en la configuración del explorador del usuario.

Por ejemplo, puede establecer la etiqueta &quot;Audiencia objetivo&quot; para que se traduzca a la palabra alemana &quot;Zielgruppe&quot;. Cualquier usuario con el alemán seleccionado como idioma principal del navegador ve la palabra &quot;Zielgruppe&quot; como una etiqueta para cualquier campo etiquetado como &quot;Audiencia objetivo&quot; en inglés.

Puede configurar las traducciones a varios idiomas. Los idiomas disponibles actualmente incluyen:

* Chino (tradicional)
* Chino (simplificado)
* Francés
* Alemán
* Italiano
* Japonés
* Coreano
* Portugués (Brasil)
* Español

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Flujo de trabajo Prime o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront para configurar las traducciones.</p>  </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al configurar la localización

Tenga en cuenta lo siguiente al configurar la localización:

* Puede configurar un término para traducirlo a varios idiomas.
* La localización se aplica a las etiquetas de campo personalizado (incluso cuando se utiliza como encabezado de columna) y a la información sobre herramientas.
* La localización personalizada puede aplicarse a mensajes generados a partir de reglas de negocio, pero debe habilitarse en la regla de negocio.

  Para obtener instrucciones, vea [Habilitar la localización en una regla de negocio](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) en el artículo Crear y editar reglas de negocio.

## Configuración de traducciones

Las traducciones se configuran en el área de Configuración.

1. Haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o, si está disponible, haga clic en el icono **[!UICONTROL Main Menu]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Setup]** ![Icono de Configuración](/help/_includes/assets/gear-icon-setup.png).
1. En el área Configuración, haga clic en **Localización** en el panel de navegación izquierdo.
1. Para agregar una nueva traducción, haga clic en **Nueva fila**.
1. En la columna **English**, escriba el término en inglés que se debe traducir.
1. En la columna del idioma al que desee traducir el término, introduzca el término en el idioma de destino.
1. Para traducir la palabra a otros idiomas, añada la traducción a la columna de idioma correspondiente.
1. Para reordenar las columnas de idioma, haga clic en el encabezado de la columna que desee mover y arrástrela a la ubicación deseada.
