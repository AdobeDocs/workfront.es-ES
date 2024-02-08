---
title: Diseñar un formulario con el diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede diseñar un formulario personalizado con el diseñador de formularios. Puede adjuntar formularios personalizados a diferentes objetos de Workfront para capturar datos sobre esos objetos.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: a9d9ae15f4d80fa6e09414459417cfd2b57daf42
workflow-type: tm+mt
source-wordcount: '5075'
ht-degree: 3%

---

# Diseñar un formulario con el diseñador de formularios

Puede diseñar un formulario personalizado con el diseñador de formularios. Puede adjuntar formularios personalizados a diferentes objetos de Workfront para capturar datos sobre esos objetos.

## Requisitos de acceso

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

## Empezar a diseñar un formulario personalizado

{{step-1-to-setup}}

1. Clic **Forms personalizado** en el panel izquierdo.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Clic **Nuevo formulario personalizado.**
1. Seleccione a qué tipos de objetos desea adjuntar el formulario personalizado y, a continuación, haga clic en **Continuar**.

   ![](assets/choose-object-type.jpg)

1. En el **El título es obligatorio** , escriba el título del formulario personalizado.
1. (Opcional) Si desea agregar más tipos de objetos al formulario para que se pueda adjuntar a más objetos, haga clic en **Añadir** icono ![](assets/add-objects-icon.png) después **Tipos de objetos**, a continuación, seleccione el tipo que desee en el menú que se muestra. Puede repetir esto para agregar todos los tipos de objetos que desee.

   También puede hacer clic en la X de un tipo de objeto para eliminarlo del formulario.

   >[!CAUTION]
   >
   >Al eliminar un formulario personalizado, también se eliminan todos los datos personalizados de los objetos asociados con el formulario. Los datos eliminados no se pueden recuperar. Considere la posibilidad de desactivar un formulario personalizado en su lugar; cuando desactive un formulario personalizado que ya no utilice, conservará todos los datos históricos asociados.
   >
   >Para obtener más información, consulte [Eliminar tipos de objetos en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. A continuación, puede empezar a agregar campos de al formulario personalizado. Consulte las secciones siguientes:
   * [Reutilizar un campo o widget existente ya utilizado en otro formulario personalizado](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Añadir campos de texto](#add-text-fields)
   * [Añadir campos calculados](#add-calculated-fields)
   * [Agregar botones de opción, grupos de casillas de verificación y menús desplegables](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adición de campos de fecha y tipo anticipado](#add-typeahead-and-date-fields)
   * [Agregar imágenes, PDF y vídeos](#add-images-pdfs-and-videos)
   * [Añadir archivos de Adobe XD](#add-adobe-xd-files)

## Agregar campos nuevos o existentes al formulario personalizado

Puede utilizar campos nuevos o existentes al diseñar el formulario personalizado.

## Reutilizar un campo o widget existente ya utilizado en otro formulario personalizado

1. En la parte superior izquierda de la pantalla, haga clic en **Biblioteca de campos**.

1. Arrastre el campo o widget donde desee en el formulario personalizado.
1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   >[!NOTE]
   >
   >Puede agregar hasta 500 campos y widgets en un solo formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existen más de 100 en un formulario, según su complejidad.
   >
   >
   >Algunos ejemplos de formularios complejos son formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un único campo.

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

### Añadir campos de texto

Puede agregar varios campos de texto diferentes a un formulario personalizado.

+++ **Amplíe para ver las descripciones de los campos de texto disponibles**

* **Campo de texto de línea única**: permite a los usuarios escribir una sola línea de texto en el campo.
* **Campo de texto de párrafo**: permite a los usuarios escribir varias líneas de texto en el campo.
* **Campo de texto con formato**: permite a los usuarios escribir varias líneas de texto en el campo y dar formato al texto con negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque. Un límite de 15 000 caracteres permite texto y formato abundantes.

  Para obtener información sobre el acceso a este campo a través de la API, consulte Almacenamiento de campos de texto enriquecido en la API.

  >[!NOTE]
  >
  >Los campos de texto con formato no están disponibles para las aplicaciones móviles de Workfront (disponibles en próximas versiones).

* **Texto descriptivo**: Permite incluir instrucciones y vínculos a páginas fuera de Workfront.

+++

Para agregar un campo de texto:

1. En la parte izquierda de la pantalla, busque uno de los siguientes campos de texto y arrástrelo a una sección del lienzo:

   * Texto de línea única
   * Texto de párrafo
   * Campo de texto con formato
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
    <li>Texto de parágrafos</li>
    <li>Texto con formato</li>
    <li>Texto descriptivo: próximamente</li>
    </ul></td>
    </tr>
    <tr>
    <td>Etiqueta</td>
    <td><p>Escriba una etiqueta descriptiva para mostrar encima del widget. Puede cambiar la etiqueta en cualquier momento.<p>
    <p>IMPORTANTE: Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p></td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Texto de parágrafos</li>
    <li>Texto con formato</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nombre</td>
    <td><p>(Obligatorio) Así es como el sistema identifica el campo. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p>
    <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado, donde ahora se podría hacer referencia a él en otras áreas de Workfront. <p>Por ejemplo, si agrega el campo personalizado a un informe y posteriormente cambia su nombre, Workfront no lo reconocerá en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.</p> </li>
      <li> <p>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.</p> </li>
      <li><p>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.</p></li>
    </td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Texto de parágrafos</li>
    <li>Texto con formato</li>
    <li>Texto descriptivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instrucciones</td>
    <td>Escriba cualquier información adicional sobre el widget. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Texto de parágrafos</li>
    <li>Texto con formato</li>
    </ul></td>
    </tr>
    <tr>
    <td>Formato</td>
    <td><p>Seleccione el tipo de datos que se capturarán en el campo personalizado.</p> <p><b>NOTA</b>:   
    <ul> 
    <li>Este campo no se puede editar después de guardar el formulario. Si tiene intención de utilizar el campo en cálculos matemáticos, asegúrese de seleccionar un formato de número o de moneda.</li> 
    <li>Al seleccionar Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Texto de parágrafos</li>
    </ul></td>
    </tr>
    <tr>
    <td>Tipo de presentación</td>
    <td>Cambiar entre campos de texto de una sola línea y de párrafo.</td>
    <td><ul>
    <li>Texto de línea única</li>
    <li>Texto de parágrafos</li>
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

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

### Añadir campos calculados

En un formulario personalizado, puede agregar un campo personalizado calculado que utilice datos existentes para generar datos nuevos cuando el formulario personalizado se adjunta a un objeto.

Para agregar un campo calculado, consulte [Agregar campos calculados con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Agregar botones de opción, casillas de verificación y listas desplegables

Puede agregar botones de opción, casillas de verificación y listas desplegables a un formulario personalizado.

+++ **Amplíe para ver las descripciones de los campos disponibles**

* **Botones de radio**: requiere que los usuarios seleccionen solo una opción.
* **Grupo de casillas**: permite a los usuarios seleccionar varias opciones.
* **Desplegable**: Proporciona una lista de opciones desplegables.

+++

>[!NOTE]
>
>Los campos que permiten varias selecciones, como el Grupo de casillas de verificación y la Lista desplegable, son difíciles de trazar y agrupar en los informes. Para facilitar la creación de gráficos y la agrupación en los informes, puede crear campos independientes para cada opción (por ejemplo, un campo de texto de una sola línea).

Para agregar botones de opción y casillas de verificación:

1. En la parte izquierda de la pantalla, busque uno de los siguientes campos y arrástrelo a una sección del lienzo.

   * Botones de radio
   * Grupo de casillas de verificación
   * Lista desplegable

   ![](assets/drag-field-to-section.png)

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
     <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nombre</td> 
     <td> <p>(Obligatorio) Este nombre es el modo en que el sistema identifica el campo personalizado cuando se agrega a varias áreas de Workfront, como informes, Inicio e interacciones de API.</p> <p>Cuando configure el campo personalizado por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> 
    <p><b>IMPORTANTE</b>:   
     <ul> 
    <li>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado, donde ahora se podría hacer referencia a él en otras áreas de Workfront. <p>Por ejemplo, si agrega el campo personalizado a un informe y posteriormente cambia su nombre, Workfront no lo reconocerá en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.</p> </li>
    <li> <p>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.</p> </li>
     <li><p>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.</p></li>
     </ul> <p>Cada nombre de campo personalizado debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar uno que ya se haya creado para otro formulario personalizado. Para obtener más información, consulte <a href="#Add" class="MCXref xref">Agregar un campo personalizado a un formulario personalizado</a> en este artículo.</p> </td>
     <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable</li>
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
    <li>Lista desplegable</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Formato</td> 
    <td> <p>Seleccione el tipo de datos que se capturarán en el campo personalizado.</p> <p><b>NOTA</b>:   
     <ul> 
    <li>Este campo no se puede editar después de guardar el formulario. Si tiene intención de utilizar el campo en cálculos matemáticos, asegúrese de seleccionar un formato de número o de moneda.<br></li> 
    <li>Al seleccionar Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</li>
     </ul></p></td> 
     <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Tipo de presentación</td> 
    <td>Cambie entre botones de opción, grupos de casillas de verificación, desplegables o desplegables de selección múltiple para el campo.</td> 
    <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Cambiar un campo a obligatorio</td> 
    <td>Seleccione esta opción si desea que el campo sea obligatorio para que el usuario complete el formulario personalizado. </td> 
    <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Opciones </td> 
    <td> 
    <ol> 
    <li> <p>Clic <b>Opciones</b>y, a continuación, habilite cualquiera de las siguientes opciones:</p> 
    <ul> 
    <li><strong>Mostrar valores</strong>: Muestra los valores de cada opción en el campo. La etiqueta de cada opción se muestra de forma predeterminada.</li> 
     <li><strong>Ordenar opciones A-Z</strong>: Ordena las opciones que se agregan alfabéticamente en el campo.</li> 
    </ul> 
    </li> 
    <li> <p>Para cada opción que agregue para el usuario, haga clic en el icono de engranaje <img src="assets/gear-icon-settings.png">, luego seleccione una de las siguientes opciones:</p> 
    <ul> 
    <li><strong>Seleccionar de forma predeterminada</strong>: Seleccione la opción de forma predeterminada en el campo.</li> 
    <li> <p><strong>Ocultar opción</strong>: oculte la opción en el campo. Las opciones ocultas siguen siendo accesibles en los informes.</p> </li> 
    <li> <p><strong>Quitar opción</strong>: elimine la opción del campo.</p> <p><b>ADVERTENCIA</b>: Si tiene objetos actuales utilizando esta opción, no lo elimine del campo. Si lo elimina, se perderán datos históricos. En su lugar, seleccione la opción para ocultarla, lo que impide que los usuarios la seleccionen en el futuro.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Botones de radio</li>
    <li>Grupo de casillas de verificación</li>
    <li>Lista desplegable</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   o

   Para copiar un campo, pase el ratón sobre él y haga clic en el icono Copiar.

   ![icono de copia](assets/copy-field.png)

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

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
* **Campo de fecha**: muestra un calendario en el que los usuarios pueden seleccionar una fecha y una hora.

+++

Para agregar campos de fecha de escritura anticipada:

1. En la parte izquierda de la pantalla, busque uno de los siguientes campos y arrástrelo a una sección del lienzo.

   * Escritura anticipada
   * Campo de fecha

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
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
       <td><ul>
    <li>Escritura anticipada</li>
    <li>Campo de fecha</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es el modo en que el sistema identifica el campo personalizado cuando se agrega a varias áreas de Workfront, como informes, Inicio e interacciones de API.</p> <p>Cuando configure el campo personalizado por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado, donde ahora se podría hacer referencia a él en otras áreas de Workfront. <p>Por ejemplo, si agrega el campo personalizado a un informe y posteriormente cambia su nombre, Workfront no lo reconocerá en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.</p> </li>
      <li> <p>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.</p> </li>
      <li><p>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.</p></li>
      </ul> <p>Cada nombre de campo personalizado debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar uno que ya se haya creado para otro formulario personalizado. Para obtener más información, consulte <a href="#Add" class="MCXref xref">Agregar un campo personalizado a un formulario personalizado</a> en este artículo.</p> </td>
         <td><ul>
    <li>Escritura anticipada</li>
    <li>Campo de fecha</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el campo personalizado. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Escritura anticipada</li>
    <li>Campo de fecha</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar hora del día</td> 
      <td>Seleccione esta opción si desea mostrar la hora del día junto con la fecha en el campo.</td> 
         <td><ul>
    <li>Campo de fecha</li>
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
      <td role="rowheader">Cambiar un campo a obligatorio</td> 
      <td>Seleccione esta opción si desea que el campo sea obligatorio para que el usuario complete el formulario personalizado. </td> 
       <td><ul>
    <li>Escritura anticipada</li>
    <li>Campo de fecha</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita el paso anterior para añadir otros campos o widgets.

   o

   Para copiar un campo, pase el ratón sobre él y haga clic en el icono Copiar.

   ![icono de copia](assets/copy-field.png)

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

### Adición de campos de búsqueda externos

Un campo de búsqueda externa llama a una API externa y devuelve valores como opciones en un campo desplegable. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado pueden seleccionar una o más de estas opciones en la lista desplegable. El campo de búsqueda externa también está disponible en listas e informes.

>[!NOTE]
>
>La funcionalidad de búsqueda externa no está disponible en objetos de documento o usuario.

Para añadir una búsqueda externa:

1. En el lado izquierdo de la pantalla, busque **Búsqueda externa** y arrástrela a una sección del lienzo.
1. En el lado derecho de la pantalla, configure las opciones del campo personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Así es como el sistema identifica el campo personalizado.</p> <p>Cuando configure el campo personalizado por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado, donde ahora se podría hacer referencia a él en otras áreas de Workfront. <p>Por ejemplo, si agrega el campo personalizado a un informe y posteriormente cambia su nombre, Workfront no lo reconocerá en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.</p> </li>
      <li> <p>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.</p> </li>
      <li><p>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.</p></li>
      </ul> <p>Cada nombre de campo personalizado debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar uno que ya se haya creado para otro formulario personalizado. Para obtener más información, consulte <a href="#Add" class="MCXref xref">Agregar un campo personalizado a un formulario personalizado</a> en este artículo.</p> </td>
     </tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el campo personalizado. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td>
      <td><p>Seleccione el tipo de datos que se capturarán en el campo personalizado.</p>
      <p><strong>NOTA:</strong></p>
      <ul><li>Puede cambiar el tipo de formato después de guardar el formulario, con una limitación: todos los valores existentes en los objetos deben poder convertirse al nuevo tipo. (Por ejemplo, si el tipo de formato es Texto y un objeto almacena el valor "abc", no se puede convertir el campo y aparecerá un error que indica que el sistema no puede convertir "abc" en número/moneda.) Si tiene intención de utilizar el campo en cálculos matemáticos, asegúrese de seleccionar un formato de número o de moneda.</li>
      <li>Al seleccionar Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</li></ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">URL de API básica</td> 
      <td><p>Escriba o pegue la dirección URL de la API.</p><p>La dirección URL de la API debe devolver un contenido JSON de las opciones que desee mostrar en la lista desplegable. Puede utilizar la Ruta de JSON para seleccionar los valores específicos de las opciones desplegables de JSON que se van a devolver.</p><p>Al introducir la URL de la API, puede, opcionalmente, pasar los siguientes valores en la URL:</p>
      <ul>
      <li>$$HOST: representa el host actual de Workfront y se puede utilizar para hacer llamadas de la API /search a la API de Workfront. Cuando se utiliza este comodín, se administra la autenticación y los usuarios no necesitan enviar encabezados de autenticación. (Por ejemplo, los usuarios pueden buscar tareas utilizando la dirección URL base <code>$$HOST/attask/api/task/search</code> y permitirá buscar tareas y seleccionar valores de una lista devuelta de tareas).</li>
      <li><p>$$QUERY: representa el texto de búsqueda que el usuario final escribe en el campo y le permite implementar el filtrado de consultas para los usuarios finales. (El usuario buscará el valor en la lista desplegable).</p>
      <p>Si la API a la que hace referencia lo permite, también puede incluir modificadores en la consulta de búsqueda para identificar cómo debería funcionar la búsqueda. Por ejemplo, puede utilizar lo siguiente como URL de API base para permitir que las personas busquen cualquier proyecto de Workfront que contenga texto específico: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Obtenga más información acerca de los modificadores de búsqueda de Workfront en <a href="/help/quicksilver/wf-api/general/api-basics.md">Conceptos básicos de API</a>.</p>
      <p><strong>NOTA:</strong> Si no utiliza $$QUERY y el usuario escribe texto en el cuadro de búsqueda, se reducirán las opciones que ya tiene. Sin embargo, si utiliza $$QUERY y el usuario escribe cualquier cosa, se realiza una nueva llamada de red a la API. Por lo tanto, si tiene más de 2000 valores en la API y esta admite consultas, puede utilizar $$QUERY no solo para buscar entre los 2000 valores existentes, sino también desde la API original con las opciones reducidas.</p></li>
      <li><p>{fieldName} - Donde fieldName es cualquier campo personalizado o nativo de Workfront. De este modo, puede implementar filtros de opción desplegables en cascada cuando pase el valor de un campo ya seleccionado al campo Búsqueda externa para filtrar las opciones. (Por ejemplo, el campo Región ya existe en el formulario y está restringiendo una lista de países de la API a los que están en una región específica).</p>
      <p>Para un campo de búsqueda externo que dependa de otros campos (con el {fieldName} sintaxis), las opciones devueltas por la API se limitan a las que coinciden con cualquier cadena o valor introducido en los demás campos. (Esta funcionalidad no se admite en listas e informes).</p></li>
      <li>{referenceObject}.{fieldName} - Donde el campo forma parte de un objeto. Esta sintaxis es similar a las expresiones personalizadas. (Por ejemplo, portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>NOTA:</strong> Revise la documentación de la API con la que está trabajando para las consultas específicas que puede definir.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Método HTTP</td> 
      <td>Seleccionar <strong>Obtener</strong>, <strong>Publicar</strong>, o <strong>Put</strong> para el método.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Ruta JSON</td>
      <td><p>Escriba o pegue la ruta JSON para la API.</p> <p>Esta opción permite extraer datos del JSON devuelto por la dirección URL de la API. Sirve para seleccionar qué valores dentro del JSON aparecerán en las opciones desplegables.</p><p>Por ejemplo, si la dirección URL de la API devuelve JSON con este formato:</br>
      <pre>
      { data: { { name: "USA"}, { name: "Canada"} } }
      </pre>
      </p>
      <p>a continuación, puede utilizar "$.data[*].name" para seleccionar EE. UU. y Canadá como opciones desplegables.</p> <p>Para obtener más información sobre la ruta JSON y cómo asegurarse de escribir la ruta JSON correcta, consulte <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Encabezados</td>
      <td><p>Clic <strong>Añadir encabezado</strong>y escriba o pegue el par clave-valor necesario para la autenticación con la API.</p><p><strong>NOTA:</strong> Los campos Encabezado no son un lugar seguro para almacenar credenciales y debe tener cuidado con lo que escribe y guarda.</p></td>
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

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

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

* **Imagen**: permite a los usuarios añadir archivos de imagen _____.
* **PDF**: permite a los usuarios añadir PDF
* **Vídeos**: permite a los usuarios añadir archivos de vídeo ____.

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
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del widget. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es la forma en que el sistema identifica el widget.</p> <p>Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> <p><b>IMPORTANTE</b>: Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en el widget. Si lo hace, el sistema ya no reconocerá el widget donde ahora se podría hacer referencia a él en otras áreas de Workfront. </p> <p>Cada nombre de widget debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar uno que ya se haya creado para otro formulario personalizado. </p> </td> 
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

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

#### Agregar un widget de vídeo a un formulario personalizado desde el área Documentos{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Cuando se agrega un vídeo a un formulario personalizado de este modo, solo se aplican al vídeo los permisos establecidos para el formulario personalizado cuando los usuarios acceden al formulario en un objeto, no los permisos establecidos para el vídeo en el área Documentos.

1. Vaya al vídeo en el área Documents y genere una prueba para él, tal como se describe en [Creación de una prueba interactiva para un sitio web u otro contenido web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Abra la prueba.
1. Haga clic con el botón derecho en cualquier lugar del vídeo y seleccione **Copiar dirección de vídeo**.
1. En el formulario personalizado en el que está agregando el widget de vídeo, pegue la dirección copiada en la **URL** cuadro.
1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

### Añadir archivos de Adobe XD

Puede agregar un prototipo de Adobe XD directamente a un formulario personalizado. Los usuarios que trabajen con el objeto al que está adjunto el formulario personalizado solo podrán ver el archivo Adobe XD en las áreas siguientes:

* El área Detalles del objeto (por ejemplo, para un proyecto, el área Detalles del proyecto)
* El cuadro Editar del objeto, si tiene el nuevo aspecto y funcionamiento de la experiencia Adobe Workfront (por ejemplo, los cuadros Editar proyecto y Editar tarea)

Para agregar un archivo Adobe XD:

1. En el lado izquierdo de la pantalla, busque **Adobe XD** y arrástrela a una sección del lienzo.
1. Escriba o edite cualquiera de las siguientes propiedades para el widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del widget. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es la forma en que el sistema identifica el widget. Cuando configure el widget por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p>
    <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado, donde ahora se podría hacer referencia a él en otras áreas de Workfront. <p>Por ejemplo, si agrega el campo personalizado a un informe y posteriormente cambia su nombre, Workfront no lo reconocerá en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.</p> </li>
      <li> <p>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.</p> </li>
      <li><p>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.</p></td> 
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

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Clic **Guardar y cerrar**.

## Organizar y obtener una vista previa de un formulario con el diseñador de formularios

Para obtener información sobre cómo organizar y ver una vista previa del formulario, consulte [Organizar y obtener una vista previa de un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
