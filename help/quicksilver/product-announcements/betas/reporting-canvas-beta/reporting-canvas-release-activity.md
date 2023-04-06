---
title: '''Reporting Canvas beta: actividad de versión"'
description: Actividad de la versión semanal de Adobe Workfront Reporting Canvas beta
hidefromtoc: true
source-git-commit: 4d41779e2e93e40f295bcff2bbdc0c84ea290b41
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Reporting Canvas beta: actividad de versión

Esta página enumera las nuevas funciones que se agregan y los problemas que se resuelven semanalmente para el lienzo de informes beta.

Para obtener información general sobre la versión beta del lienzo de informes, consulte [Reporting Canvas beta: información general](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Semana del 6 de noviembre

* Se agregaron las funciones PISO, NÚMERO y CADENA en el Generador de campos

## Semana del 23 de octubre

* Se ha agregado la función IF en el Generador de campos

## Semana del 4 de septiembre

* Se ha añadido la función IN al Generador de campos

## Semana del 24 de julio

* Se ha añadido la función AÑO al Generador de campos

## Semana del 17 de julio

* Se ha agregado la función WEEKDAYDIFF en el Generador de campos

## Semana del 26 de junio

* Funciones MONTH y DATEDIFF añadidas en el Generador de campos
* La agregación promedio de la visualización de KPI ahora muestra correctamente los decimales

## Semana del 19 de junio

* Se han añadido las funciones IZQUIERDA y DERECHA en el Generador de campos

## Semana del 12 de junio

* Se han movido las opciones de formato condicional al menú Estilo de tabla

## Semana del 29 de mayo

* Se han añadido categorías de agrupación de tabla para campos de fecha: día, semana, mes, trimestre y año

## Semana del 22 de mayo

* Funciones DIV y ROUND añadidas en el generador de campos

## Semana del 15 de mayo

* Se ha corregido un problema de alineación de texto del eje x en los gráficos

## Semana del 8 de mayo

* Se añadieron las funciones SUM, PROD y SUB en el generador de campos
* Mostrar un mensaje sin resultados cuando un filtro ha eliminado todos los resultados de una tabla
* Se ha habilitado el texto al pasar el ratón y la etiqueta de columna personalizada para los campos de fórmula de una tabla
* Clientes beta cerrados rehidratados ahora que el tiempo real está en su lugar
* Se ha proporcionado más espacio para el nombre del grupo

## Semana del 1 de mayo

* #Valor! se muestra en la celda cuando no se puede realizar un cálculo por fila
* Se agregó la validación al arrastrar y soltar determinados tipos de datos en determinadas funciones del generador de campos

## Funciones planificadas

Al desarrollar el Lienzo de informes, hemos rediseñado radicalmente algunas funciones (y hemos creado algunas nuevas desde cero) con el fin de racionalizar la creación de informes. En la tabla siguiente se describen las principales funciones del Lienzo de informes en comparación con las herramientas de informes existentes, así como su estado de versión actual:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>Descripción de la función</th> 
   <th>Terminología heredada </th> 
   <th>Terminología del lienzo de informes</th> 
   <th>Estado</th> 
  </tr> 
  <tr> 
   <td>Informes</td> 
   <td>Informe</td> 
   <td>Lienzo de informes</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Paneles</td> 
   <td>Panel</td> 
   <td>Lienzo de informes</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Tablas</td> 
   <td>Ficha Detalles</td> 
   <td>Bloque de tabla</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Gráficos</td> 
   <td>Ficha Gráfico</td> 
   <td>Bloque de visualización</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Subtotales</td> 
   <td>Ficha Resumen</td> 
   <td>Visualización de KPI</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Ruta de obtención de detalles</td> 
   <td>Modo del visor de informes</td> 
   <td>Superposición del visor de informes</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Columnas</td> 
   <td>Ficha Ver</td> 
   <td>Edición de tablas</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Filtros</td> 
   <td>Ficha Filtro</td> 
   <td>Edición de tablas</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Grupos</td> 
   <td>Ficha Grupo</td> 
   <td>Edición de tablas</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Configuración de campo<br>(agregaciones y formato condicional)</td> 
   <td>Ficha Ver</td> 
   <td>Edición de tablas (columna seleccionada)</td> 
   <td>Publicado</td> 
  </tr> 
  <tr> 
   <td>Cambio del tamaño de las columnas</td> 
   <td>Modo de texto</td> 
   <td>Edición de tablas (columna seleccionada)</td> 
   <td>Publicado</td> 
  </tr> 
   <tr> 
   <td>Contenido externo</td> 
   <td>Página externa</td> 
   <td>Bloque de contenido web</td> 
   <td>Publicado</td> 
  </tr> 
   <tr> 
   <td>Exportando</td> 
   <td>Acciones de informe</td> 
   <td><strong>Más</strong> en el visor</td> 
   <td>Publicado parcialmente</td> 
  </tr> 
  <tr> 
   <td>Uso compartido de columnas</td> 
   <td>Modo de texto</td> 
   <td>Generador de campos</td> 
   <td>Publicado parcialmente</td> 
  </tr> 
  <tr> 
   <td>Columnas calculadas</td> 
   <td>Modo de texto</td> 
   <td>Generador de campos</td> 
   <td>Publicado parcialmente</td> 
  </tr> 
  <tr> 
   <td>Estilo de gráfico</td> 
   <td>Ficha Gráfico</td> 
   <td>Bloque de visualización (pestaña Estilo)</td> 
   <td>Planificados</td> 
  </tr> 
  <tr> 
   <td>Entrega programada</td> 
   <td>Acciones de informe</td> 
   <td><strong>Más</strong> en el visor</td> 
   <td>Planificados</td> 
  </tr> 
  <tr> 
   <td>Concesión de acceso a informes</td> 
   <td>Acciones de informe</td> 
   <td><strong>Más</strong> en el visor</td> 
   <td>Planificados</td> 
  </tr> 
  <tr> 
   <td>Acceso a tableros no autenticado</td> 
   <td>Acciones del panel</td> 
   <td><strong>Más</strong> en el visor</td> 
   <td>Planificados</td> 
  </tr> 
  <tr> 
   <td>Edición de datos de informes</td> 
   <td>Edición en línea</td> 
   <td>Panel de resumen</td> 
   <td>Planificados</td> 
  </tr> 
  <tr> 
   <td>Filtro de página</td> 
   <td>N/D</td> 
   <td>Filtro Lienzo</td> 
   <td>Planificados</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Las funciones enumeradas aquí se lanzarán como parte de un esquema de lanzamiento de productos por niveles. Es posible que las funciones a las que tiene acceso en esta versión beta no estén disponibles en la versión completa, según el plan de su organización.