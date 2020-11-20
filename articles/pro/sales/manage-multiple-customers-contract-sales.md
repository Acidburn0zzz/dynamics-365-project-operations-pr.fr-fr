---
title: Gérer plusieurs clients sur des contrats de projets – Simplifié
description: Cette rubrique fournit des informations sur la gestion de plusieurs clients sur des contrats de projets.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b248dabdbd5239b140da7c99d3f38609facfe75e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181314"
---
# <a name="manage-multiple-customers-on-project-contracts---lite"></a><span data-ttu-id="6051b-103">Gérer plusieurs clients sur des contrats de projets – Simplifié</span><span class="sxs-lookup"><span data-stu-id="6051b-103">Manage multiple customers on project contracts - lite</span></span>

<span data-ttu-id="6051b-104">_**S’applique à :** Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="6051b-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6051b-105">Les contrats de projet dans Dynamics 365 Project Operations prennent en charge les scénarios dans lesquels un accord contractuel implique plusieurs clients qui financent une transaction.</span><span class="sxs-lookup"><span data-stu-id="6051b-105">Project contracts in Dynamics 365 Project Operations support the scenario where a contractual agreement involves multiple customers who are funding a deal.</span></span> <span data-ttu-id="6051b-106">L’onglet **Synthèse** de la page **Contrat du projet** comprend le champ **Client**.</span><span class="sxs-lookup"><span data-stu-id="6051b-106">The **Summary** tab on the **Project Contract** page includes the **Customer** field.</span></span> <span data-ttu-id="6051b-107">Ce champ identifie le client principal de la transaction.</span><span class="sxs-lookup"><span data-stu-id="6051b-107">This field identifies the primary customer of the deal.</span></span> <span data-ttu-id="6051b-108">D’autres clients de la transaction peuvent être définis sous l’onglet **Clients** de la page **Contrat du projet**.</span><span class="sxs-lookup"><span data-stu-id="6051b-108">Other customers for the deal can be set up on the **Customers** tab of the **Project Contract** page.</span></span>

<span data-ttu-id="6051b-109">Tous les clients du contrat répertoriés sur le contrat de projet sont créés par défaut en tant que clients de ligne de contrat sur toutes les lignes de contrat basées sur un projet créées pour le contrat du projet.</span><span class="sxs-lookup"><span data-stu-id="6051b-109">All contract customers listed on the project contract default as contract line customers on any new project-based contract lines that are created for the project contract.</span></span> <span data-ttu-id="6051b-110">Une fois leur enregistrement créé, les lignes de contrat basées un projet existantes n’héritent pas des nouveaux clients de contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-110">Existing project-based contract lines don't inherit new contract customers as new records are created.</span></span>

<span data-ttu-id="6051b-111">Les lignes de contrat basées sur les produits sont automatiquement associées au client principal.</span><span class="sxs-lookup"><span data-stu-id="6051b-111">Product-based contract lines are automatically associated to the primary customer.</span></span>

<span data-ttu-id="6051b-112">Les clients de contrat et les clients de ligne de contrat peuvent être ajoutés, mis à jour ou supprimés à tout moment avant que le contrat ne soit remporté.</span><span class="sxs-lookup"><span data-stu-id="6051b-112">Contract customers and contract line customers can be added, updated, or deleted at any time before the contract is won.</span></span>

## <a name="primary-customer"></a><span data-ttu-id="6051b-113">Client principal</span><span class="sxs-lookup"><span data-stu-id="6051b-113">Primary customer</span></span>

<span data-ttu-id="6051b-114">Le client figurant dans l’onglet **Synthèse** du contrat de projet comme client potentiel est le client principal du contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-114">The customer listed on the **Summary** tab of the project contract as the potential customer is the primary customer of the contract.</span></span> <span data-ttu-id="6051b-115">Si vous essayez de supprimer le client principal de la liste des clients du contrat, un message d’erreur indiquera qu’un enregistrement de client principal d’un contrat ne peut pas être supprimé.</span><span class="sxs-lookup"><span data-stu-id="6051b-115">When you try to delete the primary customer from the customer list on the contract, you will receive an error message that a primary customer record on a contract can't be deleted.</span></span>

<span data-ttu-id="6051b-116">Le client principal ne peut pas être mis à jour à partir de la liste des clients du contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-116">The primary customer can't be updated from the contract customers list.</span></span> <span data-ttu-id="6051b-117">En revanche, vous pouvez modifier le client potentiel sous l’onglet **Synthèse** du contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-117">Instead, change the potential customer on the **Summary** tab of the contract.</span></span> <span data-ttu-id="6051b-118">Lorsque ce champ est mis à jour sur la page **Synthèse du contrat**, le nouveau client est ajouté en tant que nouveau client du contrat, marqué de l’indicateur **Principal**.</span><span class="sxs-lookup"><span data-stu-id="6051b-118">When this field is updated on the **Contract Summary** page, the new customer is added as a new contract customer with the **Primary** flag set.</span></span> <span data-ttu-id="6051b-119">Le client principal précédent demeure client du contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-119">The previous primary customer will still be a customer on the contract.</span></span>

## <a name="create-update-or-delete-a-contract-customer-record"></a><span data-ttu-id="6051b-120">Créer, mettre à jour ou supprimer un enregistrement de client de contrat</span><span class="sxs-lookup"><span data-stu-id="6051b-120">Create, update, or delete a contract customer record</span></span>

<span data-ttu-id="6051b-121">Un client de contrat peut être créé, mis à jour ou supprimé depuis l’onglet **Clients** sur la page **Contrat du projet**.</span><span class="sxs-lookup"><span data-stu-id="6051b-121">A contract customer can be created, updated, or deleted from the **Customers** tab on the **Project Contract** page.</span></span> <span data-ttu-id="6051b-122">Les champs du tableau suivant traitent de l’enregistrement de client du contrat d’un contrat de projet et doivent être pris en considération lorsque vous travaillez avec le contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-122">The fields in the following table are on the contract customer record of a project contract and should be kept in mind as you are working with the contract.</span></span>

| <span data-ttu-id="6051b-123">Champ</span><span class="sxs-lookup"><span data-stu-id="6051b-123">Field</span></span> | <span data-ttu-id="6051b-124">Emplacement</span><span class="sxs-lookup"><span data-stu-id="6051b-124">Location</span></span> | <span data-ttu-id="6051b-125">Description</span><span class="sxs-lookup"><span data-stu-id="6051b-125">Description</span></span> | <span data-ttu-id="6051b-126">Impact en aval</span><span class="sxs-lookup"><span data-stu-id="6051b-126">Downstream impact</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="6051b-127">**Compte**</span><span class="sxs-lookup"><span data-stu-id="6051b-127">**Account**</span></span> | <span data-ttu-id="6051b-128">La grille est modifiable sous l’onglet **Clients du contrat** et les formulaires **Principal** et **Création rapide** pour le client d’un contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-128">The grid can be edited on the **Contract Customers** tab and the **Main** and **Quick Create** forms for a contract customer.</span></span> | <span data-ttu-id="6051b-129">Répertorie tous les comptes actifs.</span><span class="sxs-lookup"><span data-stu-id="6051b-129">Lists all the active accounts.</span></span> <span data-ttu-id="6051b-130">Ce champ est verrouillé après la création de l’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="6051b-130">This field is locked after the record is created.</span></span> <span data-ttu-id="6051b-131">Pour mettre à jour le compte, supprimez l’enregistrement et créez un nouvel enregistrement.</span><span class="sxs-lookup"><span data-stu-id="6051b-131">To update the account, delete the record and re-create it.</span></span> <span data-ttu-id="6051b-132">Si vous avez enregistré des chiffres réels ou si l’enregistrement de client du contrat est un client principal, vous ne pouvez pas supprimer l’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="6051b-132">If you have recorded any actuals, or if the contract customer record is a primary customer, you can't delete the record.</span></span> | <span data-ttu-id="6051b-133">Les clients de contrat sont copiés comme clients de ligne de contrat lorsqu’une ligne de contrat est créée.</span><span class="sxs-lookup"><span data-stu-id="6051b-133">Contract customers are copied over as contract line customers when a contract line is created.</span></span> |
| <span data-ttu-id="6051b-134">**Pourcentage de facturation fractionnée**</span><span class="sxs-lookup"><span data-stu-id="6051b-134">**Billing Split Percent**</span></span> | <span data-ttu-id="6051b-135">La grille est modifiable sous l’onglet **Clients du contrat** et les formulaires **Principal** et **Création rapide** pour le client d’un contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-135">The grid can be edited on the **Contract Customers** tab and the **Main** and **Quick Create** forms for a contract customer.</span></span> | <span data-ttu-id="6051b-136">Comprend le pourcentage de chaque transaction commerciale non facturée qui est attribuée à ce client de contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-136">Represents the percentage of each unbilled sales transaction that is attributed to this contract customer.</span></span> | <span data-ttu-id="6051b-137">Copié dans de nouvelles lignes de contrat et permettant de projeter les clients de ligne de contrat sur de nouvelles lignes de contrat de projet.</span><span class="sxs-lookup"><span data-stu-id="6051b-137">Copied over to new contract lines and to project contract line customers on new project contract lines.</span></span> |
| <span data-ttu-id="6051b-138">**Nom du contact de facturation**</span><span class="sxs-lookup"><span data-stu-id="6051b-138">**Bill to Contact Name**</span></span> | <span data-ttu-id="6051b-139">La grille est modifiable sous l’onglet **Clients du contrat** et les formulaires **Principal** et **Création rapide** pour le client d’un contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-139">The grid can be edited on the **Contract Customers** tab and the **Main** and **Quick Create** forms for a contract customer.</span></span> | <span data-ttu-id="6051b-140">Ce champ de texte doit être utilisé pour identifier la personne à contacter pour la facture de ce client.</span><span class="sxs-lookup"><span data-stu-id="6051b-140">This text field should be used to identify the invoice contact person for this customer.</span></span> <span data-ttu-id="6051b-141">Ce champ est créé par défaut à partir de l’enregistrement de compte associé.</span><span class="sxs-lookup"><span data-stu-id="6051b-141">This field defaults from the related account record.</span></span> | <span data-ttu-id="6051b-142">Copié dans le champ **Nom du contrat de facturation** sur la facture générée pour ce client.</span><span class="sxs-lookup"><span data-stu-id="6051b-142">Copied over to the **Bill to Contract Name** field on the invoice that is generated for this customer.</span></span> |
| <span data-ttu-id="6051b-143">**Nom de facturation**</span><span class="sxs-lookup"><span data-stu-id="6051b-143">**Bill To Name**</span></span> | <span data-ttu-id="6051b-144">La grille est modifiable sous l’onglet **Clients du contrat** et les formulaires **Principal** et **Création rapide** pour le client d’un contrat</span><span class="sxs-lookup"><span data-stu-id="6051b-144">The grid can be edited on the **Contract Customers** tab and the **Main** and **Quick Create** forms for a contract customer</span></span> | <span data-ttu-id="6051b-145">Ce champ de texte doit être utilisé pour identifier la personne à contacter pour la facture de ce client.</span><span class="sxs-lookup"><span data-stu-id="6051b-145">This text field should be used to identify the invoice contact person for this customer.</span></span> <span data-ttu-id="6051b-146">Ce champ est créé par défaut à partir de l’enregistrement de compte associé.</span><span class="sxs-lookup"><span data-stu-id="6051b-146">This field defaults from the related account record.</span></span> | <span data-ttu-id="6051b-147">Copié dans le champ **Nom du contrat de facturation** sur la facture générée pour ce client.</span><span class="sxs-lookup"><span data-stu-id="6051b-147">Copied over to the **Bill to Contract Name** field on the invoice that is generated for this customer.</span></span> |
| <span data-ttu-id="6051b-148">**Conditions de paiement**</span><span class="sxs-lookup"><span data-stu-id="6051b-148">**Payment Terms**</span></span> | <span data-ttu-id="6051b-149">La grille est modifiable sous l’onglet **Clients du contrat** et les formulaires **Principal** et **Création rapide** pour le client d’un contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-149">The grid can be edited on the **Contract Customers** tab and the **Main** and **Quick Create** forms for a contract customer.</span></span> | <span data-ttu-id="6051b-150">Les valeurs sont créées par défaut à partir de l’enregistrement de compte associé.</span><span class="sxs-lookup"><span data-stu-id="6051b-150">The values default from the related account record.</span></span> | <span data-ttu-id="6051b-151">Copié dans le champ **Nom du contrat de facturation** sur la facture générée pour ce client.</span><span class="sxs-lookup"><span data-stu-id="6051b-151">Copied over to the **Bill to Contract Name** field on the invoice that is generated for this customer.</span></span> |
| <span data-ttu-id="6051b-152">**Est arrondi**</span><span class="sxs-lookup"><span data-stu-id="6051b-152">**Is Rounding**</span></span> | <span data-ttu-id="6051b-153">La grille est modifiable sous l’onglet **Clients du contrat** et les formulaires **Principal** et **Création rapide** pour le client d’un contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-153">The grid can be edited on the **Contract Customers** tab and the **Main** and **Quick Create** forms for a contract customer.</span></span> | <span data-ttu-id="6051b-154">Indique si ce client est un client arrondi par défaut pour cette transaction.</span><span class="sxs-lookup"><span data-stu-id="6051b-154">Indicates if this customer is a default rounding customer for this deal.</span></span> <span data-ttu-id="6051b-155">Il ne peut y avoir qu’un seul client d’arrondi sur un contrat de projet.</span><span class="sxs-lookup"><span data-stu-id="6051b-155">There can only be one rounding customer on a project contract.</span></span> | <span data-ttu-id="6051b-156">Lorsque le fractionnement des coûts et des ventes non facturées entraînent une différence d’arrondi, cette différence est appliquée au chiffre réel correspondant à ce client.</span><span class="sxs-lookup"><span data-stu-id="6051b-156">When cost and unbilled sales splits on quantity lead to a rounding difference, that difference is applied to the actual that maps to this customer.</span></span> |
| <span data-ttu-id="6051b-157">**Limite à ne pas dépasser**</span><span class="sxs-lookup"><span data-stu-id="6051b-157">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="6051b-158">La grille est modifiable sous l’onglet **Clients du contrat** et les formulaires **Principal** et **Création rapide** pour le client d’un contrat</span><span class="sxs-lookup"><span data-stu-id="6051b-158">The grid can be edited on the **Contract Customers** tab and the **Main** and **Quick Create** forms for a contract customer</span></span> | <span data-ttu-id="6051b-159">Indique s’il existe une limite négociée ou un plafond du montant global qui sera facturé au client pour cet engagement.</span><span class="sxs-lookup"><span data-stu-id="6051b-159">Indicates if there is a negotiated limit or cap to the overall amount that will be invoiced to the customer for this engagement.</span></span> | <span data-ttu-id="6051b-160">La **Limite à ne pas dépasser** définie au niveau du client du contrat sera évaluée selon les **Chiffres de vente réels non facturés** qui font référence à ce client de contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-160">The **Not-to-Exceed Limit** set up at the contract customer level will be evaluated on **Unbilled Sales Actuals** that reference this contract customer.</span></span> |

## <a name="edit-billing-split-percentages"></a><span data-ttu-id="6051b-161">Modifier des pourcentages de facturation fractionnée</span><span class="sxs-lookup"><span data-stu-id="6051b-161">Edit billing split percentages</span></span>

<span data-ttu-id="6051b-162">Les pourcentages de fractionnement de la facturation peuvent être modifiés en utilisant la modification de la grille en ligne.</span><span class="sxs-lookup"><span data-stu-id="6051b-162">Billing split percentages can be edited using the in-line grid edit experience.</span></span> <span data-ttu-id="6051b-163">Si le total des pourcentages de fractionnement de la facturation n’est pas égal à 100 %, vous recevrez un message d’erreur.</span><span class="sxs-lookup"><span data-stu-id="6051b-163">When the billing split percentages do not total to 100 percent, you will receive an error.</span></span> <span data-ttu-id="6051b-164">Après avoir modifié les pourcentages de fractionnement de la facturation, actualisez la page pour annuler l’erreur.</span><span class="sxs-lookup"><span data-stu-id="6051b-164">After you edit the billing split percentages, refresh the page to dismiss the error.</span></span>

<span data-ttu-id="6051b-165">Vous pouvez également sélectionner **Répartition homogène** dans la sous-grille **Clients du contrat** pour répartir les fractionnements de la facturation de façon homogène entre tous les clients du contrat.</span><span class="sxs-lookup"><span data-stu-id="6051b-165">You can also select **Evenly Distribute** on the **Contract Customers** subgrid to allocate billing splits evenly to all contract customers.</span></span> <span data-ttu-id="6051b-166">S’il existe une valeur d’arrondi, elle sera ajoutée au client d’arrondi.</span><span class="sxs-lookup"><span data-stu-id="6051b-166">If there is a rounding factor, it will be added to the rounding customer.</span></span> <span data-ttu-id="6051b-167">Un des clients de contrat est toujours identifié comme client d’**arrondi**, ce qui signifie que l’enregistrement de ce client du contrat est marqué de l’indicateur d’arrondi défini sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="6051b-167">One of the contract customers is always tagged as the **rounding** customer, which means that the contract customer record has the rounding flag set to **Yes**.</span></span> <span data-ttu-id="6051b-168">En règle générale, il s’agit du client principal du contrat, mais cela peut également être modifié.</span><span class="sxs-lookup"><span data-stu-id="6051b-168">Typically, this is the primary customer of the contract, but it can be changed as well.</span></span>