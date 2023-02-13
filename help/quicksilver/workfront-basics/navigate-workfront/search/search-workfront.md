---
navigation-topic: search
title: Buscar [!DNL Adobe Workfront]
description: Puede localizar fácilmente los elementos en [!DNL Adobe Workfront] buscarlos cuando no recuerde su ubicación exacta.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 1%

---

# Buscar [!DNL Adobe Workfront]

Puede localizar fácilmente los elementos en [!DNL Adobe Workfront] buscarlos cuando no recuerde su ubicación exacta.

Puede ver el [!UICONTROL Buscar] en la esquina superior derecha de cualquier página de [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

Debe tener permisos para Ver un objeto antes de encontrarlo en una búsqueda. Por este motivo, los resultados de la búsqueda varían de un usuario a otro.

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
   <td> <p>Acceso de [!UICONTROL View] al tipo de objeto </p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Debe tener permisos para Ver un objeto antes de encontrarlo en una búsqueda.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

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

Los campos disponibles para la búsqueda se basan en el tipo de búsqueda: Básico o [!UICONTROL Búsqueda avanzada].

* **Búsqueda básica**: Al buscar objetos en una búsqueda básica, [!DNL Workfront] busca texto que pueda contener sus palabras clave en los campos siguientes:

   * Nombres de objetos
   * Descripciones
   * Campos de datos personalizados
   * Actualizaciones
   * Nombres de documentos (en búsquedas específicas de documentos y en una búsqueda básica)

   Para obtener más información sobre la búsqueda básica en [!DNL Workfront], consulte [Búsqueda básica](#basic-search) en este artículo.

* **[!UICONTROL Búsqueda avanzada]**: En un [!UICONTROL Búsqueda avanzada], puede configurar filtros para campos de búsqueda no disponibles en la búsqueda básica. Por lo tanto, [!UICONTROL Búsqueda avanzada] permite buscar cualquier campo en el objeto.

   Para obtener más información, consulte [!UICONTROL Búsqueda avanzada], consulte [Búsqueda avanzada](#advanced-search) en este artículo.

>[!NOTE]
>
>Para realizar una [!UICONTROL Búsqueda avanzada], debe seleccionar [!UICONTROL Búsqueda avanzada] al iniciar la búsqueda. No se puede restringir una búsqueda básica a un [!UICONTROL Búsqueda avanzada].

## Comprender las limitaciones de [!DNL Workfront] búsquedas

Tenga en cuenta las siguientes limitaciones al utilizar [!UICONTROL Buscar] en [!DNL Workfront]:

* Las búsquedas no distinguen entre mayúsculas y minúsculas
* [!DNL Workfront] no corrige ni entiende errores tipográficos
* Buscando en [!DNL Workfront] no admite comodines
* Buscando en [!DNL Workfront] admite búsquedas de palabras parciales, pero no admite búsquedas de subcadenas.\
   Por ejemplo, la palabra clave de búsqueda &quot;stand&quot; devolverá resultados, incluida la palabra &quot;standard&quot;, pero no devolverá resultados, incluida la palabra &quot;Understanding&quot;.

## Buscar varias palabras

Cuando se incluyen varias palabras en una búsqueda y se desea buscar sólo objetos que coincidan con todas las palabras del cuadro Buscar, se pueden escribir las palabras en cualquier orden.

Por ejemplo, al buscar &quot;Marketing Demo&quot; (sin comillas), se encuentran objetos con los nombres siguientes:

* Demostración de marketing
* Marketing de demostración
* Demostración de análisis de mercado de enero

También encuentra objetos que podrían tener &quot;Marketing&quot; en el nombre y &quot;Demostración&quot; en la descripción.

Sin embargo, puede hacer lo siguiente en la sección [!UICONTROL Buscar] para ajustar los resultados de búsqueda que aparecen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Incluir comillas</td> 
   <td> <p>La introducción de palabras en el orden correcto dentro de comillas dobles permite buscar solo objetos que coincidan exactamente.<br>Por ejemplo, al buscar "Marketing Demo" (con comillas), se encuentran objetos con los nombres siguientes:</p> 
    <ul> 
     <li> Demostración de marketing</li> 
     <li> Demostración de marketing de enero</li> 
     <li>Plan de demostración de marketing</li> 
    </ul> <p>Sin embargo, esta búsqueda no encontraría un objeto con el nombre "Marketing de demostración".</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir O</td> 
   <td> <p>La conexión de palabras por "O" (sin comillas) permite buscar solo objetos que coincidan con al menos una de las palabras del cuadro [!UICONTROL Buscar]. Estas palabras se pueden introducir en cualquier orden.<br>Por ejemplo, al buscar "Marketing OR Demo" (sin comillas), se encuentran objetos con los nombres siguientes:</p> 
    <ul> 
     <li> Demostración de Análisis de mercado</li> 
     <li>Demostración de análisis de mercado de enero</li> 
     <li>Demostración</li> 
     <li>Análisis de mercado</li> 
    </ul> <p>Nota: "O" debe estar en mayúsculas. De lo contrario, se interpreta como otra palabra de la frase que esté buscando.</p> </td> 
  </tr> 
  <tr> 
   <td>Incluir AND</td> 
   <td> <p>La conexión de palabras por "AND" (sin comillas) le permite buscar solo objetos que coincidan con todas las palabras del cuadro [!UICONTROL Buscar]. Estas palabras se pueden introducir en cualquier orden.<br>Por ejemplo, al buscar "Marketing AND Demo" (sin comillas), se encuentran objetos con los nombres siguientes:</p> 
    <ul> 
     <li>Demostración de marketing</li> 
     <li>Marketing de demostración</li> 
     <li>Demostración de análisis de mercado de enero</li> 
    </ul> <p>Nota: "AND" debe estar en mayúsculas. De lo contrario, se interpreta como otra palabra de la frase que esté buscando. Del mismo modo, si se incluye "&amp;" (sin comillas), solo se buscarán los objetos que incluyan el símbolo &amp;.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Utilice Buscar en [!DNL Workfront]

[!DNL Workfront] incluye dos tipos de búsquedas: Básico y avanzado. Utilice la búsqueda básica si desea encontrar palabras clave en campos de objeto comunes, como nombre o descripción. Uso [!UICONTROL Búsqueda avanzada] si desea utilizar filtros para buscar en otros campos de objeto.

* [Búsqueda básica](#basic-search)
* [Búsqueda avanzada](#advanced-search)

### Búsqueda básica

Una búsqueda básica permite buscar palabras clave en todos los objetos del sistema o en un solo objeto a la vez (como proyectos). [!DNL Workfront] a continuación, busca esas palabras clave en algunos campos específicos. A continuación, puede refinar los resultados de búsqueda en función de otros campos específicos de objeto seleccionados por [!DNL Workfront].

Para obtener una lista de los campos específicos buscados en la búsqueda básica, consulte [Campos disponibles para la búsqueda](#fields-available-for-search) en este artículo.

>[!NOTE]
>
>Para realizar una [!UICONTROL Búsqueda avanzada], debe seleccionar [!UICONTROL Búsqueda avanzada] al iniciar la búsqueda. No se puede restringir una búsqueda básica a un [!UICONTROL Búsqueda avanzada].

* [Realizar una búsqueda básica](#perform-a-basic-search)
* [Restringir una búsqueda básica](#refine-a-basic-search)

#### Realizar una búsqueda básica

Puede realizar una búsqueda básica de cualquiera de estas formas:

* En todos los objetos del sistema (búsqueda general).
* Solo en un objeto a la vez (búsqueda específica del objeto).

Para realizar una búsqueda básica:

1. Haga clic en la lupa ![](assets/search-icon.png) en la esquina superior derecha de la página. También puede escribir **[!UICONTROL ALT + /]** o **[!UICONTROL Opción + /]** para abrir el [!UICONTROL Buscar] para abrir el Navegador.

1. (Opcional) Para buscar un objeto específico, haga clic en el **[!UICONTROL Todo]** menú desplegable y seleccione el objeto que desee buscar.

   ![](assets/search-objecttype.png)

1. En el **[!UICONTROL Buscar]** , empiece a escribir la información que está buscando.\
   Para obtener información sobre los campos en los que se busca [!DNL Workfront], consulte [Comprender la búsqueda](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   A medida que empieza a escribir en la barra de búsqueda, [!DNL Workfront] realiza recomendaciones en función del historial de visualización y resalta la palabra clave que está buscando en azul.

1. Si el elemento que está buscando aparece en la sección [!UICONTROL typeforward] haga clic en él.

   O

   Press **[!UICONTROL Entrar]** para realizar una búsqueda completa. Esta búsqueda consulta toda la base de datos en lugar de los artículos vistos más recientemente.

   La variable [!UICONTROL Resultados de la búsqueda] las diapositivas de la página se abren desde la izquierda y abarcan la mayor parte de la página anterior.

   Si realizó una búsqueda general, [!DNL Workfront] devuelve los resultados de cualquier objeto que coincida con el término de búsqueda en cualquiera de los campos buscados, tal como se describe en [Comprender la búsqueda](#understand-search). Los objetos que coinciden con la búsqueda se muestran en una lista.

   >[!NOTE]
   >
   >A veces, las variaciones de una palabra se muestran en la lista de elementos encontrados.\
   >Por ejemplo, al buscar &quot;marketing&quot;, se muestran objetos que contienen &quot;marketing&quot; o &quot;marketing&quot; en el nombre.

1. (Opcional) Si la búsqueda generó demasiados resultados, limite la búsqueda tal como se describe en [Restringir una búsqueda básica](#refine-a-basic-search).
1. (Opcional) Para volver a la página en la que se encontraba antes de la búsqueda, haga clic en **[!UICONTROL Cerrar]** en la esquina superior derecha.

>[!NOTE]
>
>La variable [!UICONTROL Resultados de la búsqueda] permanece abierta solo cuando está enfocada. Al hacer clic fuera de la página o abrir otra página, se cierra el [!UICONTROL Resultados de la búsqueda] página.

#### Restringir una búsqueda básica

Después de realizar una búsqueda básica, tal como se describe en [[!UICONTROL Realizar una búsqueda básica]](#perform-a-basic-search): puede restringir la búsqueda.

Utilice la barra de herramientas situada a la izquierda de los resultados de búsqueda para reducir la información que busca.

Para restringir una búsqueda:

1. (Condicional) Si ha realizado una búsqueda general, seleccione el objeto que estaba buscando en la lista de objetos situada en la parte superior izquierda de los resultados.
1. Busque los campos disponibles para los objetos mostrados en la búsqueda en la barra de herramientas situada a la izquierda de los resultados.\
   Los valores de cada campo se muestran, ordenados por recuento, hasta 10 valores para cada campo.
1. Haga clic dentro de cualquiera de los campos disponibles para acortar la lista de resultados.\
   Las selecciones que realice se resaltarán en azul y los valores de campo que no seleccione se ocultarán.\
   Después de seleccionar cada nuevo valor, los resultados a la derecha se actualizan dinámicamente.\
   ![](assets/qs-refine-search-350x175.png)

1. (Opcional) Haga clic en los valores seleccionados para anular la selección y volver a mostrar todos los valores de cada campo.

### [!UICONTROL Búsqueda avanzada]

[!UICONTROL Búsqueda avanzada] permite buscar mediante campos y filtros no disponibles para la búsqueda básica. Por ejemplo, puede buscar proyectos con una prioridad específica o un nombre de propietario del documento.

>[!NOTE]
>
>Para realizar una [!UICONTROL Búsqueda avanzada], debe seleccionar [!UICONTROL Búsqueda avanzada] al iniciar la búsqueda. No se puede restringir una búsqueda básica a un [!UICONTROL Búsqueda avanzada].

* [Use la [!UICONTROL Búsqueda avanzada]](#use-advanced-search)

#### Use la [!UICONTROL Búsqueda avanzada]

Puede usar [!UICONTROL Búsqueda avanzada] para filtrar la búsqueda según criterios específicos.\
Este tipo de búsqueda es útil cuando no se puede recordar una palabra clave asociada a un objeto, pero se conoce información específica sobre ese objeto (por ejemplo: Prioridad del proyecto, Nombre del propietario del documento, etc.).

Para realizar una búsqueda avanzada:

1. En la esquina superior derecha de cualquier página de [!DNL Workfront], haga clic en **[!UICONTROL Buscar]** icono ![](assets/search-icon.png). La variable [!DNL Search] para abrir el Navegador.

1. En la parte inferior del [!UICONTROL Buscar] , haga clic en **[!UICONTROL Búsqueda avanzada]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   La variable [!UICONTROL Búsqueda avanzada] las diapositivas de la página se abren desde la derecha y abarcan la mayor parte de la página anterior.

1. Seleccione el tipo de objeto que está buscando.\
   **[!UICONTROL Proyectos]** está seleccionado de forma predeterminada.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (Opcional) Escriba una palabra clave en el campo de la parte superior de la lista.
1. (Opcional) Haga clic en **[!UICONTROL Filtrar los resultados]** para filtrar los resultados de búsqueda según tipos de campo específicos, seleccione un campo de la lista. Si es necesario, seleccione también un valor para el campo .\
   O\
   Añada un nuevo filtro.

1. Haga clic en **[!UICONTROL Buscar]**.\
   A la derecha de la [!UICONTROL Búsqueda avanzada] barra de herramientas.

1. (Opcional) Para volver a la página en la que se encontraba antes de la búsqueda, haga clic en **[!UICONTROL Cerrar]** en la esquina superior derecha.

>[!NOTE]
>
>La variable [!UICONTROL Resultados de la búsqueda] permanece abierta solo cuando está enfocada. Al hacer clic fuera de la página o abrir otra página, se cierra el [!UICONTROL Resultados de la búsqueda] página.
