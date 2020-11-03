---
title: Champs de Project Operations en tant que dimensions de tarification
description: Cette rubrique fournit des informations sur l'utilisation des champs en tant que dimensions de tarification dans Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 56ff45169058d96d7ef81a710de309eec698a75f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4075803"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="e9999-103">Champs de Project Operations en tant que dimensions de tarification</span><span class="sxs-lookup"><span data-stu-id="e9999-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="e9999-104">_**S'applique à :** Project Operations pour les scénarios basés sur les ressources/produits non stockés Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="e9999-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e9999-105">L'entité **Chiffres réels** comporte de nombreux champs qui peuvent être utilisés comme dimensions de tarification pour la tarification basée sur les ressources.</span><span class="sxs-lookup"><span data-stu-id="e9999-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="e9999-106">Par exemple, un champ courant est **Ressource réservable**.</span><span class="sxs-lookup"><span data-stu-id="e9999-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="e9999-107">Les petites entreprises qui ont moins de 20 à 30 ressources facturables peuvent estimer qu'il est plus simple d'avoir des taux de facturation et de coût spécifiques à chaque ressource.</span><span class="sxs-lookup"><span data-stu-id="e9999-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="e9999-108">Toutefois, avec l'augmentation de la main d'œuvre facturable, la mise à jour des taux spécifiques aux ressources peut devenir beaucoup trop complexe.</span><span class="sxs-lookup"><span data-stu-id="e9999-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="e9999-109">Le coût des ressources et les taux de facturation commencent à varier à mesure que les ressources sont promues, acquièrent plus d'expérience ou acquièrent un ensemble différent de compétences.</span><span class="sxs-lookup"><span data-stu-id="e9999-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="e9999-110">Un autre exemple est le champ Catégorie de transaction.</span><span class="sxs-lookup"><span data-stu-id="e9999-110">Another example is that of transaction category.</span></span> <span data-ttu-id="e9999-111">Les clients et les responsables de l'implémentation utilisent la catégorie de transaction pour classer le travail et utilisent le champ pour évaluer le prix et le coût selon la catégorie de travail.</span><span class="sxs-lookup"><span data-stu-id="e9999-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>