---
title: Importar campos desde Adobe Workfront
description: En Adobe Workfront Planning, puede crear campos personalizados para cada tipo de registro. A continuación, puede asociar el campo con los registros de Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 31%

---

<!--add to TOC-->

# Importación de campos desde Adobe Workfront

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->


{{planning-important-intro}}

Puede importar copias de campos de Workfront existentes. Al importar campos desde Workfront, se crea una copia de cada campo para un tipo de registro de Workfront Planning.


## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar </p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos a un espacio de trabajo y tipo de registro </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon.</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Consideraciones sobre la importación de campos desde Workfront

* Puede importar campos de Workfront nativos o personalizados a un tipo de registro en Workfront Planning.
* La importación de campos de Workfront crea copias de los mismos campos y conserva el nombre del campo en Workfront Planning. Una vez copiados en Workfront Planning, los campos son independientes de los campos originales de Workfront y no comparten información.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Puede agregar campos nativos o personalizados desde los siguientes objetos de Workfront:
   * Portafolio
   * Programa
   * Proyecto
   * Tarea
   * Problema
   * Documento
   * Compañía
   * Grupo
   * Usuario
   * Función
   * Asignación
   * Hora
   * Registro de facturación
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * Gasto
   * Iteración
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* Es posible que los campos de Workfront no conserven su tipo de campo después de importarse en Workfront Planning.

  La tabla siguiente muestra los tipos de campo de Workfront y su tipo de campo de Workfront Planning correspondiente.

  | Tipo de campo de Workfront | Tipo de campo de Workfront Planning |
  |------------------------------------------|-------------------------------|
  | Texto con formato de una sola línea | Texto de línea única |
  | Texto de una sola línea con formato de número | Número |
  | Texto de una sola línea con formato de moneda | Divisa |
  | Párrafo | Párrafo |
  | Texto con formato | Párrafo |
  | Lista desplegable de selección única | Selección única |
  | Lista desplegable de selección múltiple | Selección múltiple |
  | Los filtros de escritura anticipada de usuario no son compatibles | Personas |
  | Calculado* | Fórmula |
  | Fecha | Fecha |
  | Grupo de casillas de verificación | Selección múltiple |
  | Botón de opción | Selección múltiple |

  *Los campos calculados estarán disponibles más adelante.
Todos los demás tipos de campos de Workfront no son compatibles con Workfront Planning.


## Importar campos desde Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registro desee utilizar para crear campos.

   Se abre el espacio de trabajo y se muestran los tipos de registro.

1. Haga clic en la tarjeta de un tipo de registro.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.

   >[!TIP]
   >
   >    Algunos campos pueden estar ocultos. Haga clic en **Campos** y habilite la opción para los campos que desee ver como columnas en la vista de tabla.

1. Haga clic en el icono **+** en la esquina superior derecha de la vista de tabla

   O

   Pase el puntero por encima del encabezado de cualquier columna, haga clic en la flecha hacia abajo después del nombre del campo y, a continuación, haga clic en **Insertar a la izquierda** o **Insertar a la derecha** para añadir el nuevo campo.
1. Haga clic en **Agregar** existente en la esquina inferior derecha de la ficha **Nuevo campo**. <!--check UI - did they change this??-->

   ![Agregar campos existentes del modal de Workfront](assets/add-existing-fields-from-workfront-modal.png)

1. Empiece a escribir el nombre de un campo de Workfront existente en el área de búsqueda y, a continuación, haga clic en **+** cuando se muestre en la lista.
1. (Opcional) Escriba otro campo y haga clic en **+** cuando se muestre en la lista.
1. (Opcional) Haga clic en el icono **Filtros** ![Filtros en el icono de importar campos](assets/filters-in-import-fields-icon.png) y, a continuación, actualice uno o ambos de los campos siguientes:

   * Tipo de objeto: seleccione un tipo de objeto Workfront cuyos campos desee importar.
   * Formulario personalizado: seleccione uno o varios formularios personalizados de Workfront. Puede seleccionar un formulario personalizado sin seleccionar primero un tipo de objeto.
1. Haga clic en **+** y luego en **Agregar campos**.
Los campos se agregan a la vista de tabla y a las páginas de detalles de los registros.

   >[!IMPORTANT]
   >
   >    Hay un límite de 500 campos para cualquier tipo de registro. Los campos existentes junto con los campos importados contribuyen a este límite.

   Los campos añadidos son copias de los campos de Workfront y ya no se conectan a los campos originales en Workfront.
