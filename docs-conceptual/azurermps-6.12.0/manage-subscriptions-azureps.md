---
title: Gerir subscrições do Azure com o Azure PowerShell
description: Gerir subscrições do Azure com o Azure PowerShell
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: a93461af1dafbf8f2c85ef127ecaefadf3be2f52
ms.sourcegitcommit: 06f9206e025afa7207d4657c8f57c94ddb74817a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/07/2018
ms.locfileid: "51212938"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="c503b-103">Gerir várias subscrições do Azure</span><span class="sxs-lookup"><span data-stu-id="c503b-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="c503b-104">Se só agora começou a utilizar o Azure, é provável que só tenha uma subscrição individual.</span><span class="sxs-lookup"><span data-stu-id="c503b-104">If you're brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="c503b-105">Mas se já o utilizar há algum tempo, poderá ter criado várias subscrições do Azure.</span><span class="sxs-lookup"><span data-stu-id="c503b-105">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="c503b-106">Pode configurar Azure PowerShell para executar comandos numa determinada subscrição.</span><span class="sxs-lookup"><span data-stu-id="c503b-106">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="c503b-107">Obtenha uma lista de todas as subscrições da sua conta.</span><span class="sxs-lookup"><span data-stu-id="c503b-107">Get a list of all subscriptions in your account.</span></span>

    ```azurepowershell-interactive
    Get-AzureRmSubscription
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My DevTest Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

2. <span data-ttu-id="c503b-108">Defina a predefinida.</span><span class="sxs-lookup"><span data-stu-id="c503b-108">Set the default.</span></span>

    ```azurepowershell-interactive
    Select-AzureRmSubscription -Subscription "My Demos"
    ```

3. <span data-ttu-id="c503b-109">Verifique a alteração executando o cmdlet `Get-AzureRmContext`.</span><span class="sxs-lookup"><span data-stu-id="c503b-109">Verify the change by running the `Get-AzureRmContext` cmdlet.</span></span>

    ```azurepowershell-interactive
    Get-AzureRmContext
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

<span data-ttu-id="c503b-110">Depois de definir a subscrição predefinida, todos os comandos do Azure PowerShell são executados no âmbito dessa subscrição.</span><span class="sxs-lookup"><span data-stu-id="c503b-110">Once you set your default subscription, all Azure PowerShell commands run against this subscription.</span></span>