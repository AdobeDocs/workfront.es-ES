---
navigation-topic: search
title: Buscar [!DNL Adobe Workfront]
description: Puede localizar fácilmente elementos en  [!DNL Adobe Workfront]  buscándolos cuando no pueda recordar su ubicación exacta.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1668'
ht-degree: 1%

---

# Buscar [!DNL Adobe Workfront]

Puede localizar fácilmente elementos en [!DNL Adobe Workfront] buscándolos cuando no pueda recordar su ubicación exacta.

Puede ver el cuadro [!UICONTROL Buscar] en la esquina superior derecha de cualquier página dentro de [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

Debe tener permisos para ver un objeto antes de poder encontrarlo en una búsqueda. Por este motivo, los resultados de la búsqueda varían de un usuario a otro.

## Requisitos de acceso

+++ Expanda esta sección para ver el acceso necesario para realizar los pasos de este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de [!UICONTROL View] al tipo de objeto </p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Debe tener permisos para ver un objeto antes de poder encontrarlo en una búsqueda.</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

+++

## Comprender la búsqueda

* [[!UICONTROL Objetos disponibles para la búsqueda]](#objects-available-for-search)
* [[!UICONTROL Campos disponibles para la búsqueda]](#fields-available-for-search)

### Objetos disponibles para la búsqueda

Puede buscar los siguientes objetos en Workfront:

* Proyectos
* Tareas
* Problemas
* Informes
* Usuarios
* Plantillas
* Documentos
* Portafolios
* Programas
* Paneles
* Compañías
* Notas

### Campos disponibles para la búsqueda

Los campos disponibles para la búsqueda se basan en el tipo de búsqueda: Básica o [!UICONTROL Búsqueda avanzada].

* **Búsqueda básica**: al buscar objetos en una búsqueda básica, [!DNL Workfront] busca texto que pueda contener palabras clave en los campos siguientes:

   * Nombres de objeto
   * Descripciones
   * Campos de datos personalizados
   * Actualizaciones
   * Nombres de documentos (en búsquedas de documentos específicas y en una búsqueda básica)

  Para obtener más información acerca de la búsqueda básica en [!DNL Workfront], vea [Búsqueda básica](#basic-search) en este artículo.

* **[!UICONTROL Búsqueda avanzada]**: en una [!UICONTROL Búsqueda avanzada], puede configurar filtros para buscar campos que no están disponibles en la búsqueda básica. Por lo tanto, [!UICONTROL Búsqueda avanzada] le permite buscar en cualquier campo del objeto.

  Para obtener más información sobre [!UICONTROL Búsqueda avanzada], consulte [Búsqueda avanzada](#advanced-search) en este artículo.

>[!NOTE]
>
>Para realizar una [!UICONTROL búsqueda avanzada], debe seleccionar la opción [!UICONTROL Búsqueda avanzada] al comenzar la búsqueda. No puede restringir una búsqueda básica en [!UICONTROL Búsqueda avanzada].

## Comprender las limitaciones de [!DNL Workfront] búsquedas

Tenga en cuenta las siguientes limitaciones al usar [!UICONTROL Search] en [!DNL Workfront]:

* Las búsquedas no distinguen entre mayúsculas y minúsculas
* [!DNL Workfront] no corrige ni comprende errores tipográficos
* La búsqueda en [!DNL Workfront] no admite caracteres comodín
* La búsqueda de [!DNL Workfront] admite búsquedas parciales de palabras, pero no admite búsquedas de subcadenas.\
   Por ejemplo, la palabra clave de búsqueda &quot;stand&quot; devolverá resultados que incluyan la palabra &quot;standard&quot;, pero no los resultados que incluyan la palabra &quot;Understanding&quot;.

## Buscar varias palabras

Cuando se incluyen varias palabras en una búsqueda y sólo se desea buscar objetos que coincidan con todas las palabras del cuadro Buscar, se puede escribir las palabras en cualquier orden.

Por ejemplo, si busca &quot;Demostración de marketing&quot; (sin comillas), encontrará objetos con los nombres siguientes:

* Demostración de marketing
* Marketing de demostración
* Demostración de análisis de mercado de enero

También encuentra objetos que podrían tener &quot;Marketing&quot; en el nombre y &quot;Demo&quot; en la descripción.

Sin embargo, puede hacer lo siguiente en el cuadro [!UICONTROL Buscar] para ajustar los resultados de búsqueda que aparecen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Incluir comillas</td> 
   <td> <p>La introducción de palabras en el orden correcto entre comillas dobles permite buscar sólo los objetos que coinciden exactamente.<br>Por ejemplo, si busca "Demostración de marketing" (entre comillas), encontrará objetos con los nombres siguientes:</p> 
    <ul> 
     <li> Demostración de marketing</li> 
     <li> Demostración de marketing de enero</li> 
     <li>Plan de demostración de marketing</li> 
    </ul> <p>Sin embargo, esta búsqueda no encontró un objeto con el nombre "Marketing de demostración".</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir O</td> 
   <td> <p>La conexión de palabras mediante "OR" (sin comillas) permite buscar sólo objetos que coincidan con al menos una de las palabras del cuadro [!UICONTROL Search]. Estas palabras se pueden introducir en cualquier orden.<br>Por ejemplo, si busca "Marketing O Demo" (sin comillas), encontrará objetos con los nombres siguientes:</p> 
    <ul> 
     <li> Demostración de análisis de mercado</li> 
     <li>Demostración de análisis de mercado de enero</li> 
     <li>Demostración</li> 
     <li>Análisis de mercado</li> 
    </ul> <p>Nota: "O" debe estar en mayúsculas. De lo contrario, se interpreta como otra palabra de la frase que está buscando.</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir Y</td> 
   <td> <p>La conexión de palabras mediante "Y" (sin comillas) permite buscar sólo objetos que coincidan con todas las palabras del cuadro [!UICONTROL Buscar]. Estas palabras se pueden introducir en cualquier orden.<br>Por ejemplo, si busca "Marketing Y demostración" (sin comillas), encontrará objetos con los nombres siguientes:</p> 
    <ul> 
     <li>Demostración de marketing</li> 
     <li>Marketing de demostración</li> 
     <li>Demostración de análisis de mercado de enero</li> 
    </ul> <p>Nota: "Y" debe estar en mayúsculas. De lo contrario, se interpreta como otra palabra de la frase que está buscando. Del mismo modo, si se incluye "&amp;" (sin comillas), sólo se buscarán los objetos que incluyan el carácter y comercial.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Usar la búsqueda en [!DNL Workfront]

[!DNL Workfront] presenta dos tipos de búsquedas: básica y avanzada. Utilice la búsqueda básica si desea buscar palabras clave en campos de objeto comunes, como nombre o descripción. Use [!UICONTROL Búsqueda avanzada] si desea usar filtros para buscar otros campos de objeto.

* [Búsqueda básica](#basic-search)
* [Búsqueda avanzada](#advanced-search)

### Búsqueda básica

Una búsqueda básica le permite buscar palabras clave en todos los objetos del sistema o en un solo objeto a la vez (como proyectos). [!DNL Workfront] entonces busca esas palabras clave en algunos campos específicos. Puede restringir los resultados de búsqueda basándose en otros campos específicos de objetos seleccionados por [!DNL Workfront].

Para obtener una lista de los campos específicos buscados en la búsqueda básica, consulte [Campos disponibles para la búsqueda](#fields-available-for-search) en este artículo.

>[!NOTE]
>
>Para realizar una [!UICONTROL búsqueda avanzada], debe seleccionar la opción [!UICONTROL Búsqueda avanzada] al comenzar la búsqueda. No puede restringir una búsqueda básica en [!UICONTROL Búsqueda avanzada].

* [Realizar una búsqueda básica](#perform-a-basic-search)
* [Restringir una búsqueda básica](#refine-a-basic-search)

#### Realizar una búsqueda básica

Puede realizar una búsqueda básica de cualquiera de las siguientes maneras:

* En todos los objetos del sistema (búsqueda general).
* Solo en un objeto a la vez (búsqueda específica de objetos).

Para realizar una búsqueda básica:

1. Haga clic en la lupa ![](assets/search-icon.png) en la esquina superior derecha de la página. También puede escribir **[!UICONTROL ALT + /]** u **[!UICONTROL Opción + /]** para abrir el menú [!UICONTROL Buscar].

1. (Opcional) Para buscar un objeto específico, haga clic en el menú desplegable **[!UICONTROL Todos]** y seleccione el objeto que desee buscar.

   ![](assets/search-objecttype.png)

1. En el cuadro **[!UICONTROL Buscar]**, empiece a escribir la información que está buscando.\
   Para obtener información sobre los campos que se buscan en [!DNL Workfront], consulte [Comprender la búsqueda](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   A medida que empieza a escribir en la barra de búsqueda, [!DNL Workfront] hace recomendaciones basadas en el historial de visualización y resalta la palabra clave que busca en azul.

1. Si el elemento que busca se muestra en el menú [!UICONTROL typeforward], haga clic en él.

   O

   Pulse **[!UICONTROL Intro]** para realizar una búsqueda completa. Esta búsqueda consulta toda la base de datos en lugar de los artículos vistos más recientemente.

   La página [!UICONTROL Resultados de búsqueda] se abre desde la izquierda y cubre la mayor parte de la página anterior.

   Si realizó una búsqueda general, [!DNL Workfront] devuelve los resultados de cualquier objeto que coincida con el término de búsqueda en cualquiera de los campos buscados, tal como se describe en [Comprender la búsqueda](#understand-search). Los objetos que coinciden con la búsqueda se muestran en una lista.

   >[!NOTE]
   >
   >A veces, las variaciones de una palabra se muestran en la lista de elementos encontrados.\
   >Por ejemplo, si busca &quot;marketing&quot;, se muestran objetos que contienen &quot;marketing&quot; o &quot;market&quot; en el nombre.

1. (Opcional) Si la búsqueda generó demasiados resultados, refine la búsqueda como se describe en [Refine a basic search](#refine-a-basic-search).
1. (Opcional) Para volver a la página en la que se encontraba antes de la búsqueda, haga clic en **[!UICONTROL Cerrar]** en la esquina superior derecha.

>[!NOTE]
>
>La página [!UICONTROL Resultados de búsqueda] solo permanece abierta cuando está enfocada. Si hace clic fuera de la página o abre otra página, se cerrará la página [!UICONTROL Resultados de búsqueda].

#### Restringir una búsqueda básica

Después de realizar una búsqueda básica, como se describe en [[!UICONTROL Realice una búsqueda básica]](#perform-a-basic-search), puede restringir la búsqueda.

Utilice la barra de herramientas situada a la izquierda de los resultados de búsqueda para reducir la información que está buscando.

Para restringir una búsqueda:

1. (Condicional) Si ha realizado una búsqueda general, seleccione el objeto que estaba buscando en la lista de objetos de la parte superior izquierda de los resultados.
1. Busque los campos disponibles para los objetos mostrados en la búsqueda en la barra de herramientas situada a la izquierda de los resultados.\
   Se muestran los valores de cada campo, ordenados por recuento, hasta 10 valores para cada campo.
1. Haga clic dentro de cualquiera de los campos disponibles para acortar la lista de resultados.\
   Las selecciones que realice se resaltarán en azul y los valores de campo que no seleccione se ocultarán.\
   Después de seleccionar cada nuevo valor, los resultados a la derecha se actualizan dinámicamente.\
   ![](assets/qs-refine-search-350x175.png)

1. (Opcional) Haga clic en los valores seleccionados para anular su selección y volver a mostrar todos los valores de cada campo.

### [!UICONTROL Búsqueda avanzada]

[!UICONTROL Búsqueda avanzada] le permite buscar utilizando campos y filtros que no están disponibles para la búsqueda básica. Por ejemplo, puede buscar proyectos con una prioridad específica o un nombre de propietario de documento.

>[!NOTE]
>
>Para realizar una [!UICONTROL búsqueda avanzada], debe seleccionar la opción [!UICONTROL Búsqueda avanzada] al comenzar la búsqueda. No puede restringir una búsqueda básica en [!UICONTROL Búsqueda avanzada].

* [Usar [!UICONTROL búsqueda avanzada]](#use-advanced-search)

#### Usar [!UICONTROL búsqueda avanzada]

Puede usar [!UICONTROL Búsqueda avanzada] para filtrar la búsqueda según criterios específicos.\
Este tipo de búsqueda es útil cuando no puede recordar una palabra clave asociada a un objeto pero conoce información específica sobre ese objeto (por ejemplo: Prioridad del proyecto, Nombre del propietario del documento, etc.).

Para realizar una búsqueda avanzada:

1. En la esquina superior derecha de cualquier página de [!DNL Workfront], haga clic en el icono **[!UICONTROL Buscar]** ![](assets/search-icon.png). Se muestra el menú [!DNL Search].

1. En la parte inferior del menú [!UICONTROL Buscar], haga clic en **[!UICONTROL Búsqueda avanzada]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   La página [!UICONTROL Búsqueda avanzada] se abre desde la derecha y cubre la mayor parte de la página anterior.

1. Seleccione el tipo de objeto que está buscando.\
   **[!UICONTROL Proyectos]** está seleccionado de manera predeterminada.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (Opcional) Escriba una palabra clave en el campo de la parte superior de la lista.
1. (Opcional) Haga clic en **[!UICONTROL Filtrar los resultados]** para filtrar los resultados de búsqueda según tipos de campo específicos y, a continuación, seleccione un campo de la lista. Si es necesario, seleccione también un valor para el campo.\
   O\
   Añada un nuevo filtro.

1. Haga clic en **[!UICONTROL Buscar]**.\
   A la derecha de la barra de herramientas [!UICONTROL Búsqueda avanzada], aparece una lista de elementos que coinciden con la búsqueda.

1. (Opcional) Para volver a la página en la que se encontraba antes de la búsqueda, haga clic en **[!UICONTROL Cerrar]** en la esquina superior derecha.

>[!NOTE]
>
>La página [!UICONTROL Resultados de búsqueda] solo permanece abierta cuando está enfocada. Si hace clic fuera de la página o abre otra página, se cerrará la página [!UICONTROL Resultados de búsqueda].
