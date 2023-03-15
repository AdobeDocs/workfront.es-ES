---
title: Organizar y previsualizar un formulario con el Diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede organizar un formulario personalizado con el Diseñador de formularios.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 529de9d31be883325d425dceb286d750397c5d8e
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# Organizar y previsualizar un formulario con el diseñador de formularios

{{highlighted-preview-article-level}}

Puede organizar un formulario personalizado con el diseñador de formularios.

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
   <td>
   <p>Plan actual: Estándar</p>
   <p>o</p>
   <p>Plan heredado: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Agregar un salto de sección

Puede agrupar los campos personalizados y las utilidades de un formulario personalizado en secciones con encabezados. Esto resulta útil para presentar una experiencia organizada a los usuarios que rellenen el formulario. Además, si necesita limitar el acceso a ciertos campos y utilidades personalizados a ciertos usuarios, puede colocarlos en una sección y, a continuación, conceder acceso a la sección únicamente a esos usuarios.

Por ejemplo, si necesita realizar un seguimiento de la información confidencial que solo los administradores del sistema deben poder ver o editar, puede crear un salto de sección con los permisos Solo administrador y colocar los campos confidenciales en esa sección.

La configuración de acceso que seleccione para una sección está directamente vinculada a los permisos que los usuarios tienen en el objeto Workfront al que está adjunto el formulario personalizado. Puede ocultar o mostrar una sección en función de si el usuario tiene acceso para ver, contribuir o administrar ese objeto. O puede establecer una sección en Solo administración para que solo puedan acceder a ella los usuarios con un nivel de acceso de administrador del sistema.

Para obtener información sobre los permisos de los objetos, consulte [Información general sobre cómo compartir permisos en objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obtener información sobre los campos personalizados y las utilidades de los formularios personalizados, consulte [Diseño de un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Crear y configurar el acceso a una sección en un formulario personalizado

1. Comience a crear o editar un formulario personalizado y a agregar campos, tal como se describe en [Diseño de un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Salto de sección** y arrástrela a la posición deseada en el lienzo.

1. En el panel derecho, configure las opciones que desee para la sección :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima de la sección. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba texto si desea explicar a los usuarios para qué es la sección. Se muestra debajo de la etiqueta de la sección en el formulario personalizado.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Conceder acceso</p> </td> 
      <td> <p> Seleccione los permisos que necesitan los usuarios en un objeto al que esté adjunto el formulario personalizado para ver esta sección y editar sus valores de campo. 
       <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden ver los valores de los campos</b>:</p> 
         <ul>  
          <li><p><b>Edición limitada</b>: (Disponible solo si el objeto es un proyecto, una tarea, un problema o un usuario):</p> 
          <p>Permite a los usuarios contribuir al objeto si se trata de un proyecto, una tarea o un problema.</p>
          <p>Permite a los usuarios editar el perfil o poseer el permiso de perfil del objeto si se trata de un usuario.</p></li> 
          <li><b>Editar</b>: Administrar permisos en el objeto </li> 
          <li><b>Solo administrador</b>: Nivel de acceso del administrador del sistema</li> 
         </ul> </li> 
        <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden editar los valores de los campos</b>: </p> 
         <ul> 
          <li> <p><b>Edición limitada</b>: (Disponible solo si el objeto es un proyecto, una tarea, un problema o un usuario):</p> 
           <p>Si el objeto es un proyecto, una tarea o un problema, este permiso permite a los usuarios contribuir al objeto</p>
          <p>Si el objeto es un usuario, este permiso permite a los usuarios editar el perfil o poseer el permiso de perfil del objeto.</p> 
          <li><b>Editar</b>: Administrar permisos en el objeto </li> 
          <li><b>Solo administrador</b>: Nivel de acceso del administrador del sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Para obtener información sobre los permisos de los objetos, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre cómo compartir permisos en objetos</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Los usuarios sin los permisos especificados aquí no pueden ver los campos personalizados y las utilidades de la sección . </p> <p>Esto también ocurre si se muestran los valores de los campos en los informes o se utilizan en campos calculados en los informes de modo de texto.</p> </li> 
       <li> <p>La asociación de varios tipos de objetos con el formulario puede cambiar los permisos de visualización y edición disponibles en estos pasos. Para obtener más información, consulte <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección en un formulario personalizado</a> en este artículo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Arrastre o agregue al menos un campo o widget personalizado a la nueva sección. Esto es necesario antes de guardar la sección.

1. Haga clic en **Listo**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras esté creando un formulario personalizado para guardar los cambios y mantener el formulario abierto.

### Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Los saltos de sección de permisos de edición limitada para formularios personalizados solo están disponibles para los tipos de objeto Proyecto, Tarea, Problema y Usuario.

En un formulario personalizado con un salto de sección configurado con el permiso de edición limitada, si agrega uno de los otros tipos de objeto al formulario (Portfolio, Programa, Documento, Empresa, Registro de Facturación, Iteración, Gastos o Grupo), se le pedirá que cambie al permiso de edición, que es compatible tanto con ese tipo de objeto como con los tipos de objeto existentes en el formulario.

>[!INFO]
>
>**Ejemplo:** En un formulario personalizado asociado con el tipo de objeto Project , se configura un salto de sección con el permiso de edición limitada.
>
>El tipo de objeto Portfolio se agrega al formulario, lo que significa que la opción de permiso Editar limitado ya no está disponible para el salto de sección del formulario.
>
>Un mensaje en pantalla le pedirá que cambie al permiso Editar, que es el nivel mínimo de permisos compatible tanto con el tipo de objeto Proyecto como con el tipo de objeto Portfolio.


## Colocación de campos y widgets personalizados en un formulario personalizado


1. Comience a crear o editar un formulario personalizado, tal como se describe en [Diseño de un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Para colocar los campos personalizados y las utilidades en la misma fila, arrastre uno junto al otro hasta que aparezca una línea entre ellos.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* Puede usar la variable **Vista previa** en la esquina superior derecha para obtener una idea de cómo se mostrarán los campos personalizados y las utilidades en el formulario.
>* Es posible que los campos personalizados y las utilidades no siempre se muestren del mismo modo en el formulario, dependiendo de cuánto espacio de pantalla esté disponible cuando el usuario lo vea. Por ejemplo, el tercer campo de una fila de campos puede ajustarse a la siguiente fila de campos si el espacio horizontal está limitado.


1. (Opcional) Para colocar un campo o widget personalizado encima o debajo de otro, arrástrelo por encima o por debajo hasta que aparezca una línea azul horizontal entre los elementos.

1. Para guardar los cambios, haga clic en **Aplicar**

   o

   Haga clic en **Guardar y cerrar**.

## Vista previa de un formulario personalizado

1. Comience a crear o editar un formulario personalizado y a agregar campos, tal como se describe en [Diseño de un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Vista previa** en la esquina superior izquierda para ver el aspecto que tendrá el formulario cuando se utilice, haga clic en **Finalizar vista previa** para volver a la edición del formulario.