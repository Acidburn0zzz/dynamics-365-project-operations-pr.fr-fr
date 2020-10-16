---
title: Définir des calendriers de projet
description: Cette rubrique fournit des informations sur l'utilisation d'un calendrier pour suivre l'avancée d'un projet.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1d44a2d0d8c13fb9e93b9a6da15fb3a7ce8d764c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897988"
---
# <a name="define-project-calendars"></a><span data-ttu-id="df5e3-103">Définir des calendriers de projet</span><span class="sxs-lookup"><span data-stu-id="df5e3-103">Define project calendars</span></span>

<span data-ttu-id="df5e3-104">_**S'applique à :** Project Operations pour les scénarios basés sur les ressources/produits non stockés Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="df5e3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="df5e3-105">Pour créer une planification de projet, créez un modèle de calendrier de projet qui définit le nombre d'heures de travail par jour et les heures de fermeture.</span><span class="sxs-lookup"><span data-stu-id="df5e3-105">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="df5e3-106">Pour créer un modèle de calendrier de projet, vous associez un modèle de travail au champ **Modèle de calendrier** du projet.</span><span class="sxs-lookup"><span data-stu-id="df5e3-106">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="df5e3-107">Pour créer un modèle de travail, procédez comme suit.</span><span class="sxs-lookup"><span data-stu-id="df5e3-107">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="df5e3-108">Sélectionnez **Ressources** dans le volet de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="df5e3-108">In the left navigation pane, select **Resources**.</span></span> 
2. <span data-ttu-id="df5e3-109">Sur la page de liste **Ressources**, ouvrez enregistrement utilisateur, puis sélectionnez **Afficher les heures de travail**.</span><span class="sxs-lookup"><span data-stu-id="df5e3-109">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="df5e3-110">Vérifiez que vous autorisez les fenêtres contextuelles sur la page de navigateur.</span><span class="sxs-lookup"><span data-stu-id="df5e3-110">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="df5e3-111">Cela vous permet de voir les heures de travail définies pour la ressource.</span><span class="sxs-lookup"><span data-stu-id="df5e3-111">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="df5e3-112">Dans l'onglet **Vue mensuelle**, cliquez sur **Configuration**.</span><span class="sxs-lookup"><span data-stu-id="df5e3-112">On the **Monthly View** tab, select **Set Up**.</span></span> <span data-ttu-id="df5e3-113">Une liste de trois options apparaît :</span><span class="sxs-lookup"><span data-stu-id="df5e3-113">A list of three options appears:</span></span> 

  - <span data-ttu-id="df5e3-114">Nouvelle planification hebdomadaire</span><span class="sxs-lookup"><span data-stu-id="df5e3-114">New Weekly Schedule</span></span>
  - <span data-ttu-id="df5e3-115">Planification des tâches sur un jour</span><span class="sxs-lookup"><span data-stu-id="df5e3-115">Work Schedule for One Day</span></span>
  - <span data-ttu-id="df5e3-116">Absence</span><span class="sxs-lookup"><span data-stu-id="df5e3-116">Time Off</span></span>

4. <span data-ttu-id="df5e3-117">Sélectionnez **Nouvelle planification hebdomadaire**, puis définissez les options de cette planification de ressource.</span><span class="sxs-lookup"><span data-stu-id="df5e3-117">Select **New Weekly Schedule**, and then set the options for this resource schedule.</span></span> <span data-ttu-id="df5e3-118">Vous pouvez définir une planification hebdomadaire récurrente, des paramètres d'heure quotidiens, des fermetures de bureaux, et plus encore.</span><span class="sxs-lookup"><span data-stu-id="df5e3-118">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="df5e3-119">Définissez la plage de dates, la sélectionnez **Enregistrer**, puis cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="df5e3-119">Set the date range, select **Save**, and then select **Close**.</span></span> 
6. <span data-ttu-id="df5e3-120">Revenez à la page de liste **Ressources**, puis sélectionnez la ressource pour laquelle vous avez défini les heures de travail.</span><span class="sxs-lookup"><span data-stu-id="df5e3-120">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="df5e3-121">Sélectionnez **Définir le calendrier comme** pour définir le modèle de travail.</span><span class="sxs-lookup"><span data-stu-id="df5e3-121">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="df5e3-122">Dans la boîte de dialogue **Modèle de travail**, entrez le nom pour le modèle de travail, puis sélectionnez **Appliquer**.</span><span class="sxs-lookup"><span data-stu-id="df5e3-122">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="df5e3-123">Vous pouvez désormais associer le modèle de travail à un modèle de calendrier de projet.</span><span class="sxs-lookup"><span data-stu-id="df5e3-123">You can now associate the work template with a project calendar template.</span></span>