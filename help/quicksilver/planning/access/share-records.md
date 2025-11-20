---
title: Compartir registros
description: Puede compartir registros con el botón Compartir para aumentar la colaboración en Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 7%

---


<!--update metadata with real information at release-->

# Compartir registros

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Puede ajustar los permisos de las personas a los registros individuales de un tipo de registro. O

Puede compartir un registro de Adobe Workfront Planning de las siguientes maneras:

* Compartir un vínculo al registro.

  Para obtener más información, vea [Compartir registros mediante un vínculo](/help/quicksilver/planning/records/share-records.md).

* Comparta todos los registros de un área de trabajo con otros usuarios compartiendo el área de trabajo y el tipo de registro.

  Para obtener más información, consulte los siguientes artículos:

   * [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md)

   * [Compartir un tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

* Compartir un registro con la opción **Compartir**.

  Este artículo describe cómo puede compartir un registro con otras personas mediante la opción **Compartir**.

>[!IMPORTANT]
>
>Los usuarios con acceso a un espacio de trabajo obtienen automáticamente al menos permisos de visualización para todos los registros del espacio de trabajo.
>Al compartir vistas, los usuarios no conceden permisos a los registros. Sólo los espacios de trabajo compartidos pueden conceder permisos a los usuarios para tipos de registro y registros.
>
>Para obtener información general sobre cómo compartir objetos en Workfront Planning, consulte también [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


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
<p>Cualquier paquete de Workfront y Planning</p> 
O
<p>Cualquier paquete de flujo de trabajo y planificación</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
   <p><b>NOTA</b></p>
   <p>Solo se pueden conceder permisos de administración a los registros a las personas con una licencia Standard. Todas las demás licencias solo pueden tener permisos de visualización y la opción Administrar aparece atenuada para ellas.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>  <p>Administrar permisos para un espacio de trabajo, un tipo de registro y el registro</p>  
   <p><b>IMPORTANTE</b></p>
   <p>Solo los usuarios con permisos de Administración de un espacio de trabajo pueden compartir un registro</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al compartir registros

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

* Puede compartir registros con las siguientes entidades: personas, grupos, equipos, empresas o roles.
* Cuando comparte un área de trabajo con los usuarios, también reciben los mismos permisos para los registros del área de trabajo de forma predeterminada.
* Cuando se quita una entidad de un espacio de trabajo, todos los permisos de uso compartido se quitan de los tipos de registro y de todos los registros que contiene.
* El acceso de un usuario al registro se determina mediante la combinación de las tres opciones siguientes:

   * Sus permisos se heredan del tipo de registro y del espacio de trabajo
   * Permisos agregados individualmente en el cuadro de diálogo de uso compartido de registros
   * Los siguientes permisos:

      * **Todos los usuarios del área de trabajo pueden ver**: esto hace que el registro sea visible para todos los usuarios del área de trabajo <!-- is this OK to say "workspace? should it be "record"??-->
      * **Solo las personas invitadas pueden acceder**: Esta opción está seleccionada de forma predeterminada y permite restringir el acceso al registro a personas específicas.

* Puede conceder los siguientes niveles de permisos a un registro:

   * Ver
   * Administrar

* Al compartir un registro con un usuario, se agregan con el mismo permiso que tienen en el tipo de registro de forma predeterminada.

  Por ejemplo:

   * Si tienen permisos de visualización en el tipo de registro, obtienen permisos de visualización en el registro
   * Si tiene permisos de tipo Contribuir o Administrar en el tipo de registro, obtiene permisos de Administración en el registro

* Como administrador del espacio de trabajo, puede compartir un registro con un usuario que no forme parte del espacio de trabajo. En este caso, aparece una advertencia junto a la entidad añadida que indica que no tienen acceso al espacio de trabajo. Puede aceptar agregar el usuario tanto al registro como al espacio de trabajo, o denegar su adición al espacio de trabajo, que también los elimina del registro.

* Cuando comparte un registro con usuarios que tienen permisos de Administración en el espacio de trabajo, también obtienen permisos de Administración en el registro de forma predeterminada. El permiso Ver aparece atenuado.

* Si no tiene permisos para agregar personas al espacio de trabajo, solo verá y agregará usuarios, equipos, grupos, funciones y empresas que ya se hayan agregado al espacio de trabajo. No se puede añadir ninguna otra entidad que no forme parte del espacio de trabajo.

* Puede deshabilitar los permisos heredados para un único registro, en cuyo caso puede concederles permisos individualmente, o pueden obtener permisos si pertenecen a la opción &quot;Todos en el espacio de trabajo&quot;. <!-- is this OK to say "workspace? should it be "record"??-->

* Si se aplican varios permisos de uso compartido para el mismo usuario, recibe el permiso más alto de esos permisos.

  Por ejemplo, si un registro se comparte con un usuario con permisos de visualización y su grupo con acceso de administración, obtiene permisos de administración en el registro.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Si un campo de fórmula o un campo de búsqueda de un registro conectado se basa en un campo de un registro en el que no tiene permisos, verá el cálculo correcto de los factores del registro a los que no puede tener acceso de otro modo.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Compartir permisos de registros

