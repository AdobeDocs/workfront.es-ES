---
title: Personalización de marca en Adobe Workfront mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront o de un grupo, puede utilizar una plantilla de diseño para personalizar los logotipos en el área de navegación superior y en el menú principal para determinados grupos, equipos, funciones y usuarios. Esto resulta especialmente útil en el caso de grupos de una organización grande que tienen su propia personalización de marca.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 90%

---

# Personalización de marca en Adobe Workfront mediante una plantilla de diseño

<!--Audited: 09/2024-->

{{preview-fast-release-general}}

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica solamente a las organizaciones que aún no se han incorporado a [!DNL Adobe Experience Cloud].
>
> Si su organización se ha incorporado a [!DNL Adobe Experience Cloud], la personalización de marca no está disponible.

Puede utilizar una plantilla de diseño para personalizar los logotipos en el área de navegación superior y en el menú principal para determinados grupos, equipos, funciones y usuarios. Esto resulta especialmente útil en el caso de grupos de una organización grande que tienen su propia personalización de marca.

Para obtener información sobre las plantillas de diseño para grupos, consulte [Crear y modificar las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

>[!NOTE]
>
>Un administrador de Workfront puede realizar las mismas personalizaciones de marca para toda la organización a nivel de sistema, tal como se explica en [Personalización de marca de su instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md). Sin embargo, una personalización de marca de una plantilla de diseño anula la personalización de marca del sistema.

<!-- Maybe add a section about deleting these 2 settings to revert to default branding? -->

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
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.</p>
        <p>Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalización de marca en Adobe Workfront mediante una plantilla de diseño

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en la flecha abajo ![Flecha abajo](assets/dropdown-arrow.png) bajo **Personalizar lo que ven los usuarios** y, a continuación, haga clic en **Marca**.
1. Realice cualquiera de los siguientes cambios para personalizar Workfront con imágenes de personalización de marca para los usuarios asignados a esta plantilla de diseño.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Personalice el icono Inicio <span style="font-weight: normal;">(se muestra en el extremo izquierdo del área de navegación superior)</span></p> </td> 
      <td> <p>En la sección <strong>Área de navegación superior</strong>, en <strong>Icono de inicio</strong>, haga clic en cualquier lugar del cuadro y, a continuación, busque y seleccione la imagen de su logotipo. O bien arrastre una imagen en el cuadro.</p> <p>Para recortar la imagen, utilice los controles de desplazamiento y arrastre la imagen a la posición que desee dentro del espacio especificado.</p> <p>Recomendamos una imagen de 120 x 120. Puede tener cualquiera de los siguientes formatos: GIF, JPG, PNG o SVG.</p> <p>Este icono también aparece en informes, listas, tableros e informes enviados que los usuarios exportan como archivos de PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Personalizar el logotipo de la marca del menú principal <img src="assets/main-menu-icon.png"> <span style="font-weight: normal;"> (se muestra en la esquina superior derecha del menú principal)</span></p> </td> 
      <td> <p> <p> <p>En la sección <strong>Área de navegación superior</strong>, en el <strong>Logotipo del menú principal</strong>, haga clic en cualquier lugar del cuadro y, a continuación, busque y seleccione la imagen de su logotipo. O bien arrastre una imagen en el cuadro.</p> <p>Para recortar la imagen, utilice los controles de desplazamiento y arrastre la imagen a la posición que desee dentro del espacio especificado.</p> <p>Recomendamos una imagen de 300 x 120 píxeles. Puede tener cualquiera de los siguientes formatos: GIF, JPG, PNG o SVG.</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. <span class="preview">En el entorno de vista previa: continúe personalizando la plantilla de diseño. Puede hacer clic en **Aplicar** en cualquier momento para guardar el progreso.</span>

   <span class="preview">O</span>

   <span class="preview">Si ha terminado de personalizar, haga clic en **Guardar y cerrar**.</span>

1. En el entorno de producción: continúe personalizando la plantilla de diseño.

   O

   Si ha terminado la personalización, haga clic en **Guardar**.

   >[!TIP]
   >
   >Puede hacer clic en **Guardar** en cualquier momento para guardar el progreso y luego seguir modificando la plantilla más adelante.

Para obtener más información sobre las plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
