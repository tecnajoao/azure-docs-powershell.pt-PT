---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: eec8b5960f787fa9ca1130b4f8b49c9d896aa99e
ms.sourcegitcommit: 5f946a535eccca0b3ddf3db8f617b32564a88938
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2018
ms.locfileid: "50001512"
---
# <a name="release-notes"></a><span data-ttu-id="5342c-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="5342c-103">Release notes</span></span>

<span data-ttu-id="5342c-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="5342c-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6110---october-2018"></a><span data-ttu-id="5342c-105">6.11.0 - outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-105">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5342c-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-106">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-107">Corrigir o problema do Get-AzureRmSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="5342c-107">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="5342c-108">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="5342c-108">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="5342c-109">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="5342c-109">AzureRM.Backup</span></span>
* <span data-ttu-id="5342c-110">Cmdlets do Azure Backup preteridos.</span><span class="sxs-lookup"><span data-stu-id="5342c-110">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-111">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-112">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais as redes aceleradas vão ser ativadas quando a utilizar o simples conjunto de parâmetros para "New-AzureRmVm"</span><span class="sxs-lookup"><span data-stu-id="5342c-112">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="5342c-113">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5342c-113">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5342c-114">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5342c-114">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5342c-115">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="5342c-115">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="5342c-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: obtém ou listas a regra de rede virtual do Azure Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5342c-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="5342c-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5342c-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="5342c-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: modifica a regra especificada de rede virtual na conta do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5342c-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="5342c-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: elimina uma regra de rede virtual do Azure Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5342c-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-120">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-121">Atualizar o cmdlet Test-AzureRmNetworkWatcherConnectivity, passar o valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="5342c-121">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="5342c-122">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5342c-122">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-123">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-123">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-124">Corrigir o problema em que Get-AzureRMRoleDefinition lança uma exceção ininteligível (quando o perfil predefinido não tem subscrição e não é especificado um âmbito) ao adicionar uma exceção significativa no cenário.</span><span class="sxs-lookup"><span data-stu-id="5342c-124">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="5342c-125">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="5342c-125">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="5342c-126">6.10.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-126">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="5342c-127">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-127">Azure.Storage</span></span>
* <span data-ttu-id="5342c-128">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="5342c-128">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="5342c-129">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="5342c-129">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="5342c-130">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="5342c-130">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="5342c-131">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5342c-131">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="5342c-132">Suporte para Get-AzureRmCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="5342c-132">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-133">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-133">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-134">Correção de Get-AzureRmVM -ResourceGroupName <rg> para devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="5342c-134">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="5342c-135">Adição de um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzureRmVmss.</span><span class="sxs-lookup"><span data-stu-id="5342c-135">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="5342c-136">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="5342c-136">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5342c-137">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5342c-137">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5342c-138">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="5342c-138">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-139">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-139">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-140">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="5342c-140">Added NetworkProfile functionality.</span></span> <span data-ttu-id="5342c-141">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="5342c-141">new cmdlets added</span></span>
    - <span data-ttu-id="5342c-142">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5342c-142">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5342c-143">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5342c-143">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5342c-144">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5342c-144">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5342c-145">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="5342c-145">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="5342c-146">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-146">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="5342c-147">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-147">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="5342c-148">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="5342c-148">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="5342c-149">Adição do cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="5342c-149">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="5342c-150">Adição do cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-150">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="5342c-151">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5342c-151">AzureRM.RedisCache</span></span>
* <span data-ttu-id="5342c-152">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="5342c-152">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="5342c-153">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="5342c-153">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-154">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-154">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-155">Adição do parâmetro -Mode em falta a Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="5342c-155">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="5342c-156">Correção do erro de commandlet Get-AzureRmProviderOperation para as operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="5342c-156">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5342c-157">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-157">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-158">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="5342c-158">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5342c-159">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-159">AzureRM.Storage</span></span>
* <span data-ttu-id="5342c-160">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="5342c-160">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="5342c-161">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="5342c-161">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5342c-162">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5342c-162">AzureRM.Websites</span></span>
* <span data-ttu-id="5342c-163">Novo Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="5342c-163">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="5342c-164">Novos Cmdlets New-AzureRMWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="5342c-164">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="5342c-165">6.9.0 - setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-165">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5342c-166">Geral</span><span class="sxs-lookup"><span data-stu-id="5342c-166">General</span></span>
* <span data-ttu-id="5342c-167">AzureRM.SignalR foi adicionado ao módulo de rollup AzureRM</span><span class="sxs-lookup"><span data-stu-id="5342c-167">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5342c-168">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-168">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-169">Alterações menores ao código comum do armazenamento</span><span class="sxs-lookup"><span data-stu-id="5342c-169">Minor changes to the storage common code</span></span>
* <span data-ttu-id="5342c-170">Ficheiros de ajuda atualizados para incluírem todos os tipos de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5342c-170">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="5342c-171">-ServicePrincipal alterado para non-mandatory no conjunto de parâmetros ServicePrincipalCertificateWithSubscriptionId</span><span class="sxs-lookup"><span data-stu-id="5342c-171">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="5342c-172">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-172">Azure.Storage</span></span>
* <span data-ttu-id="5342c-173">Suporte para a criação de Contexto de Armazenamento com OAuth.</span><span class="sxs-lookup"><span data-stu-id="5342c-173">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="5342c-174">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="5342c-174">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="5342c-175">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="5342c-175">AzureRM.Cdn</span></span>
* <span data-ttu-id="5342c-176">Standard_Microsoft adicionado ao sku de preços de Cdn.</span><span class="sxs-lookup"><span data-stu-id="5342c-176">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-177">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-177">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-178">Dependências no Cofre de Chaves e no Armazenamento movidas para as dependências comuns</span><span class="sxs-lookup"><span data-stu-id="5342c-178">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="5342c-179">Adicionado suporte para mais tamanhos de máquinas virtuais para cmdlets do AEM</span><span class="sxs-lookup"><span data-stu-id="5342c-179">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="5342c-180">Adicionado o parâmetro PublicIPPrefix a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-180">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="5342c-181">Adicionado o parâmetro ResourceId ao cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="5342c-181">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="5342c-182">Adicionado o cmdlet Invoke-AzureRmVmssVMRunCommand cmdlet</span><span class="sxs-lookup"><span data-stu-id="5342c-182">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="5342c-183">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="5342c-183">AzureRM.Dns</span></span>
* <span data-ttu-id="5342c-184">Suporte adicionado para registo de alias durante a criação de registo dns</span><span class="sxs-lookup"><span data-stu-id="5342c-184">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5342c-185">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5342c-185">AzureRM.Insights</span></span>
* <span data-ttu-id="5342c-186">Corrigidos os problemas n.º 6833 e 7102 (Área Definições de Diagnóstico)</span><span class="sxs-lookup"><span data-stu-id="5342c-186">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="5342c-187">Problemas com o nome predefinido, ou seja, “serviço”, durante a criação e listagem/obtenção das definições de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="5342c-187">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="5342c-188">Problemas ao criar definições de diagnóstico com categorias</span><span class="sxs-lookup"><span data-stu-id="5342c-188">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="5342c-189">Adicionada mensagem de preterição aos parâmetros time grains das métricas</span><span class="sxs-lookup"><span data-stu-id="5342c-189">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="5342c-190">Os parâmetros timegrains ainda são aceites (esta não é uma alteração interruptiva), mas são ignorados no back-end, uma vez que apenas PT1M é válido</span><span class="sxs-lookup"><span data-stu-id="5342c-190">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-191">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-191">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-192">Alterações aos cmdlets LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="5342c-192">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="5342c-193">LoadBalancerInboundNatPoolConfig: parâmetros IdleTimeoutInMinutes, EnableFloatingIp e EnableTcpReset adicionados</span><span class="sxs-lookup"><span data-stu-id="5342c-193">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="5342c-194">LoadBalancerInboundNatRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-194">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="5342c-195">LoadBalancerRuleConfig: parâmetro EnableTcpReset adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-195">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="5342c-196">LoadBalancerProbeConfig: suporte para o valor "Https" para o parâmetro Protocol adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-196">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="5342c-197">Adicionados comandos novos para o sub-recurso OutboundRule de LoadBalancer</span><span class="sxs-lookup"><span data-stu-id="5342c-197">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="5342c-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5342c-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5342c-200">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-200">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5342c-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="5342c-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="5342c-203">Adicionada propriedade HostedWorkloads nova para PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="5342c-203">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="5342c-204">Adicionados cmdlets novos para a funcionalidade: Azure Firewall através de ARM</span><span class="sxs-lookup"><span data-stu-id="5342c-204">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="5342c-205">Get-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-205">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="5342c-206">Set-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-206">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="5342c-207">New-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-207">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="5342c-208">Remove-AzureRmFirewall adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-208">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="5342c-209">New-AzureRmFirewallApplicationRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-209">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="5342c-210">New-AzureRmFirewallApplicationRule adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-210">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="5342c-211">New-AzureRmFirewallNatRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-211">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="5342c-212">New-AzureRmFirewallNatRule adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-212">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="5342c-213">New-AzureRmFirewallNetworkRuleCollection adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-213">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="5342c-214">New-AzureRmFirewallNetworkRule adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-214">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="5342c-215">Adicionado suporte para o certificado de raiz fidedigna e configuração de dimensionamento automático no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="5342c-215">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="5342c-216">Novos cmdlets adicionados:</span><span class="sxs-lookup"><span data-stu-id="5342c-216">New Cmdlets added:</span></span>
      - <span data-ttu-id="5342c-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5342c-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5342c-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5342c-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5342c-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="5342c-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="5342c-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="5342c-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="5342c-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="5342c-226">Cmdlets updated with optonal parameter -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-226">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="5342c-227">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5342c-227">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="5342c-228">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5342c-228">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="5342c-229">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="5342c-229">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="5342c-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="5342c-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="5342c-231">Cmdlets atualizados com parâmetro opcional -AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-231">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="5342c-232">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5342c-232">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="5342c-233">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="5342c-233">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="5342c-234">Adicionado cmdlet para Ponto Final da Interface Get-AzureInterfaceEndpoint</span><span class="sxs-lookup"><span data-stu-id="5342c-234">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="5342c-235">Adicionado suporte para vários prefixos de endereços numa sub-rede.</span><span class="sxs-lookup"><span data-stu-id="5342c-235">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="5342c-236">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="5342c-236">Updated cmdlets:</span></span>
  - <span data-ttu-id="5342c-237">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-237">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5342c-238">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-238">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5342c-239">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-239">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5342c-240">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-240">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="5342c-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="5342c-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="5342c-243">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-243">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="5342c-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="5342c-245">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-245">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="5342c-246">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-246">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="5342c-247">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-247">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="5342c-248">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-248">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="5342c-249">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-249">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="5342c-250">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-250">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="5342c-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="5342c-252">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-252">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="5342c-253">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-253">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="5342c-254">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-254">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="5342c-255">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="5342c-255">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="5342c-256">Adição de cmdlets para delegação de sub-rede</span><span class="sxs-lookup"><span data-stu-id="5342c-256">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="5342c-257">New-AzureRmDelegation: cria uma delegação nova, que pode ser adicionada a uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="5342c-257">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="5342c-258">Remove-AzureRmDelegation: recebe uma sub-rede e remove o nome da delegação especificado dessa sub-rede</span><span class="sxs-lookup"><span data-stu-id="5342c-258">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="5342c-259">Add-AzureRmDelegation: recebe uma sub-rede e adiciona o nome de serviço especificado como delegação a essa sub-rede</span><span class="sxs-lookup"><span data-stu-id="5342c-259">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="5342c-260">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="5342c-260">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="5342c-261">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="5342c-261">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="5342c-262">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="5342c-262">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="5342c-263">Suporte para discos geridos</span><span class="sxs-lookup"><span data-stu-id="5342c-263">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="5342c-264">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5342c-264">AzureRM.RedisCache</span></span>
* <span data-ttu-id="5342c-265">Dependência de informações atualizada</span><span class="sxs-lookup"><span data-stu-id="5342c-265">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-266">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-266">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-267">New-AzureRmResourceGroupDeployment atualizado com parâmetro novo RollbackAction</span><span class="sxs-lookup"><span data-stu-id="5342c-267">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="5342c-268">Adicionado suporte para OnErrorDeployment com o parâmetro novo.</span><span class="sxs-lookup"><span data-stu-id="5342c-268">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="5342c-269">Suporte para identidades geridas nas atribuições de políticas.</span><span class="sxs-lookup"><span data-stu-id="5342c-269">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="5342c-270">Os parâmetros com valores predefinidos já não são necessários ao atribuir uma política com “New-AzureRmPolicyAssignment”</span><span class="sxs-lookup"><span data-stu-id="5342c-270">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="5342c-271">Adicionado cmdlet novo Get-AzureRmPolicyAlias para obter aliases de políticas</span><span class="sxs-lookup"><span data-stu-id="5342c-271">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5342c-272">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5342c-272">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5342c-273">Problema n.º 7161 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-273">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="5342c-274">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="5342c-274">AzureRM.SignalR</span></span>
* <span data-ttu-id="5342c-275">Nomes dos SKUs atualizados para Free_F1 e Standard_S1</span><span class="sxs-lookup"><span data-stu-id="5342c-275">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="5342c-276">Adicionado campo de versão ao objeto PSSignalRResource e cadeia de ligação ao objeto PSSignalRKeys.</span><span class="sxs-lookup"><span data-stu-id="5342c-276">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5342c-277">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-277">AzureRM.Storage</span></span>
* <span data-ttu-id="5342c-278">Suporte para política Imutabilidade em AzureRm.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-278">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="5342c-279">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="5342c-279">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="5342c-280">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5342c-280">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5342c-281">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5342c-281">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5342c-282">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5342c-282">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5342c-283">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="5342c-283">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="5342c-284">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="5342c-284">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="5342c-285">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="5342c-285">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="5342c-286">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5342c-286">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="5342c-287">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5342c-287">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="5342c-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5342c-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="5342c-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="5342c-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5342c-290">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5342c-290">AzureRM.Websites</span></span>
* <span data-ttu-id="5342c-291">Adicionados dois cmdlets novos: Get-AzureRmDeletedWebApp e Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="5342c-291">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="5342c-292">O comutador New-AzureRmAppServicePlan -HyperV é adicionado para criar o plano do serviço de aplicações com contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="5342c-292">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="5342c-293">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - parâmetros novos (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) adicionados para criar e gerir a aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="5342c-293">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="5342c-294">6.8.1 - Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-294">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5342c-295">Geral</span><span class="sxs-lookup"><span data-stu-id="5342c-295">General</span></span>
* <span data-ttu-id="5342c-296">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5342c-296">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="5342c-297">Assemblagens de runtime comum atualizadas</span><span class="sxs-lookup"><span data-stu-id="5342c-297">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5342c-298">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5342c-298">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5342c-299">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5342c-299">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="5342c-300">Problema https://github.com/Azure/azure-powershell/issues/6603 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-300">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="5342c-301">Agora, os cmdlets Import-AzureRmApiManagementApi e \*-AzureRmApiManagementCertificate identificam caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="5342c-301">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="5342c-302">Problema https://github.com/Azure/azure-powershell/issues/6879 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-302">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="5342c-303">O CertificateInformation é uma propriedade definível que permite que o cmdlet Set-AzureRmApiManagement funcione corretamente.</span><span class="sxs-lookup"><span data-stu-id="5342c-303">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="5342c-304">Corrigido com a atualização para 4.0.4-nuget de pré-visualização</span><span class="sxs-lookup"><span data-stu-id="5342c-304">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="5342c-305">Problema https://github.com/Azure/azure-powershell/issues/6853 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-305">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="5342c-306">Foi corrigido o filtro de Odata para procurar por nome de produto</span><span class="sxs-lookup"><span data-stu-id="5342c-306">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="5342c-307">Problema https://github.com/Azure/azure-powershell/issues/6814 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-307">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="5342c-308">Foi corrigido o filtro de Odata para procurar por nome na API</span><span class="sxs-lookup"><span data-stu-id="5342c-308">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="5342c-309">Foi adicionado suporte para o logger de AzureMonitor</span><span class="sxs-lookup"><span data-stu-id="5342c-309">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="5342c-310">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-310">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-311">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="5342c-311">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="5342c-312">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="5342c-312">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="5342c-313">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5342c-313">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="5342c-314">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="5342c-314">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-315">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-315">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-316">Representação de saída de cmdlet predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="5342c-316">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="5342c-317">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="5342c-317">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="5342c-318">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="5342c-318">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="5342c-319">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-319">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-320">Corrigido o erro ao criar a aplicações geridas a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5342c-320">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5342c-321">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5342c-321">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5342c-322">Problemas corrigidos</span><span class="sxs-lookup"><span data-stu-id="5342c-322">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5342c-323">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5342c-323">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5342c-324">Suporte adicionado para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="5342c-324">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="5342c-325">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="5342c-325">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="5342c-326">Suporte adicionado para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="5342c-326">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="5342c-327">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="5342c-327">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="5342c-328">Suporte adicionado para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5342c-328">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="5342c-329">Suporte adicionado para intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5342c-329">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="5342c-330">Suporte adicionado para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="5342c-330">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="5342c-331">6.8.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-331">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5342c-332">Geral</span><span class="sxs-lookup"><span data-stu-id="5342c-332">General</span></span>
* <span data-ttu-id="5342c-333">Foi corrigido o problema com os grupos de recursos predefinidos não definidos.</span><span class="sxs-lookup"><span data-stu-id="5342c-333">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5342c-334">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-334">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-335">Foi adicionada a propriedade de expiração aos tokens devolvidos durante o Connect-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="5342c-335">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-336">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-336">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-337">Foi corrigido o problema em que o destino está em falta no resultado da saída.</span><span class="sxs-lookup"><span data-stu-id="5342c-337">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="5342c-338">Foi corrigido o problema com o tipo de conta de armazenamento para a VM com disco gerido</span><span class="sxs-lookup"><span data-stu-id="5342c-338">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="5342c-339">Corrigir os cmdlets do AEM Extension para outros ambientes, por exemplo o Azure China</span><span class="sxs-lookup"><span data-stu-id="5342c-339">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="5342c-340">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="5342c-340">AzureRM.IotHub</span></span>
* <span data-ttu-id="5342c-341">Corrigir exemplos para New-AzureRmIotHubExportDevices e New-AzureRmIotHubImportDevices</span><span class="sxs-lookup"><span data-stu-id="5342c-341">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-342">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-342">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-343">Representação de modelos predefinidos alterada para a vista de tabela</span><span class="sxs-lookup"><span data-stu-id="5342c-343">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="5342c-344">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="5342c-344">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="5342c-345">Corrigida a falha em Update-AzureRmPowerBIEmbeddedCapacity ao tentar dimensionar a capacidade em pausa</span><span class="sxs-lookup"><span data-stu-id="5342c-345">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-346">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-346">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-347">Corrigido o erro ao criar a aplicação gerida a partir do Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5342c-347">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5342c-348">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5342c-348">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5342c-349">Correção para problemas</span><span class="sxs-lookup"><span data-stu-id="5342c-349">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5342c-350">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5342c-350">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5342c-351">Suporte para o método de encaminhamento de MultiValue</span><span class="sxs-lookup"><span data-stu-id="5342c-351">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="5342c-352">Novo parâmetro "MaxReturn" para encaminhamento MultiValue</span><span class="sxs-lookup"><span data-stu-id="5342c-352">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="5342c-353">Suporte para o método de encaminhamento de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="5342c-353">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="5342c-354">Suporte para intervalos de endereços IP (sub-redes) em pontos finais</span><span class="sxs-lookup"><span data-stu-id="5342c-354">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="5342c-355">Suporte para Cabeçalhos Personalizados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5342c-355">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="5342c-356">Suporte para Intervalos de código esperados nos perfis</span><span class="sxs-lookup"><span data-stu-id="5342c-356">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="5342c-357">Suporte para Cabeçalhos Personalizados nos pontos finais</span><span class="sxs-lookup"><span data-stu-id="5342c-357">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5342c-358">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5342c-358">AzureRM.Websites</span></span>
* <span data-ttu-id="5342c-359">Foi corrigido o problema com os grupos de recursos predefinidos incorretamente.</span><span class="sxs-lookup"><span data-stu-id="5342c-359">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="5342c-360">6.7.0 - Agosto 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-360">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5342c-361">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-361">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-362">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-362">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5342c-363">Adicionado ID de utilizador ao nome de contexto predefinido para evitar conflito de contextos</span><span class="sxs-lookup"><span data-stu-id="5342c-363">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="5342c-364">Corrigidos os problemas com Clear-AzureRmContext que causavam problemas com a seleção de um contexto #6398</span><span class="sxs-lookup"><span data-stu-id="5342c-364">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="5342c-365">Permissão para o domínio de inquilino passar para o parâmetro "-TenantId" para "Connect-AzureRmAccount"</span><span class="sxs-lookup"><span data-stu-id="5342c-365">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="5342c-366">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-366">Azure.Storage</span></span>
* <span data-ttu-id="5342c-367">Remoção da limitação de 5 TB da quota da Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="5342c-367">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="5342c-368">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="5342c-368">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5342c-369">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5342c-369">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5342c-370">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-370">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="5342c-371">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5342c-371">Azure.AnalysisServices</span></span>
* <span data-ttu-id="5342c-372">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-372">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5342c-373">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5342c-373">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5342c-374">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-374">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="5342c-375">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="5342c-375">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="5342c-376">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-376">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="5342c-377">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="5342c-377">AzureRM.Automation</span></span>
* <span data-ttu-id="5342c-378">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-378">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="5342c-379">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="5342c-379">AzureRM.Backup</span></span>
* <span data-ttu-id="5342c-380">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-380">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="5342c-381">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="5342c-381">AzureRM.Batch</span></span>
* <span data-ttu-id="5342c-382">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-382">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="5342c-383">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="5342c-383">AzureRM.Billing</span></span>
* <span data-ttu-id="5342c-384">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-384">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="5342c-385">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="5342c-385">AzureRM.Cdn</span></span>
* <span data-ttu-id="5342c-386">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-386">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="5342c-387">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="5342c-387">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="5342c-388">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-389">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-389">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-390">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-390">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5342c-391">Adicionado o parâmetro EvictionPolicy a New-AzureRmVmssConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-391">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="5342c-392">Utilização da localização predefinida em DiskFileParameterSet de New-AzureRmVm se não for especificada nenhuma Localização.</span><span class="sxs-lookup"><span data-stu-id="5342c-392">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="5342c-393">Correção da descrição do parâmetro em Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="5342c-393">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="5342c-394">Correção do cmdlet Get-AzureRmVMDiskEncryptionStatus para determinados cenários relacionados com passagem única</span><span class="sxs-lookup"><span data-stu-id="5342c-394">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="5342c-395">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="5342c-395">AzureRM.Consumption</span></span>
* <span data-ttu-id="5342c-396">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="5342c-397">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="5342c-397">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="5342c-398">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="5342c-399">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="5342c-399">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="5342c-400">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="5342c-401">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="5342c-401">AzureRM.DataFactories</span></span>
* <span data-ttu-id="5342c-402">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5342c-403">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5342c-403">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5342c-404">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="5342c-405">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="5342c-405">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="5342c-406">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5342c-407">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5342c-407">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5342c-408">Correção da depuração quando DebugPreference é definida a partir da linha de comando do powershell</span><span class="sxs-lookup"><span data-stu-id="5342c-408">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="5342c-409">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="5342c-409">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="5342c-410">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5342c-411">Exemplo atualizado para Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5342c-411">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="5342c-412">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="5342c-412">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="5342c-413">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-413">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="5342c-414">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="5342c-414">AzureRM.Dns</span></span>
* <span data-ttu-id="5342c-415">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-415">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="5342c-416">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5342c-416">AzureRM.EventGrid</span></span>
* <span data-ttu-id="5342c-417">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-417">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5342c-418">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5342c-418">AzureRM.EventHub</span></span>
* <span data-ttu-id="5342c-419">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-419">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="5342c-420">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="5342c-420">AzureRM.HDInsight</span></span>
* <span data-ttu-id="5342c-421">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-421">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5342c-422">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5342c-422">AzureRM.Insights</span></span>
* <span data-ttu-id="5342c-423">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="5342c-424">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="5342c-424">AzureRM.IotHub</span></span>
* <span data-ttu-id="5342c-425">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5342c-426">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5342c-426">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5342c-427">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="5342c-428">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5342c-428">AzureRM.LogicApp</span></span>
* <span data-ttu-id="5342c-429">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="5342c-430">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="5342c-430">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="5342c-431">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="5342c-432">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="5342c-432">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="5342c-433">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="5342c-434">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="5342c-434">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="5342c-435">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="5342c-436">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="5342c-436">AzureRM.Media</span></span>
* <span data-ttu-id="5342c-437">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-438">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-438">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-439">Exemplo adicionado para Set-AzureRmLocalNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="5342c-439">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="5342c-440">Exemplos e descrições atualizados para Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey e New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="5342c-440">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="5342c-441">Exemplos adicionados para Remove-AzureRmVirtualNetworkGatewayIpConfig e Reset-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="5342c-441">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="5342c-442">Exemplo adicionado para Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="5342c-442">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="5342c-443">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span><span class="sxs-lookup"><span data-stu-id="5342c-443">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="5342c-444">Exemplo adicionado para Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="5342c-444">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="5342c-445">Cmdlets gerados novamente para ApplicationSecurityGroup, RouteTable e Usage com o gerador de códigos mais recente</span><span class="sxs-lookup"><span data-stu-id="5342c-445">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="5342c-446">Esclarecida a mensagem de erro para Get-AzureRmVirtualNetworkSubnetConfig ao tentar obter uma sub-rede que não existe</span><span class="sxs-lookup"><span data-stu-id="5342c-446">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="5342c-447">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="5342c-447">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="5342c-448">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="5342c-449">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5342c-449">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="5342c-450">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="5342c-451">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5342c-451">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="5342c-452">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="5342c-453">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="5342c-453">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="5342c-454">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="5342c-455">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="5342c-455">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="5342c-456">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-456">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5342c-457">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5342c-457">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5342c-458">Adicionado filtro de política ao cmdlet Get-AzureRmRecoveryServicesBackItem.</span><span class="sxs-lookup"><span data-stu-id="5342c-458">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="5342c-459">O comando devolve a lista de itens de cópia de segurança protegidos pelo ID de política especificado.</span><span class="sxs-lookup"><span data-stu-id="5342c-459">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="5342c-460">Atualizado Microsoft.Azure.Management.RecoveryServices.Backup para a versão 3.0.0-preview.</span><span class="sxs-lookup"><span data-stu-id="5342c-460">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="5342c-461">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-461">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="5342c-462">Adicionado o parâmetro TargetResourceGroupName a Restore-AzureRmRecoveryServicesBackupItem.</span><span class="sxs-lookup"><span data-stu-id="5342c-462">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="5342c-463">O grupo de recursos para o qual os discos geridos são restaurados.</span><span class="sxs-lookup"><span data-stu-id="5342c-463">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="5342c-464">Aplicável à cópia de segurança de VM com discos geridos.</span><span class="sxs-lookup"><span data-stu-id="5342c-464">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="5342c-465">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="5342c-465">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="5342c-466">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="5342c-467">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="5342c-467">AzureRM.RedisCache</span></span>
* <span data-ttu-id="5342c-468">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="5342c-469">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="5342c-469">AzureRM.Relay</span></span>
* <span data-ttu-id="5342c-470">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-471">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-471">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-472">Suporte para a implementação do modelo no âmbito da subscrição.</span><span class="sxs-lookup"><span data-stu-id="5342c-472">Support template deployment at subscription scope.</span></span> <span data-ttu-id="5342c-473">Adicionados novos Cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5342c-473">Add new Cmdlets:</span></span>
    - <span data-ttu-id="5342c-474">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5342c-474">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="5342c-475">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5342c-475">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="5342c-476">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5342c-476">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="5342c-477">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5342c-477">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="5342c-478">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="5342c-478">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="5342c-479">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="5342c-479">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="5342c-480">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="5342c-480">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="5342c-481">Corrigido o problema em que é apresentado um erro ao passar um contexto para Set-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="5342c-481">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="5342c-482">Corrigido o exemplo em New-AzureRmResourceGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="5342c-482">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="5342c-483">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="5342c-484">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="5342c-484">AzureRM.Scheduler</span></span>
* <span data-ttu-id="5342c-485">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5342c-486">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5342c-486">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5342c-487">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-487">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5342c-488">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5342c-488">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5342c-489">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-489">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5342c-490">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-490">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-491">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-491">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5342c-492">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-492">AzureRM.Storage</span></span>
* <span data-ttu-id="5342c-493">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-493">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="5342c-494">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="5342c-494">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="5342c-495">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-495">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="5342c-496">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="5342c-496">AzureRM.Tags</span></span>
* <span data-ttu-id="5342c-497">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-497">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5342c-498">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5342c-498">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5342c-499">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-499">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="5342c-500">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="5342c-500">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="5342c-501">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-501">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5342c-502">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5342c-502">AzureRM.Websites</span></span>
* <span data-ttu-id="5342c-503">Atualizado para a versão mais recente do Azure ClientRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-503">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="5342c-504">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-504">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5342c-505">Geral</span><span class="sxs-lookup"><span data-stu-id="5342c-505">General</span></span>
* <span data-ttu-id="5342c-506">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="5342c-506">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5342c-507">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-507">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-508">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="5342c-508">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="5342c-509">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-509">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5342c-510">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-510">Azure.Storage</span></span>
* <span data-ttu-id="5342c-511">Adicionado suporte para obter o Contexto de Armazenamento de DefaultProfile</span><span class="sxs-lookup"><span data-stu-id="5342c-511">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="5342c-512">Adicionado Ps1XmlAttribute a propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="5342c-512">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5342c-513">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5342c-513">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5342c-514">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-514">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="5342c-515">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="5342c-515">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="5342c-516">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-516">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="5342c-517">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="5342c-517">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="5342c-518">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="5342c-518">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="5342c-519">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="5342c-519">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-520">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-520">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-521">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="5342c-521">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="5342c-522">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="5342c-522">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="5342c-523">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="5342c-523">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="5342c-524">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="5342c-524">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="5342c-525">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="5342c-525">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="5342c-526">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="5342c-526">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="5342c-527">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="5342c-527">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="5342c-528">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="5342c-528">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="5342c-529">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="5342c-529">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="5342c-530">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="5342c-530">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5342c-531">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5342c-531">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5342c-532">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="5342c-532">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="5342c-533">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="5342c-533">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="5342c-534">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-534">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="5342c-535">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="5342c-535">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5342c-536">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5342c-536">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5342c-537">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="5342c-537">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5342c-538">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5342c-538">AzureRM.EventHub</span></span>
* <span data-ttu-id="5342c-539">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="5342c-539">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="5342c-540">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="5342c-540">AzureRM.Insights</span></span>
* <span data-ttu-id="5342c-541">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="5342c-541">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="5342c-542">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="5342c-542">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5342c-543">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5342c-543">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5342c-544">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5342c-544">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-545">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-545">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-546">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="5342c-546">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-547">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-547">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-548">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="5342c-548">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="5342c-549">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="5342c-549">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5342c-550">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5342c-550">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5342c-551">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="5342c-551">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="5342c-552">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="5342c-552">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="5342c-553">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-553">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-554">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5342c-554">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="5342c-555">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5342c-555">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="5342c-556">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5342c-556">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="5342c-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="5342c-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="5342c-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="5342c-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="5342c-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="5342c-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="5342c-560">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="5342c-560">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="5342c-561">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="5342c-561">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="5342c-562">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-562">AzureRM.Storage</span></span>
* <span data-ttu-id="5342c-563">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="5342c-563">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="5342c-564">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="5342c-564">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="5342c-565">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5342c-565">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="5342c-566">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5342c-566">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="5342c-567">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="5342c-567">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="5342c-568">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="5342c-568">AzureRM.Tags</span></span>
* <span data-ttu-id="5342c-569">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="5342c-569">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="5342c-570">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-570">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5342c-571">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-571">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-572">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="5342c-572">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5342c-573">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-573">Azure.Storage</span></span>
* <span data-ttu-id="5342c-574">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="5342c-574">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="5342c-575">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="5342c-575">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="5342c-576">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="5342c-576">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5342c-577">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5342c-577">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5342c-578">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="5342c-578">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="5342c-579">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="5342c-579">AzureRM.Automation</span></span>
* <span data-ttu-id="5342c-580">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="5342c-580">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-581">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-581">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-582">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="5342c-582">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="5342c-583">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="5342c-583">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="5342c-584">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="5342c-584">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="5342c-585">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="5342c-585">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="5342c-586">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="5342c-586">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5342c-587">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5342c-587">AzureRM.EventHub</span></span>
* <span data-ttu-id="5342c-588">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="5342c-588">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5342c-589">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5342c-589">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5342c-590">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="5342c-590">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="5342c-591">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="5342c-591">AzureRM.LogicApp</span></span>
* <span data-ttu-id="5342c-592">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="5342c-592">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-593">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-594">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="5342c-594">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="5342c-595">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="5342c-595">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="5342c-596">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="5342c-596">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="5342c-597">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="5342c-597">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="5342c-598">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="5342c-598">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="5342c-599">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="5342c-599">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="5342c-600">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="5342c-600">AzureRM.Relay</span></span>
* <span data-ttu-id="5342c-601">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="5342c-601">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-602">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-602">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-603">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="5342c-603">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="5342c-604">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="5342c-604">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="5342c-605">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5342c-605">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="5342c-606">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="5342c-606">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="5342c-607">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="5342c-607">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="5342c-608">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5342c-608">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5342c-609">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="5342c-609">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="5342c-610">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="5342c-610">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="5342c-611">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5342c-611">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5342c-612">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5342c-612">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5342c-613">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5342c-613">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5342c-614">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5342c-614">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="5342c-615">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="5342c-615">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="5342c-616">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="5342c-616">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5342c-617">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5342c-617">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5342c-618">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="5342c-618">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5342c-619">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-619">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-620">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="5342c-620">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="5342c-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="5342c-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5342c-623">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5342c-623">AzureRM.Websites</span></span>
* <span data-ttu-id="5342c-624">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="5342c-624">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="5342c-625">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="5342c-625">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="5342c-626">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="5342c-626">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="5342c-627">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-627">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="5342c-628">Geral</span><span class="sxs-lookup"><span data-stu-id="5342c-628">General</span></span>
* <span data-ttu-id="5342c-629">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="5342c-629">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="5342c-630">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-630">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-631">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="5342c-631">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-632">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-632">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-633">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="5342c-633">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="5342c-634">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="5342c-634">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="5342c-635">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-635">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="5342c-636">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="5342c-636">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="5342c-637">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5342c-637">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="5342c-638">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="5342c-638">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="5342c-639">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5342c-639">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="5342c-640">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="5342c-640">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="5342c-641">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="5342c-641">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="5342c-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5342c-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="5342c-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5342c-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="5342c-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5342c-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5342c-645">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5342c-645">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5342c-646">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="5342c-646">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="5342c-647">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="5342c-647">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="5342c-648">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="5342c-648">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="5342c-649">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="5342c-649">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="5342c-650">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="5342c-650">AzureRM.EventHub</span></span>
* <span data-ttu-id="5342c-651">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="5342c-651">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="5342c-652">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="5342c-652">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="5342c-653">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="5342c-653">Provided Default Parameter set.</span></span>
* <span data-ttu-id="5342c-654">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="5342c-654">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5342c-655">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5342c-655">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5342c-656">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="5342c-656">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-657">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-657">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-658">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="5342c-658">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="5342c-659">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="5342c-659">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="5342c-660">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="5342c-660">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="5342c-661">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="5342c-661">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="5342c-662">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="5342c-662">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5342c-663">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="5342c-663">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5342c-664">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="5342c-664">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="5342c-665">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="5342c-665">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="5342c-666">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="5342c-666">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="5342c-667">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="5342c-667">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5342c-668">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5342c-668">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5342c-669">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="5342c-669">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="5342c-670">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="5342c-670">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="5342c-671">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="5342c-671">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-672">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-672">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-673">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="5342c-673">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="5342c-674">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5342c-674">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="5342c-675">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5342c-675">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="5342c-676">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="5342c-676">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="5342c-677">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="5342c-677">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="5342c-678">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5342c-678">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="5342c-679">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="5342c-679">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="5342c-680">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="5342c-680">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="5342c-681">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="5342c-681">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="5342c-682">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="5342c-682">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="5342c-683">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="5342c-683">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="5342c-684">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="5342c-684">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="5342c-685">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="5342c-685">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="5342c-686">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5342c-686">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="5342c-687">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="5342c-687">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5342c-688">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-688">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-689">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="5342c-689">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="5342c-690">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="5342c-690">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="5342c-691">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-691">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5342c-692">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-692">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-693">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="5342c-693">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="5342c-694">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="5342c-694">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="5342c-695">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="5342c-695">Azure.Storage</span></span>
* <span data-ttu-id="5342c-696">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="5342c-696">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-697">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-697">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-698">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="5342c-698">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="5342c-699">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="5342c-699">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="5342c-700">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="5342c-700">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="5342c-701">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="5342c-701">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="5342c-702">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="5342c-702">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="5342c-703">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="5342c-703">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="5342c-704">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5342c-704">Start-AzureRmVM</span></span>
    - <span data-ttu-id="5342c-705">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5342c-705">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="5342c-706">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5342c-706">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="5342c-707">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="5342c-707">Set-AzureRmVM</span></span>
    - <span data-ttu-id="5342c-708">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="5342c-708">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="5342c-709">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5342c-709">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="5342c-710">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="5342c-710">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="5342c-711">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="5342c-711">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="5342c-712">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5342c-712">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="5342c-713">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5342c-713">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="5342c-714">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5342c-714">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="5342c-715">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="5342c-715">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="5342c-716">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="5342c-716">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="5342c-717">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="5342c-717">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="5342c-718">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="5342c-718">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="5342c-719">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="5342c-719">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="5342c-720">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="5342c-720">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="5342c-721">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="5342c-721">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="5342c-722">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="5342c-722">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="5342c-723">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="5342c-723">AzureRM.EventGrid</span></span>
* <span data-ttu-id="5342c-724">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="5342c-724">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="5342c-725">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5342c-725">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5342c-726">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="5342c-726">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="5342c-727">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="5342c-727">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="5342c-728">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="5342c-728">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="5342c-729">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="5342c-729">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="5342c-730">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="5342c-730">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="5342c-731">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="5342c-731">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="5342c-732">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="5342c-732">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="5342c-733">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="5342c-733">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5342c-734">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-734">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-735">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="5342c-735">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5342c-736">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5342c-736">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5342c-737">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-737">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5342c-738">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5342c-738">AzureRM.Websites</span></span>
* <span data-ttu-id="5342c-739">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="5342c-739">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="5342c-740">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="5342c-740">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="5342c-741">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-741">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="5342c-742">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="5342c-742">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="5342c-743">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="5342c-743">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="5342c-744">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-744">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5342c-745">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-745">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-746">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="5342c-746">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="5342c-747">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="5342c-747">AzureRM.Compute</span></span>
* <span data-ttu-id="5342c-748">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="5342c-748">VMSS VM Update feature</span></span>
    - <span data-ttu-id="5342c-749">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="5342c-749">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="5342c-750">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="5342c-750">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="5342c-751">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="5342c-751">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="5342c-752">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="5342c-752">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="5342c-753">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="5342c-753">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="5342c-754">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="5342c-754">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="5342c-755">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="5342c-755">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="5342c-756">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="5342c-756">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="5342c-757">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="5342c-757">AzureRM.KeyVault</span></span>
* <span data-ttu-id="5342c-758">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="5342c-758">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="5342c-759">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-759">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-760">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="5342c-760">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="5342c-761">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="5342c-761">AzureRM.Resources</span></span>
* <span data-ttu-id="5342c-762">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="5342c-762">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="5342c-763">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="5342c-763">AzureRM.Scheduler</span></span>
* <span data-ttu-id="5342c-764">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="5342c-764">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="5342c-765">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-765">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-766">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="5342c-766">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="5342c-767">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5342c-767">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="5342c-768">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="5342c-768">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="5342c-769">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="5342c-769">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="5342c-770">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="5342c-770">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="5342c-771">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5342c-771">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="5342c-772">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="5342c-772">AzureRM.Websites</span></span>
* <span data-ttu-id="5342c-773">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="5342c-773">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="5342c-774">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="5342c-774">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="5342c-775">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="5342c-775">AzureRM.Profile</span></span>
* <span data-ttu-id="5342c-776">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="5342c-776">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="5342c-777">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="5342c-777">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="5342c-778">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="5342c-778">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="5342c-779">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="5342c-779">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="5342c-780">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="5342c-780">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="5342c-781">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5342c-781">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="5342c-782">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="5342c-782">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="5342c-783">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="5342c-783">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="5342c-784">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="5342c-784">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="5342c-785">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="5342c-785">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="5342c-786">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="5342c-786">Added support for MSI identity</span></span>
* <span data-ttu-id="5342c-787">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="5342c-787">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="5342c-788">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="5342c-788">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="5342c-789">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-789">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="5342c-790">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="5342c-790">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="5342c-791">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="5342c-791">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="5342c-792">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="5342c-792">AzureRM.Batch</span></span>
* <span data-ttu-id="5342c-793">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="5342c-793">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="5342c-794">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="5342c-794">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="5342c-795">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="5342c-795">AzureRM.Consumption</span></span>
* <span data-ttu-id="5342c-796">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="5342c-796">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="5342c-797">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="5342c-797">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="5342c-798">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="5342c-798">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="5342c-799">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5342c-799">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="5342c-800">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="5342c-800">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="5342c-801">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="5342c-801">AzureRM.Network</span></span>
* <span data-ttu-id="5342c-802">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="5342c-802">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="5342c-803">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="5342c-803">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="5342c-804">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="5342c-804">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="5342c-805">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5342c-805">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="5342c-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="5342c-807">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5342c-807">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="5342c-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="5342c-809">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="5342c-809">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="5342c-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="5342c-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="5342c-811">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="5342c-811">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="5342c-812">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="5342c-812">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="5342c-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="5342c-813">AzureRM.Sql</span></span>
* <span data-ttu-id="5342c-814">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="5342c-814">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="5342c-815">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="5342c-815">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="5342c-816">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="5342c-816">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="5342c-817">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="5342c-817">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="5342c-818">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="5342c-818">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="5342c-819">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5342c-819">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="5342c-820">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="5342c-820">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="5342c-821">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="5342c-821">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="5342c-822">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="5342c-822">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="5342c-823">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="5342c-823">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="5342c-824">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="5342c-824">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="5342c-825">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="5342c-825">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>