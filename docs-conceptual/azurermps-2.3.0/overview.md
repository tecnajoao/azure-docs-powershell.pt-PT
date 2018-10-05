---
title: Descrição Geral do Azure Stack do PowerShell | Microsoft Docs
description: Descrição geral do Azure Stack do PowerShell com instruções para instalação e configuração.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: d514e43d82bcb51f65831dc506e58e8747db0381
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/04/2018
ms.locfileid: "47425470"
---
# <a name="azurerm-module-230"></a><span data-ttu-id="1a231-103">Módulo AzureRM 2.3.0</span><span class="sxs-lookup"><span data-stu-id="1a231-103">AzureRM Module 2.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="1a231-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="1a231-104">Requirements:</span></span>
<span data-ttu-id="1a231-105">A versão mínima suportada do Azure Stack é a 1808.</span><span class="sxs-lookup"><span data-stu-id="1a231-105">Minimum supported Azure Stack version is 1808.</span></span>

<span data-ttu-id="1a231-106">Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.2.11</span><span class="sxs-lookup"><span data-stu-id="1a231-106">Note: If you are using an earlier version install version 1.2.11</span></span>


## <a name="install"></a><span data-ttu-id="1a231-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="1a231-107">Install</span></span>
```powershell
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module -Name AzureRM -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force -ErrorAction Continue
Uninstall-Module AzureRM.AzureStackStorage -Force -ErrorAction Continue
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force
Get-Module Azure.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

```

##<a name="release-notes"></a><span data-ttu-id="1a231-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="1a231-108">Release Notes</span></span>
* <span data-ttu-id="1a231-109">A versão 2.3.0 inclui uma lista de alterações interruptivas.</span><span class="sxs-lookup"><span data-stu-id="1a231-109">The release 2.3.0 comes with a list of breaking changes.</span></span> <span data-ttu-id="1a231-110">Para atualizar da versão 1.2.11, criámos um guia de migração em https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="1a231-110">To upgrade from the 1.2.11 version, we have created a migration guide at https://aka.ms/azspowershellmigration</span></span>
* <span data-ttu-id="1a231-111">Esta versão corresponde ao perfil de api específico azurestack 2018-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="1a231-111">This release corresponds to the azurestack specific api profile 2018-03-01-hybrid</span></span>
* <span data-ttu-id="1a231-112">Todos os módulos têm uma dependência igual ou superior no módulo AzureRm.Profile</span><span class="sxs-lookup"><span data-stu-id="1a231-112">All the modules are taking greater than or equal to dependency on the AzureRm.Profile module.</span></span>
* <span data-ttu-id="1a231-113">A versão de api suportada por cada um dos módulos foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="1a231-113">Api version suppoerted by  each of the modules are updated.</span></span> 
    * <span data-ttu-id="1a231-114">Computação - 2017-03-30</span><span class="sxs-lookup"><span data-stu-id="1a231-114">Compute - 2017-03-30</span></span>
    * <span data-ttu-id="1a231-115">Rede - 2017-10-01</span><span class="sxs-lookup"><span data-stu-id="1a231-115">Network - 2017-10-01</span></span>
    * <span data-ttu-id="1a231-116">Armazenamento - 2016-01-01</span><span class="sxs-lookup"><span data-stu-id="1a231-116">Storage - 2016-01-01</span></span>
    * <span data-ttu-id="1a231-117">Recursos - 2018-02-01</span><span class="sxs-lookup"><span data-stu-id="1a231-117">Resources - 2018-02-01</span></span>
    * <span data-ttu-id="1a231-118">Key Vault - 2016-10-01</span><span class="sxs-lookup"><span data-stu-id="1a231-118">Keyvault - 2016-10-01</span></span>
    * <span data-ttu-id="1a231-119">DNS - 2016-04-01</span><span class="sxs-lookup"><span data-stu-id="1a231-119">Dns - 2016-04-01</span></span>
* <span data-ttu-id="1a231-120">O mapa das versões de api completo para cada um dos tipos de recursos está disponível em https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span><span class="sxs-lookup"><span data-stu-id="1a231-120">The complete api version map for each of the resource types can be found at https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span></span>

## <a name="content"></a><span data-ttu-id="1a231-121">Conteúdo:</span><span class="sxs-lookup"><span data-stu-id="1a231-121">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="1a231-122">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="1a231-122">Azure Bridge</span></span>
<span data-ttu-id="1a231-123">Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.</span><span class="sxs-lookup"><span data-stu-id="1a231-123">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="1a231-124">Cópia de segurança</span><span class="sxs-lookup"><span data-stu-id="1a231-124">Backup</span></span>
<span data-ttu-id="1a231-125">Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="1a231-125">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="1a231-126">Configurar em que local as cópias de segurança são armazenadas</span><span class="sxs-lookup"><span data-stu-id="1a231-126">Configure where backups are stored</span></span>
- <span data-ttu-id="1a231-127">Fazer cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="1a231-127">Perform backups</span></span>
- <span data-ttu-id="1a231-128">Listar e restaurar cópias de segurança concluídas</span><span class="sxs-lookup"><span data-stu-id="1a231-128">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="1a231-129">Comércio</span><span class="sxs-lookup"><span data-stu-id="1a231-129">Commerce</span></span>
<span data-ttu-id="1a231-130">Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1a231-130">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="1a231-131">Computação</span><span class="sxs-lookup"><span data-stu-id="1a231-131">Compute</span></span>
<span data-ttu-id="1a231-132">Versão de pré-visualização do módulo de administrador Computação do Azure Stack, que fornece uma funcionalidade que permite gerir quotas de computação, imagens de plataformas, discos geridos e extensões de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="1a231-132">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="1a231-133">Recursos de infraestrutura</span><span class="sxs-lookup"><span data-stu-id="1a231-133">Fabric</span></span>
<span data-ttu-id="1a231-134">Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:</span><span class="sxs-lookup"><span data-stu-id="1a231-134">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="1a231-135">Parar, Iniciar e Encerrar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="1a231-135">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="1a231-136">Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU</span><span class="sxs-lookup"><span data-stu-id="1a231-136">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="1a231-137">Reparar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="1a231-137">Repair of scale unit nodes</span></span>
- <span data-ttu-id="1a231-138">Reiniciar a função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="1a231-138">Restart of Infrastructure role</span></span>
- <span data-ttu-id="1a231-139">Parar, Iniciar e Encerrar instâncias de função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="1a231-139">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="1a231-140">Criar novos Conjuntos IP</span><span class="sxs-lookup"><span data-stu-id="1a231-140">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="1a231-141">Galeria</span><span class="sxs-lookup"><span data-stu-id="1a231-141">Gallery</span></span>
<span data-ttu-id="1a231-142">Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1a231-142">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="1a231-143">Informações de Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="1a231-143">Infrastructure Insights</span></span>
<span data-ttu-id="1a231-144">Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="1a231-144">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="1a231-145">Ver o estado de funcionamento dos recursos de carimbo do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="1a231-145">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="1a231-146">Ver e gerir alertas</span><span class="sxs-lookup"><span data-stu-id="1a231-146">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="1a231-147">KeyVault</span><span class="sxs-lookup"><span data-stu-id="1a231-147">KeyVault</span></span>
<span data-ttu-id="1a231-148">Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.</span><span class="sxs-lookup"><span data-stu-id="1a231-148">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="1a231-149">Rede</span><span class="sxs-lookup"><span data-stu-id="1a231-149">Network</span></span>
<span data-ttu-id="1a231-150">Versão de pré-visualização do módulo de administrador Rede que permite:</span><span class="sxs-lookup"><span data-stu-id="1a231-150">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="1a231-151">Gerir quotas de rede</span><span class="sxs-lookup"><span data-stu-id="1a231-151">Management of network quotas</span></span>
- <span data-ttu-id="1a231-152">Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga</span><span class="sxs-lookup"><span data-stu-id="1a231-152">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="1a231-153">Fornece um cmdlet que apresenta uma descrição geral de administrador</span><span class="sxs-lookup"><span data-stu-id="1a231-153">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="1a231-154">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="1a231-154">Storage</span></span>
<span data-ttu-id="1a231-155">Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1a231-155">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="1a231-156">Nesta versão, fornecemos funcionalidade para:</span><span class="sxs-lookup"><span data-stu-id="1a231-156">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="1a231-157">Gerir quotas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="1a231-157">Manage storage quotas</span></span>
- <span data-ttu-id="1a231-158">Libertar memória de recursos de armazenamento eliminados</span><span class="sxs-lookup"><span data-stu-id="1a231-158">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="1a231-159">Restaurar contas de armazenamento eliminadas</span><span class="sxs-lookup"><span data-stu-id="1a231-159">Restore deleted storage accounts</span></span>
- <span data-ttu-id="1a231-160">Migrar contentores de uma partilha para outra</span><span class="sxs-lookup"><span data-stu-id="1a231-160">Migrate containers from one share to another</span></span>
- <span data-ttu-id="1a231-161">Ver informações sobre os componentes de armazenamento individuais</span><span class="sxs-lookup"><span data-stu-id="1a231-161">View information about the individual storage components</span></span>
- <span data-ttu-id="1a231-162">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="1a231-162">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="1a231-163">Administrador da Subscrição</span><span class="sxs-lookup"><span data-stu-id="1a231-163">Subscription Admin</span></span>
<span data-ttu-id="1a231-164">Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1a231-164">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="1a231-165">Este módulo fornece funcionalidade que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="1a231-165">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="1a231-166">Gerir planos e ofertas</span><span class="sxs-lookup"><span data-stu-id="1a231-166">Manage plans and offers</span></span>
- <span data-ttu-id="1a231-167">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="1a231-167">View usage and performance information</span></span>
- <span data-ttu-id="1a231-168">Gerir o RBAC</span><span class="sxs-lookup"><span data-stu-id="1a231-168">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="1a231-169">Subscrição</span><span class="sxs-lookup"><span data-stu-id="1a231-169">Subscription</span></span>
<span data-ttu-id="1a231-170">Versão de pré-visualização do módulo Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1a231-170">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="1a231-171">Este módulo fornece funcionalidade que permite aos Utilizadores:</span><span class="sxs-lookup"><span data-stu-id="1a231-171">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="1a231-172">Criar, Eliminar e Atualizar Subscrições</span><span class="sxs-lookup"><span data-stu-id="1a231-172">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="1a231-173">Atualizar</span><span class="sxs-lookup"><span data-stu-id="1a231-173">Update</span></span>
<span data-ttu-id="1a231-174">Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1a231-174">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="1a231-175">Neste módulo, os administradores podem:</span><span class="sxs-lookup"><span data-stu-id="1a231-175">In this module administrators can:</span></span>
- <span data-ttu-id="1a231-176">Listar e instalar atualizações disponíveis</span><span class="sxs-lookup"><span data-stu-id="1a231-176">List and install available updates</span></span>
- <span data-ttu-id="1a231-177">Retomar atualizações interrompidas</span><span class="sxs-lookup"><span data-stu-id="1a231-177">Resume interrupted updates</span></span>
- <span data-ttu-id="1a231-178">Ver atualizações instaladas</span><span class="sxs-lookup"><span data-stu-id="1a231-178">View installed updates</span></span>