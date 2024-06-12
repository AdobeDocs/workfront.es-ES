---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Mover objetos de un entorno a otro dentro de Workfront
description: La función Promoción de entornos está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. No admite la capacidad de mover objetos transaccionales (con excepciones limitadas).
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: d249751b78e9d40fe7a351db14cbf0f3b7c79889
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 1%

---

# Descripción general del movimiento de objetos entre entornos de Workfront (Promoción de entornos)

La capacidad de promoción de entornos permite mover objetos de un entorno de Workfront a otro. Por ejemplo, puede crear una plantilla y configurarla en el entorno de zona protegida, sabiendo que las pruebas que realice no afectarán a los datos reales de su organización. Una vez configurada y probada la plantilla, puede moverla al entorno de producción, lista para usar.

Este proceso se denomina &quot;promoción del medio ambiente&quot;.

Puede realizar este proceso en Workfront creando un paquete de objetos para mover y luego instalando ese paquete en el nuevo entorno.

* Para obtener instrucciones específicas sobre cómo realizar este proceso en Workfront, consulte:

   * [Crear o editar un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Instalación de un paquete de promoción de entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Para obtener instrucciones sobre cómo realizar este proceso mediante la API de Workfront, consulte [Mover objetos entre [!DNL Workfront] entornos que utilizan la variable [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## Objetos compatibles para la promoción del entorno

La capacidad de promoción del entorno está diseñada para proporcionar la capacidad de mover objetos relacionados con la configuración de un entorno a otro. Se trata de objetos que se pueden configurar, como proyectos, equipos o formularios personalizados.

Debido a que la promoción del entorno trata la configuración de objetos, los objetos transaccionales (objetos que cambian con frecuencia o que dependen en gran medida del caso de uso) no se incluyen. Algunos ejemplos de objetos transaccionales son documentos, problemas, solicitudes, actualizaciones y decisiones de revisión y prueba.

* [Objetos de trabajo](#work-objects)
* [Objetos de informes](#reporting-objects)
* [Objetos de datos personalizados](#custom-data-objects)
* [Objetos de organización](#organization-objects)
* [Otros objetos de configuración](#other-configuration-objects)


### Objetos de trabajo

| Objeto promocionable | Objetos vinculados promocionales incluidos |
| --- | --- |
| Proyecto (PROJ) | Proyecto<br>Tarea<br>Asignación<br>Predecesora<br>Compañía<br>Tasa de anulación<br>Grupo<br>Rol<br>Equipo<br>Proceso de aprobación<br>Ruta de aprobación<br>Paso de aprobación<br>Aprobador de etapa<br>Programación<br>Día no laborable<br>Definición de cola<br>Grupo de temas de cola<br>Tema de cola<br>Regla de enrutamiento<br>Ruta de hitos<br>Hito<br>Tipo de hora<br>Conjunto de recursos<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |
| Plantilla (TMPL) | Plantilla<br>Tarea de plantilla<br>Asignación de tarea de plantilla<br>Tarea de plantilla predecesora<br>Compañía<br>Tasa de anulación<br>Grupo<br>Rol<br>Equipo<br>Proceso de aprobación<br>Ruta de aprobación<br>Paso de aprobación<br>Aprobador de etapa<br>Programación<br>Día no laborable<br>Definición de cola<br>Grupo de temas de cola<br>Tema de cola<br>Regla de enrutamiento<br>Ruta de hitos<br>Hito<br>Tipo de hora<br>Conjunto de recursos<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |

### Objetos de informes

| Objeto promocionable | Objetos vinculados promocionales incluidos |
| --- | --- |
| Plantilla de diseño (UITMPL) | Plantilla de diseño<br>Tablero<br>Calendario<br>Sección de calendario<br>Página externa<br>Informe<br>Filtrar<br>Agrupación<br>Ver<br>Parámetro |
| Tablero (PTLTAB) | Tablero<br>Calendario<br>Sección de calendario<br>Página externa<br>Informe<br>Filtrar<br>Agrupación<br>Ver<br>Parámetro |
| Calendario (CALEND) | Calendario<br>Sección de calendario |
| Página externa (EXTSEC) | Página externa |
| Informe (PTLSEC) | Informe<br>Filtrar<br>Agrupación<br>Ver<br>Parámetro |
| Filtro (UIFT) | Filtrar<br>Parámetro |
| Agrupación (UIGB) | Agrupación<br>Parámetro |
| Vista (UIVW) | Ver<br>Parámetro |

### Objetos de datos personalizados

| Objeto promocionable | Objetos vinculados promocionales incluidos |
| --- | --- |
| Categoría (CTGY) | Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría<br>Grupo |
| Parámetro (PARAM) | Parámetro<br>Opción de parámetro |
| Grupo de parámetros (PGRP) | Grupo de parámetros |

### Objetos de organización

| Objeto promocionable | Objetos vinculados promocionales incluidos |
| --- | --- |
| Grupo (GROUP) | Grupo <br>Subgrupos (hasta 5 niveles) *<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |
| Rol (ROLE) | Función |
| Equipo (EQUIPO) | Equipo<br>Grupo |
| Empresa (CMPY) | Compañía<br>Tasa de anulación<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Parámetro <br>Lógica de visualización de categoría<br>Grupo |
| Portfolio (PUERTO) | Portfolio<br>Programa<br>Grupo<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |
| Programa (PRGM) | Programa<br>Portfolio<br>Grupo<br>Categoría<br>Parámetro de categoría<br>Parámetro<br>Grupo de parámetros<br>Opción de parámetro<br>Lógica de visualización de categoría |

### Otros objetos de configuración

| Objeto promocionable | Objetos vinculados promocionales incluidos |
| --- | --- |
| Proceso de aprobación (ARVPRC) | Proceso de aprobación<br>Ruta de aprobación<br>Paso de aprobación<br>Aprobador de etapa<br>Rol<br>Equipo<br>Grupo |
| Programa (SCHED) | Programación<br>Día no laborable<br>Grupo |
| Ruta de hitos (MPATH) | Ruta de hitos<br>Hito |
| Perfil de hoja de horas (TSPRO) | Perfil de hoja de horas<br>Tipo de hora |
| Tipo de hora (HOURT) | Tipo de hora |
| Tipo de gasto (EXPTYPE) | Tipo de gasto |
| Tipo de riesgo (RSKTYPE) | Tipo de riesgo |
| Conjunto de recursos (RSPL) | Conjunto de recursos |

\* No disponible actualmente

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## Estados de promoción del entorno

Los paquetes de promoción de entornos pasan por varios estados a medida que se crean y preparan para moverse entre entornos. Puede ver estos estados en la lista de paquetes dentro de Workfront o en las respuestas de API si utiliza la API de Workfront.

Estos estados incluyen los siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>SIN MONTAR</td> 
   <td><p>Este estado se asigna automáticamente y representa un paquete que se ha guardado, pero que aún no se ha ensamblado. </p><p>Un usuario no puede establecer este estado directamente.</p></td> 
  </tr> 
  <tr> 
   <td>MONTAJE</td> 
   <td><p>Este estado se asigna automáticamente mientras se montan los objetos. </p><p>El ensamblado hace referencia al proceso automatizado de identificación de objetos y subobjetos que se van a incluir en un paquete y de adición de dichos objetos y sus datos al paquete.</p><p>Un usuario no puede establecer este estado directamente.</p></td> 
  </tr> 
  <tr> 
   <td>BORRADOR</td> 
   <td><p>Este estado se asigna al finalizar un proceso de ensamblado o al crear un paquete de promoción vacío.</p><p>Un usuario puede volver a mover el paquete de promoción a este estado.</p><p>En este estado, el paquete de promoción no se puede instalar en ningún entorno.</p></td> 
  </tr> 
  <tr> 
   <td>PRUEBAS</td> 
   <td><p>Este estado permite instalar un paquete de promoción en cualquier zona protegida de vista previa o actualización personalizada. Mientras se encuentre en este estado, el paquete no se podrá instalar en Producción.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIVO</td> 
   <td><p>Este estado permite instalar un paquete de promoción en cualquier entorno, incluido el de producción.</p><p>Cuando el estado de un paquete se establece en ACTIVO, la variable <code>publishedAt</code> La fecha se establece automáticamente en la marca de tiempo actual de la solicitud.</p></td> 
  </tr> 
  <tr> 
   <td>DESACTIVADO</td> 
   <td><p>Este estado se utiliza para ocultar los paquetes de promoción utilizados anteriormente que no se instalarán en ningún entorno en el futuro.</p><p>Cuando un paquete se encuentra en este estado, no se puede instalar en ningún entorno.</p><p>Cuando el estado de un paquete se establece en DESHABILITADO, la variable <code>retiredAt</code> La fecha se establece automáticamente en la marca de tiempo actual de la solicitud.</p><p>Se recomienda usar este estado en lugar de usar el <code>DELETE /package</code> extremo porque se puede recuperar y el historial de instalación se conserva para cualquier implementación realizada con este paquete.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>El paquete de promoción pasa automáticamente a este estado si falla la fase de MONTAJE.</p><p>Para devolver el paquete a la fase de MONTAJE, debe volver a almacenar en déclencheur el proceso de montaje.</p><p>Para obtener más información sobre cómo montar un paquete, consulte la sección <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">Editar o montar un paquete existente</a> en el artículo Crear o editar un paquete de promoción de entorno.</td> 
  </tr> 
  </tbody> 
</table>

