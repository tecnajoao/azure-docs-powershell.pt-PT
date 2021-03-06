---
title: Apresentação do módulo do Azure PowerShell Az
description: Apresentação do novo módulo do Azure PowerShell Az, a substituição do módulo AzureRM.
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 10665a72bc7dcae8ecf36b5ef4e2ab285a0e78b7
ms.sourcegitcommit: 89066b7c4b527357bb2024e1ad708df84c131804
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/09/2019
ms.locfileid: "59364100"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>Apresentação do novo módulo do Azure PowerShell Az

A partir de dezembro de 2018, o módulo do Az do Azure PowerShell passa a ser uma versão de disponibilidade geral e é agora o módulo indicado do PowerShell para interagir com o Azure. O Az oferece comandos mais curtos, maior estabilidade e suporte para várias plataformas. O Az também oferece paridade de funcionalidades e um caminho de migração fácil a partir do AzureRM.

O Az utiliza a biblioteca .NET Standard, o que significa pode ser executado no PowerShell 5 e no PowerShell 6.
Uma vez que o PowerShell 6 pode ser executado em Linux, macOS e Windows, o Azure PowerShell encontra-se agora disponível para todas as plataformas.
A utilização do .NET Standard permite-nos unificar a base de código do Azure PowerShell com o mínimo impacto nos utilizadores.

O Az é um módulo novo, pelo que a versão foi reposta para 1.0.0.

## <a name="upgrade-to-az"></a>Atualizar para Az

Recomenda-se que todos os utilizadores façam a atualização para o novo módulo do Az. Para tal:

* __RECOMENDADO__: [Desinstalar o módulo do Azure PowerShell AzureRM](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)
* [Instalar o módulo do Azure PowerShell Az](/powershell/azure/install-az-ps)
* Ative o modo de compatibilidade para adicionar aliases para cmdlets do AzureRM com `Enable-AzureRMAlias` enquanto se familiariza com o novo conjunto de comandos. Ative os aliases __apenas__ se não tiver o AzureRM instalado.

## <a name="migrate-existing-scripts-to-az"></a>Migrar scripts existentes para o Az

As atualizações importantes podem ser inconvenientes. No entanto, o módulo do Az tem um modo de compatibilidade para o ajudar a utilizar os scripts existentes enquanto trabalha nas atualizações para a nova sintaxe. Utilize o cmdlet `Enable-AzureRmAlias` para ativar o modo de compatibilidade do AzureRM. Este cmdlet define os nomes de cmdlets do AzureRM como aliases para os novos nomes de cmdlets do Az.

Os novos nomes de cmdlet foram criados para serem fáceis de aprender. Em vez de utilizar `AzureRm` ou `Azure` em nomes de cmdlet, utilize `Az`. Por exemplo, o comando antigo `New-AzureRMVm` tornou-se `New-AzVm`.

Para obter uma descrição completa do processo de migração, veja [Migrar do AzureRM para o Az](migrate-from-azurerm-to-az.md).

## <a name="the-future-of-support-for-azurerm"></a>O futuro do suporte para o AzureRM

O módulo do AzureRM existente deixará de receber novos cmdlets ou funcionalidades. No entanto, o AzureRM ainda é oficialmente mantido e será alvo de correções de erros até dezembro de 2020. Para se manter a par dos serviços e funcionalidades mais recentes do Azure, mude para o módulo Az.
