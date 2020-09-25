---
title: Nouveautés de la mise à jour (version 12) de Project Service Automation, V3
description: Cette rubrique donne des informations sur les nouveautés de la mise à jour (version 12) de Project Service Automation, V3.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: af8dbfe3-7ce9-4374-9c03-17b2e1d6ac32
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 758717562c12a72848f1a874fa8b1171139ebb0c
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "3168049"
---
# <a name="project-service-automation-v3-update-release-12"></a>Mise à jour (version 12) de Project Service Automation, V3
Nous sommes heureux d'annoncer la dernière mise à jour de l'application Dynamics 365 Project Service Automation (PSA). Cette version comprend des améliorations importantes de la qualité, des performances et de l'utilisation. Cette version est compatible avec Dynamics 365 9.x. Pour effectuer une mise à jour vers cette version, visitez le centre d'administration de Dynamics 365 Online et accédez à la page des solutions pour installer la mise à jour. Pour plus d'informations, voir [Installer, mettre à jour ou supprimer une solution par défaut](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

Cette rubrique répertorie les fonctionnalités et les correctifs nouveaux ou modifiés pour la mise à jour (version 12) de Project Service Automation V3. Cette version a le numéro de build V3.10.2.34 et est généralement disponible par mise à jour automatique en octobre 2019.

## <a name="update-release-12"></a>Mise à jour (version 12)

### <a name="bug-fixes"></a>Correctifs de bogues

- Temps et dépenses

    - Correction : les messages d'erreur d'entrée de temps ont été mis à jour avec un contexte plus pertinent.
    - Correction : la grille d'entrée de temps et le planning affichent correctement la barre de défilement verticale lorsque cela est nécessaire.
    - Correction : les entrées de dépenses et de temps envoyées peuvent être approuvées.
    - Correction : le message de la boîte de dialogue de confirmation de l'annulation de l'approbation a été corrigé pour refléter le statut de l'approbation lorsqu'il passe de **Approuvé** à **Envoyé**.
    - Correction : les champs **Prix**, **Unité** et **Quantité** sont désormais verrouillés sur l'enregistrement de dépenses une fois qu'il a été approuvé.

- Gestion du projet

    - Correction : l'action **Nouveau** sur le formulaire principal **Membre de l'équipe** a été supprimé.
    - Correction : les affectations de ressources ont été mises à jour pour tenir compte des erreurs d'arrondi inexact, qui entraînent un changement dans la date de fin d'une tâche.
    - Correction : dans la grille des tâches, les erreurs côté serveur pertinentes seront signalées à l'utilisateur.
    - Correction : le nom du membre de l'équipe s'affiche désormais dans le sélecteur de personnes au lieu du nom du poste.

- Gestion des ressources

    - Correction : les détails des ressources requises pour les projets créés à partir d'un modèle utilisent désormais le calendrier du projet.
    - Correction : les qualifications et les compétences affichent désormais par défaut les ressources requises créées pour le rôle au lieu des données de référence du rôle.

- Ventes

    - Correction : ID d'objet en double trouvés sur le formulaire principal **Contrat**.
    - Correction : la logique a été mise à jour pour rendre l'onglet **Analyse du devis** visible afin d'afficher la configuration des métadonnées de l'onglet.
    - Correction : la date comptable de l'enregistrement réel provient désormais de la date de l'entrée de temps/dépenses au lieu de la date de l'approbation.