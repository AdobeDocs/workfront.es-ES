---
title: Compartir solicitudes de Planning
description: Una vez enviada, puede compartir una solicitud de Workfront Planning con otros usuarios.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 4ee702aeded88e330ec456a0e6b5cf1813bfb64e
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 6%
---
# Compartir solicitudes de Planning

<!--add to TOC, and miniTOC-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Después de enviar una solicitud de Planning, puede controlar quién la ve, quién puede trabajar en ella y qué acciones puede realizar cada persona o equipo. Esto mantiene a las personas adecuadas centradas en las solicitudes correctas y garantiza que puedan realizar únicamente las acciones adecuadas a su función.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p> 
O
<p>Cualquier planificación de Workfront cuando se compra como producto independiente</p> 
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
   <td>   <p>Permisos de visualización o superiores para un espacio de trabajo y tipo de registro, si es un usuario de Workfront</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al compartir solicitudes

* Puede conceder los siguientes permisos a los usuarios de una solicitud:

  * Ver: Los usuarios solo pueden ver la solicitud.
  * Contribute: los usuarios pueden ver, editar y comentar la solicitud.
  * Administrar: los usuarios pueden ver, editar, comentar y eliminar la solicitud.

* A los solicitantes se les concede automáticamente acceso de administración a las solicitudes que envían, a menos que un administrador haya configurado un valor predeterminado diferente.

  Para obtener más información, consulte [Crear formulario de solicitud](/help/quicksilver/planning/requests/create-request-form.md).

* Los administradores de Workfront pueden acceder a todas las solicitudes y gestionarlas.
* Los usuarios con acceso de Administración a un tipo de registro heredan el acceso de Administración al formulario de admisión de ese tipo de registro y a todas las solicitudes enviadas a través de él.
* Cualquier persona con permisos para una solicitud puede compartirla con el mismo nivel de permisos o con un nivel inferior al suyo.

  Los usuarios con permisos de tipo Contribuir no pueden conceder a nadie más permisos de administración para la solicitud.

* Distintas personas y equipos pueden tener diferentes niveles de acceso en la misma solicitud.
* Los permisos se pueden asignar a través de varias entidades. Si un usuario tiene permisos de contribución en una solicitud pero su grupo o función de trabajo tiene permisos de visualización, conserva el nivel más alto de permisos, que es de contribución.

## Compartir una solicitud

Asegúrese de utilizar la nueva experiencia de solicitud.

1. {{step1-to-requests}}
1. Busque una solicitud de Planning y haga clic en ella para abrirla.
1. Haga clic en **Compartir**.

   Se abre el cuadro **Compartir** para la solicitud seleccionada.

   ![Cuadro para compartir solicitudes](assets/requests-sharing-box.png)

1. En el campo **Conceder acceso a esta solicitud**, empiece a escribir el nombre de un usuario, equipo, rol, grupo o compañía y haga clic en él cuando aparezca en la lista.

   En la lista solo se muestran las entidades activas.
1. En el menú desplegable situado a la derecha del nombre de cada entidad, seleccione uno de los siguientes niveles de permisos:

   * Administrar
   * Aportar
   * Ver
1. (Opcional) Para cada nivel de permiso, haga clic en el icono de permiso granular y seleccione o anule la selección de cualquier permiso granular, como **Editar**, **Comentario**, **Compartir** o **Eliminar**.

   ![Permisos granulares en solicitudes](assets/granular-permissions-on-requests.png)
1. Haga clic en **Guardar**.

   La solicitud se comparte con las entidades seleccionadas.


