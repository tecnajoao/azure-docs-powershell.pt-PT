---
title: Consultar recursos e resultados de formatação do Azure | Microsoft Docs
description: Como consultar recursos no Azure e formatar os resultados.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: 9a7627a25f9bbd196b1d615229e45a6e1ce7a7d9
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153763"
---
# <a name="querying-for-azure-resources"></a>Consultar recursos do Azure

A consulta no PowerShell pode ser concluída através de cmdlets incorporados. No PowerShell, os nomes dos cmdlets têm a forma de  **_Verbo-Nome_**. Os cmdlets com o verbo **_Get_** são os cmdlets de consulta. Os nomes dos cmdlets são os tipos de recursos do Azure alterados pelos verbos dos cmdlets.

## <a name="selecting-simple-properties"></a>Selecionar propriedades simples

O Azure PowerShell tem formatação predefinida para cada cmdlet. As propriedades mais comuns para cada tipo de recurso são apresentadas automaticamente num formato de tabela ou lista. Para obter mais informações sobre como formatar o resultado, veja [Formatar resultados da consulta](formatting-output.md).

Utilize o cmdlet `Get-AzureRmVM` para consultar uma lista de VMs na sua conta.

```powershell-interactive
Get-AzureRmVM
```

O resultado predefinido é formatado automaticamente como uma tabela.

```output
ResourceGroupName          Name   Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----   --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610 westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```

O cmdlet `Select-Object` pode ser utilizado para selecionar as propriedades específicas que lhe interessam.

```powershell-interactive
Get-AzureRmVM | Select Name,ResourceGroupName,Location
```

```output
Name          ResourceGroupName Location
----          ----------------- --------
MyUnbuntu1610 MYWESTEURG        westeurope
MyWin2016VM   MYWESTEURG        westeurope
```

## <a name="selecting-complex-nested-properties"></a>Selecionar propriedades aninhadas complexas

Se a propriedade que quer selecionar estiver muito aninhada na saída JSON, tem de indicar o caminho completo para essa propriedade aninhada. O exemplo seguinte mostra como selecionar o Nome da VM e o tipo de SO a partir do cmdlet `Get-AzureRmVM`.

```powershell-interactive
Get-AzureRmVM | Select Name,@{Name='OSType'; Expression={$_.StorageProfile.OSDisk.OSType}}
```

```output
Name           OSType
----           ------
MyUnbuntu1610   Linux
MyWin2016VM   Windows
```

## <a name="filter-result-using-the-where-object-cmdlet"></a>Filtrar resultado com o cmdlet Where-Object

O cmdlet `Where-Object` permite filtrar o resultado com base em qualquer valor de propriedade. No exemplo seguinte, filtro seleciona apenas as VMs com o texto "RGD" no respetivo nome.

```powershell-interactive
Get-AzureRmVM | Where ResourceGroupName -like RGD* | Select ResourceGroupName,Name
```

```output
ResourceGroupName  Name
-----------------  ----
RGDEMO001          KBDemo001VM
RGDEMO001          KBDemo020
```

No próximo exemplo, os resultados vão devolver as VMs que tenham o tamanho de VM “Standard_DS1_V2”.

```powershell-interactive
Get-AzureRmVM | Where vmSize -eq Standard_DS1_V2
```

```output
ResourceGroupName          Name     Location          VmSize  OsType              NIC ProvisioningState
-----------------          ----     --------          ------  ------              --- -----------------
MYWESTEURG        MyUnbuntu1610   westeurope Standard_DS1_v2   Linux myunbuntu1610980         Succeeded
MYWESTEURG          MyWin2016VM   westeurope Standard_DS1_v2 Windows   mywin2016vm880         Succeeded
```
