---
title: Définir les calendriers de ressources
description: Cette rubrique fournit des informations sur la définition des calendriers d’heures de travail pour les ressources dans Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ab39d7e5dc2d8c01ed49ca0f1a4d1691aaf15637
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4075588"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="c1eed-103">Définir les calendriers de ressources</span><span class="sxs-lookup"><span data-stu-id="c1eed-103">Define resource calendars</span></span>

<span data-ttu-id="c1eed-104">_**S’applique à :** Project Operations pour les scénarios basés sur les ressources/produits non stockés Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="c1eed-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c1eed-105">Chaque ressource réservable travaillant sur un projet doit disposer d’un calendrier d’heures de travail pour définir sa disponibilité.</span><span class="sxs-lookup"><span data-stu-id="c1eed-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="c1eed-106">Les heures de travail d’une ressource peuvent être définies de deux manières :</span><span class="sxs-lookup"><span data-stu-id="c1eed-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="c1eed-107">Définir des règles de calendrier individuelles pour une ressource</span><span class="sxs-lookup"><span data-stu-id="c1eed-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="c1eed-108">Appliquer un modèle de calendrier existant pour la ressource</span><span class="sxs-lookup"><span data-stu-id="c1eed-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="c1eed-109">Définir les heures de travail d’une ressource</span><span class="sxs-lookup"><span data-stu-id="c1eed-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="c1eed-110">Sur le menu **Ressources** , sélectionnez **Ressources**.</span><span class="sxs-lookup"><span data-stu-id="c1eed-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="c1eed-111">Dans la vue de la grille, sélectionnez la **Ressource réservable** applicable.</span><span class="sxs-lookup"><span data-stu-id="c1eed-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="c1eed-112">Sur la page **Détails de la ressource** , sélectionnez l’onglet **Heures d’ouverture**. Par défaut, le calendrier des ressources réservables utilise par défaut les heures de travail du modèle d’heures de travail par défaut défini pour l’organisation.</span><span class="sxs-lookup"><span data-stu-id="c1eed-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="c1eed-113">Pour mettre à jour les heures de travail, cliquez avec le bouton droit sur la date de début de la règle de calendrier proposée à définir.</span><span class="sxs-lookup"><span data-stu-id="c1eed-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="c1eed-114">Utilisez le menu des règles de calendrier pour définir une règle de calendrier pour un jour spécifique, le reste de la série ou le calendrier entier.</span><span class="sxs-lookup"><span data-stu-id="c1eed-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="c1eed-115">Une fois l’option sélectionnée, vous pouvez définir :</span><span class="sxs-lookup"><span data-stu-id="c1eed-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="c1eed-116">Le jour de la semaine où les heures de travail s’appliqueront.</span><span class="sxs-lookup"><span data-stu-id="c1eed-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="c1eed-117">Les temps de travail dans chaque jour.</span><span class="sxs-lookup"><span data-stu-id="c1eed-117">The working times within each day.</span></span>
    - <span data-ttu-id="c1eed-118">Fuseau horaire local de la règle de calendrier.</span><span class="sxs-lookup"><span data-stu-id="c1eed-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="c1eed-119">Le cas échéant, le temps non travaillé peut également être spécifié pour la règle.</span><span class="sxs-lookup"><span data-stu-id="c1eed-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="c1eed-120">Application d’un modèle de calendrier à une ressource</span><span class="sxs-lookup"><span data-stu-id="c1eed-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="c1eed-121">Sur le menu **Ressources** , sélectionnez **Ressources**.</span><span class="sxs-lookup"><span data-stu-id="c1eed-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="c1eed-122">Dans la vue en grille, sélectionnez jusqu’à 25 **Ressources réservables** à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="c1eed-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="c1eed-123">Sélectionnez **Définir le calendrier** et une boîte de dialogue vous proposera une liste des modèles d’heures de travail disponibles.</span><span class="sxs-lookup"><span data-stu-id="c1eed-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="c1eed-124">Sélectionnez le modèle à utiliser, puis sélectionnez **Appliquer**.</span><span class="sxs-lookup"><span data-stu-id="c1eed-124">Select the template you want to use, and then select **Apply**.</span></span>