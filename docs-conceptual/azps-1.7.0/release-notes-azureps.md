---
ms.openlocfilehash: 54d7a9da878e085e90479fb229876c9be6dafd74
ms.sourcegitcommit: 89066b7c4b527357bb2024e1ad708df84c131804
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/09/2019
ms.locfileid: "59364139"
---
## <a name="170---april-2019"></a><span data-ttu-id="a9f6b-101">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-101">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a9f6b-102">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a9f6b-102">Highlights since the last major release</span></span>
* <span data-ttu-id="a9f6b-103">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a9f6b-103">General availability of `Az` module</span></span>
* <span data-ttu-id="a9f6b-104">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a9f6b-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a9f6b-105">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a9f6b-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a9f6b-106">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a9f6b-107">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a9f6b-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a9f6b-108">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a9f6b-109">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a9f6b-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="a9f6b-110">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-110">Az.Accounts</span></span>
* <span data-ttu-id="a9f6b-111">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="a9f6b-111">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a9f6b-112">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-112">Az.AnalysisServices</span></span>
* <span data-ttu-id="a9f6b-113">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="a9f6b-113">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="a9f6b-114">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="a9f6b-114">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a9f6b-115">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-115">Az.Automation</span></span>
* <span data-ttu-id="a9f6b-116">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-116">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="a9f6b-117">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-117">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="a9f6b-118">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="a9f6b-118">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-119">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-120">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="a9f6b-120">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="a9f6b-121">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-121">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="a9f6b-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a9f6b-122">Az.ContainerInstance</span></span>
* <span data-ttu-id="a9f6b-123">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="a9f6b-123">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a9f6b-124">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a9f6b-124">Az.DataFactory</span></span>
* <span data-ttu-id="a9f6b-125">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="a9f6b-125">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="a9f6b-126">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-126">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-127">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-127">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-128">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-128">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="a9f6b-129">Melhor processamento de erros de "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-129">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="a9f6b-130">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="a9f6b-130">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="a9f6b-131">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a9f6b-131">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="a9f6b-132">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="a9f6b-132">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="a9f6b-133">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="a9f6b-133">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-134">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-134">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-135">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-135">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a9f6b-136">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-136">Az.Storage</span></span>
* <span data-ttu-id="a9f6b-137">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="a9f6b-137">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="a9f6b-138">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a9f6b-138">New-AzStorageContext</span></span>
* <span data-ttu-id="a9f6b-139">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="a9f6b-139">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="a9f6b-140">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a9f6b-140">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a9f6b-141">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="a9f6b-141">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="a9f6b-142">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-142">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="a9f6b-143">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-143">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="a9f6b-144">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="a9f6b-144">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="a9f6b-145">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a9f6b-145">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a9f6b-146">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a9f6b-146">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="a9f6b-147">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a9f6b-147">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="a9f6b-148">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a9f6b-148">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="a9f6b-149">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-149">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="a9f6b-150">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="a9f6b-150">Highlights since the last major release</span></span>
* <span data-ttu-id="a9f6b-151">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="a9f6b-151">General availability of `Az` module</span></span>
* <span data-ttu-id="a9f6b-152">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="a9f6b-152">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="a9f6b-153">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="a9f6b-153">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="a9f6b-154">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-154">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="a9f6b-155">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a9f6b-155">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a9f6b-156">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-156">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="a9f6b-157">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="a9f6b-157">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a9f6b-158">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-158">Az.Automation</span></span>
* <span data-ttu-id="a9f6b-159">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="a9f6b-159">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="a9f6b-160">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="a9f6b-160">Dynamic grouping</span></span>
    * <span data-ttu-id="a9f6b-161">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="a9f6b-161">Pre-Post script</span></span>
    * <span data-ttu-id="a9f6b-162">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="a9f6b-162">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-163">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-163">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-164">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="a9f6b-164">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="a9f6b-165">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-165">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a9f6b-166">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a9f6b-166">Az.KeyVault</span></span>
* <span data-ttu-id="a9f6b-167">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="a9f6b-167">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a9f6b-168">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-168">Az.Network</span></span>
* <span data-ttu-id="a9f6b-169">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="a9f6b-169">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="a9f6b-170">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a9f6b-170">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a9f6b-171">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-171">Az.RecoveryServices</span></span>
* <span data-ttu-id="a9f6b-172">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="a9f6b-172">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="a9f6b-173">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="a9f6b-173">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-174">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-174">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-175">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="a9f6b-175">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="a9f6b-176">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="a9f6b-176">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-177">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-177">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-178">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-178">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a9f6b-179">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-179">Az.Storage</span></span>
* <span data-ttu-id="a9f6b-180">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a9f6b-180">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="a9f6b-181">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-181">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a9f6b-182">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-182">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a9f6b-183">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-183">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="a9f6b-184">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="a9f6b-184">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="a9f6b-185">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="a9f6b-185">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="a9f6b-186">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="a9f6b-186">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a9f6b-187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a9f6b-187">Az.Websites</span></span>
* <span data-ttu-id="a9f6b-188">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-188">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="a9f6b-189">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-189">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a9f6b-190">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-190">Az.Accounts</span></span>
* <span data-ttu-id="a9f6b-191">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="a9f6b-191">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="a9f6b-192">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="a9f6b-192">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a9f6b-193">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-193">Az.Automation</span></span>
* <span data-ttu-id="a9f6b-194">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="a9f6b-194">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="a9f6b-195">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-195">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="a9f6b-196">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="a9f6b-196">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a9f6b-197">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a9f6b-197">Az.Cdn</span></span>
* <span data-ttu-id="a9f6b-198">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-198">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-199">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-200">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="a9f6b-200">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a9f6b-201">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a9f6b-201">Az.DataFactory</span></span>
* <span data-ttu-id="a9f6b-202">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="a9f6b-202">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a9f6b-203">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a9f6b-203">Az.LogicApp</span></span>
* <span data-ttu-id="a9f6b-204">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="a9f6b-204">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a9f6b-205">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-205">Az.Network</span></span>
* <span data-ttu-id="a9f6b-206">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-206">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a9f6b-207">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-207">Az.RecoveryServices</span></span>
* <span data-ttu-id="a9f6b-208">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="a9f6b-208">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="a9f6b-209">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="a9f6b-209">SDK Update</span></span>
* <span data-ttu-id="a9f6b-210">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a9f6b-210">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="a9f6b-211">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a9f6b-211">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-212">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-212">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-213">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="a9f6b-213">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="a9f6b-214">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="a9f6b-214">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="a9f6b-215">Correção do problema de encaminhamento do resultado de `Get-AzResource` para</span><span class="sxs-lookup"><span data-stu-id="a9f6b-215">Fix issue when piping the result of `Get-AzResource` to</span></span> `Set-AzResource`
    - <span data-ttu-id="a9f6b-216">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="a9f6b-216">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="a9f6b-217">Correção do problema na alteração do tipo de dados JSON ao executar</span><span class="sxs-lookup"><span data-stu-id="a9f6b-217">Fix issue with JSON data type change when running</span></span> `Set-AzResource`
    - <span data-ttu-id="a9f6b-218">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="a9f6b-218">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-219">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-219">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-220">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-220">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="a9f6b-221">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-221">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a9f6b-222">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-222">Az.Storage</span></span>
* <span data-ttu-id="a9f6b-223">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a9f6b-223">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="a9f6b-224">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-224">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="a9f6b-225">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-225">Az.AnalysisServices</span></span>
* <span data-ttu-id="a9f6b-226">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="a9f6b-226">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a9f6b-227">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-227">Az.Automation</span></span>
* <span data-ttu-id="a9f6b-228">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-228">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="a9f6b-229">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-229">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="a9f6b-230">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-230">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a9f6b-231">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-231">Az.CognitiveServices</span></span>
* <span data-ttu-id="a9f6b-232">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-232">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-233">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-233">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-234">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="a9f6b-234">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="a9f6b-235">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="a9f6b-235">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="a9f6b-236">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-236">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="a9f6b-237">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-237">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a9f6b-238">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a9f6b-238">Az.DataLakeStore</span></span>
* <span data-ttu-id="a9f6b-239">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="a9f6b-239">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a9f6b-240">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a9f6b-240">Az.EventHub</span></span>
* <span data-ttu-id="a9f6b-241">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="a9f6b-241">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="a9f6b-242">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a9f6b-242">Az.KeyVault</span></span>
* <span data-ttu-id="a9f6b-243">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a9f6b-243">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a9f6b-244">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a9f6b-244">Az.LogicApp</span></span>
* <span data-ttu-id="a9f6b-245">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a9f6b-245">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="a9f6b-246">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-246">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="a9f6b-247">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a9f6b-247">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="a9f6b-248">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a9f6b-248">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a9f6b-249">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a9f6b-249">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a9f6b-250">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a9f6b-250">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a9f6b-251">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a9f6b-251">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="a9f6b-252">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="a9f6b-252">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="a9f6b-253">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-253">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a9f6b-254">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-254">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a9f6b-255">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-255">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a9f6b-256">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-256">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="a9f6b-257">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a9f6b-257">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a9f6b-258">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a9f6b-258">Az.Monitor</span></span>
* <span data-ttu-id="a9f6b-259">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="a9f6b-259">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a9f6b-260">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-260">Az.Network</span></span>
* <span data-ttu-id="a9f6b-261">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="a9f6b-261">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a9f6b-262">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a9f6b-262">Az.OperationalInsights</span></span>
* <span data-ttu-id="a9f6b-263">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-263">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="a9f6b-264">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-264">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="a9f6b-265">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-265">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="a9f6b-266">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-266">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-267">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a9f6b-267">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a9f6b-268">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a9f6b-268">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="a9f6b-269">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="a9f6b-269">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="a9f6b-270">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="a9f6b-270">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-271">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-271">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-272">Suporte adicionado para a camada Hiperescala da BD SQL</span><span class="sxs-lookup"><span data-stu-id="a9f6b-272">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="a9f6b-273">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="a9f6b-273">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a9f6b-274">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a9f6b-274">Az.Websites</span></span>
* <span data-ttu-id="a9f6b-275">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="a9f6b-275">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="a9f6b-276">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-276">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a9f6b-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-277">Az.Accounts</span></span>
* <span data-ttu-id="a9f6b-278">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a9f6b-278">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a9f6b-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-279">Az.AnalysisServices</span></span>
<span data-ttu-id="a9f6b-280">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-280">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-281">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-282">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="a9f6b-282">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="a9f6b-283">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="a9f6b-283">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="a9f6b-284">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-284">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a9f6b-285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-285">Az.RecoveryServices</span></span>
<span data-ttu-id="a9f6b-286">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-286">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-287">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-287">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-288">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="a9f6b-288">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="a9f6b-289">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a9f6b-289">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a9f6b-290">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="a9f6b-290">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="a9f6b-291">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a9f6b-291">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-292">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-292">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-293">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-293">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="a9f6b-294">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="a9f6b-294">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="a9f6b-295">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="a9f6b-295">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="a9f6b-296">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-296">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a9f6b-297">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-297">Az.Accounts</span></span>
* <span data-ttu-id="a9f6b-298">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="a9f6b-298">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a9f6b-299">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-299">Az.AnalysisServices</span></span>
* <span data-ttu-id="a9f6b-300">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a9f6b-300">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a9f6b-301">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-301">Az.RecoveryServices</span></span>
* <span data-ttu-id="a9f6b-302">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="a9f6b-302">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="a9f6b-303">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-303">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a9f6b-304">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-304">Az.Accounts</span></span>
* <span data-ttu-id="a9f6b-305">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="a9f6b-305">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a9f6b-306">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-306">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a9f6b-307">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="a9f6b-307">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="a9f6b-308">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a9f6b-308">Az.Aks</span></span>
* <span data-ttu-id="a9f6b-309">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-309">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a9f6b-310">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-310">Az.Automation</span></span>
* <span data-ttu-id="a9f6b-311">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="a9f6b-311">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="a9f6b-312">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-312">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a9f6b-313">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a9f6b-313">Az.Cdn</span></span>
* <span data-ttu-id="a9f6b-314">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-314">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-315">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-316">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-316">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="a9f6b-317">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="a9f6b-317">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="a9f6b-318">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="a9f6b-318">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a9f6b-319">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a9f6b-319">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a9f6b-320">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-320">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a9f6b-321">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a9f6b-321">Az.DataFactory</span></span>
* <span data-ttu-id="a9f6b-322">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="a9f6b-322">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a9f6b-323">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a9f6b-323">Az.DataLakeStore</span></span>
* <span data-ttu-id="a9f6b-324">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="a9f6b-324">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="a9f6b-325">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="a9f6b-325">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="a9f6b-326">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-326">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a9f6b-327">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a9f6b-327">Az.IotHub</span></span>
* <span data-ttu-id="a9f6b-328">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-328">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a9f6b-329">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a9f6b-329">Az.KeyVault</span></span>
* <span data-ttu-id="a9f6b-330">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-330">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a9f6b-331">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-331">Az.Network</span></span>
* <span data-ttu-id="a9f6b-332">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-332">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-333">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-333">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-334">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-334">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="a9f6b-335">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-335">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="a9f6b-336">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="a9f6b-336">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="a9f6b-337">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="a9f6b-337">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="a9f6b-338">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="a9f6b-338">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="a9f6b-339">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-339">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="a9f6b-340">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="a9f6b-340">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a9f6b-341">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a9f6b-341">Az.ServiceFabric</span></span>
* <span data-ttu-id="a9f6b-342">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="a9f6b-342">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="a9f6b-343">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-343">Fix some error messages.</span></span>
* <span data-ttu-id="a9f6b-344">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-344">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="a9f6b-345">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-345">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a9f6b-346">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a9f6b-346">Az.SignalR</span></span>
* <span data-ttu-id="a9f6b-347">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-347">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-348">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-348">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-349">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-349">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a9f6b-350">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="a9f6b-350">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="a9f6b-351">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="a9f6b-351">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="a9f6b-352">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="a9f6b-352">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a9f6b-353">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-353">Az.Storage</span></span>
* <span data-ttu-id="a9f6b-354">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-354">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a9f6b-355">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-355">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="a9f6b-356">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="a9f6b-356">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="a9f6b-357">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="a9f6b-357">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="a9f6b-358">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a9f6b-358">Az.TrafficManager</span></span>
* <span data-ttu-id="a9f6b-359">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-359">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a9f6b-360">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a9f6b-360">Az.Websites</span></span>
* <span data-ttu-id="a9f6b-361">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-361">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a9f6b-362">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-362">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="a9f6b-363">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="a9f6b-363">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="a9f6b-364">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a9f6b-364">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a9f6b-365">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-365">Az.Accounts</span></span>
* <span data-ttu-id="a9f6b-366">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="a9f6b-366">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-367">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-367">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-368">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-368">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="a9f6b-369">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="a9f6b-369">Updated the description of ID in help files</span></span>
* <span data-ttu-id="a9f6b-370">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-370">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a9f6b-371">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a9f6b-371">Az.DataLakeStore</span></span>
* <span data-ttu-id="a9f6b-372">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-372">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="a9f6b-373">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="a9f6b-373">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a9f6b-374">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a9f6b-374">Az.EventGrid</span></span>
* <span data-ttu-id="a9f6b-375">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-375">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="a9f6b-376">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="a9f6b-376">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="a9f6b-377">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a9f6b-377">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a9f6b-378">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a9f6b-378">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a9f6b-379">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a9f6b-379">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a9f6b-380">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-380">Dead letter endpoint.</span></span>
    - <span data-ttu-id="a9f6b-381">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="a9f6b-381">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a9f6b-382">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="a9f6b-382">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a9f6b-383">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="a9f6b-383">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a9f6b-384">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-384">Dead letter endpoint.</span></span>
* <span data-ttu-id="a9f6b-385">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-385">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="a9f6b-386">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-386">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a9f6b-387">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a9f6b-387">Az.IotHub</span></span>
* <span data-ttu-id="a9f6b-388">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="a9f6b-388">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a9f6b-389">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a9f6b-389">Az.LogicApp</span></span>
* <span data-ttu-id="a9f6b-390">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="a9f6b-390">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-391">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-391">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-392">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-392">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="a9f6b-393">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="a9f6b-393">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="a9f6b-394">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a9f6b-394">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a9f6b-395">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="a9f6b-395">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="a9f6b-396">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-396">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="a9f6b-397">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="a9f6b-397">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a9f6b-398">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a9f6b-398">Az.SignalR</span></span>
* <span data-ttu-id="a9f6b-399">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-399">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-400">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-400">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-401">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-401">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a9f6b-402">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-402">Az.Storage</span></span>
* <span data-ttu-id="a9f6b-403">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="a9f6b-403">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="a9f6b-404">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a9f6b-404">New-AzStorageContext</span></span>
* <span data-ttu-id="a9f6b-405">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="a9f6b-405">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="a9f6b-406">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="a9f6b-406">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a9f6b-407">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a9f6b-407">Az.Websites</span></span>
* <span data-ttu-id="a9f6b-408">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-408">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="a9f6b-409">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-409">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="a9f6b-410">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a9f6b-410">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="a9f6b-411">Geral</span><span class="sxs-lookup"><span data-stu-id="a9f6b-411">General</span></span>

- <span data-ttu-id="a9f6b-412">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="a9f6b-412">General Availability of Az Module</span></span>
- <span data-ttu-id="a9f6b-413">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="a9f6b-413">Online help for each module</span></span>
- <span data-ttu-id="a9f6b-414">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="a9f6b-414">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="a9f6b-415">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="a9f6b-415">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="a9f6b-416">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-416">Az.Accounts</span></span>
- <span data-ttu-id="a9f6b-417">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-417">Changed from Az.Profile</span></span>
- <span data-ttu-id="a9f6b-418">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="a9f6b-418">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a9f6b-419">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a9f6b-419">Az.ApiManagement</span></span>
- <span data-ttu-id="a9f6b-420">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="a9f6b-420">Fixes for #7002</span></span>
- <span data-ttu-id="a9f6b-421">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-421">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="a9f6b-422">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a9f6b-422">Az.Batch</span></span>
- <span data-ttu-id="a9f6b-423">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-423">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="a9f6b-424">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-424">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="a9f6b-425">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-425">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="a9f6b-426">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="a9f6b-426">Az.Billing</span></span>
- <span data-ttu-id="a9f6b-427">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-427">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="a9f6b-428">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-428">Az.CognitivServices</span></span>
- <span data-ttu-id="a9f6b-429">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="a9f6b-429">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="a9f6b-430">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="a9f6b-430">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a9f6b-431">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a9f6b-431">Az.ContainerInstance</span></span>
- <span data-ttu-id="a9f6b-432">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="a9f6b-432">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="a9f6b-433">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a9f6b-433">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="a9f6b-434">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-434">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a9f6b-435">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a9f6b-435">Az.DataLakeStore</span></span>
- <span data-ttu-id="a9f6b-436">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-436">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="a9f6b-437">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a9f6b-437">Az.Monitor</span></span>
- <span data-ttu-id="a9f6b-438">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-438">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="a9f6b-439">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a9f6b-439">Az.KeyVault</span></span>
- <span data-ttu-id="a9f6b-440">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="a9f6b-440">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="a9f6b-441">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a9f6b-441">Az.MachineLearning</span></span>
- <span data-ttu-id="a9f6b-442">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-442">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="a9f6b-443">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a9f6b-443">Az.Media</span></span>
- <span data-ttu-id="a9f6b-444">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="a9f6b-444">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a9f6b-445">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-445">Az.Network</span></span>
<span data-ttu-id="a9f6b-446">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="a9f6b-446">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="a9f6b-447">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="a9f6b-447">New cmdlets added:</span></span>
        - <span data-ttu-id="a9f6b-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a9f6b-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a9f6b-450">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-450">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a9f6b-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a9f6b-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a9f6b-453">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="a9f6b-453">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="a9f6b-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="a9f6b-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9f6b-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="a9f6b-456">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-456">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="a9f6b-457">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a9f6b-457">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="a9f6b-458">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a9f6b-458">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a9f6b-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a9f6b-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a9f6b-460">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a9f6b-460">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="a9f6b-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="a9f6b-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="a9f6b-462">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-462">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="a9f6b-463">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="a9f6b-463">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="a9f6b-464">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a9f6b-464">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a9f6b-465">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a9f6b-465">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a9f6b-466">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a9f6b-466">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="a9f6b-467">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="a9f6b-467">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="a9f6b-468">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-468">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="a9f6b-469">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a9f6b-469">Az.OperationalInsights</span></span>
- <span data-ttu-id="a9f6b-470">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-470">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="a9f6b-471">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-471">Az.Profile</span></span>
- <span data-ttu-id="a9f6b-472">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a9f6b-472">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a9f6b-473">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-473">Az.RecoveryServices</span></span>
- <span data-ttu-id="a9f6b-474">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-474">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="a9f6b-475">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-475">Az.Resources</span></span>
- <span data-ttu-id="a9f6b-476">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-476">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a9f6b-477">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a9f6b-477">Az.ServiceFabric</span></span>
- <span data-ttu-id="a9f6b-478">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="a9f6b-478">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="a9f6b-479">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-479">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="a9f6b-480">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="a9f6b-480">Az.SIgnalR</span></span>
- <span data-ttu-id="a9f6b-481">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="a9f6b-481">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="a9f6b-482">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-482">Az.Sql</span></span>
- <span data-ttu-id="a9f6b-483">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="a9f6b-483">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="a9f6b-484">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="a9f6b-484">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="a9f6b-485">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-485">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="a9f6b-486">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-486">Az.Storage</span></span>
- <span data-ttu-id="a9f6b-487">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-487">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a9f6b-488">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a9f6b-488">Az.Websites</span></span>
- <span data-ttu-id="a9f6b-489">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="a9f6b-489">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="a9f6b-490">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a9f6b-490">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="a9f6b-491">Geral</span><span class="sxs-lookup"><span data-stu-id="a9f6b-491">General</span></span>

* <span data-ttu-id="a9f6b-492">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a9f6b-492">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="a9f6b-493">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-493">Az.Compute</span></span>

* <span data-ttu-id="a9f6b-494">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-494">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a9f6b-495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a9f6b-495">Az.DataLakeStore</span></span>

* <span data-ttu-id="a9f6b-496">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="a9f6b-496">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="a9f6b-497">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a9f6b-497">Az.FrontDoor</span></span>

* <span data-ttu-id="a9f6b-498">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="a9f6b-498">Fixed some broken links</span></span>
    - <span data-ttu-id="a9f6b-499">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-499">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="a9f6b-500">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-500">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a9f6b-501">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-501">Az.RecoveryServices</span></span>

* <span data-ttu-id="a9f6b-502">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-502">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="a9f6b-503">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-503">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="a9f6b-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-504">Az.Resources</span></span>

* <span data-ttu-id="a9f6b-505">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="a9f6b-505">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="a9f6b-506">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-506">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="a9f6b-507">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-507">Az.Sql</span></span>

* <span data-ttu-id="a9f6b-508">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="a9f6b-508">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="a9f6b-509">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="a9f6b-509">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="a9f6b-510">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-510">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="a9f6b-511">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-511">Az.Storage</span></span>

* <span data-ttu-id="a9f6b-512">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a9f6b-512">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="a9f6b-513">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="a9f6b-513">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="a9f6b-514">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-514">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a9f6b-515">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="a9f6b-515">Support Static Website configuration</span></span>
    - <span data-ttu-id="a9f6b-516">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a9f6b-516">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="a9f6b-517">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a9f6b-517">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a9f6b-518">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a9f6b-518">Az.Websites</span></span>

* <span data-ttu-id="a9f6b-519">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="a9f6b-519">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="a9f6b-520">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-520">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="a9f6b-521">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-521">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="a9f6b-522">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a9f6b-522">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a9f6b-523">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a9f6b-523">Az.ApiManagement</span></span>
* <span data-ttu-id="a9f6b-524">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-524">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="a9f6b-525">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a9f6b-525">Az.Automation</span></span>
* <span data-ttu-id="a9f6b-526">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="a9f6b-526">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="a9f6b-527">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="a9f6b-527">Added Update Management cmdlets</span></span>
* <span data-ttu-id="a9f6b-528">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="a9f6b-528">Added Source Control cmdlets</span></span>
* <span data-ttu-id="a9f6b-529">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="a9f6b-529">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="a9f6b-530">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="a9f6b-530">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="a9f6b-531">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-531">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-532">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="a9f6b-532">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="a9f6b-533">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-533">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a9f6b-534">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a9f6b-534">Az.ContainerInstance</span></span>
* <span data-ttu-id="a9f6b-535">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-535">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="a9f6b-536">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a9f6b-536">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="a9f6b-537">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="a9f6b-537">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a9f6b-538">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-538">Az.Network</span></span>
* <span data-ttu-id="a9f6b-539">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="a9f6b-539">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="a9f6b-540">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="a9f6b-540">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="a9f6b-541">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-541">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="a9f6b-542">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="a9f6b-542">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="a9f6b-543">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a9f6b-543">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a9f6b-544">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-544">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="a9f6b-545">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-545">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="a9f6b-546">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="a9f6b-546">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="a9f6b-547">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="a9f6b-547">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="a9f6b-548">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="a9f6b-548">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="a9f6b-549">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a9f6b-549">Az.Relay</span></span>
* <span data-ttu-id="a9f6b-550">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-550">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="a9f6b-551">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-551">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-552">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e</span><span class="sxs-lookup"><span data-stu-id="a9f6b-552">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and</span></span> `Set-AzureRmPolicyAssignment`
* <span data-ttu-id="a9f6b-553">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="a9f6b-553">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="a9f6b-554">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="a9f6b-554">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a9f6b-555">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a9f6b-555">Az.ServiceFabric</span></span>
* <span data-ttu-id="a9f6b-556">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="a9f6b-556">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="a9f6b-557">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-557">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-558">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="a9f6b-558">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="a9f6b-559">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a9f6b-559">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a9f6b-560">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a9f6b-560">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a9f6b-561">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a9f6b-561">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a9f6b-562">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a9f6b-562">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a9f6b-563">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a9f6b-563">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a9f6b-564">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a9f6b-564">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a9f6b-565">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a9f6b-565">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a9f6b-566">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a9f6b-566">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="a9f6b-567">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-567">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="a9f6b-568">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-568">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="a9f6b-569">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-569">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="a9f6b-570">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-570">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a9f6b-571">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-571">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a9f6b-572">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-572">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="a9f6b-573">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-573">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="a9f6b-574">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="a9f6b-574">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="a9f6b-575">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a9f6b-575">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a9f6b-576">Geral</span><span class="sxs-lookup"><span data-stu-id="a9f6b-576">General</span></span>
* <span data-ttu-id="a9f6b-577">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="a9f6b-577">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="a9f6b-578">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-578">Az.Profile</span></span>
* <span data-ttu-id="a9f6b-579">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a9f6b-579">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="a9f6b-580">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="a9f6b-580">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="a9f6b-581">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="a9f6b-581">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="a9f6b-582">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="a9f6b-582">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="a9f6b-583">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="a9f6b-583">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="a9f6b-584">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="a9f6b-584">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="a9f6b-585">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="a9f6b-585">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="a9f6b-586">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-586">Az.CognitiveServices</span></span>
* <span data-ttu-id="a9f6b-587">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-587">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-588">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-588">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-589">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="a9f6b-589">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="a9f6b-590">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="a9f6b-590">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="a9f6b-591">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-591">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a9f6b-592">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a9f6b-592">Az.DataLakeStore</span></span>
* <span data-ttu-id="a9f6b-593">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-593">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="a9f6b-594">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-594">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="a9f6b-595">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="a9f6b-595">Az.Insights</span></span>
* <span data-ttu-id="a9f6b-596">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="a9f6b-596">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="a9f6b-597">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="a9f6b-597">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="a9f6b-598">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="a9f6b-598">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="a9f6b-599">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="a9f6b-599">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a9f6b-600">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-600">Az.Network</span></span>
* <span data-ttu-id="a9f6b-601">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="a9f6b-601">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="a9f6b-602">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="a9f6b-602">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="a9f6b-603">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="a9f6b-603">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="a9f6b-604">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a9f6b-604">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="a9f6b-605">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="a9f6b-605">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="a9f6b-606">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="a9f6b-606">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="a9f6b-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a9f6b-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a9f6b-608">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a9f6b-608">Az.PolicyInsights</span></span>
* <span data-ttu-id="a9f6b-609">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="a9f6b-609">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-610">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-610">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-611">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="a9f6b-611">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="a9f6b-612">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-612">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a9f6b-613">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a9f6b-613">Az.ServiceBus</span></span>
* <span data-ttu-id="a9f6b-614">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-614">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a9f6b-615">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a9f6b-615">Az.ServiceFabric</span></span>
* <span data-ttu-id="a9f6b-616">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-616">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="a9f6b-617">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-617">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="a9f6b-618">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="a9f6b-618">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="a9f6b-619">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="a9f6b-619">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="a9f6b-620">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-620">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="a9f6b-621">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a9f6b-621">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="a9f6b-622">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-622">Az.Profile</span></span>
* <span data-ttu-id="a9f6b-623">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="a9f6b-623">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="a9f6b-624">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="a9f6b-624">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-625">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-625">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-626">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="a9f6b-626">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="a9f6b-627">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-627">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a9f6b-628">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a9f6b-628">Az.DataLakeStore</span></span>
* <span data-ttu-id="a9f6b-629">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="a9f6b-629">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="a9f6b-630">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-630">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="a9f6b-631">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-631">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a9f6b-632">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-632">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a9f6b-633">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-633">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a9f6b-634">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-634">Az.Network</span></span>
* <span data-ttu-id="a9f6b-635">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-635">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="a9f6b-636">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-636">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-637">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-637">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-638">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-638">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="a9f6b-639">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="a9f6b-639">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="a9f6b-640">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a9f6b-640">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="a9f6b-641">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-641">Azure.Storage</span></span>
* <span data-ttu-id="a9f6b-642">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="a9f6b-642">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="a9f6b-643">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-643">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="a9f6b-644">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a9f6b-644">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a9f6b-645">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-645">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="a9f6b-646">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="a9f6b-646">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="a9f6b-647">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a9f6b-647">Az.CognitiveServices</span></span>
* <span data-ttu-id="a9f6b-648">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-648">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a9f6b-649">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a9f6b-649">Az.Compute</span></span>
* <span data-ttu-id="a9f6b-650">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="a9f6b-650">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="a9f6b-651">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-651">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="a9f6b-652">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="a9f6b-652">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="a9f6b-653">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a9f6b-653">Az.DataFactoryV2</span></span>
* <span data-ttu-id="a9f6b-654">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-654">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a9f6b-655">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a9f6b-655">Az.Network</span></span>
* <span data-ttu-id="a9f6b-656">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-656">Added NetworkProfile functionality.</span></span> <span data-ttu-id="a9f6b-657">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="a9f6b-657">new cmdlets added</span></span>
    - <span data-ttu-id="a9f6b-658">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-658">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="a9f6b-659">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-659">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="a9f6b-660">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-660">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="a9f6b-661">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a9f6b-661">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="a9f6b-662">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="a9f6b-662">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="a9f6b-663">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="a9f6b-663">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="a9f6b-664">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="a9f6b-664">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="a9f6b-665">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="a9f6b-665">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="a9f6b-666">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="a9f6b-666">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a9f6b-667">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a9f6b-667">Az.RedisCache</span></span>
* <span data-ttu-id="a9f6b-668">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="a9f6b-668">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="a9f6b-669">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="a9f6b-669">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="a9f6b-670">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a9f6b-670">Az.Resources</span></span>
* <span data-ttu-id="a9f6b-671">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="a9f6b-671">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a9f6b-672">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="a9f6b-672">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="a9f6b-673">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a9f6b-673">Az.Sql</span></span>
* <span data-ttu-id="a9f6b-674">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="a9f6b-674">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a9f6b-675">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a9f6b-675">Az.Websites</span></span>
* <span data-ttu-id="a9f6b-676">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="a9f6b-676">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="a9f6b-677">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="a9f6b-677">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="a9f6b-678">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a9f6b-678">0.2.0 - September 2018</span></span>
 <span data-ttu-id="a9f6b-679">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="a9f6b-679">Initial Release</span></span>