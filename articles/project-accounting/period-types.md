---
title: Types de période
description: Cette rubrique fournit des informations sur la manière de configurer des types de période pour une estimation de revenus.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6bcd988fbd074c66d64f7e327b4329d3de27e950
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531419"
---
# <a name="period-types"></a>Types de période

_**S’applique à :** Project Operations pour les scénarios selon les ressources/produits non stockés_

Un type de période définit la fréquence à laquelle les revenus d'un projet sont estimés. Cette rubrique fournit des informations sur la manière de configurer des types de période pour une estimation de revenus. 

## <a name="create-and-work-with-period-types"></a>Créer et utiliser des types de période
Pour créer et utiliser des types de période, procédez comme suit :

1. Dans votre environnement Dynamics 365 Finance, accédez à **Gestion et comptabilité des projets** > **Configurer** > **Estimations** > **Types de période**.
2. Sélectionnez **Nouveau** pour créer un nouveau type de période. Entrez un nom et une description.
3. Dans le champ **Fréquence**, sélectionnez une valeur :

    - Si vous sélectionnez **Semaine**, **Bihebdomadaire**, **Semi-mensuelle**, **Mois**, **Jour**, **Trimestre** ou **Année**, le calendrier sera utilisé pour générer les périodes. 
    - Si vous sélectionnez **Période comptable**, les périodes comptables de la configuration de comptabilité seront utilisées pour générer des périodes.
    - Si vous sélectionnez **Illimité**, vous pouvez spécifier des périodes personnalisées.
4. Sélectionnez l'enregistrement de type de période, puis sélectionnez **Générer des périodes** pour créer des périodes pour le type de période. En fonction de la fréquence de période que vous avez sélectionnée, vous avez la possibilité de spécifier une date de début ou le nombre de périodes à générer.
5. Sélectionnez **Périodes** pour revoir les périodes générées.
