---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Las carpetas vinculadas no son compatibles con el objeto DOCU
description: Las carpetas vinculadas no son compatibles con el objeto DOCU
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# No se admite el uso de la API para agregar una carpeta vinculada

No se admite el uso de la API para agregar una carpeta vinculada a la matriz de carpetas para un objeto de documento (DOCU). La solicitud se realizará correctamente, pero algunos proveedores externos pueden eliminar el documento del sistema. Esto se debe a que el sistema externo se utilizará como la fuente final de la verdad. Por lo tanto, si se quita el documento del proveedor externo, se considera que el documento ya no existe. Cualquier documento que no se encuentre en la carpeta vinculada (externa) puede eliminarse automáticamente de [!DNL Workfront] sin forma de recuperarlos.
