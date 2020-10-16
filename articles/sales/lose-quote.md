---
title: Copier les devis selon les projets
description: Cette rubrique offre des informations sur la copie des devis selon les projets dans Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d7234958d542dec4cba55cb0516f1222937389e1
ms.sourcegitcommit: f255b2cbf290973ce62fe2c1c121bd1df15a7392
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/01/2020
ms.locfileid: "3928563"
---
# <a name="copy-project-based-quotes"></a><span data-ttu-id="1f148-103">Copier les devis selon les projets</span><span class="sxs-lookup"><span data-stu-id="1f148-103">Copy project-based quotes</span></span>

<span data-ttu-id="1f148-104">_**S’applique à :** Project Operations pour les scénarios basés sur les ressources/produits non stockés Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="1f148-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1f148-105">Vous pouvez facilement créer un devis de projet en copiant un existant.</span><span class="sxs-lookup"><span data-stu-id="1f148-105">You can easily create a new Project quote by copying an existing one.</span></span> 

- <span data-ttu-id="1f148-106">Pour copier un devis de projet, sur la page de liste **Devis de projets** ou la page des détails **Devis de projet**, sélectionnez le devis de projet à copier, puis sélectionnez **Copier**.</span><span class="sxs-lookup"><span data-stu-id="1f148-106">To copy a Project quote, on the **Project Quotes** list page or the **Project Quote** details page, select the Project quote you want to copy, and then select **Copy**.</span></span>

<span data-ttu-id="1f148-107">Cela ouvrira une page de dialogue où vous pourrez entrer les paramètres de la copie.</span><span class="sxs-lookup"><span data-stu-id="1f148-107">This will open a dialog page where you can enter the parameters of the copy.</span></span> <span data-ttu-id="1f148-108">Le tableau suivant répertorie les champs inclus dans la page de dialogue :</span><span class="sxs-lookup"><span data-stu-id="1f148-108">The following table lists the fields that are included in the dialog page.</span></span> <span data-ttu-id="1f148-109">Selon les valeurs que vous sélectionnez, le processus de copie peut changer.</span><span class="sxs-lookup"><span data-stu-id="1f148-109">Depending on the values you select, the copy process may change.</span></span>

| <span data-ttu-id="1f148-110">**Champ**</span><span class="sxs-lookup"><span data-stu-id="1f148-110">**Field**</span></span> | <span data-ttu-id="1f148-111">**Pertinence, objectif et conseils**</span><span class="sxs-lookup"><span data-stu-id="1f148-111">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="1f148-112">**Impact en aval**</span><span class="sxs-lookup"><span data-stu-id="1f148-112">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1f148-113">Rubrique</span><span class="sxs-lookup"><span data-stu-id="1f148-113">Topic</span></span> | <span data-ttu-id="1f148-114">Saisissez le sujet, ou le nom, du devis cible.</span><span class="sxs-lookup"><span data-stu-id="1f148-114">Enter the relevant topic, or name, of the target quote.</span></span> <span data-ttu-id="1f148-115">Lorsque la boîte de dialogue s’ouvre, le système le définira sur le sujet du devis source avec **-copie** comme suffixe.</span><span class="sxs-lookup"><span data-stu-id="1f148-115">When the dialog opens, the system will set it to the topic of the source quote with **-copy** appended to it.</span></span> | |
| <span data-ttu-id="1f148-116">Prospect</span><span class="sxs-lookup"><span data-stu-id="1f148-116">Potential Customer</span></span> | <span data-ttu-id="1f148-117">Référence à la société ou à l’enregistrement de compte du client.</span><span class="sxs-lookup"><span data-stu-id="1f148-117">Reference to the customer's company or account record.</span></span> <span data-ttu-id="1f148-118">Lorsque la boîte de dialogue s’ouvre, le système le définira sur le compte du devis source.</span><span class="sxs-lookup"><span data-stu-id="1f148-118">When the dialog opens, the system will set it to the account on the source quote.</span></span> | <span data-ttu-id="1f148-119">Ce champ est le client principal du devis.</span><span class="sxs-lookup"><span data-stu-id="1f148-119">This field is the primary customer on the quote.</span></span> |
| <span data-ttu-id="1f148-120">Unité contractuelle</span><span class="sxs-lookup"><span data-stu-id="1f148-120">Contracting Unit</span></span> | <span data-ttu-id="1f148-121">Unité organisationnelle responsable de la livraison du ou des projets associés à cette transaction.</span><span class="sxs-lookup"><span data-stu-id="1f148-121">The organization unit that is responsible for the delivery of the project(s) associated with this deal.</span></span>
<span data-ttu-id="1f148-122">Lorsque la boîte de dialogue s’ouvre, le système le définira sur l’unité contractuelle du devis source.</span><span class="sxs-lookup"><span data-stu-id="1f148-122">When the dialog opens, the system will set it to the contracting unit of the source quote.</span></span> | <span data-ttu-id="1f148-123">L’unité contractuelle est la division de l’entreprise qui exécutera les projets après la conclusion de la transaction.</span><span class="sxs-lookup"><span data-stu-id="1f148-123">Contracting unit is the division of the company that will execute the projects after the deal is closed.</span></span> <span data-ttu-id="1f148-124">Chaque unité contractuelle dispose d’une devise.</span><span class="sxs-lookup"><span data-stu-id="1f148-124">Every contracting unit has a currency.</span></span> <span data-ttu-id="1f148-125">La devise est utilisée pour déclarer les coûts estimés et réels engagés pendant l’exécution du projet.</span><span class="sxs-lookup"><span data-stu-id="1f148-125">The currency is used to report estimated and actual costs incurred during the execution of the project.</span></span> |
| <span data-ttu-id="1f148-126">Devise</span><span class="sxs-lookup"><span data-stu-id="1f148-126">Currency</span></span> | <span data-ttu-id="1f148-127">Il s’agit de la devise dans laquelle la transaction est réalisée.</span><span class="sxs-lookup"><span data-stu-id="1f148-127">This is the currency that the deal is transacted in.</span></span> <span data-ttu-id="1f148-128">Lorsque la boîte de dialogue s’ouvre, le système le définira sur la devise du devis source.</span><span class="sxs-lookup"><span data-stu-id="1f148-128">When the dialog opens, the system will set it to the currency of the source quote.</span></span> <span data-ttu-id="1f148-129">Cela peut être modifié et si c’est le cas, le champ **Copier le prix** est toujours défini sur **Non**.</span><span class="sxs-lookup"><span data-stu-id="1f148-129">This can be modified and if it is change, the **Copy Pricing** field is always set to **No**.</span></span> <span data-ttu-id="1f148-130">En effet, les tarifs sur le devis source ne sont plus pertinentes.</span><span class="sxs-lookup"><span data-stu-id="1f148-130">This is because the price lists on source quote are no longer relevant.</span></span> | <span data-ttu-id="1f148-131">La devise est utilisée par défaut pour un tarif, pour générer une estimation financière sur le devis et finalement pour facturer le client lorsque la transaction est gagnée.</span><span class="sxs-lookup"><span data-stu-id="1f148-131">Currency is used to default a price list, to build a financial estimate on the quote,  and eventually to invoice the customer when the deal is won.</span></span> |
| <span data-ttu-id="1f148-132">Date de livraison demandée</span><span class="sxs-lookup"><span data-stu-id="1f148-132">Requested Delivery Date</span></span> | <span data-ttu-id="1f148-133">Il s’agit de la date de livraison demandée par le client.</span><span class="sxs-lookup"><span data-stu-id="1f148-133">This is the date of delivery requested by the customer.</span></span> | <span data-ttu-id="1f148-134">Elle est utilisée comme date de fin lors de la création de dates de facturation selon une fréquence spécifique.</span><span class="sxs-lookup"><span data-stu-id="1f148-134">This is used as the end date when creating invoicing dates along a specific frequency.</span></span> |
| <span data-ttu-id="1f148-135">Copier la tarification</span><span class="sxs-lookup"><span data-stu-id="1f148-135">Copy pricing</span></span> | <span data-ttu-id="1f148-136">Une valeur Oui/Non indique si la tarification du devis doit être copiée à partir du devis source.</span><span class="sxs-lookup"><span data-stu-id="1f148-136">A Yes/No value indicates whether the pricing on the quote should be copied from the source quote.</span></span> | <span data-ttu-id="1f148-137">Si **Oui** est sélectionné, le tarif du projet et les références du tarif du produit sont copiés du devis source vers le devis cible.</span><span class="sxs-lookup"><span data-stu-id="1f148-137">If **Yes** is selected, the project price list and product price list references are copied from the source quote to the target quote.</span></span> <span data-ttu-id="1f148-138">Si **Non** est sélectionné, les tarifs sont rétablis par défaut en fonction des derniers tarifs qui ont été configurés sur les paramètres du compte ou du projet.</span><span class="sxs-lookup"><span data-stu-id="1f148-138">If **No** is selected, price lists are re-defaulted based on the latest price lists that were set up on the account or project parameters.</span></span> |

<span data-ttu-id="1f148-139">Lorsque vous sélectionnez **OK** sur la page de dialogue, le système crée une copie du devis de projet en fonction des paramètres sélectionnés dans la boîte de dialogue.</span><span class="sxs-lookup"><span data-stu-id="1f148-139">When you select **OK** on the dialog page, the system creates a copy of the project quote based on the parameters selected in the dialog.</span></span> <span data-ttu-id="1f148-140">Le nouveau devis de projet s’ouvre.</span><span class="sxs-lookup"><span data-stu-id="1f148-140">The new project quote opens.</span></span> 

> [!NOTE]
> <span data-ttu-id="1f148-141">Les informations suivantes ne sont pas copiées de la source vers le devis cible :</span><span class="sxs-lookup"><span data-stu-id="1f148-141">The following information is not copied from the Source to the Target quote:</span></span>
>
> - <span data-ttu-id="1f148-142">Planifications de facture</span><span class="sxs-lookup"><span data-stu-id="1f148-142">Invoice schedules</span></span>
> - <span data-ttu-id="1f148-143">Devis et clients de la ligne de devis</span><span class="sxs-lookup"><span data-stu-id="1f148-143">Quote and quote line customers</span></span>
> - <span data-ttu-id="1f148-144">Référence du projet sur le projet – lignes de devis basées sur les informations budgétaires client</span><span class="sxs-lookup"><span data-stu-id="1f148-144">Project reference on the project – based quote lines -Customer budget information</span></span>
>
><span data-ttu-id="1f148-145">Étant donné que ces informations sont très spécifiques à chaque devis, ces champs et enregistrements ne sont pas copiés.</span><span class="sxs-lookup"><span data-stu-id="1f148-145">Because this information is very specific to each quote, these fields and records are not copied.</span></span> <span data-ttu-id="1f148-146">Les lignes de devis pour les projets et les produits, les estimations sur les détails de la ligne de devis et les valeurs à ne pas dépasser au niveau du devis sont copiées.</span><span class="sxs-lookup"><span data-stu-id="1f148-146">Quote lines for projects and products, estimates on quote line details, and not-to-exceed values at the quote level are copied.</span></span> <span data-ttu-id="1f148-147">Les valeurs par défaut de prix et de taux de coût dépendent de l’option **Copier la tarification** sélectionnée sur la page de dialogue **Copier les paramètres**.</span><span class="sxs-lookup"><span data-stu-id="1f148-147">Price and cost rate defaults depend on the **Copy pricing** option selected on the **Copy parameters** dialog page.</span></span>