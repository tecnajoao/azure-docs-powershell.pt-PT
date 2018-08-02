---
title: Iniciar sessão com o Azure PowerShell
description: Como iniciar sessão com o Azure PowerShell como um utilizador, principal de serviço ou com o MSI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 20194ac2282d602ba61bf130791edac9f4ffae6c
ms.sourcegitcommit: fd11600079ee3844986552bccc4e274a231332b6
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/02/2018
ms.locfileid: "39368148"
---
# <a name="sign-in-with-azure-powershell"></a>Iniciar sessão com o Azure PowerShell

O Azure PowerShell suporta vários métodos de autenticação. A forma mais simples de começar é iniciar sessão interativamente na linha de comandos.

## <a name="sign-in-interactively"></a>Iniciar sessão interativamente

Para iniciar sessão interativamente, utilize o cmdlet [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount).

```azurepowershell
Connect-AzureRmAccount
```

Quando é executado, este cmdlet apresenta uma caixa de diálogo que lhe pede para indicar o endereço de e-mail e a palavra-passe associados à sua conta do Azure. Quando efetuar a autenticação, essas informações são guardadas para a sessão atual do PowerShell, a caixa de diálogo é fechada e tem acesso a todos os cmdlets do Azure PowerShell.

> [!IMPORTANT]
> A partir do Azure PowerShell 6.3.0, as suas credenciais são partilhadas entre várias sessões do PowerShell, desde que mantenha sessão iniciada no Windows. Para obter mais informações, veja o artigo sobre [Credenciais Persistentes](context-persistence.md).

## <a name="sign-in-with-a-service-principal"></a>Iniciar sessão com um principal de serviço

Os principais de serviço proporcionam uma forma de criar contas não interativas que pode ser utilizar para manipular recursos. Os principais de serviço são como contas de utilizador às quais pode aplicar regras com o Azure Active Directory. Ao conceder as permissões mínimas necessárias para um principal de serviço, pode garantir que os seus scripts de automatização estão ainda mais protegidos.

Se precisar de criar um principal de serviço para utilizar com o Azure PowerShell, veja [Criar um principal de serviço do Azure com o Azure PowerShell](create-azure-service-principal-azureps.md).

Para iniciar sessão com um principal de serviço, utilize o argumento `-ServicePrincipal` com o cmdlet `Connect-AzureRmAccount`. Também irá precisar do ID de aplicação do principal de serviço, das credenciais de início de sessão e da associação do ID de inquilino ao principal de serviço. Para obter as credenciais do principal de serviço como o objeto adequado, utilize o cmdlet [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential). Este cmdlet irá apresentar uma caixa de diálogo para introduzir o ID de utilizador e a palavra-passe do principal de serviço.

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-vm-managed-service-identity"></a>Iniciar sessão com uma Identidade de Serviço Gerida de VM do Azure

Identidade do Serviço Gerido (MSI) é uma funcionalidade de pré-visualização do Azure Active Directory. Pode utilizar um principal de serviço do MSI para início de sessão e adquirir um token de acesso só de aplicação para aceder a outros recursos. O MSI só está disponível em máquinas virtuais em execução numa cloud do Azure.

Para obter mais informações sobre o MSI, veja [Como utilizar uma Identidade do Serviço Gerido de VM (MSI) do Azure para início de sessão e aquisição de token](/azure/active-directory/msi-how-to-get-access-token-using-msi).

## <a name="sign-in-to-another-cloud"></a>Iniciar sessão noutra Cloud

Os serviços cloud do Azure fornecem diferentes ambientes que cumprem os regulamentos de processamento de dados de várias regiões. Se a sua conta do Azure estiver numa cloud associada a uma destas regiões, terá de especificar o ambiente quando iniciar sessão. Por exemplo, se a sua conta está na cloud da China, inicia sessão com o seguinte comando:

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

Utilize o seguinte comando para obter uma lista de ambientes disponíveis:

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Saiba mais sobre como gerir o acesso baseado em funções do Azure

Para obter mais informações sobre a gestão de autenticação e de subscrições do Azure, veja [Gerir Contas, Subscrições e Funções Administrativas](/azure/active-directory/role-based-access-control-configure).

Cmdlets do Azure PowerShell para a gestão de funções:

* [Get-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [Get-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [New-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [Remove-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)