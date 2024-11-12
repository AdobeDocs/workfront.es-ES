---
title: Creación de objetos de Workfront mediante automatizaciones de registros de Workfront Planning
description: Puede configurar automatizaciones en Workfront Planning para que, cuando se activen, creen objetos en Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: bac3ed2a169e070b541192ab312d4fc1a1b467d1
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# Creación de objetos de Workfront mediante automatizaciones de registros de Workfront Planning

Puede configurar automatizaciones en Workfront Planning para que, cuando se activen, creen objetos en Workfront.

La automatización se activa en los registros. El objeto de Workfront está conectado al registro de Planning donde activó la automatización.

Por ejemplo, puede crear una automatización que tome una campaña de Workfront Planning y cree un proyecto en Workfront para rastrear el progreso de esa campaña. El proyecto estaría conectado a la campaña de Workfront Planning.

Para obtener más información sobre los registros conectados, consulte [Información general sobre los registros conectados](/help/quicksilver/planning/records/connected-records-overview.md).


## Configuración de una automatización en Workfront Planning

Debe configurar una automatización en Workfront Planning para poder utilizarla para crear objetos de Workfront.

1. Haga clic en el menú **Más** ![](assets/more-menu.png) y seleccione **Automaciones**.

   Se abre la lista de automatizaciones disponibles.

1. Haga clic en **Crear nueva automatización** en la esquina superior derecha de la pantalla.
1. En el campo **Texto del botón**, escriba el texto que desea que aparezca en el botón. Los usuarios harán clic en este botón al utilizar la automatización para crear un objeto de Workfront.
1. (Opcional) Para añadir un icono al botón, seleccione un icono de las opciones disponibles.
1. En el campo **Crear un tipo de**, seleccione el objeto que desea que cree la automatización.

   Los objetos disponibles son:

   * Proyecto
   * Portafolio
   * Programar
   * Grupo

1. En el campo **Seleccione el campo que desea utilizar en el nombre del proyecto**, seleccione un campo de registro. El nuevo proyecto de Workfront tendrá el contenido de este campo como nombre.
1. En el campo **Seleccione el campo al que desea vincular el proyecto creado**, seleccione un campo de registro. El nuevo proyecto de Workfront aparecerá en este campo al ver el registro en Workfront Planning.
1. Seleccione otras opciones disponibles para el tipo de objeto que está creando.
1. Haga clic en **Crear**

La automatización aparece en la lista de automatizaciones y está disponible para su uso en registros.

## Utilice una automatización de Workfront Planning para crear un objeto de Workfront

1. En Workfront Planning, abra la página de tipo de registro que contiene los registros que desea utilizar para crear objetos de Workfront.
1. Seleccione uno o varios registros.
1. Haga clic en el botón de automatización cerca de la esquina inferior derecha de la pantalla.

   En este ejemplo, es el botón Crear proyecto.

   ![Botón de automatización](assets/automation-custom-button.png)

>[!NOTE]
>
>Se recomienda comprobar que el objeto se ha creado y conectado según lo esperado.
