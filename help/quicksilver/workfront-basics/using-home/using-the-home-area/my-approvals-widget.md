---
product-area: home
navigation-topic: use-the-home-area
title: Administrar las aprobaciones con el widget Mis aprobaciones
description: El widget Mis aprobaciones muestra todas las aprobaciones pendientes, asignadas, delegadas y enviadas en un solo lugar. Aquí puede filtrar y organizar sus aprobaciones, tomar decisiones y delegar aprobaciones según sea necesario.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 19%

---

# Administrar las aprobaciones con el widget Mis aprobaciones

El widget Mis aprobaciones muestra todas las aprobaciones pendientes, asignadas, delegadas y enviadas en un solo lugar. Aquí puede filtrar y organizar sus aprobaciones, tomar decisiones y delegar aprobaciones según sea necesario.

El widget Mis aprobaciones admite aprobaciones de los siguientes objetos de Workfront:

* Tareas
* Problemas
* Proyectos
* Documentos
* Pruebas
* Solicitudes de registro de planificación
* Hojas de horas

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p>
   <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Vista o acceso superior a los objetos asociados con las aprobaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Vista o permisos superiores a los objetos asociados a aprobaciones</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aprobar trabajo desde el widget Mis aprobaciones

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Haga clic en **Personalizar** para agregar el widget **Mis aprobaciones**.
1. (Condicional) Haga clic en el menú desplegable **Filtro** y, a continuación, seleccione **Todos** para ver las aprobaciones que se le han asignado y delegado.

   >[!NOTE]
   >
   >Las aprobaciones asignadas a roles o grupos de trabajos no se muestran en Inicio. Las aprobaciones asignadas a los equipos se muestran en el widget Mis aprobaciones para cada miembro del equipo.


1. Seleccione el elemento en el que desea tomar una decisión de aprobación.

   ![Widget de mis aprobaciones](assets/my-approvals-widget.png)

1. Haga clic en una de las opciones disponibles al tomar una decisión de aprobación en el panel derecho. Las siguientes opciones se muestran en la esquina superior derecha de la página, según el tipo de elemento que apruebe:

   <table>
   <tr>
      <td>
      <p><strong>Acceso</strong></p>
      </td>
      <td>
      <p><strong>Elementos de trabajo</strong></p>
      </td>
      <td>
      <p><strong>Documentos</strong></p>
      </td>
      <td>
      <p><strong>Pruebas</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Conceder</li>
      <li>Ignorar</li>
      </ul>
      Si lo desea, puede ajustar el nivel de acceso en el menú desplegable <b>Cambiar acceso</b>.
      </td>
      <td>
         <ul>
         <li>Aprobar</li>
         <li>Reject</li>
         </ul>
      Puede dejar un comentario con su decisión haciendo clic en el menú desplegable del botón de decisión.
      </td>
      <td>
   Asignado como aprobador
         <ul>
         <li>Aprobar</li>
         <li>Aprobar con cambios</li>
         <li>Necesita trabajo</li>
         </ul>
   Asignado como revisor
         <ul>
         <li>Completar mi revisión</li>
         </ul>
      Las opciones de esta columna se aplican únicamente a las aprobaciones unificadas. Las aprobaciones de documentos heredados aparecen igual que las aprobaciones de elementos de trabajo. 
      </td>
      <td>
         <ul>
         <li>Ir a la revisión</li>
         </ul>
         La decisión se toma en el visualizador de pruebas. Para obtener información acerca de cómo revisar una revisión, vea <a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Revisar pruebas en Adobe Workfront</a>.
      </td>
   </tr>
   </table>

Después de tomar una decisión, la aprobación se elimina del widget Mi aprobación.