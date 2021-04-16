---
title: Configurer la facturation intersociétés
description: Cette rubrique fournit des informations et des exemples sur la configuration de la facturation intersociétés pour les projets.
author: sigitac
manager: tfehr
ms.date: 11/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2dec6669a41161a23f74ea962df6d8708b905315
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287550"
---
# <a name="configure-intercompany-invoicing"></a><span data-ttu-id="3be9c-103">Configurer la facturation intersociétés</span><span class="sxs-lookup"><span data-stu-id="3be9c-103">Configure intercompany invoicing</span></span>

<span data-ttu-id="3be9c-104">_**S’applique à :** Project Operations pour les scénarios selon les ressources/produits non stockés_</span><span class="sxs-lookup"><span data-stu-id="3be9c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3be9c-105">Effectuez les étapes suivantes pour configurer la facturation intersociétés pour les projets dans Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="3be9c-105">Complete the following steps to set up intercompany invoicing for projects in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="3be9c-106">Les transactions intersociétés sont des transactions de temps et de dépenses d'un contrat de projet qui appartiennent à une société ou une unité d'organisation, tandis que les ressources du contrat de projet font partie d'une société ou d'une unité d'organisation différente.</span><span class="sxs-lookup"><span data-stu-id="3be9c-106">Intercompany transactions are time and expense transactions from a project contract that belong to one company or organizational unit, while the resources on the project contract are part of a different company or organizational unit.</span></span>

## <a name="example-configure-intercompany-invoicing"></a><span data-ttu-id="3be9c-107">Exemple : Configurer la facturation intersociétés</span><span class="sxs-lookup"><span data-stu-id="3be9c-107">Example: Configure intercompany invoicing</span></span>

<span data-ttu-id="3be9c-108">Dans l'exemple suivant, Contoso Robotics USA (USPM) est l'entité juridique emprunteuse et Contoso Robotics UK (GBPM) est l'entité juridique prêteuse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-108">In the following example, Contoso Robotics USA (USPM) is the borrowing legal entity and Contoso Robotics UK (GBPM) is the lending legal entity.</span></span> 

1. <span data-ttu-id="3be9c-109">**Configurer la comptabilité intersociétés entre des entités juridiques**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-109">**Configure intercompany accounting between legal entities**.</span></span> <span data-ttu-id="3be9c-110">Chaque paire d'entités juridiques emprunteuses et prêteuses doit être configurée dans la page Comptabilité [Comptabilité intersociétés](https://docs.microsoft.com/dynamics365/finance/general-ledger/intercompany-accounting-setup).</span><span class="sxs-lookup"><span data-stu-id="3be9c-110">Each pair of borrowing and lending legal entities must be configured on the General ledger [Intercompany accounting](https://docs.microsoft.com/dynamics365/finance/general-ledger/intercompany-accounting-setup) page.</span></span>
    
    1. <span data-ttu-id="3be9c-111">Dans Dynamics 365 Finance, accédez à **Comptabilité** > **Paramétrage de la validation** > **Comptabilité intersociétés**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-111">In Dynamics 365 Finance, go to **General Ledger** > **Posting setup** > **Intercompany accounting**.</span></span> <span data-ttu-id="3be9c-112">Créez un enregistrement contenant les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3be9c-112">Create a record with the following information:</span></span>

        - <span data-ttu-id="3be9c-113">**Société d’origine** = **GBPM**</span><span class="sxs-lookup"><span data-stu-id="3be9c-113">**Originating company** = **GBPM**</span></span>
        - <span data-ttu-id="3be9c-114">**Société de destination** = **USPM**</span><span class="sxs-lookup"><span data-stu-id="3be9c-114">**Destination company** = **USPM**</span></span>

2. <span data-ttu-id="3be9c-115">**Configurez la relation commerciale entre des entités juridiques**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-115">**Configure the trading relationship between legal entities**.</span></span> <span data-ttu-id="3be9c-116">L'enregistrement client représentant l'entité juridique emprunteuse doit être créé dans l'entité juridique prêteuse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-116">The customer record representing the borrowing legal entity must be created in the lending legal entity.</span></span> <span data-ttu-id="3be9c-117">L'enregistrement fournisseur représentant l'entité juridique prêteuse doit être créé dans l'entité juridique emprunteuse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-117">The vendor record representing the lending legal entity must be created in the borrowing legal entity.</span></span>

     1. <span data-ttu-id="3be9c-118">Dans Finance, sélectionnez l'entité juridique **GBPM**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-118">In Finance, select the legal entity **GBPM**.</span></span>
     2. <span data-ttu-id="3be9c-119">Accédez à **Comptabilité client** > **Client** > **Tous les clients**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-119">Go to **Accounts receivable** > **Customer** > **All customers**.</span></span> <span data-ttu-id="3be9c-120">Créez un nouvel enregistrement pour l'entité juridiques, **USPM**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-120">Create a new record for the legal entity, **USPM**.</span></span>
     3. <span data-ttu-id="3be9c-121">Développez **Nom**, filtrez les enregistrements par **Type** et sélectionnez **Entités juridiques**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-121">Expand **Name**, filter the records by **Type** and select **Legal entities**.</span></span> 
     4. <span data-ttu-id="3be9c-122">Recherchez et sélectionnez l'enregistrement client pour **Contoso Robotics USA (USPM)**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-122">Find and select the customer record for **Contoso Robotics USA (USPM)**.</span></span>
     5. <span data-ttu-id="3be9c-123">Cliquez sur **Utiliser une correspondance**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-123">Select **Use match**.</span></span> 
     6. <span data-ttu-id="3be9c-124">Sélectionnez le groupe de clients, puis enregistrez l'enregistrement.</span><span class="sxs-lookup"><span data-stu-id="3be9c-124">Select the customer group and then save the record.</span></span>
     7. <span data-ttu-id="3be9c-125">Sélectionnez l’entité juridique **USPM**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-125">Select the legal entity **USPM**.</span></span>
     8. <span data-ttu-id="3be9c-126">Accédez à **Comptabilité fournisseur** > **Fournisseurs** > **Tous les fournisseurs**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-126">Go to **Accounts payable** > **Vendors** > **All vendors**.</span></span> <span data-ttu-id="3be9c-127">Créez un nouvel enregistrement pour l'entité juridique, **GBPM**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-127">Create a new record for the legal entity, **GBPM**.</span></span>
     9. <span data-ttu-id="3be9c-128">Développez **Nom**, filtrez les enregistrements par **Type** et sélectionnez **Entités juridiques**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-128">Expand **Name**, filter records by **Type**, and select **Legal entities**.</span></span> 
     10. <span data-ttu-id="3be9c-129">Recherchez et sélectionnez l'enregistrement client pour **Contoso Robotics UK (GBPM)**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-129">Find and select the customer record for **Contoso Robotics UK (GBPM)**.</span></span>
     11. <span data-ttu-id="3be9c-130">Sélectionnez **Utiliser une correspondance**, sélectionnez le groupe de fournisseurs, puis enregistrez l'enregistrement.</span><span class="sxs-lookup"><span data-stu-id="3be9c-130">Select **Use match**, select the vendor group, and then save the record.</span></span>
     12. <span data-ttu-id="3be9c-131">Dans l'enregistrement du fournisseur, sélectionnez **Général** > **Installer** > **Intersociétés**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-131">In the vendor record, select **General** > **Set up** > **Intercompany**.</span></span>
     13. <span data-ttu-id="3be9c-132">Sur l'onglet **Relation commerciale**, définissez **Actif** sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-132">On the **Trading relationship** tab, set **Active** to **Yes**.</span></span>
     14. <span data-ttu-id="3be9c-133">Sélectionnez la société du fournisseur **GBPM** et dans **Mon enregistrement de compte**, sélectionnez l'enregistrement client que vous avez créé plus tôt dans la procédure.</span><span class="sxs-lookup"><span data-stu-id="3be9c-133">Select the vendor company **GBPM** and in **My account record**, select the customer record that you created earlier in the procedure.</span></span>

3. <span data-ttu-id="3be9c-134">**Configurez les paramètres intersociétés dans la gestion de projet et les paramètres de comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-134">**Configure intercompany settings in Project management and accounting parameters**.</span></span> 

    1. <span data-ttu-id="3be9c-135">Sélectionnez l'entité juridique **USPM** et accédez à **Gestion et comptabilité des projets** > **Configurer** > **Paramètres de gestion et comptabilité des projets**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-135">Select the legal entity **USPM** and go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**.</span></span>
    2. <span data-ttu-id="3be9c-136">Sur l'onglet **Intersociétés**, sélectionnez la catégorie d'approvisionnement correspondant aux factures fournisseurs générées automatiquement.</span><span class="sxs-lookup"><span data-stu-id="3be9c-136">On the **Intercompany** tab, select the procurement category to match the vendor invoices that are automatically generated.</span></span>
    3. <span data-ttu-id="3be9c-137">Dans **Catégorie par défaut**, sélectionnez **Ressources intersociétés**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-137">In **Default category**, select **Intercompany resources**.</span></span>
    4. <span data-ttu-id="3be9c-138">Sélectionnez l'entité juridique **GBPM** et accédez à **Gestion et comptabilité des projets** > **Configurer** > **Paramètres de gestion et comptabilité des projets**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-138">Select the legal entity **GBPM** and go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**.</span></span>
    5. <span data-ttu-id="3be9c-139">Sur l'onglet **Intersociétés**, sélectionnez une catégorie de projet par défaut pour chaque type de transaction.</span><span class="sxs-lookup"><span data-stu-id="3be9c-139">On the **Intercompany** tab, select a default project category for each transaction type.</span></span> <span data-ttu-id="3be9c-140">Les catégories de projet sont utilisées pour la configuration fiscale lorsque la catégorie facturée dans les transactions intersociétés existe uniquement dans l’entité juridique emprunteuse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-140">Project categories are used for tax configuration when the invoiced category in intercompany transactions exists only in the borrowing legal entity.</span></span> <span data-ttu-id="3be9c-141">Vous pouvez choisir de provisionner un produit pour les transactions intersociétés.</span><span class="sxs-lookup"><span data-stu-id="3be9c-141">You can choose to accrue revenue for intercompany transactions.</span></span> <span data-ttu-id="3be9c-142">Une régularisation a lieu lorsque les transactions sont validées via le journal d’intégration de Project Operations dans l'entité juridique prêteuse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-142">Accrual happens when the transactions are posted through the Project Operations Integration journal in the lending legal entity.</span></span> <span data-ttu-id="3be9c-143">Le journal est inversé lorsque la facture intersociétés est validée.</span><span class="sxs-lookup"><span data-stu-id="3be9c-143">The journal is reversed when the intercompany invoice is posted.</span></span>
    6. <span data-ttu-id="3be9c-144">Dans le groupe **Lors du prêt de ressources**, sélectionnez **...** > **Nouveau**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-144">In the **When lending resources** group, select **...** > **New**.</span></span> 
    7. <span data-ttu-id="3be9c-145">Dans la grille, sélectionnez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3be9c-145">In the grid, select the following information:</span></span>

          - <span data-ttu-id="3be9c-146">**Entité juridique emprunteuse** = **GBPM**</span><span class="sxs-lookup"><span data-stu-id="3be9c-146">**Borrowing legal entity** = **GBPM**</span></span>
          - <span data-ttu-id="3be9c-147">**Régulariser revenus** = **Oui**</span><span class="sxs-lookup"><span data-stu-id="3be9c-147">**Accrue revenue** = **Yes**</span></span>
          - <span data-ttu-id="3be9c-148">**Catégorie de feuille de temps par défaut** = **Par défaut - Heure**</span><span class="sxs-lookup"><span data-stu-id="3be9c-148">**Default timesheet category** = **Default – Hour**</span></span>
          - <span data-ttu-id="3be9c-149">**Catégorie de dépense par défaut** = **Défaut - dépense**</span><span class="sxs-lookup"><span data-stu-id="3be9c-149">**Default expense category** = **Default – expense**</span></span>

4. <span data-ttu-id="3be9c-150">**Définissez les comptes de coûts et de revenus intersociétés dans le paramétrage de la validation dans la comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-150">**Set intercompany cost and revenue accounts in Ledger posting setup**.</span></span> <span data-ttu-id="3be9c-151">Le compte de revenus intersociétés est crédité lorsque la facture client intersociétés est validée dans l'entité juridique prêteuse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-151">The intercompany revenue account is credited when the Intercompany customer invoice is posted in the lending legal entity.</span></span> <span data-ttu-id="3be9c-152">Le compte de coûts intersociétés est débité lorsque la facture fournisseur en attente correspondante est validée dans l'entité juridique emprunteuse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-152">The intercompany cost account is debited when the  matching pending vendor invoice is posted in the borrowing legal entity.</span></span> <span data-ttu-id="3be9c-153">Ces comptes sont configurés dans les entités juridiques correspondantes.</span><span class="sxs-lookup"><span data-stu-id="3be9c-153">These accounts are set up in corresponding legal entities.</span></span> 
      
     1. <span data-ttu-id="3be9c-154">Dans Finance, sélectionnez l'entité juridique emprunteuse **USPM**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-154">In Finance, select the borrowing legal entity **USPM**.</span></span> 
     2. <span data-ttu-id="3be9c-155">Accédezr à **Gestion et comptabilité des projets** > **Configurer** > **Validation** > **Paramétrage de la validation dans la comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-155">Go to **Project management and accounting** > **Setup** > **Posting** > **Ledger posting setup**.</span></span> 
     3. <span data-ttu-id="3be9c-156">Sur l'onglet **Comptes de coûts**, dans **Type de compte général**, sélectionnez **Coût intersociétés**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-156">On the **Cost accounts** tab, in **Ledger account type**, select **Intercompany cost**.</span></span> <span data-ttu-id="3be9c-157">Créez un nouvel enregistrement contenant les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3be9c-157">Create a new record with the following information:</span></span>
      
        - <span data-ttu-id="3be9c-158">**Entité juridique prêteuse** = **GBPM**</span><span class="sxs-lookup"><span data-stu-id="3be9c-158">**Lending legal entity** = **GBPM**</span></span>
        - <span data-ttu-id="3be9c-159">**Compte principal** = Sélectionnez le compte principal pour le coût intersociétés</span><span class="sxs-lookup"><span data-stu-id="3be9c-159">**Main account** = Select the main account for intercompany cost</span></span>
        
     4. <span data-ttu-id="3be9c-160">Sélectionnez l’entité juridique prêteuse **GBPM**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-160">Select lending legal entity, **GBPM**.</span></span> 
     5. <span data-ttu-id="3be9c-161">Accédezr à **Gestion et comptabilité des projets** > **Configurer** > **Validation** > **Paramétrage de la validation dans la comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-161">Go to **Project management and accounting** > **Setup** > **Posting** > **Ledger posting setup**.</span></span> 
     6. <span data-ttu-id="3be9c-162">Sur l'onglet **Comptes de revenus**, dans **Type de compte général**, sélectionnez **Revenu intersociétés**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-162">On the **Revenue accounts** tab, in **Ledger account type**, select **Intercompany revenue**.</span></span> <span data-ttu-id="3be9c-163">Créez un nouvel enregistrement contenant les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3be9c-163">Create a new record with the following information:</span></span>

        - <span data-ttu-id="3be9c-164">**Entité juridique emprunteuse** = **USPM**</span><span class="sxs-lookup"><span data-stu-id="3be9c-164">**Borrowing legal entity** = **USPM**</span></span>
        - <span data-ttu-id="3be9c-165">**Compte principal** = Sélectionnez le compte principal pour le revenu intersociétés</span><span class="sxs-lookup"><span data-stu-id="3be9c-165">**Main account** = Select the main account for intercompany revenue</span></span> 

5. <span data-ttu-id="3be9c-166">**Configurez la tarification de transfert pour la main-d'œuvre**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-166">**Set up transfer pricing for labor**.</span></span> <span data-ttu-id="3be9c-167">La tarification de transfert intersociétés est configurée dans Project Operations sur Dataverse.</span><span class="sxs-lookup"><span data-stu-id="3be9c-167">Intercompany transfer pricing is configured in Project Operations on Dataverse.</span></span> <span data-ttu-id="3be9c-168">Configurez les [taux de coûts de la main-d’œuvre](../pricing-costing/set-up-labor-cost-rate.md#transfer-pricing-and-costs-for-resources-outside-of-your-division-or-legal-entity) et les [taux de facturation de la main-d’œuvre](../pricing-costing/set-up-labor-bill-rate.md#transfer-pricing-or-set-up-bill-rates-for-resources-from-other-organizational-units-or-divisions) pour la facturation intersociétés.</span><span class="sxs-lookup"><span data-stu-id="3be9c-168">Configure [labor cost rates](../pricing-costing/set-up-labor-cost-rate.md#transfer-pricing-and-costs-for-resources-outside-of-your-division-or-legal-entity) and [labor bill rates](../pricing-costing/set-up-labor-bill-rate.md#transfer-pricing-or-set-up-bill-rates-for-resources-from-other-organizational-units-or-divisions) for intercompany invoicing.</span></span> <span data-ttu-id="3be9c-169">La tarification de transfert n'est pas prise en charge pour les transactions de dépenses intersociétés.</span><span class="sxs-lookup"><span data-stu-id="3be9c-169">Transfer pricing isn't supported for intercompany expense transactions.</span></span> <span data-ttu-id="3be9c-170">Le prix de vente unitaire inter-organisationnel sera toujours fixé à la même valeur que le prix de revient unitaire de ressourcement.</span><span class="sxs-lookup"><span data-stu-id="3be9c-170">The inter-organization unit sale price will always be set to the same value as the resourcing unit cost price.</span></span>

      <span data-ttu-id="3be9c-171">Le coût des ressources de développeur dans Contoso Robotics UK est de 88 GBP par heure.</span><span class="sxs-lookup"><span data-stu-id="3be9c-171">The developer resource cost in Contoso Robotics UK is 88 GBP per hour.</span></span> <span data-ttu-id="3be9c-172">Contoso Robotics UK facturera Contoso Robotics USA 120 USD pour chaque heure de travail de cette ressource sur des projets américains.</span><span class="sxs-lookup"><span data-stu-id="3be9c-172">Contoso Robotics UK will bill Contoso Robotics USA 120 USD for each hour this resource worked on US projects.</span></span> <span data-ttu-id="3be9c-173">Contoso Robotics USA facturera le client Adventure Works 200 USD pour le travail effectué par la ressource développeur de Contoso Robotics UK.</span><span class="sxs-lookup"><span data-stu-id="3be9c-173">Contoso Robotics USA will bill the customer Adventure Works 200 USD for the work done by the Contoso Robotics UK developer resource.</span></span>

      1. <span data-ttu-id="3be9c-174">Dans Project Operations sur Dataverse, accédez à **Vente** > **Listes de prix**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-174">In Project Operations on Dataverse, go to **Sale** > **Price lists**.</span></span> <span data-ttu-id="3be9c-175">Créez une nouvelle liste de prix de revient appelée **Tarifs de Contoso Robotics UK.**</span><span class="sxs-lookup"><span data-stu-id="3be9c-175">Create a new cost price list called **Contoso Robotics UK cost rates.**</span></span> 
      2. <span data-ttu-id="3be9c-176">Dans la liste des prix de revient, créez un enregistrement avec les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3be9c-176">In the cost price list, create a record with the following information:</span></span>
         - <span data-ttu-id="3be9c-177">**Rôle** = **Développeur**</span><span class="sxs-lookup"><span data-stu-id="3be9c-177">**Role** = **Developer**</span></span>
         - <span data-ttu-id="3be9c-178">**Coût** = **88 GBP**</span><span class="sxs-lookup"><span data-stu-id="3be9c-178">**Cost** = **88 GBP**</span></span>
      3. <span data-ttu-id="3be9c-179">Accédez à **Paramètres** > **Unités d'organisation** et joignez cette liste de prix de revient à l'unité d’organisation **Contoso Robotics UK**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-179">Go to **Settings** > **Organizational units** and attach this cost price list to the **Contoso Robotics UK** organizational unit.</span></span>
      4. <span data-ttu-id="3be9c-180">Accédez à **Ventes** > **Listes de prix**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-180">Go to **Sales** > **Price lists**.</span></span> <span data-ttu-id="3be9c-181">Créez une liste de prix de revient appelée **Tarifs de Contoso Robotics USA**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-181">Create a cost price list called **Contoso Robotics USA cost rates**.</span></span> 
      5. <span data-ttu-id="3be9c-182">Dans la liste des prix de revient, créez un enregistrement avec les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3be9c-182">In the cost price list, create a record with the following information:</span></span>
          - <span data-ttu-id="3be9c-183">**Rôle** = **Développeur**</span><span class="sxs-lookup"><span data-stu-id="3be9c-183">**Role** = **Developer**</span></span>
          - <span data-ttu-id="3be9c-184">**Société d’allocation de ressources** = **Contoso Robotics UK**</span><span class="sxs-lookup"><span data-stu-id="3be9c-184">**Resourcing company** = **Contoso Robotics UK**</span></span>
          - <span data-ttu-id="3be9c-185">**Coût** = **120 USD**</span><span class="sxs-lookup"><span data-stu-id="3be9c-185">**Cost** = **120 USD**</span></span>
      6. <span data-ttu-id="3be9c-186">Accédez à **Paramètres** > **Unités d'organisation** et joignez cette liste de prix de revient **Tarifs de Contoso Robotics USA** à l'unité d’organisation **Contoso Robotics USA**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-186">Go to **Settings** > **Organizational units** and attach the **Contoso Robotics USA cost rates** cost price list to the **Contoso Robotics USA** organizational unit.</span></span>
      7. <span data-ttu-id="3be9c-187">Accédez à **Ventes** > **Listes de prix**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-187">Go to **Sales** > **Price lists**.</span></span> <span data-ttu-id="3be9c-188">Créez une liste de prix de vente appelée **Taux de facturation Adventure Works**.</span><span class="sxs-lookup"><span data-stu-id="3be9c-188">Create a sales price list called **Adventure Works bill rates**.</span></span> 
      8. <span data-ttu-id="3be9c-189">Dans la liste des prix de vente, créez un enregistrement avec les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3be9c-189">In the sales price list, create a record with the following information:</span></span>
          - <span data-ttu-id="3be9c-190">**Rôle** = **Développeur**</span><span class="sxs-lookup"><span data-stu-id="3be9c-190">**Role** = **Developer**</span></span>
          - <span data-ttu-id="3be9c-191">**Société d’allocation de ressources** = **Contoso Robotics UK**</span><span class="sxs-lookup"><span data-stu-id="3be9c-191">**Resourcing company** = **Contoso Robotics UK**</span></span>
          - <span data-ttu-id="3be9c-192">**Taux de facturation** = **200 USD**</span><span class="sxs-lookup"><span data-stu-id="3be9c-192">**Bill rate** = **200 USD**</span></span>
      9. <span data-ttu-id="3be9c-193">Accédez à **Ventes** > **Contrats de projet** et joignez la liste de prix **Taux de facturation Adventure Works** à la liste de prix du projet Adventure Works du contrat de projet.</span><span class="sxs-lookup"><span data-stu-id="3be9c-193">Go to **Sales** > **Project contracts** and attach the **Adventure Works bill rates** price list to the Adventure Works project price list of the project contract.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]