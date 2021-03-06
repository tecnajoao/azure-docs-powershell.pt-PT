---
title: Instalar o Azure PowerShell no macOS ou Linux
description: Como instalar o Azure PowerShell no macOS ou Linux.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 936bb24eecb4077080e172bf0d29fe57ec652187
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153693"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>Instalar o Azure PowerShell no macOS ou Linux

É possível executar o Azure PowerShell no PowerShell Core v6 em plataformas não Windows. Esta versão do PowerShell foi concebida para ser utilizada em qualquer plataforma que suporte o .NET Core. Para trabalhar com estas plataformas, existe uma versão especial do Azure PowerShell disponível para o .NET Core.

[!INCLUDE[az-replacing-azurerm.md](../includes/az-replacing-azurerm.md)]

## <a name="install-powershell-core"></a>Instalar o PowerShell Core

As instruções de instalação do PowerShell Core são diferentes para o macOS e para a maioria das distribuições do Linux.
Pode encontrar instruções detalhadas nos seguintes artigos:

* [Instalar o PowerShell Core no macOS](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Instalar o PowerShell Core no Linux](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>Instalar o Azure PowerShell para o .NET Core

O PowerShell Core é fornecido com o módulo do PowerShellGet já instalado. A instalação de módulos no PowerShell exige privilégios elevados, pelo que irá precisar de iniciar a sua sessão como um superutilizador:

```bash
sudo pwsh
```

Para instalar o Azure PowerShell, execute o seguinte comando:

```powershell-interactive
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> O módulo `AzureRM` descrito noutros artigos não é criado para o .NET Core e não irá funcionar com o PowerShell Core. Tanto `AzureRM` como `AzureRM.NetCore` utilizam os mesmos nomes de cmdlet, pelo que a única diferença é o nome do módulo de rollup e a versão de .NET para a qual são criados.

Por predefinição, a galeria do PowerShell não está configurada como um repositório fidedigno para o PowerShellGet. Na primeira vez que utilizar o PSGallery verá a seguinte linha de comandos:

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

Responda `Yes` ou `Yes to All` para continuar com a instalação.

## <a name="sign-in"></a>Iniciar sessão

Para começar a utilizar o Azure PowerShell, precisa de carregar `AzureRM.Netcore` para a sua sessão do PowerShell com o cmdlet [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) e, em seguida, iniciar sessão com as suas credenciais do Azure. __Não__ precisa de privilégios elevados para importar um módulo.

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

Irá precisar de repetir estes passos para cada nova sessão do PowerShell iniciada. A importação automática do módulo `AzureRM` implica configurar um perfil do PowerShell, um processo sobre o qual pode obter mais informações em [Acerca de Perfis](/powershell/module/microsoft.powershell.core/about/about_profiles).
No macOS e no Linux, deve trabalhar com o seu perfil através da variável de ambiente `$Profile`. Para saber como manter o início de sessão do Azure entre as sessões, veja [Manter credenciais do utilizador nas sessões do PowerShell](context-persistence.md).

## <a name="available-cmdlets"></a>Cmdlets disponíveis

Os módulos do Azure PowerShell para o .NET Core ainda estão em desenvolvimento. Estes módulos não fornecem o conjunto completo de cmdlets que estão disponíveis para a versão do Windows dos módulos. As seguintes funções estão implementadas nos módulos AzureRM.Netcore:

* Gestão de contas
  * Inicie sessão com a Conta Microsoft, a Conta escolar ou profissional, ou o Principal de Serviço através do Microsoft Azure Active Directory
  * Guarde as Credenciais no disco com o AzureRmContext guardar e carregue as credenciais guardadas com o Import-AzureRmContext
* Ambiente
  * Obtenha os diferentes ambientes do Microsoft Azure prontos a utilizar
  * Adicione/Defina/Remova ambientes personalizados (por exemplo, os ambientes do Azure Stack ou do Windows Azure Pack)
* Cmdlets do plano de gestão para os serviços do Azure através das interfaces do Resource Manager e da Gestão do Serviço.
  * Máquina Virtual
  * Serviço de Aplicações (Sites)
  * SQL Database
  * Armazenamento
  * Rede

## <a name="next-steps"></a>Passos Seguintes

Para obter mais informações sobre como utilizar o Azure PowerShell, veja o artigo [Introdução ao Azure PowerShell](get-started-azureps.md).
