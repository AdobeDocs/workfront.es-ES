---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Agregue un campo personalizado a un formulario personalizado con el creador de formularios heredado
description: Cuando se trabaja en un formulario personalizado, se puede crear un nuevo campo personalizado y agregarlo a un formulario personalizado. También puede agregar un campo personalizado que ya se haya agregado a otro formulario personalizado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: f9fce2715cad3e2ea2bf16de5f4ba457f981725c
workflow-type: tm+mt
source-wordcount: '2264'
ht-degree: 3%

---

# Agregue un campo personalizado a un formulario personalizado con el creador de formularios heredado

Cuando se trabaja en un formulario personalizado, se puede crear un nuevo campo personalizado y agregarlo a un formulario personalizado.

También puede agregar un campo personalizado que ya se haya agregado a otro formulario personalizado. Para obtener instrucciones, consulte [Reutilizar un campo o un widget personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Para obtener información sobre cómo agregar un widget de recursos a un formulario personalizado, que es un proceso similar a agregar un campo personalizado, consulte [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>En un formulario personalizado que contiene muchos campos personalizados o muchas opciones de selección múltiple en campos personalizados, los usuarios pueden experimentar un rendimiento más lento al agregar o cambiar valores en esos campos. Por ejemplo, un formulario que contenga 100 campos personalizados o campos personalizados de selección múltiple con más de 200 opciones, puede ser más lento cuando los usuarios interactúan con él.

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
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Añadir un campo personalizado a un formulario personalizado

1. Comience a crear o editar un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Abra el **Añadir un campo** pestaña .

   ![](assets/add-a-field.jpg)

1. con **Campo nuevo** ![](assets/new-field.jpg) seleccione uno de los tipos de campo que se enumeran a continuación:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Campo de texto de línea única</td> 
      <td>Permite a los usuarios escribir una sola línea de texto en el campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo de texto de párrafo</td> 
      <td>Permite a los usuarios escribir varias líneas de texto en el campo.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Campo de texto con formato</td> 
      <td>Permite a los usuarios escribir varias líneas de texto en el campo y dar formato al texto con negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque. Esta opción está disponible en Inicio, el área Actualizaciones, las listas y el área Detalles de los objetos de Workfront. Un límite de caracteres de 15.000 permite un montón de texto y formato.</p> <p>Para obtener información sobre el acceso a este campo a través de la API, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Almacenamiento de campos de texto enriquecido en la API</a>.</p> <p><b>NOTA</b>: Los campos de texto con formato no están disponibles para las aplicaciones móviles de Workfront (disponibles en las próximas versiones). </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lista desplegable</td> 
      <td>Proporciona una lista de opciones desplegables.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Escritura anticipada </td> 
      <td>Permite a los usuarios escribir el nombre de un objeto que existe en Workfront. Cuando el usuario empieza a escribir, aparece una lista de sugerencias.
      Este tipo de campo admite los siguientes objetos:
      <ul><li>Usuario</li>
      <li>Grupo</li>
      <li>Función</li>
      <li>Portafolio</li>
      <li>Programar</li>
      <li>Proyecto</li>
      <li>Equipo</li>
      <li>Plantilla</li>
      <li>Compañía</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calculado</td> 
      <td>Permite definir una expresión y mostrar el resultado en el formulario personalizado. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Agregar datos calculados a un formulario personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha</td> 
      <td>Muestra un calendario en el que los usuarios pueden seleccionar una fecha y una hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Casillas de verificación</td> 
      <td>Permite a los usuarios seleccionar varias opciones.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botones de radio</td> 
      <td>Requiere que los usuarios seleccionen solo una opción.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descriptivo</td> 
      <td>Permite incluir instrucciones y vínculos a páginas fuera de Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Salto de sección</td> 
      <td>Un salto de sección en realidad no es un campo. Puede utilizar un salto de sección para organizar los campos personalizados y las utilidades en secciones y, si es necesario, configurar diferentes permisos de visualización y edición para cada sección. Para obtener información sobre cómo agregar y configurar saltos de sección, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Agregar un salto de sección a un formulario personalizado</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Configuración de campos** , configure las opciones disponibles para el tipo de campo personalizado que está agregando:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es el modo en que el sistema identifica el campo personalizado cuando lo agrega a varias áreas de Workfront, como informes, Inicio e interacciones de API.</p> <p>Cuando configura el campo personalizado por primera vez y escribe la etiqueta, el campo Nombre se rellena automáticamente para que coincida con él. Sin embargo, los campos Etiqueta y Nombre no están sincronizados: esto le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a usar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado en el que podría hacerse referencia a él en otras áreas de Workfront. <p>Por ejemplo, si agrega el campo personalizado a un informe y más tarde cambia su nombre, Workfront no lo reconoce en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.</p> </li>
      <li> <p>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.</p> </li>
      <li><p>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.</p></li>
      </ul> <p>Cada nombre de campo personalizado debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar una que ya se haya creado para otro formulario personalizado. Para obtener más información, consulte <a href="#Add" class="MCXref xref">Añadir un campo personalizado a un formulario personalizado</a> en este artículo.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el campo personalizado. Cuando los usuarios rellenen el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver una información que contenga la información que escriba aquí.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Seleccione el tipo de datos que desea capturar en el campo personalizado. Puede cambiar la selección de formato después de guardar el formulario, pero el nuevo formato debe admitir el valor introducido.</p>

   <p><strong>Ejemplo:</strong> Si guarda un valor numérico para un campo con formato de texto en al menos un objeto y cambia el formato a Número o Moneda posteriormente, no se producirá un error. </p>
      <p>Sin embargo, si guarda un valor alfanumérico en un campo con formato de texto en al menos un objeto y después intenta cambiar el formato a Número o Moneda, se producirá un error porque el valor alfanumérico guardado no es compatible con los formatos Número o Moneda. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de presentación</td> 
      <td>(Solo botones de menú desplegable, casillas de verificación y radio) Cambie el tipo de selección de opciones que desee para el campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamaño</td> 
      <td>(Solo campos de texto) Seleccione una anchura para el campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar hora del día</td> 
      <td>(Solo campos de fecha) Seleccione esta opción si desea mostrar la hora del día junto con la fecha en el campo .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto referenciado</td> 
      <td> <p>(Solo campos Typeforward) Seleccione el tipo de objeto que desea asociar al campo.</p> <p>Una vez que haya hecho clic en Aplicar o en Guardar+Cerrar, no podrá cambiar el tipo de objeto del campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Si el administrador de Workfront ha personalizado el nombre para Portfolio, Programas o Proyectos en la interfaz de usuario de Workfront, el nombre predeterminado de Workfront para el objeto aparece en esta lista desplegable, no en el nombre personalizado. Consulte con el administrador de Workfront si necesita ayuda con esto.<br></li> 
         <li>Los siguientes tipos de objetos son compatibles con las aplicaciones móviles iOS y Android Workfront : Usuario, Empresa, Grupo, Función de trabajo, Portfolio, Programa, Proyecto y Plantilla.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Agregar filtro</td> 
      <td> <p>(Solo campos Typeforward) Añada un filtro para un tipo de objeto para limitar los objetos que los usuarios pueden elegir cuando utilizan el campo. </p> <p>Por ejemplo, puede limitar un campo para que los nombres de usuario solo se puedan seleccionar si cumplen los siguientes criterios:</p> 
       <ul> 
        <li>Pertenecen a uno o varios grupos que especifique</li> 
        <li>Están asociados a una función o un puesto que especifique</li> 
        <li>Pertenecen al mismo grupo que la persona que utiliza el campo</li> 
       </ul> <p>Debe definir el filtro para el tipo de objeto seleccionado mediante la sintaxis del modo de texto. Para obtener información sobre la creación de un filtro mediante el modo de texto, consulte la sección <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">Editar el modo de texto en un filtro</a> en el artículo <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Información general sobre el modo de texto</a>. </p> <p><b>NOTA</b>:   
        <ul> 
         <li>Si está editando un formulario personalizado existente, agregar un filtro a un campo de Typeforward no elimina ningún objeto (fuera del ámbito del filtro) que los usuarios ya hayan agregado usando el campo.</li> 
         <li>Este filtro no está disponible en dispositivos móviles. Si utiliza el filtro para un campo Typeforward , el campo aparecerá en los dispositivos móviles de los usuarios sin que el filtro lo afecte.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descriptivo</td> 
      <td>(Solo campos de texto descriptivo) Escriba el texto que desea mostrar para proporcionar instrucciones o un vínculo en el formulario personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hipervínculo</td> 
      <td>(Solo campos de texto descriptivo) Si desea aplicar un hipervínculo al texto descriptivo que ha escrito, agréguelo aquí.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cambiar un campo a obligatorio</td> 
      <td>Seleccione esta opción si desea que el campo sea obligatorio para que el usuario complete el formulario personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seguir cambios de los campos en las fuentes de actualización</td> 
      <td><p>Haga clic en la lista desplegable y, a continuación, seleccione los tipos de objeto en los que desea rastrear automáticamente los cambios de valor del campo.</p> 
      <p><b>NOTA</b>: Esta opción no está disponible para lo siguiente:</p> 
      <ul> 
      <li>Formularios personalizados asociados a los siguientes tipos de objetos: Gastos, Empresa, Iteración, Registro de Facturación y Grupo.</li> 
      <li>Los siguientes tipos de campo: Texto calculado , Texto descriptivo y Salto de sección</li> 
      </ul>
      <p><b>IMPORTANTE</b>: Seleccionar o anular la selección de un tipo de objeto aquí afecta a todos los formularios personalizados asociados al tipo de objeto seleccionado y que contienen este campo. Por ejemplo, si anula la selección de un tipo de objeto aquí y guarda el formulario personalizado, ya no se realiza un seguimiento de los cambios de valor del campo para ese tipo de objeto en cualquier formulario personalizado que contenga el campo.</p>
       <p>Después de seleccionar un tipo de objeto aquí para un campo y guardar el formulario personalizado, el campo aparece en la ficha Campos personalizados del área Actualizar fuentes en Configuración.</p> 
       <p>Por el contrario, si este campo se elimina del área Actualizar fuentes de Configuración, el tipo de objeto de esta configuración no se selecciona en todos los formularios personalizados que estén asociados al tipo de objeto y que contengan este campo.</p> 
       <p>Para obtener más información, consulte la sección <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">Añada los campos que desee que Workfront rastree</a> en el artículo <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">Configurar actualizaciones del sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agregar lógica</td> 
      <td>Especifique qué campos deben aparecer en el formulario, según las selecciones que realicen los usuarios en los campos existentes. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Agregar lógica de visualización y de omisión de lógica a un formulario personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opciones </td> 
      <td> <p>(Solo desplegables, casillas de verificación o botones de opción); opcional)</p> 
       <ol> 
        <li> <p>Haga clic en <b>Opciones</b>y, a continuación, active cualquiera de las siguientes opciones:</p> 
           <ul> 
            <li><strong>Mostrar valores</strong>: Muestra los valores de cada opción en el campo . La etiqueta de cada opción se muestra de forma predeterminada.</li> 
            <li><strong>Opciones de orden A-Z</strong>: Ordena las opciones que se agregan alfabéticamente en el campo.</li> 
           </ul> 
        </li> 
        <li> <p>Para cada opción que añada para el usuario, haga clic en el icono de engranaje <img src="assets/gear-icon-settings.png">y, a continuación, seleccione una de las siguientes opciones:</p> 
           <ul> 
            <li><strong>Seleccionar por defecto</strong>: Seleccione la opción de forma predeterminada en el campo .</li> 
            <li> <p><strong>Ocultar opción</strong>: Oculte la opción en el campo . Las opciones ocultas siguen siendo accesibles en los informes.</p> </li> 
            <li> <p><strong>Eliminar opción</strong>: Elimine la opción del campo .</p> <p><b>ADVERTENCIA</b>: Si tiene objetos actuales utilizando esta opción, no la elimine del campo. Si se elimina, se perderán datos históricos. En su lugar, seleccione la opción para ocultarla, lo que impide que los usuarios la seleccionen en el futuro.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Para cambiar el tipo de visualización de un campo en el formulario personalizado, haga clic en el botón **Tipo de visualización** a continuación, haga clic en el tipo que desee.

   Puede cambiar entre los siguientes tipos de visualización de campos:

   * **Campos de tipo selección**: Casillas de verificación, menú desplegable, botones de opción.
   * **Campos de tipo texto**: Campo De Texto De Una Sola Línea, Campo De Texto De Párrafo. (No se puede cambiar un campo de texto con formato a otro tipo de visualización. Sin embargo, puede eliminarlo y agregar otro tipo de campo).

   Por ejemplo, si ha creado un campo Casillas de verificación, puede cambiarlo a un campo Desplegable o a un campo Botones de radio . O bien, si ha creado un campo de texto de una sola línea, puede cambiarlo a un campo de texto de párrafo.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente cuando desee cambiar el tipo de visualización de un campo de una casilla de verificación o de un campo desplegable de selección múltiple (un menú desplegable que permite seleccionar más de una opción) a un tipo de campo de selección única:
   >
   >* Si cambia a Botones de radio, Workfront conserva los valores de selección múltiple que un usuario haya introducido en el campo hasta que el usuario cambie y guarde los datos en cualquier parte del formulario. En este punto, cualquier valor que se haya seleccionado utilizando el campo de selección múltiple se sustituye por el valor de botón de radio seleccionado.
   >* Si cambia a una lista desplegable de selección única, Workfront conserva los valores de selección múltiple que un usuario haya introducido en el campo hasta que el usuario cambie y guarde los valores en el campo. En este punto, cualquier valor que se haya seleccionado utilizando el campo de selección múltiple se sustituye por el valor desplegable seleccionado.


1. (Opcional) Repita los pasos del 2 al 6 para agregar otros campos personalizados.

   O

   Añada campos que ya se hayan creado para su organización, tal como se explica en [Reutilizar un campo o un widget personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >Puede agregar hasta 500 campos y utilidades en un solo formulario personalizado. Sin embargo, la degradación del rendimiento puede producirse cuando existen más de 100 en un formulario, según su complejidad. Algunos ejemplos de formularios complejos son los formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un solo campo.

1. Haga clic en **Aplicar**.
1. Si desea seguir creando el formulario personalizado de otras formas, continúe con uno de los siguientes artículos:

   * [Colocación de campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Agregar un salto de sección a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y de omisión de lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Obtener una vista previa y completar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
