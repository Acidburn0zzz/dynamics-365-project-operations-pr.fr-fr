---
title: Mettre à niveau la page d'accueil
description: Cette rubrique décrit où trouver des informations importantes concernant les fonctionnalités nouvelles et modifiées dans Dynamics 365 Project Service Automation, ainsi que le processus de mise à niveau vers la nouvelle version.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 for Project Service 3.x
author: rumant
ms.assetid: c92d0849-e40c-4a56-9719-34030fbf5991
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 55f544636f39fc4faae06fdd512f859800bb7b44
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3168087"
---
# <a name="upgrade-home-page"></a>Mettre à niveau la page d'accueil

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a>Mise à niveau de PSA version 2.x ou 1.x vers la version 3.x

### <a name="new-instances"></a>Nouvelles instances

À compter du 17 mai 2019, lorsque Project Service Automation est sélectionnée pendant la mise en service d'une nouvelle instance, la version 3.x est installée par défaut.

### <a name="existing-instances"></a>Instances existantes

Précédemment, les clients qui disposaient d'une instance de PSA version 2.x et qui devaient effectuer une mise à niveau vers la version 3.x, qui est la version basée sur l'interface Unified Client (UCI) de PSA, devaient contacter le support et fournir les détails de leur instance, afin que le support puisse activer l'instance pour la mise à niveau vers la version 3.x. À compter du 1er mars 2020, les clients qui ont une instance de PSA version 2.x et qui doivent effectuer une mise à niveau vers la version 3.x, pourront mettre à niveau leurs instances directement depuis le portail d'administration sans avoir à contacter le support Microsoft.  

> [!NOTE]
> PSA version 3.x comprend des modifications importantes. Elle est bâtie sur la structure Unified Interface pour offrir une expérience utilisateur améliorée. L'application modifiée offre une interface utilisateur cohérente et uniforme et elle applique les principes de conception réactive pour un affichage optimal sur n'importe quelle taille d'écran ou n'importe quel appareil. D'autres modifications ont été apportées dans l'application. Parmi les zones qui ont été modifiées, on peut citer la tarification, la réservation et l'affectation de ressources, le temps, les dépenses et les approbations.

Avant de commencer le processus de mise à niveau, nous vous recommandons d'effectuer les tâches suivantes :

- Vérifiez si Dynamics 365 Field Service et Project Service Automation sont installées sur l'instance identifiée. Si les deux solutions sont installées, vous devez prévoir de les mettre à niveau toutes les deux avant de recommencer à utiliser normalement l'instance.
- Examinez attentivement les rubriques suivantes. Prendre connaissance et comprendre les modifications entre les versions vous aideront dans le processus de mise à niveau. Ces rubriques donnent des informations sur les modifications majeures dans PSA, ainsi que les considérations et les recommandations pour la planification de votre mise à niveau vers la version 3.x.

    - [Nouveautés ou modifications dans Project Service Automation version 3](whats-new-changed-v3.md)
    - [Considérations relatives à la mise à niveau - Project Service Automation version 2.x ou 1.x vers la version 3.x](upgrade-v3.md)

- Mettez à niveau votre instance sandbox pour évaluer les modifications de votre implémentation avant de mettre à niveau votre instance de production.

Une fois que vous avez examiné les rubriques précédemment mentionnées et que vous êtes prêt à effectuer une mise à niveau vers PSA version 3.x ou la version basée sur UCI, envoyez une demande au Support Microsoft pour rendre la mise à niveau accessible à partir du Centre d'administration. Dans votre demande, fournissez les détails de votre instance.

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a>Anciennes versions de PSA (PSA version 2.x) dans une nouvelle instance créée

À compter du 17 mai 2019, toutes les nouvelles instances ont UCI comme client par défaut. Afin de s'aligner sur cette modification, PSA version 3.x and Field Service version 8.x seront mises en service par défaut, car ces versions sont conçues pour fonctionner avec le client UCI.

À partir du 1er mars 2020, les clients de Dynamics PSA ne pourront plus créer de nouveaux environnements avec des versions plus anciennes de PSA, par exemple PSA version 2.x ou inférieure. Tout nouvel environnement devra obtenir uniquement la version 3.x de PSA.

> [!NOTE]
> Pour optimiser l'expérience lorsque vous utilisez les anciennes versions des applications Field Service et PSA, accédez à la page **Paramètres système** et pour le champ, **Utiliser uniquement la nouvelle Unified Interface (recommandé)**, sélectionnez **Non**, car ces versions ne sont pas conçues pour être chargées correctement dans UCI. Après avoir désactivé UCI, vous pouvez ouvrir et exécuter ces versions de Field Service et de PSA en utilisant l'ancien client Web. Pour savoir comment désactiver le client UCI, consultez [Activer Unified Interface uniquement](../admin/enable-unified-interface-only.md).