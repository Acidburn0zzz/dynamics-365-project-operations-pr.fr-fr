---
title: Lignes du devis selon les projets (Pro)
description: Cette rubrique fournit des informations sur l’utilisation des lignes de devis basées sur un projet pour le travail du projet. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4075670"
---
# <a name="project-based-quote-lines-pro"></a><span data-ttu-id="35734-104">Lignes du devis selon les projets (Pro)</span><span class="sxs-lookup"><span data-stu-id="35734-104">Project-based quote lines (Pro)</span></span>

<span data-ttu-id="35734-105">_**S’applique à :** Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="35734-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="35734-106">Les lignes de devis basées sur un projet sont conçues pour aider à estimer le travail du projet sur un engagement.</span><span class="sxs-lookup"><span data-stu-id="35734-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="35734-107">La structure d’une ligne de devis basée sur un projet est étendue pour les devis du projet avec les concepts suivants :</span><span class="sxs-lookup"><span data-stu-id="35734-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="35734-108">Mode de facturation</span><span class="sxs-lookup"><span data-stu-id="35734-108">Billing Method</span></span>
- <span data-ttu-id="35734-109">Mappage des tâches et projets</span><span class="sxs-lookup"><span data-stu-id="35734-109">Project and Task Mapping</span></span>
- <span data-ttu-id="35734-110">Classes de transaction incluses</span><span class="sxs-lookup"><span data-stu-id="35734-110">Included Transaction classes</span></span>
- <span data-ttu-id="35734-111">Limite à ne pas dépasser</span><span class="sxs-lookup"><span data-stu-id="35734-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="35734-112">Configuration de l’exigibilité</span><span class="sxs-lookup"><span data-stu-id="35734-112">Chargeability setup</span></span>
- <span data-ttu-id="35734-113">Estimation à l’aide des détails de la ligne de devis</span><span class="sxs-lookup"><span data-stu-id="35734-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="35734-114">Clients de la ligne de devis</span><span class="sxs-lookup"><span data-stu-id="35734-114">Quote line Customers</span></span>

<span data-ttu-id="35734-115">Le tableau suivant fournit des informations sur les champs de l’onglet **Général** de la ligne de devis basée sur le projet.</span><span class="sxs-lookup"><span data-stu-id="35734-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="35734-116">Ces champs aident à jeter les bases d’une estimation détaillée et à la base du travail du projet.</span><span class="sxs-lookup"><span data-stu-id="35734-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="35734-117">**Champ**</span><span class="sxs-lookup"><span data-stu-id="35734-117">**Field**</span></span> | <span data-ttu-id="35734-118">**Pertinence, objectif et conseils**</span><span class="sxs-lookup"><span data-stu-id="35734-118">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="35734-119">**Impact en aval**</span><span class="sxs-lookup"><span data-stu-id="35734-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="35734-120">Nom</span><span class="sxs-lookup"><span data-stu-id="35734-120">Name</span></span> | <span data-ttu-id="35734-121">Nom de la ligne de devis qui devrait vous aider à identifier le composant discret du devis qui est estimé.</span><span class="sxs-lookup"><span data-stu-id="35734-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="35734-122">Copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-123">Mode de facturation</span><span class="sxs-lookup"><span data-stu-id="35734-123">Billing Method</span></span> | <span data-ttu-id="35734-124">Sur un devis créé à partir d’une opportunité, cette valeur est copiée à partir du champ correspondant sur la ligne d’opportunité.</span><span class="sxs-lookup"><span data-stu-id="35734-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="35734-125">Ce champ comprend les deux principaux modèles de contrats pris en charge par Dynamics 365 Project Operations :</span><span class="sxs-lookup"><span data-stu-id="35734-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="35734-126">- Prix fixe</span><span class="sxs-lookup"><span data-stu-id="35734-126">- Fixed price</span></span></br><span data-ttu-id="35734-127">- Temps et matériel.</span><span class="sxs-lookup"><span data-stu-id="35734-127">- Time and material.</span></span>| <span data-ttu-id="35734-128">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-129">Project</span><span class="sxs-lookup"><span data-stu-id="35734-129">Project</span></span> | <span data-ttu-id="35734-130">Utilisez ce champ facultatif pour identifier le projet qui sera utilisé pour livrer le travail sur cet engagement.</span><span class="sxs-lookup"><span data-stu-id="35734-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="35734-131">Lorsqu’un projet est mappé à une ligne de devis, cela aide à configurer des tâches facturables et également à intégrer une estimation basée sur le projet à la ligne de devis en tant que détails de la ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="35734-132">Lorsqu’un projet n’est pas mappé à une ligne de devis basée sur un projet, l’estimation doit être créée manuellement en créant chaque détail de ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="35734-133">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="35734-134">Tâches incluses</span><span class="sxs-lookup"><span data-stu-id="35734-134">Included Tasks</span></span> | <span data-ttu-id="35734-135">Indique si cette ligne de devis est utilisée pour tout ou partie des tâches du projet pour le projet sélectionné.</span><span class="sxs-lookup"><span data-stu-id="35734-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="35734-136">Ce champ contient les valeurs possibles suivantes :</span><span class="sxs-lookup"><span data-stu-id="35734-136">This field has the following possible values:</span></span></br><span data-ttu-id="35734-137">- Toutes les tâches du projet</span><span class="sxs-lookup"><span data-stu-id="35734-137">- All project tasks</span></span></br><span data-ttu-id="35734-138">- Tâches du projet sélectionnées uniquement</span><span class="sxs-lookup"><span data-stu-id="35734-138">- Selected project tasks only</span></span></br><span data-ttu-id="35734-139">Une valeur vide dans ce champ équivaut à l’option **Toutes les tâches du projet**.</span><span class="sxs-lookup"><span data-stu-id="35734-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="35734-140">Lorsque **Tâches de projet sélectionnées uniquement** est sélectionné sur la page du projet, l’onglet **Configuration de la facturation des tâches** vous permet de sélectionner des tâches spécifiques pour les associer à cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="35734-141">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-142">Inclure le temps</span><span class="sxs-lookup"><span data-stu-id="35734-142">Include Time</span></span> | <span data-ttu-id="35734-143">Un indicateur **Oui**/**Non** indique si les transactions de temps ou les coûts de main-d’œuvre sur le projet sélectionné seront inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="35734-144">Une valeur de **Non** indique que le coût des transactions de temps ou de coûts de main-d’œuvre ne seront pas inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="35734-145">Une valeur de **Oui** indique que le coût des transactions de temps ou de coûts de main-d’œuvre seront inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="35734-146">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-147">Inclure la dépense</span><span class="sxs-lookup"><span data-stu-id="35734-147">Include Expense</span></span> | <span data-ttu-id="35734-148">Un indicateur **Oui**/**Non** indique si les coûts de dépenses sur le projet sélectionné seront inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="35734-149">Une valeur de **Non** indique que le coût de dépenses ne seront pas inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="35734-150">Une valeur de **Oui** indique que le coût de dépenses seront inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="35734-151">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-152">Inclure les frais</span><span class="sxs-lookup"><span data-stu-id="35734-152">Include Fee</span></span> | <span data-ttu-id="35734-153">Un indicateur **Oui**/**Non** indique si les frais sur le projet sélectionné seront inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="35734-154">Une valeur de **Non** indique que les frais ne seront pas inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="35734-155">Une valeur de **Oui** indique que les frais seront inclus dans l’estimation sur cette ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="35734-156">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-157">Montant du devis</span><span class="sxs-lookup"><span data-stu-id="35734-157">Quoted Amount</span></span> | <span data-ttu-id="35734-158">Il s’agit du montant qui sera proposé au client pour tous les travaux prévus sur cette ligne de devis projet.</span><span class="sxs-lookup"><span data-stu-id="35734-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="35734-159">Sur un devis créé à partir d’une opportunité, cette valeur est copiée à partir du champ **Budget client** sur la ligne d’opportunité.</span><span class="sxs-lookup"><span data-stu-id="35734-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="35734-160">Lorsque la ligne de devis basée sur le projet comporte des détails de ligne, ce champ est verrouillé pour modification et est résumé à partir du montant sur les détails de la ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="35734-161">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-162">Estimation de taxe</span><span class="sxs-lookup"><span data-stu-id="35734-162">Estimated Tax</span></span> | <span data-ttu-id="35734-163">Il s’agit d’un champ modifiable permettant à l’utilisateur d’ajouter le montant estimé de la taxe sur la ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="35734-164">Lorsqu’une ligne de devis basée sur le projet comporte des détails de ligne, ce champ est verrouillé pour modification et est résumé à partir du montant de la taxe sur les détails de la ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="35734-165">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-166">Montant du devis après taxes</span><span class="sxs-lookup"><span data-stu-id="35734-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="35734-167">Ce champ est le montant de la ligne de devis après taxes et est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="35734-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="35734-168">Le montant dans ce champ est calculé comme suit *Montant estimé + taxes*.</span><span class="sxs-lookup"><span data-stu-id="35734-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="35734-169">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-170">Limite à ne pas dépasser</span><span class="sxs-lookup"><span data-stu-id="35734-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="35734-171">Ce champ est modifiable et n’est disponible que sur les lignes de devis basées sur un projet qui ont une méthode de facturation **Temps et matériel**.</span><span class="sxs-lookup"><span data-stu-id="35734-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="35734-172">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="35734-173">Budget client</span><span class="sxs-lookup"><span data-stu-id="35734-173">Customer Budget</span></span> | <span data-ttu-id="35734-174">Ce champ est modifiable et copié à partir du champ correspondant sur la ligne d’opportunité si le devis a été créé à partir d’une opportunité.</span><span class="sxs-lookup"><span data-stu-id="35734-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="35734-175">Ce champ est copié dans la ligne de contrat de projet créée à partir de cette ligne de devis lorsque le devis est conclu.</span><span class="sxs-lookup"><span data-stu-id="35734-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="35734-176">Règles de validation pour les champs de l’onglet Général des lignes de devis basées sur le projet</span><span class="sxs-lookup"><span data-stu-id="35734-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="35734-177">**Règle 1**  : Si le champ **Tâches incluses** est vide ou s’il est défini sur **Toutes les tâches du projet** , un projet est inclus dans la ligne de devis.</span><span class="sxs-lookup"><span data-stu-id="35734-177">**Rule 1** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project is included in the quote line.</span></span>

<span data-ttu-id="35734-178">**Règle 2**  : Si le champ **Tâches incluses** est vide ou s’il est défini sur **Toutes les tâches du projet** , un projet et une certaine classe de transaction ne peuvent être inclus que sur une seule ligne de devis basée sur un projet d’un devis.</span><span class="sxs-lookup"><span data-stu-id="35734-178">**Rule 2** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="35734-179">**Règle 3**  : Si le champ **Tâches incluses** est défini sur **Tâches du projet sélectionnées uniquement** , un projet et une certaine classe de transaction ne peuvent être inclus que sur plusieurs lignes de devis basées sur un projet d’un devis.</span><span class="sxs-lookup"><span data-stu-id="35734-179">**Rule 3** : If the **Included Tasks** field is set to **Selected project tasks only** , a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="35734-180">**Règle 4**  : Si une opportunité comporte plusieurs devis, il peut y avoir des lignes de devis de différents devis qui font toutes référence au même projet et incluent la même classe de transaction.</span><span class="sxs-lookup"><span data-stu-id="35734-180">**Rule 4** : If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="35734-181">**Règle 5**  : Si les devis n’appartiennent pas à la même opportunité, ils ne peuvent pas inclure le même projet et la même classe de transaction.</span><span class="sxs-lookup"><span data-stu-id="35734-181">**Rule 5** : If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="35734-182">
                    <strong>Opportunité</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="35734-183">
                    <strong>devis</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="35734-184">
                    <strong>Ligne de devis</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="35734-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="35734-186">
                    <strong>Tâches incluses</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="35734-187">
                    <strong>Inclure le temps</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="35734-188">
                    <strong>Inclure la dépense</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="35734-189">
                    <strong>Inclure</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="35734-190">
                    <strong>Frais</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="35734-191">
                    <strong>Valide/Non valide</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="35734-192">
                    <strong>Motif</strong>
                </span><span class="sxs-lookup"><span data-stu-id="35734-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-193">O1</span><span class="sxs-lookup"><span data-stu-id="35734-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-194">T1</span><span class="sxs-lookup"><span data-stu-id="35734-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-195">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-196">P1</span><span class="sxs-lookup"><span data-stu-id="35734-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-197">Vierge</span><span class="sxs-lookup"><span data-stu-id="35734-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-198">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-199">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-200">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-201">Non valide</span><span class="sxs-lookup"><span data-stu-id="35734-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-202">Violation de la règle n° 2.</span><span class="sxs-lookup"><span data-stu-id="35734-202">Violation of Rule #2.</span></span> <span data-ttu-id="35734-203">Le temps, les dépenses et les frais du projet P1 sont inclus dans les lignes de devis, QL1 et QL2.</span><span class="sxs-lookup"><span data-stu-id="35734-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-204">O1</span><span class="sxs-lookup"><span data-stu-id="35734-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-205">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-206">QL2</span><span class="sxs-lookup"><span data-stu-id="35734-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-207">P1</span><span class="sxs-lookup"><span data-stu-id="35734-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-208">Vierge</span><span class="sxs-lookup"><span data-stu-id="35734-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-209">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-210">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-211">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-211">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-212">O1</span><span class="sxs-lookup"><span data-stu-id="35734-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-213">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-214">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-215">P1</span><span class="sxs-lookup"><span data-stu-id="35734-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-216">Vierge</span><span class="sxs-lookup"><span data-stu-id="35734-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-217">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-218">Non</span><span class="sxs-lookup"><span data-stu-id="35734-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-219">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-220">Non valide</span><span class="sxs-lookup"><span data-stu-id="35734-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-221">Violation de la règle n° 2.</span><span class="sxs-lookup"><span data-stu-id="35734-221">Violation of Rule #2.</span></span> <span data-ttu-id="35734-222">Le temps et les frais du projet P1 sont inclus dans les lignes de devis, QL1 et QL2.</span><span class="sxs-lookup"><span data-stu-id="35734-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-223">O1</span><span class="sxs-lookup"><span data-stu-id="35734-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-224">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-225">QL2</span><span class="sxs-lookup"><span data-stu-id="35734-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-226">P1</span><span class="sxs-lookup"><span data-stu-id="35734-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-227">Vierge</span><span class="sxs-lookup"><span data-stu-id="35734-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-228">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-229">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-230">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-230">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-231">O1</span><span class="sxs-lookup"><span data-stu-id="35734-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-232">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-233">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-234">P1</span><span class="sxs-lookup"><span data-stu-id="35734-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-235">Vierge</span><span class="sxs-lookup"><span data-stu-id="35734-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-236">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-237">Non</span><span class="sxs-lookup"><span data-stu-id="35734-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-238">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-239">Valide</span><span class="sxs-lookup"><span data-stu-id="35734-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="35734-240">Le temps et les frais du projet P1 sont inclus sur QL1.</span><span class="sxs-lookup"><span data-stu-id="35734-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="35734-241">Les dépenses du projet P1 sont inclus sur QL2.</span><span class="sxs-lookup"><span data-stu-id="35734-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="35734-242">Il n’y a pas de chevauchement dans ce qui est inclus sur chaque ligne de devis et est valide.</span><span class="sxs-lookup"><span data-stu-id="35734-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-243">O1</span><span class="sxs-lookup"><span data-stu-id="35734-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-244">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-245">QL2</span><span class="sxs-lookup"><span data-stu-id="35734-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-246">P1</span><span class="sxs-lookup"><span data-stu-id="35734-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-247">Vierge</span><span class="sxs-lookup"><span data-stu-id="35734-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-248">Non</span><span class="sxs-lookup"><span data-stu-id="35734-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-249">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-250">Non</span><span class="sxs-lookup"><span data-stu-id="35734-250">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-251">O1</span><span class="sxs-lookup"><span data-stu-id="35734-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-252">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-253">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-254">P1</span><span class="sxs-lookup"><span data-stu-id="35734-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-255">Tâches sélectionnées uniquement</span><span class="sxs-lookup"><span data-stu-id="35734-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-256">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-257">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-258">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-259">Non valide</span><span class="sxs-lookup"><span data-stu-id="35734-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-260">Violation de la règle n° 2 ci-dessus</span><span class="sxs-lookup"><span data-stu-id="35734-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="35734-261">Q1 comprend le temps, les dépenses et les frais sur un sous-ensemble de tâches du projet P1.</span><span class="sxs-lookup"><span data-stu-id="35734-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="35734-262">QL2 comprend le temps, les dépenses et les frais pour l’ensemble du projet P1 et chevauche ce qui est inclus dans Q1.</span><span class="sxs-lookup"><span data-stu-id="35734-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-263">O1</span><span class="sxs-lookup"><span data-stu-id="35734-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-264">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-265">QL2</span><span class="sxs-lookup"><span data-stu-id="35734-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-266">P1</span><span class="sxs-lookup"><span data-stu-id="35734-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-267">Vierge</span><span class="sxs-lookup"><span data-stu-id="35734-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-268">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-269">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-270">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-270">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-271">O1</span><span class="sxs-lookup"><span data-stu-id="35734-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-272">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-273">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-274">P1</span><span class="sxs-lookup"><span data-stu-id="35734-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-275">Tâches sélectionnées uniquement</span><span class="sxs-lookup"><span data-stu-id="35734-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-276">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-277">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-278">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-279">Valide</span><span class="sxs-lookup"><span data-stu-id="35734-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-280">Conformément à la règle n° 3 ci-dessus,</span><span class="sxs-lookup"><span data-stu-id="35734-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="35734-281">Q1 comprend le temps, les dépenses et les frais sur un sous-ensemble de tâches du projet P1.</span><span class="sxs-lookup"><span data-stu-id="35734-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="35734-282">QL2 comprend le temps, les dépenses et les frais pour un sous-ensemble de tâches du projet P1.</span><span class="sxs-lookup"><span data-stu-id="35734-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="35734-283">La seule validation supplémentaire concerne le sous-ensemble de tâches sur QL1 qui est différent du sous-ensemble de tâches sur QL2.</span><span class="sxs-lookup"><span data-stu-id="35734-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="35734-284">Cela garantit qu’il n’y a pas de chevauchements.</span><span class="sxs-lookup"><span data-stu-id="35734-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="35734-285">Ceci est fait par le système lorsque des tâches sont associées.</span><span class="sxs-lookup"><span data-stu-id="35734-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-286">O1</span><span class="sxs-lookup"><span data-stu-id="35734-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-287">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-288">QL2</span><span class="sxs-lookup"><span data-stu-id="35734-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-289">P1</span><span class="sxs-lookup"><span data-stu-id="35734-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-290">Tâches sélectionnées uniquement</span><span class="sxs-lookup"><span data-stu-id="35734-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-291">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-292">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-293">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-293">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-294">O1</span><span class="sxs-lookup"><span data-stu-id="35734-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-295">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-296">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-297">P1</span><span class="sxs-lookup"><span data-stu-id="35734-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-298">Toutes les tâches du projet ou vides</span><span class="sxs-lookup"><span data-stu-id="35734-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-299">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-300">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-301">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="35734-302">Valide</span><span class="sxs-lookup"><span data-stu-id="35734-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-303">Basé sur la règle n° 5, Q1 et Q2 sont deux citations sur la même opportunité, de sorte qu’ils peuvent tous les deux estimer pour les mêmes composants d’un projet.</span><span class="sxs-lookup"><span data-stu-id="35734-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-304">O1</span><span class="sxs-lookup"><span data-stu-id="35734-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-305">Q2</span><span class="sxs-lookup"><span data-stu-id="35734-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-306">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-307">P1</span><span class="sxs-lookup"><span data-stu-id="35734-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-308">Toutes les tâches du projet ou vides</span><span class="sxs-lookup"><span data-stu-id="35734-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-309">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-310">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-311">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-311">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-312">O1</span><span class="sxs-lookup"><span data-stu-id="35734-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-313">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-314">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-315">P1</span><span class="sxs-lookup"><span data-stu-id="35734-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-316">Toutes les tâches du projet ou vides</span><span class="sxs-lookup"><span data-stu-id="35734-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-317">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-318">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-319">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="35734-320">Valide</span><span class="sxs-lookup"><span data-stu-id="35734-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="35734-321">Basé sur la règle n° 4, Q1 et Q2 sont deux citations sur différentes opportunités, de sorte qu’ils peuvent tous les deux estimer pour les mêmes composants d’un même projet.</span><span class="sxs-lookup"><span data-stu-id="35734-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="35734-322">O2</span><span class="sxs-lookup"><span data-stu-id="35734-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="35734-323">Q1</span><span class="sxs-lookup"><span data-stu-id="35734-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-324">QL1</span><span class="sxs-lookup"><span data-stu-id="35734-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-325">P1</span><span class="sxs-lookup"><span data-stu-id="35734-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="35734-326">Toutes les tâches du projet ou vides</span><span class="sxs-lookup"><span data-stu-id="35734-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-327">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="35734-328">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="35734-329">Oui</span><span class="sxs-lookup"><span data-stu-id="35734-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="35734-330">Non valide</span><span class="sxs-lookup"><span data-stu-id="35734-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>
