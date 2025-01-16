---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Términos básicos en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 88%

---

# Términos básicos de [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Glosario de Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/fusion-glossary.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere una licencia de [!DNL Adobe Workfront Fusion], además de una licencia de [!UICONTROL Adobe Workfront].


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Acción</p> </td> 
   <td>Módulo que permite leer o escribir paquetes desde o hacia una aplicación o servicio seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>Tipo de módulo que combina varios paquetes (varias matrices de datos) en uno solo. Para obtener más información, consulte <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">el módulo [!UICONTROL Aggregator] en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Clave API</td> 
   <td>Código único que identifica al usuario, desarrollador o programa que llama a la API de un software y que se utiliza para la autenticación. Dado que los módulos de [!DNL Adobe Workfront Fusion] funcionan conectando API, a veces son necesarias las claves de API. La aplicación que las requiere distribuye las claves de API. Por ejemplo, si se necesita una clave de API para [!DNL ActiveCampaign], es necesario solicitarla a través de la cuenta de [!DNL ActiveCampaign].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aplicación o servicio</td> 
   <td> <p>Normalmente, una aplicación de software.</p> <p>Una aplicación también puede ser una función especial que manipule datos, como un iterador o un agregador. </p> <p>Un servicio es una fuente de paquetes que pueden incluir una API web, una página web, distintos tipos de servidores (FTP, SMTP o IMAP), etc. </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conector de la aplicación</td> 
   <td>Aplicación que se conecta a otro sistema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Paquete</p> </td> 
   <td> <p>Un paquete es una unidad básica que los módulos devuelven o reciben. Un paquete consta de elementos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Al añadir una aplicación o servicio a un escenario, lo más probable es que tenga que crear primero una conexión entre [!DNL Workfront Fusion] y la aplicación o servicio para recuperar o enviar los datos seleccionados. Para obtener más información, consulte <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Información general sobre las conexiones</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ciclo</p> </td> 
   <td> <p>Los ciclos hacen referencia a dos fases de la ejecución del escenario: operación y confirmación. El escenario puede consistir en uno o más ciclos. Para obtener información más detallada, consulte <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Fases, ciclos y ejecución de escenarios en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Almacén de datos</p> </td> 
   <td> <p>Herramienta que almacena datos de escenarios o permite transferir datos entre escenarios individuales o ejecuciones de escenarios. Para obtener más información, consulte <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Almacenes de datos en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transferencia de datos</p> </td> 
   <td> <p>Cantidad de datos transferidos a través de su escenario. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Detalles del escenario en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filtro</p> </td> 
   <td> <p>Funciones adicionales que se pueden aplicar entre dos módulos. Los filtros permiten trabajar únicamente con paquetes que se ajusten a determinados criterios. Es posible aplicar una serie de filtros diferentes. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Añadir filtros a escenarios en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Identificador</p> </td> 
   <td> <p>Nombre que se utiliza para identificar paquetes de forma exclusiva. Se usa generalmente un ID para diferenciar un paquete que se actualizará o eliminará de un servicio determinado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Elementos</p> </td> 
   <td> <p>Parte de un paquete. Los paquetes pueden constar de varios elementos. Existen varios tipos diferentes de elementos: texto, número, booleano (sí/no), fecha, hora, búfer (datos binarios), colecciones, menú de selección, matriz y validación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>Tipo de módulo que permite tomar un paquete de datos (una matriz de datos) y dividirlo en paquetes separados. Para obtener más información, consulte <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">el módulo [!UICONTROL Iterator] en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Módulo</p> </td> 
   <td> <p>Un solo paso dentro de un escenario que realiza una función, como crear un registro, dentro de la aplicación o servicio asociado.</p> <p>Cada aplicación o servicio tiene varios módulos que definen la forma en que responde a solicitudes.</p> <p>Existen 4 tipos de módulos: acciones, activadores, iteradores y agregadores.</p> <p> <img src="assets/module.jpg"> </p> <p>Para obtener más información, consulte <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Operación</p> </td> 
   <td> <p>Tarea realizada por un módulo.</p><p>Para obtener más información, consulte <a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">Operaciones en [!DNL Adobe Workfront Fusion]</a>.</p>
  </tr> 
  <tr> 
   <td role="rowheader">Claves públicas/privadas</td> 
   <td>Las claves públicas y privadas se utilizan para cifrar y descifrar datos. La clave pública se puede distribuir y cualquier persona que la tenga puede cifrar datos, pero solo la clave privada puede descifrarlos. Del mismo modo, un usuario con una clave privada podrá cifrar datos que cualquier persona que tenga la clave pública podrá descifrar. El cifrado de clave privada garantiza que los datos provengan del propietario de la misma y sirve como validación de la fuente de los datos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>Permite duplicar datos o añadir nuevas rutas a un escenario para volver a enrutar datos y administrar diferentes grupos de datos por separado. Para obtener más información, consulte <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">el módulo [!UICONTROL Router] en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Escenario</p> </td> 
   <td> <p>Serie creada por el usuario de pasos automatizados, cada uno representado y realizado por un módulo. El propósito de un escenario es mover y manipular datos.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creación de escenarios en[!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Segmento de escenario</p> </td> 
   <td> <p> Sección de un escenario que consta de una serie de módulos que se conectan a la misma aplicación. Los segmentos de escenario suelen representar un flujo de trabajo corto en la aplicación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Las transacciones</p> </td> 
   <td> <p>[!DNL Workfront Fusion] utilizan el procesamiento transaccional para capturar el ciclo de vida del escenario. Una transacción consta de varias fases durante las cuales los datos se transforman de un estado coherente a otro. Existen 4 fases: inicialización, operación (lectura o escritura), confirmación/reversión y finalización.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Activador</p> </td> 
   <td> <p>Módulo que permite obtener paquetes que se añadieron o actualizaron desde la última ejecución de un escenario. Existen 2 tipos de activador: sondeo e instantáneo (webhooks). Para obtener más información, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">activadores instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Tipo especial de activador que permite ejecutar escenarios inmediatamente después de que haya un nuevo paquete disponible. Para obtener más información, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Activadores instantáneos (webhooks) en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
