---
title: Gérer plusieurs clients sur les lignes de devis selon les projets
description: Cette rubrique fournit des informations sur la manière de gérer plusieurs clients sur des lignes de devis basées sur des projets.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ffb89a954b8af9d726c64cceeafca638c3393130
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965775"
---
# <a name="manage-multiple-customers-on-project-based-quote-lines"></a><span data-ttu-id="7c729-103">Gérer plusieurs clients sur les lignes de devis selon les projets</span><span class="sxs-lookup"><span data-stu-id="7c729-103">Manage multiple customers on project-based quote lines</span></span>

<span data-ttu-id="7c729-104">Les lignes de devis basées sur des projets prennent en charge des scénarios où chaque ligne de devis a une liste de clients qui paient pour cela.</span><span class="sxs-lookup"><span data-stu-id="7c729-104">Project-based quote lines support scenarios where each quote line has a list of customers that are paying for it.</span></span> <span data-ttu-id="7c729-105">Cette liste de clients sur la ligne de devis basée sur le projet peut être la même que la liste de clients sur le devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-105">This list of customers on the project-based quote line can be same as the list of customers on the quote.</span></span> <span data-ttu-id="7c729-106">Vous pouvez également modifier la liste des clients pour qu’elle soit différente.</span><span class="sxs-lookup"><span data-stu-id="7c729-106">You can also change the list of customers to be different.</span></span> <span data-ttu-id="7c729-107">Pour créer le contrat de projet potentiel lorsqu’un devis de projet est remporté, la liste des clients de la ligne de devis basée sur le projet est copiée dans la ligne de contrat basée sur le projet correspondante.</span><span class="sxs-lookup"><span data-stu-id="7c729-107">To create the eventual project contract when a project quote is won, the customer list on project-based quote line is copied to the corresponding project–based contract line.</span></span> <span data-ttu-id="7c729-108">Les clients du devis basé sur le projet sont copiés dans le contrat de projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-108">Customers on the project-based quote are copied to the project contract.</span></span>

<span data-ttu-id="7c729-109">Lorsque vous facturez l’éventuel contrat de projet, la liste de clients de la ligne de contrat de projet est prioritaire sur la liste du contrat de projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-109">When you invoice the eventual project contract, the customer list on the project-based contract line takes priority over the list on the project contract.</span></span> <span data-ttu-id="7c729-110">La liste des clients du contrat de projet n’est utilisée que pour les valeurs par défaut sur les nouvelles lignes de contrat de projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-110">The customer list on the project contract is only used to default new project contract lines.</span></span>

<span data-ttu-id="7c729-111">Tous les clients du devis sur l’onglet **Clients** du devis de projet par défaut en tant que clients de la ligne de devis sur toutes les nouvelles lignes de devis selon le projet créées pour le devis de projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-111">All quote customers on the **Customers** tab of the project quote default as quote line customers on any new project-based quote lines created for the project quote.</span></span> <span data-ttu-id="7c729-112">Les lignes de devis existantes selon un projet n’héritent pas des enregistrements client de devis créés après elles.</span><span class="sxs-lookup"><span data-stu-id="7c729-112">Any existing project-based quote lines don't inherit new quote customer records created after them.</span></span>

## <a name="create-update-or-delete-a-quote-line-customer-record"></a><span data-ttu-id="7c729-113">Créer, mettre à jour ou supprimer un enregistrement client de ligne de devis</span><span class="sxs-lookup"><span data-stu-id="7c729-113">Create, update, or delete a quote line customer record</span></span>

<span data-ttu-id="7c729-114">Vous pouvez créer, mettre à jour ou supprimer un client de ligne de devis sur l’onglet **Clients de la ligne de devis** sur la page **Ligne de devis basée sur le projet**.</span><span class="sxs-lookup"><span data-stu-id="7c729-114">You can create, update, or delete a quote line customer on the **Quote line customers** tab on the **Project-based quote line** page.</span></span> <span data-ttu-id="7c729-115">Lorsque vous ajoutez un nouveau client sur la ligne de devis basée sur le projet, le client est également ajouté au devis global en tant que client du devis, avec un pourcentage de répartition de facturation par défaut sur le devis global de 0 %.</span><span class="sxs-lookup"><span data-stu-id="7c729-115">When you add a new customer on the project-based quote line, the customer is also added to the overall quote as a quote customer, with a default billing split percentage on the overall quote of 0%.</span></span> <span data-ttu-id="7c729-116">Le pourcentage de facturation fractionnée sur le devis global est copié dans les nouvelles lignes de devis et dans l’éventuel contrat de projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-116">The billing split percentage on the overall quote is copied to new quote lines and to the eventual project contract.</span></span> <span data-ttu-id="7c729-117">Cependant, lorsque vous facturez à partir du contrat, le pourcentage de facturation fractionnée au niveau de la ligne de devis est utilisé, et non le pourcentage de facturation fractionnée au niveau du contrat global.</span><span class="sxs-lookup"><span data-stu-id="7c729-117">However, when you invoice from the contract, the billing split percentage at the quote line level is used, not the billing split percentage at the overall contract level.</span></span> 

<span data-ttu-id="7c729-118">Le tableau suivant affiche les champs sur l’enregistrement de client de la ligne de devis d’une ligne de devis selon un projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-118">The following table shows the fields on the quote line customer record of a project-based quote line.</span></span>

| <span data-ttu-id="7c729-119">Champ</span><span class="sxs-lookup"><span data-stu-id="7c729-119">Field</span></span> | <span data-ttu-id="7c729-120">Emplacement</span><span class="sxs-lookup"><span data-stu-id="7c729-120">Location</span></span> | <span data-ttu-id="7c729-121">Description et conseils</span><span class="sxs-lookup"><span data-stu-id="7c729-121">Description and guidance</span></span> | <span data-ttu-id="7c729-122">Impact en aval</span><span class="sxs-lookup"><span data-stu-id="7c729-122">Downstream impact</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="7c729-123">**Compte**</span><span class="sxs-lookup"><span data-stu-id="7c729-123">**Account**</span></span> | <span data-ttu-id="7c729-124">Grille modifiable sur l’onglet **Clients de ligne du devis**, le formulaire principal et le formulaire de création rapide pour un client de ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-124">An editable grid on the **Quote line customers** tab, the main form, and the quick create form for a quote line customer.</span></span> | <span data-ttu-id="7c729-125">Répertorie tous les comptes actifs.</span><span class="sxs-lookup"><span data-stu-id="7c729-125">Lists all active accounts.</span></span> <span data-ttu-id="7c729-126">Ce champ est verrouillé après la création de l’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="7c729-126">This field is locked after the record is created.</span></span> <span data-ttu-id="7c729-127">Si vous devez mettre à jour le champ, supprimez et recréez l’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="7c729-127">If you need to update the field, delete and recreate the record.</span></span> <span data-ttu-id="7c729-128">Si vous avez enregistré des chiffres réels, vous ne pouvez pas supprimer l’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="7c729-128">If you recorded any actuals, you can't delete the record.</span></span> | <span data-ttu-id="7c729-129">Lorsque vous sélectionnez un compte dans la liste principale des comptes à ajouter, le client de la ligne de devis est également ajouté en tant que client de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-129">When you pick an account from the master list of accounts to add, the Quote line customer is also added as a Quote customer.</span></span> <span data-ttu-id="7c729-130">Les clients de la ligne de devis sont également copiés vers les clients de la ligne du contrat de projet lorsqu’un devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="7c729-130">Quote line customers are copied to the project contract line customers when a quote is won.</span></span> |
| <span data-ttu-id="7c729-131">**Pourcentage de facturation fractionnée**</span><span class="sxs-lookup"><span data-stu-id="7c729-131">**Billing split percent**</span></span> | <span data-ttu-id="7c729-132">Grille modifiable sur l’onglet **Clients de ligne du devis**, le formulaire principal et le formulaire de création rapide pour un client de ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-132">An editable grid on the **Quote line customers** tab, the main form, and the quick create form for a quote line customer.</span></span> | <span data-ttu-id="7c729-133">Représente le pourcentage de chaque transaction de vente non facturée qui sera attribuée à ce client de ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-133">Represents the percentage of each unbilled sales transaction that will be attributed to this quote line customer.</span></span> | <span data-ttu-id="7c729-134">Copié vers les clients de la ligne du contrat du projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-134">Copied over to project contract line customers.</span></span> |
| <span data-ttu-id="7c729-135">**Limite à ne pas dépasser**</span><span class="sxs-lookup"><span data-stu-id="7c729-135">**Not-to-exceed limit**</span></span> | <span data-ttu-id="7c729-136">Grille modifiable sur l’onglet **Clients de ligne du devis**, le formulaire principal et le formulaire de création rapide pour un client de ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-136">An editable grid on the **Quote line customers** tab, the main form, and the quick create form for a quote line customer.</span></span> | <span data-ttu-id="7c729-137">Indique s’il existe une limite ou un plafond négocié au montant global qui sera facturé à ce client pour cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-137">Indicates whether there is a negotiated limit or cap to the overall amount that will be invoiced to this customer for this quoted line.</span></span> | <span data-ttu-id="7c729-138">Copié vers les clients de la ligne du contrat de projet lorsqu’un devis est remporté.</span><span class="sxs-lookup"><span data-stu-id="7c729-138">Copied over to project contract line customers when a quote is won.</span></span> |
| <span data-ttu-id="7c729-139">**Société propriétaire**</span><span class="sxs-lookup"><span data-stu-id="7c729-139">**Owning company**</span></span> | <span data-ttu-id="7c729-140">Grille modifiable sur l’onglet **Clients de ligne du devis**, le formulaire principal et le formulaire de création rapide pour un client de ligne de devis,</span><span class="sxs-lookup"><span data-stu-id="7c729-140">An editable grid on the **Quote line customers** tab, the main form, and the quick create form for a quote line customer,</span></span> | <span data-ttu-id="7c729-141">L’entité juridique dans laquelle ce client est installé dans le module **Gestion de projet et comptabilité**.</span><span class="sxs-lookup"><span data-stu-id="7c729-141">The legal entity in which this customer is set up in the **Project management and accounting** module.</span></span> <span data-ttu-id="7c729-142">Ce champ est en lecture seule et est défini sur la société propriétaire du devis lui-même.</span><span class="sxs-lookup"><span data-stu-id="7c729-142">This field is read-only and is set to the owning company of the quote itself.</span></span> <span data-ttu-id="7c729-143">La liste des clients à ajouter dans le champ **Compte** est déjà filtré dans la liste de la société propriétaire dans le module **Gestion de projet et comptabilité** de Project Operations.</span><span class="sxs-lookup"><span data-stu-id="7c729-143">The list of customers to add in the **Account** field is already filtered to the list from the owning company in the **Project management and accounting** module of Project Operations.</span></span> | <span data-ttu-id="7c729-144">La société propriétaire équivaut au concept d’entité juridique.</span><span class="sxs-lookup"><span data-stu-id="7c729-144">The owning company equates to the concept of legal entity.</span></span> <span data-ttu-id="7c729-145">Tous les coûts et revenus générés par ce projet sont comptabilisés dans la comptabilité de la société propriétaire.</span><span class="sxs-lookup"><span data-stu-id="7c729-145">All costs and revenue that accrue from this project are accounted in the General ledger of the owning company.</span></span> |
| <span data-ttu-id="7c729-146">**Est arrondi**</span><span class="sxs-lookup"><span data-stu-id="7c729-146">**Is rounding**</span></span> | <span data-ttu-id="7c729-147">Grille modifiable sur l’onglet **Clients de ligne du devis**, le formulaire principal et le formulaire de création rapide pour un client de ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-147">An editable grid on the **Quote line customers** tab, the main form, and the quick create form for a quote line customer.</span></span> | <span data-ttu-id="7c729-148">Indique si ce client est un client arrondi par défaut pour cette ligne de devis basée sur un projet.</span><span class="sxs-lookup"><span data-stu-id="7c729-148">Indicates whether this customer is a default rounding customer for this project-based quote line.</span></span> | <span data-ttu-id="7c729-149">Copié vers les clients du contrat de projet lorsqu’un devis est remporté.</span><span class="sxs-lookup"><span data-stu-id="7c729-149">Copied over to project contract customers when a quote is won.</span></span> |

## <a name="edit-billing-split-percentages"></a><span data-ttu-id="7c729-150">Modifier des pourcentages de facturation fractionnée</span><span class="sxs-lookup"><span data-stu-id="7c729-150">Edit billing split percentages</span></span>

<span data-ttu-id="7c729-151">Vous pouvez modifier les pourcentages de facturation fractionnée en ligne.</span><span class="sxs-lookup"><span data-stu-id="7c729-151">You can edit billing split percentages in-line.</span></span> <span data-ttu-id="7c729-152">Lorsque les pourcentages de facturation fractionnée ne totalisent pas 100 %, une erreur se produit.</span><span class="sxs-lookup"><span data-stu-id="7c729-152">When the billing split percentages don't total 100%, an error occurs.</span></span> <span data-ttu-id="7c729-153">Après avoir modifié les pourcentages de facturation fractionnée, actualisez la page de ligne de devis pour supprimer l’erreur.</span><span class="sxs-lookup"><span data-stu-id="7c729-153">After you edit the billing split percentages, refresh the quote line page to remove the error.</span></span>

<span data-ttu-id="7c729-154">Utilisez l’action de répartition homogène sur la sous-grille des clients de la ligne de devis pour attribuer des facturations fractionnées à tous les clients de la ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="7c729-154">Use the evenly distribute action on the quote line customers subgrid to allocate billing splits to all quote line customers.</span></span> <span data-ttu-id="7c729-155">S’il y a un facteur d’arrondi, il sera ajouté au client d’arrondi.</span><span class="sxs-lookup"><span data-stu-id="7c729-155">If there's a rounding factor, that will be added to the rounding customer.</span></span> <span data-ttu-id="7c729-156">L’un des clients de la ligne de devis est toujours marqué comme client d’arrondi, ce qui signifie que l’enregistrement de client de la ligne de devis a l’indicateur d’arrondi défini sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="7c729-156">One of the quote line customers is always tagged as the rounding customer, which means that quote line customer record has the rounding flag set to **Yes**.</span></span> 