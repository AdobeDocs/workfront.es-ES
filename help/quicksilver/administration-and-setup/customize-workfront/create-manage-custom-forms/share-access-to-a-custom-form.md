---
title: Compartir un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede configurar el acceso de un formulario personalizado para controlar quién (persona, función, grupo, equipo o empresa) puede verlo, compartirlo y editarlo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: f43a0aae33b96f5a061d9134122078d73fc21e40
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---

# Compartir un formulario personalizado

Puede configurar el acceso de un formulario personalizado para controlar quién (persona, función, grupo, equipo o empresa) puede verlo, compartirlo y editarlo.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo conceden este acceso los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Acceso a formularios personalizados {#access-to-custom-forms}

De forma predeterminada, cuando se crea un nuevo formulario personalizado y alguien lo adjunta a un objeto, cualquier usuario asignado al objeto puede ver y rellenar el formulario. Esto incluye a los usuarios con licencias de Solicitud y a los usuarios externos.

Sin embargo, en un objeto en el que el formulario personalizado no está adjunto, un usuario (incluso si tiene un nivel de acceso de Planificador) no puede adjuntarlo desde el menú desplegable Forms personalizado a menos que uno de los siguientes sea verdadero:

* Alguien ha compartido el formulario personalizado con el usuario o con su equipo, función de trabajo, grupo o empresa, concediendo al menos permiso de visualización con la opción Adjuntar a datos personalizados seleccionada
* El usuario tiene una licencia Plan y su nivel de acceso permite el acceso administrativo a los formularios personalizados

## Compartir un formulario personalizado

En lugar de dejar un formulario personalizado en el estado de uso compartido predeterminado (descrito en [Acceso a formularios personalizados](#access-to-custom-forms) en este artículo), puede configurar niveles específicos de acceso al formulario para determinados usuarios, funciones de trabajo, grupos, equipos y empresas.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Seleccione el formulario personalizado y haga clic en **Compartir**.
1. En el cuadro que aparece, debajo de **Proporcionar acceso de formulario personalizado a**, empiece a escribir el nombre del usuario, equipo, función de trabajo, grupo o empresa con la que desee compartir el formulario personalizado y, a continuación, presione **Entrar** cuando se muestre el nombre.
1. Para ajustar el acceso del usuario, equipo, función de trabajo, grupo o empresa que acaba de agregar, haga clic en el menú desplegable a la derecha del nombre y, a continuación, configure una de las siguientes opciones disponibles y cualquiera de sus ajustes avanzados:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verlo</td> 
      <td> <p>Capacidad para ver y rellenar el formulario personalizado en objetos.</p> <p><b>NOTA</b>: Para los usuarios con licencias de trabajo, revisión y solicitud, esta es la opción más alta disponible.</p> <p>Haga clic en <strong>Configuración avanzada</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li><strong>Adjuntar a datos personalizados</strong>: Posibilidad de adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen acceso de gestión</li> 
        <li> <p><strong>Compartir</strong>: Capacidad para compartir el formulario personalizado con otros usuarios del sistema</p> <p>Los usuarios con una licencia de trabajo, revisión o solicitud pueden compartir un formulario personalizado solo a través de la API o un informe de formularios personalizados. Para obtener más información, consulte .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrarlo</td> 
      <td> <p>Disponible solamente para usuarios con una licencia de Plan. </p> <p>Además de poder agregar el formulario a los objetos a los que tienen acceso para editarlo, los usuarios también pueden editar completamente el formulario personalizado, lo que incluye agregar, editar y eliminar campos.</p> <p>Haga clic en <strong>Configuración avanzada</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li> <p><strong>Adjuntar a datos personalizados</strong>: Posibilidad de adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen acceso de gestión</p> </li> 
        <li><strong>Eliminar</strong>: Eliminar el formulario personalizado del sistema</li> 
        <li><strong>Compartir</strong>: Compartir el formulario personalizado con otros usuarios del sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita los pasos del 4 al 5 para agregar otros nombres a la lista y configurar sus opciones.
1. (Opcional) Si desea limitar el acceso al formulario personalizado (en los objetos adjuntos) a los especificados en los pasos anteriores, haga clic en el icono de engranaje ![](assets/gear-icon-settings-with-dn-arrow.jpg) en la esquina superior derecha del cuadro de uso compartido, haga clic en **Eliminar el acceso a todo el sistema**.

   Si cambia de opinión, puede hacer clic en **Hacer que esto sea visible en todo el sistema** (la opción predeterminada).

   >[!NOTE]
   >
   >* Cuando hace visible un formulario personalizado en todo el sistema, permite que los usuarios solo lo vean y lo rellenen en los objetos a los que están asignados, no que lo adjunten a otros objetos. Se puede conceder la capacidad de adjuntar el formulario personalizado a los objetos mediante la opción &quot;Adjuntar a datos personalizados&quot; explicada en el paso 5.
   >* La mayoría de las organizaciones desean garantizar que todos los miembros del sistema puedan rellenar un formulario personalizado cuando esté adjunto a los objetos en los que trabajan y ver sus datos en los informes. Si esto ocurre en su organización, le recomendamos que utilice &quot;**Hacer que esto sea visible en todo el sistema**.&quot; Cuando la opción está configurada de esta manera, aparece &quot;Visible para todo el sistema&quot; en el cuadro de diálogo:

   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Si le preocupa un formulario personalizado en el que los usuarios pueden introducir datos confidenciales cuando están adjuntos a determinados objetos, lo que limita el uso compartido para estos *objetos* puede ser mejor que limitar el acceso al propio formulario.

1. Haga clic en **Guardar**.

## Eliminación del acceso a un formulario personalizado

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Seleccione el formulario personalizado y haga clic en **Compartir**.
1. En el cuadro que aparece, haga clic en la X a la derecha del nombre del usuario, equipo, función, grupo o empresa a los que ya no desee tener acceso especial al formulario.
1. (Opcional) Repita el paso anterior a para los demás nombres que desee eliminar.
1. Haga clic en **Guardar**.
