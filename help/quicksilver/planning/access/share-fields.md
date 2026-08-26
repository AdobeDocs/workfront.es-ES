---
title: Compartir campos de planificación de Workfront
description: Puede compartir el campo de un registro de Workfront Planning con otros usuarios para garantizar la colaboración al utilizar Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 3%

---


# Compartir campos de Workfront Planning

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Puede compartir el campo de un registro de Workfront Planning con otros usuarios para garantizar la colaboración al utilizar Adobe Workfront Planning.

El uso compartido de campos permite a los administradores del espacio de trabajo controlar el acceso a un campo individual. Cada campo de un tipo de registro tiene su propio cuadro de diálogo de uso compartido, donde el acceso se puede establecer en Sin acceso, Ver valores de campo o Administrar valores de campo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p> 
O
<p>Cualquier Workfront Planning como paquete de producto independiente</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td><p>Administre permisos en un campo para cambiar los valores del campo</p>  
   <p>Permisos de contribución o superiores a un tipo de registro para heredar los permisos de administración en el campo</p>  
   </td> 
  </tr>
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre el uso compartido de campos

* Puede compartir campos con usuarios, funciones del puesto, grupos, equipos o empresas.
* El acceso a un campo se obtiene combinando las siguientes configuraciones:

  * **Permisos heredados**: de forma predeterminada, un campo hereda el mismo acceso que alguien tiene en el tipo de registro (los permisos de Ver tipo de registro proporcionan a un usuario permisos para ver los valores de los campos; los permisos de Contribuir o Administrar tipo de registro proporcionan a un usuario permisos para administrar los valores de los campos). Puede desactivar los permisos heredados y proporcionar a los usuarios un acceso al campo menor que el que tienen para el tipo de registro.
  * **Todos los usuarios del área de trabajo pueden ver** o **Sólo los invitados pueden tener acceso a la selección**. Puede permitir que todos los usuarios con permisos en el espacio de trabajo vean el campo o conceder permisos solo a entidades individuales.

  Si se aplican varias reglas a la misma persona, reciben el permiso más alto disponible de una de las reglas.

* Solo los propietarios y administradores del espacio de trabajo pueden ajustar los permisos de los campos; los administradores del espacio de trabajo siempre conservan el acceso de Administración a todos los campos y esto no se puede reducir.
* El uso compartido de campos controla el acceso a los valores, no la configuración de los campos. Solo los administradores de espacio de trabajo pueden cambiar la configuración de un campo.
* Agregar a alguien a la lista de uso compartido de un campo no les concede acceso de tipo de registro o de espacio de trabajo. Si no tienen ese acceso, un icono de advertencia indica que el permiso solo surtirá efecto una vez que se añadan al tipo de registro.
* Los campos del sistema (por ejemplo, Creado por, Id. de registro) y los campos principales no pueden tener un uso compartido restringido.
* Los campos restringidos se aplican en todas partes donde se muestra el campo. Esto incluye todas las vistas, páginas de detalles de registro, formularios de solicitud, conexiones y campos de búsqueda, paneles de lienzo, la API y las herramientas de MCP.
* Los campos de búsqueda heredan los permisos de su campo de origen.
* Las vistas públicas siguen siendo totalmente visibles y de solo lectura para cualquier persona que pueda acceder a ellas.
* Cuando se duplica un registro, los valores restringidos no se copian en los registros nuevos.
* Los cambios de valor de campo restringidos no se registran en el historial de un registro.
* Los cambios de permisos para los campos no almacenan en déclencheur las notificaciones.
* Para los tipos de registro globales, los permisos de campo se aplican a todos los espacios de trabajo secundarios y no se pueden ajustar localmente.


De Claude:
Permisos adicionales para campos: puede añadir esto al artículo Información general para todo el uso compartido?? - help/quicksilver/planning/access/sharing-permissions-overview.md

Así se asigna el acceso de tipo de registro/espacio de trabajo al acceso de nivel de campo en el documento:

Niveles de permiso de campo (solo dos, más ninguno):

Sin acceso: el campo está completamente oculto
Ver valores de campo: puede ver el valor, no puede editarlo
Administrar valores de campo: puede ver y editar

Herencia predeterminada de la función de tipo de registro

Tipo de registro/acceso al espacio de trabajo Permiso de campo predeterminado
Ver valores de campo de vista
Contribute Administrar valores de campo
Administrar (administrador del espacio de trabajo) Administrar valores de campo (bloqueado; no se puede reducir)

De forma predeterminada, un campo simplemente refleja la función que alguien tenga en el tipo de registro: los visualizadores son de solo lectura, los colaboradores y los administradores obtienen derechos de edición. Los administradores de Workspace son un caso especial: cada vez que se añaden a la lista de uso compartido de un campo, &quot;Administrar valores de campo&quot; está preseleccionada y la opción &quot;Ver valores de campo&quot; está desactivada, ya que su acceso de edición nunca se puede quitar.

Configuración de comodín (reserva)
Independientemente de la herencia, cada campo tiene un comodín predeterminado:

Todos los usuarios del espacio de trabajo pueden ver (opción predeterminada)
Solo pueden acceder las personas invitadas

Cálculo del permiso final

Si los permisos heredados están habilitados: el acceso de una persona = el mayor de los permisos (heredado del tipo de registro, comodín, permiso concedido individualmente).
Si los permisos heredados están deshabilitados: el acceso de una persona = el más alto de (comodín, permiso concedido individualmente) — la función de tipo de registro ya no tiene en cuenta los permisos.
Si la herencia está deshabilitada, el comodín es &quot;Solo las personas invitadas pueden acceder&quot; y la persona no se agrega individualmente → no obtiene acceso.

Otras notas de permisos

Al conceder acceso individualmente a alguien, no se le concede acceso de tipo de registro o espacio de trabajo; simplemente permanece inactivo (con un icono de advertencia) hasta que se agrega por separado al espacio de trabajo.
Para los tipos de registro global, los permisos de campo se establecen una vez y se aplican a todos los espacios de trabajo secundarios; los administradores de espacios de trabajo secundarios/de equipo no pueden anularlos localmente.

## Compartir campos

