---
title: Crear un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede diseñar un formulario personalizado con el diseñador de formularios. Puede adjuntar formularios personalizados a diferentes objetos de Workfront para capturar datos sobre esos objetos.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '5537'
ht-degree: 5%

---

# Creación de un formulario personalizado

Puede diseñar un formulario personalizado con el diseñador de formularios en Adobe Workfront. Puede adjuntar formularios personalizados a diferentes objetos de Workfront para capturar datos sobre esos objetos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Empezar a diseñar un formulario personalizado

{{step-1-to-setup}}

1. Haga clic en **Forms personalizado** en el panel izquierdo.

1. Haga clic en **Nuevo formulario personalizado.**
1. Seleccione a qué tipos de objetos desea adjuntar el formulario personalizado y, a continuación, haga clic en **Continuar**.

   ![](assets/choose-object-type.jpg)

1. En el área **Se requiere título**, escriba el título del formulario personalizado.
1. (Opcional) Si desea agregar más tipos de objetos al formulario para que se pueda adjuntar a más objetos, haga clic en el icono **Agregar** ![](assets/add-objects-icon.png) después de **Tipos de objetos** y, a continuación, seleccione el tipo que desee en el menú que aparece. Puede repetir esto para agregar todos los tipos de objetos que desee.

   También puede hacer clic en la X de un tipo de objeto para eliminarlo del formulario.

   >[!CAUTION]
   >
   >Al eliminar un formulario personalizado, también se eliminan todos los datos personalizados de los objetos asociados con el formulario. Los datos eliminados no se pueden recuperar. Considere la posibilidad de desactivar un formulario personalizado en su lugar; cuando desactive un formulario personalizado que ya no utilice, conservará todos los datos históricos asociados.
   >
   >Para obtener más información, vea [Agregar o eliminar tipos de objetos de un formulario personalizado existente](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) y [Desactivar o reactivar un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md).


1. A continuación, puede empezar a agregar campos de al formulario personalizado. Consulte las secciones siguientes:
   * [Reutilizar un campo o widget existente ya utilizado en otro formulario personalizado](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Notas sobre nombres de campo y etiquetas](#notes-on-field-names-and-labels)
   * [Añadir campos de texto](#add-text-fields)
   * [Añadir campos calculados](#add-calculated-fields)
   * [Agregar botones de opción, grupos de casillas de verificación y menús desplegables](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adición de campos de fecha y tipo anticipado](#add-typeahead-and-date-fields)
   * [Adición de campos de búsqueda externos](#add-external-lookup-fields)
   * [Agregar imágenes, PDF y vídeos](#add-images-pdfs-and-videos)
   * [Añadir campos nativos de Workfront](#add-workfront-native-fields)
   * [Agregar archivos de Adobe XD](#add-adobe-xd-files)
     <!--* [Add Planning connection fields](#add-planning-connection-fields)-->

## Agregar campos nuevos o existentes al formulario personalizado

Puede utilizar campos nuevos o existentes al diseñar el formulario personalizado.

Los formularios personalizados están limitados a 500 campos. Un contador situado en la parte inferior izquierda muestra cuántos campos se utilizan en el formulario y siempre está visible a medida que se desplaza por el diseñador de formularios.

### Reutilizar un campo o widget existente ya utilizado en otro formulario personalizado

1. En la parte superior izquierda de la pantalla, haga clic en **Biblioteca de campos**.

1. Arrastre el campo o widget donde desee en el formulario personalizado.
1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   >[!NOTE]
   >
   >Puede agregar hasta 500 campos y widgets en un solo formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existen más de 100 en un formulario, según su complejidad.
   >
   >
   >Algunos ejemplos de formularios complejos son formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un único campo.

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

### Notas sobre nombres de campo y etiquetas {#notes-on-field-names-and-labels}

La **etiqueta** está disponible para la mayoría de los campos. Es una etiqueta descriptiva que aparece encima del campo o widget en el formulario personalizado. Puede cambiar la etiqueta en cualquier momento.

>[!NOTE]
>
>Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.

Se requiere un **nombre** para cada campo. Este nombre es el modo en que el sistema identifica el campo personalizado cuando se agrega a varias áreas a través de Workfront, como informes, Página de inicio e interacciones de API. Cuando configure el campo o widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.

Cada nombre de campo personalizado debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar uno que ya se haya creado para otro formulario personalizado.

>[!NOTE]
>
>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado, donde ahora se podría hacer referencia a él en otras áreas de Workfront.
>Por ejemplo, si agrega el campo personalizado a un informe y posteriormente cambia su nombre, Workfront no lo reconocerá en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.
>
>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.
>
>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.

Los nombres y etiquetas de campo personalizado no admiten los siguientes caracteres especiales.

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* :
* `{`
* `}`

### Añadir campos de texto

Puede agregar varios campos de texto diferentes a un formulario personalizado.

+++ **Amplíe para ver las descripciones de los campos de texto disponibles**

* **Campo de texto de una sola línea**: permite a los usuarios escribir una sola línea de texto en el campo.
* **Campo de párrafo**: permite a los usuarios escribir varias líneas de texto en el campo.
* **Campo de texto con formato**: permite a los usuarios escribir varias líneas de texto en el campo y aplicar al texto negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque. Un límite de 15 000 caracteres permite texto y formato abundantes.

  Este tipo de campo personalizado no se admite en filtros de listas e informes.

  Para obtener información sobre cómo obtener acceso a este campo a través de la API, consulte [Almacenamiento de campo de texto enriquecido en la API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >Los campos de texto con formato no están disponibles para las aplicaciones móviles de Workfront (disponibles en próximas versiones).

* **Texto descriptivo**: permite incluir instrucciones y vínculos a páginas fuera de Workfront.

+++

Para agregar un campo de texto:

1. En la parte izquierda de la pantalla, busque uno de los siguientes campos de texto y arrástrelo a una sección del lienzo:

   * Texto de línea única
   * Párrafo
   * Texto con formato
   * Texto descriptivo

   ![](assets/drag-field-to-section.png)

1. En el lado derecho de la pantalla, configure las opciones disponibles para el tipo de campo personalizado que está agregando:

   <table>
    <tr>
    <td>Entrada en</td>
    <td>Descripción</td>
    <td>Disponible para </td>
    </tr>
    <tr>
    <td>Tamaño</td>
    <td><p>Cambie el tamaño de los campos de texto del formulario.<p>
   </td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Párrafo</li>
    <li>Texto con formato</li>
    <li>Texto descriptivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Etiqueta</td>
    <td><p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo. Puede cambiar la etiqueta en cualquier momento.<p>
    <p>IMPORTANTE: Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes. Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p></td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Párrafo</li>
    <li>Texto con formato</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nombre</td>
    <td><p>(Obligatorio) Así es como el sistema identifica el campo. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p>
    <p>Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p>
    </td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Párrafo</li>
    <li>Texto con formato</li>
    <li>Texto descriptivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instrucciones</td>
    <td>Escriba cualquier información adicional sobre el campo. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Párrafo</li>
    <li>Texto con formato</li>
    </ul></td>
    </tr>
    <tr>
    <td>Formato</td>
    <td><p>Seleccione el tipo de datos que se capturarán en el campo personalizado.</p> <p><b>NOTA</b>:   
    <ul> 
    <li>Este campo no se puede editar después de guardar el formulario. Si tiene intención de utilizar el campo en cálculos matemáticos, asegúrese de seleccionar un formato de número o de moneda.</li> 
    <li>Al seleccionar Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</li>
    <li>El límite de caracteres para los campos Número es de 16. También puede utilizar un campo Text para introducir números y evitar el límite.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Párrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Tipo de presentación</td>
    <td>Cambiar entre campos de texto de una sola línea y de párrafo.</td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Párrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hipervínculo</td>
    <td> Si desea aplicar un hipervínculo al texto descriptivo que ha escrito, agréguelo aquí. El texto descriptivo se muestra como un vínculo en los objetos en los que está adjunto el formulario.</td>
    <td><ul><li>Texto descriptivo</li></ul></td>
    </tr>
   </table>

1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   o

   Para copiar un campo, pase el ratón sobre él y haga clic en el icono Copiar.

   ![icono de copia](assets/copy-field.png)

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

### Añadir campos calculados

En un formulario personalizado, puede agregar un campo personalizado calculado que utilice datos existentes para generar datos nuevos cuando el formulario personalizado se adjunta a un objeto.

Para agregar un campo calculado, consulte [Agregar campos calculados con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Agregar botones de opción, grupos de casillas de verificación y menús desplegables

Puede agregar botones de opción, grupos de casillas de verificación, listas desplegables y listas desplegables de selección múltiple a un formulario personalizado.

+++ **Amplíe para ver las descripciones de los campos disponibles**

* **Botones de radio**: Requiere que los usuarios seleccionen solo una opción.
* **Grupo de casillas de verificación**: permite a los usuarios seleccionar varias opciones.
* **Menú desplegable de selección única**: Proporciona una lista de opciones desplegables.
* **Lista desplegable de selección múltiple**: permite a los usuarios seleccionar varias opciones en una lista desplegable.

+++

>[!NOTE]
>
>Los campos que permiten varias selecciones, como el grupo de casillas de verificación y la lista desplegable de selección múltiple, son difíciles de trazar y agrupar en los informes. Para facilitar la creación de gráficos y la agrupación en los informes, puede crear campos independientes para cada opción (por ejemplo, un campo de texto de una sola línea).

Para agregar botones de opción, grupos de casillas de verificación y menús desplegables:

1. En la parte izquierda de la pantalla, busque uno de los siguientes campos y arrástrelo a una sección del lienzo.

   * Botones de radio
   * Grupo de casillas de verificación
   * Lista desplegable de selección única
   * Lista desplegable de selección múltiple

   ![Arrastrar un campo al lienzo](assets/drag-field-to-section.png)

1. En el lado derecho de la pantalla, configure las opciones disponibles para el tipo de campo personalizado que está agregando:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Entrada en</td>
    <td>Descripción</td>
    <td>Disponible para </td>
    </tr>
    <tr> 
     <td role="rowheader">Etiqueta</td> 
     <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes. Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td> 
     <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable de selección única</li>
    <li>Lista desplegable de selección múltiple</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nombre</td> 
     <td> <p>(Obligatorio) Así es como el sistema identifica el campo. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> 
    <p>Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td>
     <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable de selección única</li>
    <li>Lista desplegable de selección múltiple</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Instrucciones</td> 
    <td> <p>Escriba cualquier información adicional sobre el campo personalizado. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable de selección única</li>
    <li>Lista desplegable de selección múltiple</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Formato</td> 
    <td> <p>Seleccione el tipo de datos que se capturarán en el campo personalizado.</p> <p><b>NOTA</b>:   
     <ul> 
    <li>Este campo no se puede editar después de guardar el formulario. Si tiene intención de utilizar el campo en cálculos matemáticos, asegúrese de seleccionar un formato de número o de moneda.<br></li> 
    <li>Al seleccionar Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</li>
    <li>El límite de caracteres para los campos Número es de 16. También puede utilizar un campo Text para introducir números y evitar el límite.</li>
     </ul></p></td> 
     <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable de selección única</li>
    <li>Lista desplegable de selección múltiple</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Tipo de presentación</td> 
    <td>Cambie entre botones de opción, grupos de casillas de verificación, listas desplegables de selección única o de selección múltiple para el campo.</td> 
    <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable de selección única</li>
    <li>Lista desplegable de selección múltiple</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Cambiar un campo a obligatorio</td> 
    <td>Seleccione esta opción si desea que el campo sea obligatorio para que el usuario complete el formulario personalizado. </td> 
    <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable de selección única</li>
    <li>Lista desplegable de selección múltiple</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Opciones </td> 
    <td> 
    <ol> 
    <li> <p>Haga clic en <b>Opciones</b> y, a continuación, habilite cualquiera de las siguientes opciones:</p> 
    <ul> 
    <li><strong>Mostrar valores</strong>: muestra los valores de cada opción en el campo. La etiqueta de cada opción se muestra de forma predeterminada.</li> 
     <li><strong>Ordenar opciones A-Z</strong>: ordena las opciones que se agregan alfabéticamente en el campo.</li> 
    </ul> 
    </li> 
    <li> <p>Para cada opción que agregue para el usuario, haga clic en el icono de engranaje <img src="assets/gear-icon-settings.png"> y, a continuación, seleccione una de las siguientes opciones:</p> 
    <ul> 
    <li><strong>Seleccionar de forma predeterminada</strong>: seleccione la opción de forma predeterminada en el campo.</li> 
    <li> <p><strong>Ocultar opción</strong>: oculta la opción en el campo. Las opciones ocultas siguen siendo accesibles en los informes.</p> </li> 
    <li> <p><strong>Quitar opción</strong>: quite la opción del campo.</p> <p><b>ADVERTENCIA</b>: Si tiene objetos actuales que utilizan esta opción, no la quite del campo. Si lo elimina, se perderán datos históricos. En su lugar, seleccione la opción para ocultarla, lo que impide que los usuarios la seleccionen en el futuro.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable de selección única</li>
    <li>Lista desplegable de selección múltiple</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   o

   Para copiar un campo, pase el ratón sobre él y haga clic en el icono Copiar.

   ![icono de copia](assets/copy-field.png)

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

### Adición de campos de fecha y tipo anticipado

Puede agregar campos de escritura anticipada y fecha a un formulario personalizado.

+++ **Amplíe para ver las descripciones de los campos disponibles**

* **Escritura anticipada**: permite a los usuarios escribir el nombre de un objeto que existe en Workfront. Aparece una lista de sugerencias cuando el usuario empieza a escribir. Este tipo de campo admite los siguientes objetos:
   * Usuario
   * Grupo
   * Función
   * Portafolio
   * Programar
   * Proyecto
   * Equipo
   * Plantilla
   * Compañía
* **Fecha**: muestra un calendario donde los usuarios pueden seleccionar una fecha y una hora.

+++

Para añadir los campos de fecha y tipo &quot;delante&quot;:

1. En la parte izquierda de la pantalla, busque uno de los siguientes campos y arrástrelo a una sección del lienzo.

   * Escritura anticipada
   * Fecha

   ![](assets/drag-field-to-section.png)

1. En el lado derecho de la pantalla, configure las opciones disponibles para el tipo de campo personalizado que está agregando:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Configuración de campo</td>
    <td>Descripción</td>
    <td>Disponible para </td>
    </tr>
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes. Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td> 
       <td><ul>
    <li>Escritura anticipada</li>
    <li>Fecha</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Así es como el sistema identifica el campo. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> 
      <p>Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td>
    <td><ul>
    <li>Escritura anticipada</li>
    <li>Fecha</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el campo personalizado. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Escritura anticipada</li>
    <li>Fecha</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar hora del día</td> 
      <td>Seleccione esta opción si desea mostrar la hora del día junto con la fecha en el campo.</td> 
         <td><ul>
    <li>Fecha</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto referenciado</td> 
      <td> <p>Seleccione el tipo de objeto que desea asociar al campo.</p> <p>Una vez que haya hecho clic en Aplicar o en Guardar+Cerrar, no puede cambiar el tipo de objeto del campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Si el administrador de Workfront personalizó el nombre para Portfolio, Programas o Proyectos en la interfaz de usuario de Workfront, el nombre de Workfront predeterminado para el objeto aparecerá en esta lista desplegable, no en el nombre personalizado. Póngase en contacto con el administrador de Workfront si necesita ayuda con esto.<br></li> 
         <li>Los siguientes tipos de objetos son compatibles con las aplicaciones móviles de iOS y Android Workfront: usuario, empresa, grupo, función de trabajo, Portfolio, programa, proyecto y plantilla.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Escritura anticipada</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Agregar filtro</td>
      <td><p>Añada un filtro para un tipo de objeto para limitar los objetos que los usuarios pueden elegir cuando utilizan el campo. </p> <p>Por ejemplo, puede limitar un campo para que los nombres de usuario solo se puedan seleccionar si cumplen los siguientes criterios:</p> 
       <ul> 
        <li>Pertenecen a uno o varios grupos especificados</li> 
        <li>Están asociados a un rol o cargo que especifique</li> 
        <li>Pertenecen al mismo grupo que la persona que utiliza el campo</li> 
       </ul> <p>Debe definir el filtro para el tipo de objeto seleccionado mediante la sintaxis de Modo de texto. Para obtener información acerca de cómo crear un filtro mediante el modo de texto, vea <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Editar un filtro mediante el modo de texto</a>.</p>
       <p><b>NOTA</b>:
       <ul> 
        <li>Si está editando un formulario personalizado existente, al agregar un filtro a un campo de escritura anticipada no se elimina ningún objeto (fuera del ámbito del filtro) que los usuarios ya hayan agregado mediante el campo.</li> 
        <li>Este filtro no está disponible en dispositivos móviles. Si utiliza el filtro para un campo de escritura anticipada, el campo aparecerá en los dispositivos móviles de los usuarios no afectados por el filtro.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>Escritura anticipada</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Cambiar un campo a obligatorio</td> 
      <td>Seleccione esta opción si desea que el campo sea obligatorio para que el usuario complete el formulario personalizado. </td> 
       <td><ul>
    <li>Escritura anticipada</li>
    <li>Fecha</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   o

   Para copiar un campo, pase el ratón sobre él y haga clic en el icono Copiar.

   ![icono de copia](assets/copy-field.png)

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

### Adición de campos de búsqueda externos

Un campo de búsqueda externa llama a una API externa y devuelve valores como opciones en un campo desplegable. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado pueden seleccionar una o más de estas opciones en la lista desplegable. El campo de búsqueda externa también está disponible en listas e informes.

Para obtener ejemplos sobre el uso del campo de búsqueda externa para llamar a la misma instancia de Workfront o a una API pública, consulte [Ejemplos del campo de búsqueda externa en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>* Los campos de búsqueda externos no son compatibles con el complemento de Outlook.
>* Los campos de búsqueda externos no están disponibles en las listas cuando el campo depende de otro campo.

Para añadir una búsqueda externa:

1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. En el lado derecho de la pantalla, configure las opciones del campo personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes. Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Así es como el sistema identifica el campo. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p>
      <p>Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td>
     </tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el campo personalizado. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td>
      <td><p>Seleccione el tipo de datos que se capturarán en el campo personalizado.</p>
      <p><strong>NOTA:</strong></p>
      <ul><li>Puede cambiar el tipo de formato después de guardar el formulario, con una limitación: todos los valores existentes en los objetos deben poder convertirse al nuevo tipo. (Por ejemplo, si el tipo de formato es Texto y un objeto almacena el valor "abc", no se puede convertir el campo y aparecerá un error que indica que el sistema no puede convertir "abc" en número/moneda.) Si tiene intención de utilizar el campo en cálculos matemáticos, asegúrese de seleccionar un formato de número o de moneda.</li>
      <li>Al seleccionar Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</li>
      <li>El límite de caracteres para los campos Número es de 16. También puede utilizar un campo Text para introducir números y evitar el límite.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">URL de API básica</td> 
      <td><p>Escriba o pegue la dirección URL de la API.</p><p>La dirección URL de la API debe devolver un contenido JSON de las opciones que desee mostrar en la lista desplegable. Puede utilizar la Ruta de JSON para seleccionar los valores específicos de las opciones desplegables de JSON que se van a devolver.</p><p>Al introducir la URL de la API, puede, opcionalmente, pasar los siguientes valores en la URL:</p>
      <ul>
      <li>$$HOST: representa el host actual de Workfront y se puede utilizar para hacer llamadas de la API /search a la API de Workfront. Cuando se utiliza este comodín, se administra la autenticación y los usuarios no necesitan enviar encabezados de autenticación. (Por ejemplo, los usuarios pueden buscar tareas utilizando la dirección URL base <code>$$HOST/attask/api/task/search</code> y permitirá buscar tareas y seleccionar valores de una lista de tareas devuelta).</li>
      <li><p>$$QUERY: representa el texto de búsqueda que el usuario final escribe en el campo y le permite implementar el filtrado de consultas para los usuarios finales. (El usuario buscará el valor en la lista desplegable).</p>
      <p>Si la API a la que hace referencia lo permite, también puede incluir modificadores en la consulta de búsqueda para identificar cómo debería funcionar la búsqueda. Por ejemplo, puede usar lo siguiente como dirección URL de la API base para permitir que las personas busquen cualquier proyecto de Workfront que contenga texto específico: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Obtenga más información acerca de los modificadores de búsqueda de Workfront en <a href="/help/quicksilver/wf-api/general/api-basics.md">Conceptos básicos de API</a>.</p>
      <p><strong>NOTA:</strong> Si no usa $$QUERY y el usuario escribe texto en el cuadro de búsqueda, reducirá las opciones que ya tiene. Sin embargo, si utiliza $$QUERY y el usuario escribe cualquier cosa, se realiza una nueva llamada de red a la API. Por lo tanto, si tiene más de 2000 valores en la API y esta admite consultas, puede utilizar $$QUERY no solo para buscar entre los 2000 valores existentes, sino también desde la API original con las opciones reducidas.</p></li>
      <li><p>{fieldName} - Donde fieldName es cualquier campo personalizado o nativo en Workfront. De este modo, puede implementar filtros de opciones desplegables en cascada cuando pase el valor de un campo ya seleccionado al campo Búsqueda externa para filtrar las opciones. (Por ejemplo, el campo Región ya existe en el formulario y está restringiendo una lista de países de la API a los que están en una región específica).</p>
      <p>Para un campo de búsqueda externo que dependa de otros campos (con la sintaxis {fieldName}), las opciones devueltas por la API se limitan a las que coinciden con cualquier cadena o valor introducido en los demás campos. (Esta funcionalidad no se admite en listas e informes).</p></li>
      <li>{referenceObject}.{fieldName} - Donde el campo es parte de un objeto. Esta sintaxis es similar a las expresiones personalizadas. (Por ejemplo, portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>NOTA:</strong> Revise la documentación de la API con la que está trabajando para las consultas específicas que puede definir.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Método HTTP</td> 
      <td>Seleccione <strong>Get</strong>, <strong>Post</strong> o <strong>Put</strong> para el método.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Ruta JSON</td>
      <td><p>Escriba o pegue la ruta JSON para la API.</p> <p>Esta opción permite extraer datos del JSON devuelto por la dirección URL de la API. Sirve para seleccionar qué valores dentro del JSON aparecerán en las opciones desplegables.</p><p>Por ejemplo, si la dirección URL de la API devuelve JSON con este formato:</br>
      <pre>
      {
       datos: {
         { name: "USA"},
         { name: "Canada"}
       }
      }
      </pre>
      </p>
      <p>a continuación, puede utilizar "$.data[*].name" para seleccionar EE. UU. y Canadá como opciones desplegables.</p> <p>Para obtener más información sobre la ruta JSON y cómo asegurarse de que escribe la ruta JSON correcta, consulte <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Encabezados</td>
      <td><p>Haga clic en <strong>Agregar encabezado</strong> y escriba o pegue el par clave-valor necesario para la autenticación con la API.</p><p><strong>NOTA:</strong> Los campos de encabezado no son un lugar seguro para almacenar credenciales, y debe tener cuidado con lo que escribe y guarda.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Lista desplegable de selección múltiple</td>
      <td><p>Seleccione esta opción para permitir que el usuario seleccione más de un valor en la lista desplegable.</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">Cambiar un campo a obligatorio</td>
      <td><p>Seleccione esta opción si desea que el campo sea obligatorio para que el usuario complete el formulario personalizado.</p></td>
     </tr>       
    </tbody>
   </table>

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

>[!NOTE]
>
>Los siguientes elementos son limitaciones técnicas de la llamada a la API externa:
>
>* Número máximo de opciones: 2000 (solo se muestran las 2000 primeras opciones únicas del JSON devuelto)
>* Tiempo de espera: 3 segundos
>* Número de reintentos: 3
>* Duración de espera entre reintentos: 500 ms
>* Estados de respuesta esperados: 2xx

### Agregar imágenes, PDF y vídeos

Puede agregar imágenes, PDF y vídeos a un formulario personalizado. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado solo podrán ver la imagen, el PDF o el vídeo en las áreas siguientes:

* El área Detalles del objeto (por ejemplo, para un proyecto, el área Detalles del proyecto)
* El cuadro Editar del objeto, si tiene el nuevo aspecto y funcionamiento de la experiencia Adobe Workfront (por ejemplo, los cuadros Editar proyecto y Editar tarea)

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Amplíe para ver las descripciones de los campos disponibles**

* **Imagen**: permite a los usuarios agregar archivos de imagen.
* **PDF**: permite a los usuarios agregar PDF
* **Vídeos**: Permite a los usuarios agregar archivos de vídeo.

+++

Para agregar imágenes, PDF o vídeos:

1. En la parte izquierda de la pantalla, busque uno de los siguientes campos y arrástrelo a una sección del lienzo.

   * Imagen
   * PDF
   * Vídeo

   ![](assets/drag-field-to-section.png)

1. Escriba o edite cualquiera de las siguientes propiedades para el widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del widget. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes. Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es la forma en que el sistema identifica el widget. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> <p>Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatorio) Escriba o pegue la dirección URL del widget donde se almacena en Internet.</p> 
      <p>Si está agregando un widget de vídeo, actualmente puede hacerlo agregando lo siguiente en el cuadro URL:</p> 
      <ul> 
      <li> <p>Vínculo de YouTube o Vimeo</p> </li> 
      <li> <p>Vínculo de vídeo de Google Drive</p> </li> 
      <li> <p>Vínculo a vídeo con extensión MP4 y MOV</p> </li> 
      <li> <p>Vínculo a un vídeo ya cargado en el área Documentos de la instancia de Workfront. Para obtener instrucciones, consulte <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Agregar un widget de vídeo a un formulario personalizado desde el área Documentos</a> en este artículo.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el widget. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamaño</td> 
      <td>Cambie el tamaño de visualización del widget según sea necesario.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   o

   Para copiar un campo, pase el ratón sobre él y haga clic en el icono Copiar.

   ![icono de copia](assets/copy-field.png)

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

#### Agregar un widget de vídeo a un formulario personalizado desde el área Documentos{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Cuando se agrega un vídeo a un formulario personalizado de este modo, solo se aplican al vídeo los permisos establecidos para el formulario personalizado cuando los usuarios acceden al formulario en un objeto, no los permisos establecidos para el vídeo en el área Documentos.

1. Vaya al vídeo en el área Documentos y genere una prueba para él, tal como se describe en [Crear una prueba interactiva para un sitio web u otro contenido web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Abra la prueba.
1. Haga clic con el botón derecho en cualquier lugar del vídeo y, a continuación, seleccione **Copiar dirección de vídeo**.
1. En el formulario personalizado donde esté agregando el widget de vídeo, pegue la dirección copiada en el cuadro **URL**.
1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

### Añadir campos nativos de Workfront

Puede agregar campos nativos de Workfront a los formularios personalizados. Cuando el formulario personalizado se adjunta a un objeto, el campo se rellena a partir de los datos del objeto. Por ejemplo, el campo Descripción de un formulario personalizado adjunto a un proyecto extraerá la descripción del proyecto. (El campo puede mostrar &quot;N/D&quot; si no hay datos disponibles).

+++ **Amplíe para ver la lista de campos nativos admitidos**

Esta tabla enumera los campos nativos disponibles para objetos de Workfront específicos en un formulario personalizado.

| Nombre de campo | Proyecto | Tarea | Problema | Plantilla | Tarea de plantilla | Portafolio | Programar | Grupo |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Fecha real de finalización | ✓ | ✓ | ✓ |   |   |   |   |   |
| Duración real | ✓ |   |   |   |   |   |   |   |
| Horas reales | ✓ |   | ✓ |   |   |   |   |   |
| Fecha real de inicio | ✓ | ✓ | ✓ |   |   |   |   |   |
| Compañía | ✓ |   |   | ✓ |   |   |   |   |
| Condición | ✓ | ✓ | ✓ |   |   |   |   |   |
| Tipo de condición | ✓ |   |   | ✓ |   |   |   |   |
| Descripción | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Duración |   | ✓ |   |   | ✓ |   |   |   |
| Tipo de duración |   | ✓ |   |   | ✓ |   |   |   |
| Unidad de duración |   | ✓ |   |   | ✓ |   |   |   |
| Introducido por | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Fecha de entrada | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Grupo | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Última actualización por | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Fecha de última actualización | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Nombre | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Propietario | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Fecha planificada de finalización | ✓ | ✓ | ✓ |   |   |   |   |   |
| Duración planificada | ✓ |   |   | ✓ |   |   |   |   |
| Horas planificadas | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| Fecha planificada de inicio | ✓ |   |   |   |   |   |   |   |
| Portafolio | ✓ |   |   | ✓ |   |   | ✓ |   |
| Prioridad | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Programar | ✓ |   |   | ✓ |   |   |   |   |
| Fecha proyectada de finalización | ✓ | ✓ |   |   |   |   |   |   |
| Minutos de duración proyectada |   | ✓ |   |   |   |   |   |   |
| Fecha proyectada de inicio | ✓ | ✓ |   |   |   |   |   |   |
| Número de referencia | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Modo de programación | ✓ |   |   | ✓ |   |   |   |   |
| Gravedad |   |   | ✓ |   |   |   |   |   |
| Patrocinador | ✓ |   |   | ✓ |   |   |   |   |
| Estado | ✓ | ✓ |   |   |   |   |   |   |
| Puntos de la historia |   | ✓ |   |   |   |   |   |   |
| Plantilla | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. En el lado izquierdo de la pantalla, busque **Referencia de campo nativo** y arrástrela a una sección del lienzo.
1. En el lado derecho de la pantalla, configure las opciones del campo personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes. Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td>
      <td> <p>(Obligatorio) Así es como el sistema identifica el campo. Cuando configure el campo por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p>
      <p>Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el campo. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo de referencia</td> 
      <td><p>(Obligatorio) Seleccione un campo nativo de Workfront.<p><p>Solo están disponibles los campos nativos de los objetos del formulario. Por ejemplo, si la lista Tipos de objetos de la parte superior del diseñador de formularios muestra Proyecto, podrá seleccionar campos nativos para proyectos, pero no campos específicos de tareas.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Tamaño</td> 
      <td>(Opcional) Cambie el tamaño de visualización del campo según sea necesario.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

### Añadir archivos de Adobe XD

Puede agregar un prototipo de Adobe XD directamente a un formulario personalizado. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado solo podrán ver el archivo Adobe XD en las áreas siguientes:

* El área Detalles del objeto (por ejemplo, para un proyecto, el área Detalles del proyecto)
* El cuadro Editar del objeto, si tiene el nuevo aspecto y funcionamiento de la experiencia Adobe Workfront (por ejemplo, los cuadros Editar proyecto y Editar tarea)

Para agregar un archivo Adobe XD:

1. En el lado izquierdo de la pantalla, busca **Adobe XD** y arrástralo a una sección del lienzo.
1. Escriba o edite cualquiera de las siguientes propiedades para el widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del widget. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes. Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es la forma en que el sistema identifica el widget. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p>
    <p>Para obtener más información, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nombres de campo y etiquetas</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>XD (Obligatorio) Escriba o pegue un vínculo válido de prototipo de.</p> 
      <p>Nota: La configuración Acceso a vínculos de la pestaña Compartir de Adobe XD debe establecerse en Cualquiera que tenga el vínculo. De lo contrario, los usuarios no podrán ver el prototipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el widget. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamaño</td> 
      <td>(Opcional) Cambie el tamaño de visualización del widget según sea necesario.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   o

   Para copiar un campo, pase el ratón sobre él y haga clic en el icono Copiar.

   ![icono de copia](assets/copy-field.png)

1. Para guardar los cambios, haz clic en **Aplicar** y pasa a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

<!--
### Add Planning connection fields

>[!IMPORTANT]
>
>The information in this section refers to Adobe Workfront Planning, an additional capability from Adobe Workfront. 
>
>You must have the following to access Workfront Planning:
>
>* A new Workfront plan and license. Workfront Planning is not available for legacy Workfront plans or licenses. 
>* An additional license for Workfront Planning. 
>* Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.
>
> For a complete list of requirements to access Workfront Planning, see [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md). 
> 
>For more information about Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md).

You can view records connected from Workfront Planning in a custom field on a Workfront object by adding a  Planning connection custom field to an object's custom form. 

You can add the Planning connection field to all objects' custom forms. However, you can display connected records only on the custom forms associated with Workfront objects that can be connected from Workfront Planning. 

>[!NOTE]
>
>Users viewing information in the custom field must have access to Workfront Planning and to the workspaces that contain the record types connected to Workfront objects.


To add a Planning connection field:

1. On the left side of the screen, find **Planning connection** and drag it to a section on the canvas. 
1. On the right side of the screen, configure the options for the custom field:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the field. You can change the label at any time.</p> <p><b>IMPORTANT</b>:</p> <p>Avoid using special characters in this label.</p> 
      <p>We recommend that you choose a label by which you can easily identify where the Planning record is coming from. Add information like the name of the workspace or the name of the record type. </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td>
      <td> <p>(Required) The name is how the system identifies the field. When you are configuring the field for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>(Recommended) Type any additional information about the field. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p>
      <p>Here, you can add explicit information about the record and the objects you are connecting. </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Object type</td> 
      <td><p>(Required) Select a Workfront object type that is connected to a record type in Workfront Planning.</p>
      You may select from the following object types:
      <ul><li> Project</li>
      <li> Portfolio</li><li> Program</li><li> Company</li><li> Group</li></ul>
       <p>Only Workfront object types for the form's object types are available.</p> <p> For example, if the Object Types list at the top of the form designer shows Project, you can only select Project in this field, and you cannot select Portfolios, although portfolios can also be connected to record types.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Workspace</td> 
      <td> <p>(Required) Select the workspace where the records you want to display in Workfront come from in Workfront Planning.</p> <p> Only workspaces that are connected to the object types you selected in the I=Object type field display. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Record Type</td> 
      <td><p>(Required) Select the Workfornt Planning record type whose records are connected to the Workfront object associated with this form.</p><p>Only record types that have connections to the object type you selected in the Object type field display. </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Connection field</td> 
      <td><p>(Required) Select the Workfront Planning connection field that displays the Workfront objects that are associated with this form.</p> <p> <b>NOTE</b></p><p>You can have multiple connection fields between the same object and record types.</p>  </td> 
     </tr>
    </tbody> 
   </table>

1. (Optional) Repeat the previous steps to add any other fields. 

    or

    To copy a field, hover over a field, and click the copy icon.

    ![copy icon](assets/copy-field.png)

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**.

    You can now attach the form to an object connected from Workfront Planning and do one of the following:

    * View Workfront Planning record types connected to the Workfront object
    * Connect or disconnect records from the Workfront object associated with the form. 

    For more information, see [Manage record connections from Workfront objects](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

-->

## Organizar y obtener una vista previa de un formulario con el diseñador de formularios

Para obtener información sobre cómo organizar un formulario personalizado con saltos de sección y obtener una vista previa del formulario, consulte [Organizar y obtener una vista previa de un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
