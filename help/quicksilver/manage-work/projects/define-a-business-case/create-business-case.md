---
navigation-topic: business-case-and-scorecards
title: Creación de un caso empresarial para un proyecto
description: Puede utilizar el caso empresarial para solicitar un proyecto y definir el propósito, el presupuesto y el beneficio potencial del proyecto. El administrador de Portafolios o el patrocinador del proyecto utilizan la información del caso empresarial para analizar y priorizar el proyecto antes de aprobarlo.
author: Becky
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 63%

---

# Creación de un caso empresarial para un proyecto

<!--Audited: 6/2025-->

Puede utilizar el caso empresarial para solicitar un proyecto y definir el propósito, el presupuesto y el beneficio potencial del proyecto. El administrador de Portafolios o el patrocinador del proyecto utilizan la información del caso empresarial para analizar y priorizar el proyecto antes de aprobarlo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront</p></td> 
   <td> 
   <p>Prime o superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td> 
   <p>Estándar </p> 
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td> 
   <td> <p>Editar acceso a Proyectos, Datos financieros y Administración de recursos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Administrar permisos superiores en el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Tenga en cuenta lo siguiente al solicitar un proyecto a través de un caso empresarial:

* El administrador de Adobe Workfront o del administrador de grupos debe habilitar las secciones del caso empresarial para que aparezcan en el proyecto.\
  Para obtener información acerca de cómo habilitar las secciones del caso empresarial en el sistema, consulte el artículo [Configurar las preferencias del proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Para obtener información acerca de las áreas del caso empresarial, vea el artículo [Información general de las áreas del caso empresarial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Debe completar todas las áreas del caso empresarial, excepto el área de metas, si desea que el proyecto reciba una puntuación en el Optimizador de portafolios. Completar el área de Metas es opcional. El proyecto recibe una puntuación en el Optimizador de portafolios aunque esta área no esté completada.

  Para obtener información sobre cómo trabajar con cuadros de resultados y con el Optimizador de portafolios, consulte el artículo [Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Creación de un caso empresarial

{{step1-to-projects}}

1. Haga clic en **Nuevo proyecto** y, a continuación, seleccione **Solicitar proyecto** en la lista desplegable que aparece. El proyecto se crea y el estado **Idea** se asigna de manera predeterminada.

   >[!CAUTION]
   >
   >Si el estado de Idea se ha eliminado en la instancia de Workfront, el proyecto se coloca en el estado predeterminado para nuevos proyectos, tal como se define en el área Preferencias del proyecto. Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias del proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Escriba un nombre en el campo Título del proyecto.
1. (Opcional) Haga clic en el icono **Más** ![Icono de más](assets/qs-more-icon-on-an-object.png) y, a continuación, **Adjuntar plantilla** para crear la estructura de desglose de trabajo de su proyecto.

   O

   Empiece a añadir tareas al proyecto manualmente.

1. (Condicional) Si ha seleccionado adjuntar una plantilla, continúe adjuntándola al proyecto.
1. En el panel izquierdo, haga clic en **Caso comercial**.
1. (Opcional) Para editar la sección **Información del proyecto**, haga clic en **Editar información del proyecto**.

   Para obtener más información sobre cómo editar los campos de sección **Información del proyecto**, consulte la sección [Información del proyecto](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) en el artículo [Información general sobre las áreas del caso empresarial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Para editar la sección **Metas**, haga clic en **Editar metas**.

   Para obtener más información acerca de cómo editar la sección **Goals** del caso comercial, vea la sección [Goals](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) en el artículo [Overview of the Areas of the Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Para editar la sección **Gastos**, haga clic en **Editar gastos**.

   Para obtener más información sobre cómo editar la sección **Gastos** del caso comercial, consulte la sección [Gastos](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) en el artículo [Información general sobre las áreas del caso comercial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Haga clic en **Editar presupuesto de recursos** para presupuestar sus recursos y obtener el costo de mano de obra presupuestado asociado con los roles del proyecto. Para obtener más información, consulte [Recursos de presupuesto en el caso empresarial](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >La información que se muestra aquí es la misma que la que aparece en las herramientas de presupuestación de recursos en el sistema.

1. (Opcional) Haga clic en **Editar riesgos** para agregar posibles riesgos a este proyecto. Para obtener información acerca de cómo añadir riesgos al caso empresarial, vea la sección [Riesgos](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) en el artículo [Información general sobre las áreas del caso empresarial](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Opcional) Seleccione un **informe de valoración** en el menú desplegable **Agregar un informe de valoración a este proyecto**.

   Se deben crear cuadros de resultados para poder adjuntarlos a los proyectos.

   Para obtener más información sobre los cuadros de resultados, vea el artículo [Aplicar un cuadro de resultados a un proyecto y generar una puntuación de alineación](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Opcional) Seleccione un **Formulario personalizado** en el menú desplegable **Formularios personalizados**.

   Se deben crear formularios personalizados para poder adjuntarlos a los proyectos.

   Para obtener más información acerca de Forms personalizado, vea el artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Enviar**. El estado del proyecto se cambió a **Solicitado** y se envía para que se apruebe el caso empresarial.

   Para obtener más información acerca de cómo aprobar un caso empresarial, vea el artículo [Aprobar un caso empresarial](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> Después de completar el caso empresarial, puede exportar una copia a un archivo .pdf. Para obtener más información sobre cómo exportar el caso empresarial a un archivo .pdf, vea [Exportar el caso empresarial de un proyecto](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).


