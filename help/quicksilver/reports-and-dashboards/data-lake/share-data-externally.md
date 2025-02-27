---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Establezca una conexión con Workfront Data Connect
description: Workfront Data Connect le permite utilizar los datos de Workfront de su organización con herramientas de inteligencia empresarial o almacenarlos en un almacén de datos externo.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 55%

---

# Establezca una conexión con Workfront Data Connect

Workfront Data Connect le permite utilizar los datos de Workfront de su organización con herramientas de inteligencia empresarial o almacenarlos en un almacén de datos externo.

Para conectar el repositorio de datos de Data Connect con un producto externo, primero debe crear una conexión como se describe en [Crear una cuenta de lector o una conexión para Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). A continuación, debe agregar las IP necesarias a la lista de permitidos tal como se describe en [Agregar IP a la lista de permitidos](#add-ips-to-the-allowlist) siguiente.

La mayoría de los productos necesitarán la siguiente información sobre su lago de datos para establecer una conexión:

| Nombre de campo | Valor |
|---------------|-------------|
| Servidor | Dirección URL de la conexión, sin la parte `https://` (que se encuentra en la página **Conexión de datos** de Workfront*) |
| Puerto | `443` |
| Base de datos | `WORKFRONT` |
| Almacén | `READER_WH` |
| Esquema | `WF` |
| Función | `READER_ROLE` |
| Nombre de usuario | Nombre de usuario elegido al crear la conexión (encontrado en la página **Data Connect** de Workfront*) |
| Contraseña | Contraseña elegida en el primer inicio de sesión en Snowflake* |

*Para obtener información sobre dónde encontrar la página de **Data Connect** que contiene sus conexiones, consulte [Crear una cuenta de lector o una conexión para Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una vez añadida una entrada a la lista de permitidos IP, ya no se permitirán otras direcciones IP. Asegúrese de haber introducido todas las direcciones IP necesarias (tanto para las experiencias de creación como de lectura de la herramienta de visualización) antes de intentar utilizar la herramienta. Si no es así, puede encontrarse un error relacionado con las credenciales no válidas.
>
>Si no tiene ninguna dirección IP incluida en la lista de permitidos pero sigue teniendo problemas para conectarse a una herramienta de BI, compruebe en la configuración del servidor proxy la herramienta de BI.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td><p>Incluido en los siguientes planes:</p>
    <ul>
        <li><p>Ultimate</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect no está disponible para los planes Workfront heredados.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir direcciones IP a la lista de permitidos

1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configuración**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en la pestaña **IP permitidas** y luego haga clic en el botón **Añadir una dirección IP a su lista de permitidos**.

1. Escriba un nombre de la dirección IP en **Descripción de la dirección IP** e introduzca la dirección IP (o bloque CIDR) para la herramienta que desea utilizar en **Dirección IP**; a continuación, haga clic en **Añadir IP a la Lista de permitidos**.

   ![Añadir dirección IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Eliminar una dirección IP de la lista de permitidos

1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configuración**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en la pestaña **IP permitidas** y, a continuación, haga clic en el icono de la papelera ![Eliminar icono](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la dirección IP que desea eliminar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.

## Uso compartido de datos con herramientas de inteligencia empresarial

A continuación se enumeran una serie de herramientas comunes de inteligencia empresarial; visite sus sitios de documentación para obtener más información sobre la conexión a su lago de datos.

* Tableau
* Power BI
* Domo
* SAP HANA

## Almacenar datos en un almacén de datos externo

A continuación se enumeran una serie de almacenes de datos comunes; visite sus sitios de documentación para obtener más información sobre la conexión a su lago de datos.

* Databricks
* AWS Redshift
