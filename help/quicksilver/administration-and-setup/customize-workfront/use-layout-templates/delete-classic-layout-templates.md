---
title: Eliminar plantillas de diseño clásicas
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Las plantillas de diseño de la experiencia clásica de Workfront ya no están disponibles en la interfaz de Workfront, pero pueden afectar a los datos de Workfront. Esto puede provocar incoherencias en los campos afectados por las plantillas de diseño (como Compartido con) en los informes o paneles.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c68b63230b07ea8c8475b710e256b5e0f049b1eb
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Concesión de acceso administrativo a una plantilla de diseño

Las plantillas de diseño de la experiencia clásica de Workfront ya no están disponibles en la interfaz de Workfront, pero pueden afectar a los datos de Workfront. Esto puede provocar incoherencias en los campos afectados por las plantillas de diseño (como Compartido con) en los informes o paneles.

Puede resolver estas incoherencias eliminando las plantillas de diseño clásicas. Dado que no están disponibles en la interfaz de Workfront, el usuario debe utilizar la API de Workfront para eliminarlos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Eliminar las plantillas de diseño clásicas mediante una llamada de API

Puede introducir llamadas de API en la barra URL del navegador y pulsar Intro. La respuesta de la API se muestra en el explorador.

>[!NOTE]
>
>Las plantillas de diseño Global y Sistema no se pueden eliminar.

1. Inicie sesión en Workfront.
1. Busque la plantilla de diseño que desea eliminar mediante la siguiente llamada de API:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Tome nota del ID de la plantilla de diseño que desea eliminar.
1. Localice el ID de sesión con la siguiente llamada de API:
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Nunca comparta su ID de sesión con nadie.

1. Inserte el ID de la plantilla de diseño y el ID de sesión en la siguiente llamada de API:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Pegue la llamada de API del paso 4 en la barra URL del explorador y pulse Entrar.

   Esto elimina la plantilla de diseño.



