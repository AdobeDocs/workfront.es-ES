---
user-type: administrator
product-area: system-administration;user-management
keywords: inicio rápido,inicio inicial,inicio rápido,inicio inicial
navigation-topic: use-kick-starts
title: 'Escenario de inicio rápido: Empresa, grupo, función y usuario - Inicio de preparación'''
description: Cuando empiece a implementar Adobe Workfront, en lugar de introducir datos manualmente, puede importar la lista de clientes, los departamentos internos, las funciones de trabajo y la información de usuario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 10%

---

# Escenario de inicio rápido: Empresa, grupo, función y preparación del inicio de sesión del usuario

Cuando empiece a implementar Adobe Workfront, en lugar de introducir datos manualmente, puede importar la lista de clientes, los departamentos internos, las funciones de trabajo y la información de usuario.

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Qué se puede importar

En la tabla siguiente se muestran las compañías, los grupos y las funciones que se van a importar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Compañías</strong> </th> 
   <th><strong>Grupos</strong> </th> 
   <th><strong>Funciones</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em>Su empresa</em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Finanzas</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Ventas</p> </td> 
   <td valign="top"> <p valign="top">Analista empresarial</p> <p valign="top">Controlador creativo</p> <p valign="top">Diseñador</p> <p valign="top">Gerente de recursos</p> <p valign="top">Patrón de depuración</p> <p valign="top">Escritor técnico</p> <p valign="top">Desarrollador web</p> </td> 
  </tr> 
 </tbody> 
</table>

Los nombres de funciones deben ser únicos, las funciones de trabajo existentes no se pueden importar.

En las tablas siguientes se muestran los usuarios que se van a importar y varios atributos de usuario para cada uno:

### Usuario 1

| **Nombre** | Chris |
|---|---|
| **Apellido** | Manning |
| **Nombre de usuario/correo electrónico** | mailto:cmanning@foo.com |
| **Contraseña** | updateMe |
| **Acceso** | Miembro del equipo |
| **Compañía** | &lt;*Su empresa>* |
| **Grupo de inicio** | Marketing |
| **Función** | Analista empresarial |

{style=&quot;table-layout:auto&quot;}

### Usuario 2

| **Nombre** | Jennifer |
|---|---|
| **Apellido** | Campbell |
| **Nombre de usuario/correo electrónico** | jcampbell@foo.com |
| **Contraseña** | updateMe |
| **Acceso** | Gerente del proyecto |
| **Compañía** | &lt;*Su empresa>* |
| **Grupo de inicio** | Marketing |
| **Función** | Gerente del proyecto |

{style=&quot;table-layout:auto&quot;}

### Usuario 3

| **Nombre** | Jill |
|---|---|
| **Apellido** | Sullivan |
| **Nombre de usuario/correo electrónico** | jsullivan@foo.com |
| **Contraseña** | updateMe |
| **Acceso** | Servicios de asistencia |
| **Compañía** | &lt;*Su empresa>* |
| **Grupo de inicio** | Ventas |
| **Función** | Representante de ventas |

{style=&quot;table-layout:auto&quot;}

### Usuario 4

| **Nombre** | Marc |
|---|---|
| **Apellido** | Lewis |
| **Nombre de usuario/correo electrónico** | mlewis@foo.com |
| **Contraseña** | updateMe |
| **Acceso** | Administrador de portafolios |
| **Compañía** | &lt;*Su empresa>* |
| **Grupo de inicio** | Finanzas |
| **Función** | Controlador |

{style=&quot;table-layout:auto&quot;}

### Usuario 5

| **Nombre** | Pam |
|---|---|
| **Apellido** | Reynolds |
| **Nombre de usuario/correo electrónico** | preynolds@foo.com |
| **Contraseña** | updateMe |
| **Acceso** | Gerente del proyecto |
| **Compañía** | *Su empresa>* |
| **Grupo de inicio** | Marketing |
| **Función** | IT |

{style=&quot;table-layout:auto&quot;}

### Usuario 6

| **Nombre** | Ray |
|---|---|
| **Apellido** | Andrews |
| **Nombre de usuario/correo electrónico** | randrews@foo.com |
| **Contraseña** | updateMe |
| **Acceso** | Administrador |
| **Compañía** | *Su empresa>* |
| **Grupo de inicio** | Gerente de recursos |
| **Función** | ninguno |

{style=&quot;table-layout:auto&quot;}

## Descargar una plantilla de inicio rápido

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Inicio** > **Importar datos.**

1. Haga clic en **Más opciones** para ver la lista completa de opciones de importación.
1. Seleccione los objetos Nivel de acceso, Empresa, Grupo, Función de trabajo y Usuario que desea importar.

## Información de la empresa de entrada

1. Abra el **Workfront.xlsx** archivo que acaba de descargar.

   >[!TIP]
   >
   >Al trabajar con hojas de datos muy anchas, puede que desee utilizar la herramienta Panel de congelación (o equivalente) del editor de hojas de cálculo para que sea más fácil trabajar con la hoja de cálculo.

1. Vaya a la hoja &#39;CMPY Company&#39;.

   Debería estar vacío a menos que las empresas ya estén en el sistema. ![](assets/cmpysheet-350x16.png)

   ![](assets/companyid--1--350x78.png)

1. Especifique TRUE en la variable **isNew** para abrir el Navegador.
1. Repita esta acción para cada empresa agregada. (En este ejemplo, complete esta acción para las filas 3-6 porque se están agregando cuatro empresas).

   ![](assets/cmpyisnew-350x86.png)

1. Especifique un ID único.

   Esto debe hacerse para cada fila de la columna ID. Los enteros que comienzan en 1 funcionan bien al crear registros nuevos.

   ![](assets/cmpyisnew-350x86.png)

1. Establezca un Nombre.

   Especifique los nombres de cada cliente en la variable **setName** para abrir el Navegador.

   ![](assets/companyid-350x78.png)

1. Vaya a la hoja Grupo GRUPO .

   A menos que ya haya creado grupos en Workfront, esta hoja debería mostrar solo el grupo predeterminado aprovisionado con cada cuenta de Workfront.

   ![](assets/groupsheet-350x15.png) ![](assets/emptygroupsheet-350x85.png)

1. Configure las variables **isNew** column.Según el escenario, se importarán 4 grupos, así que especifique TRUE en las filas 4 a 7 para la columna &#39;isNew&#39;.
1. Especifique un ID único.

   Esto debe hacerse para cada fila de la columna ID. Los enteros que comienzan en 1 funcionan bien al crear registros nuevos.

   ![](assets/groupids-350x85.png)

1. Establezca un Nombre.

   Especifique los nombres de cada departamento en la **setName** para abrir el Navegador.

   ![](assets/groupnames-350x85.png)

   Especifique la información de la función. Vaya a la hoja Función ROLE.

1. A menos que ya haya creado o eliminado roles en la cuenta, esta hoja debería mostrar 8 roles que se aprovisionan con cada cuenta de Workfront.

   ![](assets/groupnames-350x85.png)

1. Establezca True.

   Se están importando siete funciones de trabajo, escriba TRUE en las filas 12 a 18 para la columna &#39;isNew&#39;.

   ![](assets/roleisnew-350x104.png)

1. Especifique un ID único.

   Esto debe hacerse para cada fila de la columna ID. Los enteros que comienzan en 1 funcionan bien al crear registros nuevos.

   ![](assets/usersheet-350x16.png)

   ![](assets/roleisnew--1--350x104.png)

1. Escriba los nombres de cada función en la columna setName.

   ![](assets/roleisnew-350x104.png)

1. Proporcione detalles adicionales según sea necesario.

   Incluya tasas de facturación, tasas de coste y descripciones para las funciones que está creando, según sea necesario.

1. Vaya a la hoja USUARIO para introducir Información de Usuario.

   A menos que ya haya creado usuarios en su cuenta, esta hoja debería mostrar solamente el usuario administrador que está aprovisionado con cada cuenta de Workfront.

   ![](assets/rolenames-350x104.png) ![](assets/emptyusersheet-350x52.png)

1. Establezca el valor True especificando TRUE en las filas 4 a 9 para la columna &#39;isNew&#39;, ya que se están importando 6 usuarios.

   ![](assets/userisnew-350x52.png)

1. Para establecer un ID único, especifique un ID único en cada fila de la columna ID. Normalmente, los enteros que comienzan en 1 funcionan bien para registros nuevos.

   ![](assets/userisnew-350x52.png)

1. Introduzca los nombres de cada usuario en las columnas &quot;setFirstName&quot; y &quot;setLastName&quot;.

   ![](assets/usernames-350x52.png)

1. Defina valores de detalle especificando valores en las columnas &#39;setEmail&#39;, &#39;setPassword&#39; y &#39;setUsername&#39;.

   ![](assets/usercredentials-350x52.png)

1. Especifique los valores de nivel de acceso.

   Por ejemplo, Chris Manning, que es miembro del equipo, busque el ID en la hoja Nivel de acceso ACSLVL para el nivel de acceso de los miembros del equipo. Copie el ID en el portapapeles y, en la hoja Usuario de USUARIO, péguelo en el **setAccessLevelID** en la fila de Chris.

   Repita este paso para cada usuario y nivel de acceso.

   ![](assets/copyalid-350x171.png) ![](assets/pastealid-350x59.png)

1. Especifique los detalles del grupo en el hogar.

   Según el escenario, Chris Manning pertenece al grupo Marketing . En la hoja Grupo de GRUPOS, busque el ID del grupo de marketing, cópielo en el portapapeles y, en la hoja Usuario de USUARIO, péguelo en la **setHomeGroupID** en la fila de Chris. &#x200B;Repita este paso para cada asignación de usuario y grupo.

   ![](assets/copygroupid-1-350x133.png) ![](assets/pastegroupid-350x59.png)

1. Especifique los detalles de la empresa.

   Todos los usuarios de este escenario pertenecen a la misma empresa. En la hoja Empresa CMPY, busque el ID de la empresa *Su propia empresa *, copie el ID en el portapapeles y, en la ficha Usuario de usuario, pegue este valor en cada fila de la columna &quot;setCompanyID&quot;. &#x200B;

   Repita este paso para cada asignación de usuario y grupo.

   ![](assets/companyid--1--350x78.png)

   ![](assets/pastecompanyid-350x84.png)

1. Especifique los detalles de la función del trabajo.

   Según el escenario, Chris Manning tendrá la función de analista de negocios. En la hoja Función ROLE, localice el ID para el rol de analista de negocios, cópielo en el portapapeles y, en la hoja Usuario de USUARIO, péguelo en la columna &quot;setRoleID&quot; de la fila Chris. &#x200B;Repita este paso para cada asignación de usuario y grupo.

   ![](assets/copyroleid-350x149.png)

   ![](assets/pasteroleid-350x95.png)

1. Rellene otros detalles del usuario, según sea necesario, y luego guarde el archivo.
1. Importe el archivo de Excel.

   Siga las instrucciones proporcionadas en la **Importación de archivos de inicio rápido** de este artículo.
