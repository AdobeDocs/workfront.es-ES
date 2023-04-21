---
title: Acceso configurable a la funcionalidad para cada tipo de objeto
description: Este artículo explica lo que puede permitir como administrador de Adobe Workfront para cada tipo de objeto, en cada nivel de acceso. También explica cuál es la configuración predeterminada para cada tipo de nivel de acceso.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '3435'
ht-degree: 10%

---

# Acceso configurable a la funcionalidad para cada tipo de objeto

Este artículo explica lo que puede permitir como administrador de Adobe Workfront para cada tipo de objeto, en cada nivel de acceso. También explica cuál es la configuración predeterminada para cada tipo de nivel de acceso.

Para obtener información sobre toda la funcionalidad disponible para un tipo de objeto en cada nivel de acceso, consulte [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Proyectos

En cada nivel de acceso, puede configurar las siguientes opciones para los proyectos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador (tipo de licencia de plan)</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir proyectos. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de los proyectos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Copiar</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Vista</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir proyectos. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite acceso limitado a la edición de proyectos. Para ver cómo el acceso de edición está limitado en un nivel de acceso de trabajador en comparación con un nivel de acceso de planificador (que permite el acceso de edición completo a los proyectos), consulte la sección <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Proyectos</a> en el artículo <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Funcionalidad disponible para cada tipo de objeto</a>.</p> <p>Para ajustar esto, puede configurar la capacidad de compartir proyectos. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Editar, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> (selección predeterminada) <p>El acceso a la vista es limitado porque no se puede ajustar para habilitar o deshabilitar el uso compartido de proyectos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los proyectos no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tareas

En cada nivel de acceso, puede configurar las siguientes opciones para las tareas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir tareas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a las tareas de edición.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir tareas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a las tareas de edición.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> (selección predeterminada)<p>El acceso a la vista es limitado porque no se puede ajustar para habilitar o deshabilitar el uso compartido de proyectos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a las tareas no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problemas

En cada nivel de acceso, puede configurar las siguientes opciones para los problemas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <p><b>Vista</b></p><p>Para ajustar esto, puede configurar la capacidad de compartir problemas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de problemas.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir problemas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de problemas.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir problemas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de problemas.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir problemas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de problemas.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los problemas no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portafolios

En cada nivel de acceso, puede configurar las siguientes opciones para portafolios:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir portafolios. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de portafolios.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> <p>El acceso a los portafolios no está disponible.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los portafolios no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programas

En cada nivel de acceso, puede configurar las siguientes opciones para los programas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir programas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de los programas.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> <p>El acceso a los programas no está disponible.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los programas no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informes, tableros y calendarios

En cada nivel de acceso, puede configurar las siguientes opciones para informes, tableros y calendarios:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <p><b>Vista</b></p><p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> ) y después deshabilitar o habilitar cualquiera de las siguientes acciones. Ambos están habilitados de forma predeterminada:</p> 
      <ul> 
       <li> <p>Ver informes integrados</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de informes, tableros y calendarios.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todas están activadas de forma predeterminada, excepto <b>Ver informes integrados</b>, <b>Compartir informes públicamente</b>y <b>Compartir en todo el sistema</b>.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Ver informes integrados</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir informes públicamente (externamente)</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> (selección predeterminada)<p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes acciones. Ambos están habilitados de forma predeterminada:</p> 
      <ul> 
       <li> <p>Ver informes integrados</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <p><b>Ver</b> (selección predeterminada)<p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes acciones. De forma predeterminada, solo está habilitada la opción Compartir .</p> 
      <ul> 
       <li> <p>Ver informes integrados</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <p><b>Ver</b> (selección predeterminada): Permite el acceso de solo vista a informes, tableros y calendarios que se han compartido con ellos.</p> <p>Para ajustar esto, puede configurar la capacidad de ver informes integrados. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> a continuación, deshabilite o habilite <b>Ver integrado</b>(deshabilitado de forma predeterminada).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los informes, tableros y calendarios no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filtros, vistas y agrupaciones

En cada nivel de acceso, puede configurar las siguientes opciones para filtros, vistas y agrupaciones:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <p><b>Vista</b></p><p>Para ajustar esto, puede configurar la capacidad de compartir filtros, vistas y agrupaciones. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de filtros, vistas y agrupaciones.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <p><b>Vista</b></p><p>Para ajustar esto, puede configurar la capacidad de compartir filtros, vistas y agrupaciones. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de filtros, vistas y agrupaciones.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir filtros, vistas y agrupaciones. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de filtros, vistas y agrupaciones.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Vista</b>:</p> <p>Para ajustar esto, puede configurar la capacidad de compartir filtros, vistas y agrupaciones. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de filtros, vistas y agrupaciones.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a filtros, vistas y agrupaciones no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Documentos

En cada nivel de acceso, puede configurar las siguientes opciones para los documentos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir documentos. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de documentos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todas están activadas de forma predeterminada, excepto <b>Compartir documentos públicamente</b> y <b>Compartir en todo el sistema</b>.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir documentos públicamente (externamente)</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <p><b>Vista</b></p><p>Para ajustar esto, puede configurar la capacidad de compartir documentos. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de documentos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todas están activadas de forma predeterminada, excepto <b>Compartir documentos públicamente</b> y <b>Compartir en todo el sistema</b>.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir documentos públicamente (externamente)</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir documentos. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de documentos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes acciones. Todas están activadas de forma predeterminada, excepto las dos últimas, <b>Compartir documentos públicamente</b> y <b>Compartir en todo el sistema</b>.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir documentos públicamente (externamente)</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <p><b>Vista</b></p><p>Para ajustar esto, puede configurar la capacidad de compartir documentos. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de documentos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los documentos no se puede configurar en este nivel de acceso. Pero los usuarios externos pueden usar Workfront para ver, revisar y descargar documentos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Usuarios

En cada nivel de acceso, puede configurar las siguientes opciones para los usuarios:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <p><b>Vista</b></p><p>Para ajustar esto, puede configurar la capacidad de ver la información de contacto de los usuarios. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> a continuación, deshabilite o habilite el <b>Ver información de contacto</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición a los usuarios.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes acciones. Solo las dos primeras opciones, <b>Crear</b> y <b>Eliminar</b>, están activados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li>Administrador de usuarios (todos los usuarios)</li> 
       <li> <p>Administrador de usuarios (usuarios de grupo)</p> </li> 
      </ul> <p>Para obtener más información sobre las dos opciones de Administración de usuarios, consulte la sección <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configuración del acceso de los usuarios para editar los usuarios mediante un nivel de acceso personalizado</a> en el artículo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li><p> <b>Ver</b> (solo opción disponible)</p><p>Para ajustar esto, puede configurar la capacidad de ver la información de contacto de los usuarios. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> a continuación, deshabilite o habilite el <b>Ver información de contacto</b> (activada de forma predeterminada).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li><p> <b>Ver</b> (solo opción disponible)</p> <p>Para ajustar esto, puede configurar la capacidad de ver la información de contacto de los usuarios. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> y, a continuación, activar o desactivar el <b>Ver información de contacto</b> (desactivada de forma predeterminada).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Ver</b> (solo opción disponible)</p><p>Para ajustar esto, puede configurar la capacidad de ver la información de contacto de los usuarios. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> y, a continuación, activar o desactivar el <b>Ver información de contacto</b> (desactivada de forma predeterminada).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los usuarios no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Equipos

En cada nivel de acceso, puede configurar las siguientes opciones para equipos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li><b>Vista</b> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Ambas están deshabilitadas de forma predeterminada.</p> 
      <ul> 
       <li>Ver todos los equipos</li> 
       <li> <p>Ver equipos asociados con mis grupos</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición para los equipos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Todas están activadas de forma predeterminada, excepto para <b>Editar equipos en los que estoy</b>.</p> 
      <ul> 
       <li>Crear</li> 
       <li>Eliminar</li> 
       <li> <p>Editar los equipos en los que estoy</p> </li> 
       <li> <p>Editar los equipos de los grupos que administro (solo para Administradores de grupos)</p> </li> 
       <li> <p>Ver todos los equipos</p> </li> 
       <li> <p>Ver equipos asociados con mis grupos</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <b>Vista</b>
      <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Ambos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li>Ver todos los equipos</li> 
       <li> <p>Ver equipos asociados con mis grupos</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición para los equipos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Solo la primera opción, <b>Editar equipos en los que estoy</b>, está desactivado de forma predeterminada.</p> 
      <ul> 
       <li> <p>Editar los equipos en los que estoy</p> </li> 
       <li> <p>Ver todos los equipos</p> </li> 
       <li> <p>Ver equipos asociados con mis grupos</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b>Ver</b> (solo opción disponible)</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Ambos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Ver todos los equipos</p> </li> 
       <li>Ver equipos asociados con mis grupos</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Ver</b> (solo opción disponible)</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Ambos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Ver todos los equipos</p> </li> 
       <li>Ver equipos asociados con mis grupos</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los equipos no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Plantillas

En cada nivel de acceso, puede configurar las siguientes opciones para las plantillas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li><p> <b>Vista</b></p> <p>Para ajustar esto, puede configurar la capacidad de compartir plantillas. Haga clic en el icono del engranaje <img src="assets/gear-icon-in-access-levels.png"> en el botón Ver, desactive o habilite el <b>Compartir</b> (activada de forma predeterminada).</p> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de plantillas.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Todos ellos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li> <p>Crear</p> </li> 
       <li> <p>Eliminar</p> </li> 
       <li> <p>Compartir</p> </li> 
       <li> <p>Compartir en todo el sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <p><b>Sin acceso</b> (solo opción disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b>Sin acceso</b> (solo opción disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Sin acceso</b> (solo opción disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a las plantillas no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Datos financieros

En cada nivel de acceso, puede configurar las siguientes opciones para los datos financieros:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <p><b>Vista</b>:</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Ambos están habilitados de forma predeterminada.</p> 
      <ul> 
       <li>Ver tarifas de facturación y de costo de rol</li> 
       <li> <p>Ver tarifas de facturación y de costo de usuario</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de datos financieros.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Ver</b> , luego deshabilite o habilite cualquiera de las siguientes opciones*. Solo las dos últimas opciones, <b>Ver tasas de costes y facturación de funciones</b> y <b>Ver Tasas de Facturación y Costes de Usuario</b>, están activados de forma predeterminada.</p> 
      <ul> 
       <li>Editar tarifas de facturación y de costo de rol</li> 
       <li> <p>Editar tarifas de facturación y de costo de usuario</p> </li> 
       <li>Ver tarifas de facturación y de costo de rol</li> 
       <li> <p>Ver tarifas de facturación y de costo de usuario</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li> <p><b>Sin acceso</b> (selección predeterminada)</p> </li> 
     <li> <b>Vista</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b>Sin acceso</b> (selección predeterminada)</p> </li> 
     <li><b>Vista</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Sin acceso</b> (solo opción disponible)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso a los datos financieros no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Para obtener información sobre estas opciones, consulte [Información general sobre facturación e ingresos](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Administración de recursos

En cada nivel de acceso, puede configurar las siguientes opciones para la Administración de recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nivel de acceso</th> 
   <th>Opciones</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planificador </td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Vista</b> </li> 
     <li> <p><b>Editar</b> (selección predeterminada): Permite el acceso completo a la edición de la Administración de recursos.</p> <p>Para ajustar esto, haga clic en el icono de engranaje <img src="assets/gear-icon-in-access-levels.png"> en el <b>Editar</b> , luego deshabilite o habilite cualquiera de las siguientes opciones. Solo la primera opción, <b>Editar prioridades y horas de presupuesto en el Planificador</b>, está habilitado de forma predeterminada.</p> 
      <ul> 
       <li> <p> Editar prioridades y horas presupuestadas en el Planificador</p> </li> 
       <li> <p>Administrar conjuntos de recursos</p> <p><b>NOTA</b>: Para administrar los grupos de recursos, un usuario necesita acceso adicional a los datos financieros y permisos para las finanzas de los proyectos. Si concede acceso a la Administración de Recursos a un usuario de Planificador que no tenga acceso a datos financieros, el usuario podrá ver las asignaciones por hora en el Planificador de Recursos, pero no podrá cambiar a la vista Costes ni ver el Caso de Negocio. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Concesión de acceso a datos financieros</a> y <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartir permisos financieros en un objeto</a>.</p> </li> 
       <li> <p>Actualizar horas planificadas en el Distribuidor de cargas de trabajo</p> <p><b>NOTA</b>: Para actualizar las horas planificadas en el equilibrador de carga de trabajo, un usuario necesita permiso para contribuir al objeto, con la opción Crear asignaciones habilitada en Configuración avanzada . Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre cómo compartir permisos en objetos</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabajador </td> 
   <td> 
    <ul> 
     <li><b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> </li> 
     <li> <b>Ver</b> (selección predeterminada)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sin acceso</b> (solo opción disponible) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuario externo</td> 
   <td> <p>El acceso no está disponible. Los usuarios externos solo pueden usar Workfront para revisar y descargar documentos y ver calendarios que se han compartido con ellos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Área de Planificador de escenario

La configuración predeterminada para todos los niveles de acceso es Sin acceso. Un administrador de Workfront puede cambiar esto a Ver o Editar acceso para cualquier nivel de acceso de Planificador, Trabajador y Revisor.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Los usuarios pueden ver un plan que otro usuario creó solo si se comparte con ellos un vínculo al plan.

## Área de objetivos de Workfront

Los seis niveles de acceso predeterminados (y los cuatro tipos de licencia) pueden editar y ver los objetivos de Workfront.

Editar es la opción predeterminada.
