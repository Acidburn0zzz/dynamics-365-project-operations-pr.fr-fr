---
title: Mettre à jour un projet
description: Cette rubrique offre des informations sur la mise à jour des projets dans Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 5c9cd0c7c6886bd454c5f2ef2ae7f20d1707293f
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/16/2020
ms.locfileid: "4075595"
---
# <a name="update-a-project"></a><span data-ttu-id="b4ee3-103">Mettre à jour un projet</span><span class="sxs-lookup"><span data-stu-id="b4ee3-103">Update a project</span></span>

<span data-ttu-id="b4ee3-104">_**S’applique à :** Project Operations pour les scénarios basés sur les ressources/produits non stockés Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="b4ee3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b4ee3-105">Vous trouverez ci-dessous un résumé des champs qui peuvent être mis à jour sur un projet après sa création et toutes les implications applicables des mises à jour.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="b4ee3-106">Champs de détail du projet</span><span class="sxs-lookup"><span data-stu-id="b4ee3-106">Project detail fields</span></span>

- <span data-ttu-id="b4ee3-107">**Nom**  : Titre du projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-107">**Name** : The title of the project.</span></span>
- <span data-ttu-id="b4ee3-108">**Description**  : Vue d’ensemble du projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-108">**Description** : An overview of the project.</span></span>
- <span data-ttu-id="b4ee3-109">**Client**  : L’entreprise à laquelle le projet sera fourni.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-109">**Customer** : The company the project will be delivered to.</span></span>
- <span data-ttu-id="b4ee3-110">**Modèle de calendrier**  : Heures de travail du projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-110">**Calendar template** : The working hours of the project.</span></span> <span data-ttu-id="b4ee3-111">Lorsque le champ est modifié, la planification entière est recalculée.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="b4ee3-112">**Devise**  : Devise du projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-112">**Currency** : The currency for the project.</span></span> <span data-ttu-id="b4ee3-113">Ce champ est par défaut basé sur la devise définie dans l’unité contractuelle.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="b4ee3-114">Lorsque l’unité contractuelle est mise à jour, le champ est également mis à jour.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="b4ee3-115">**Unité contractuelle**  : Unité d’organisation qui représente le groupe de sociétés ou la division principalement responsables de remporter la vente et de gérer la prestation du travail et des services au client.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-115">**Contracting Unit** : The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="b4ee3-116">**Gestionnaire de projet**  : Membre de l’équipe de projet qui a le pouvoir d’examiner et d’approuver les entrées de temps et les dépenses.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-116">**Project Manager** : The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="b4ee3-117">Champs d’estimation</span><span class="sxs-lookup"><span data-stu-id="b4ee3-117">Estimate fields</span></span>

- <span data-ttu-id="b4ee3-118">**Date de début estimée**  : Date à laquelle le projet commencera.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-118">**Estimated Start Date** : The date that the project will begin.</span></span> <span data-ttu-id="b4ee3-119">Lorsque ce champ est mis à jour, toutes les tâches du projet seront déplacées proportionnellement à la nouvelle date de début.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="b4ee3-120">**Date de fin**  : Date à laquelle le projet doit se terminer.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-120">**Finish Date** : The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="b4ee3-121">**Effort**  : Effort estimé du projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-121">**Effort** : The estimated effort of the project.</span></span> <span data-ttu-id="b4ee3-122">Lorsque des tâches sont ajoutées au projet, ce champ n’est plus modifiable.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="b4ee3-123">**Coût estimé de la main-d’œuvre**  : Coût estimé de la main-d’œuvre du projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-123">**Estimated Labor Cost** : The estimated labor cost of the project.</span></span> <span data-ttu-id="b4ee3-124">Lorsque des coûts de main-d’œuvre sont ajoutés au projet, ce champ n’est plus modifiable.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="b4ee3-125">**Dépenses estimées**  : Dépenses estimées du projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-125">**Estimated Expenses** : The estimated expenses of the project.</span></span> <span data-ttu-id="b4ee3-126">Lorsque des dépenses sont ajoutées au projet, ce champ n’est plus modifiable.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="b4ee3-127">Champs des chiffres réels du projet</span><span class="sxs-lookup"><span data-stu-id="b4ee3-127">Project actual fields</span></span>
- <span data-ttu-id="b4ee3-128">**Début réel**  : Date à laquelle le projet a commencé.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-128">**Actual Start** : The date that the project started.</span></span>
- <span data-ttu-id="b4ee3-129">**Fin réelle**  : À mettre à jour lorsqu’un projet est terminé.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-129">**Actual Finish** : To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="b4ee3-130">Champs de statut du projet</span><span class="sxs-lookup"><span data-stu-id="b4ee3-130">Project status fields</span></span>

- <span data-ttu-id="b4ee3-131">**Statut général du projet**  : Intégrité globale du projet fournie par le chef de projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-131">**Overall Project Status** : The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="b4ee3-132">**Commentaires**  : Récit concernant l’intégrité actuelle du projet fourni par le chef de projet.</span><span class="sxs-lookup"><span data-stu-id="b4ee3-132">**Comments** : A narrative regarding the current health of the project provided by the Project manager.</span></span>
