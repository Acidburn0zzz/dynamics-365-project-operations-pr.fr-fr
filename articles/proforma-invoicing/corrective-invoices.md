---
title: Correction de factures
description: Cette rubrique fournit des informations sur la correction de factures.
author: rumant
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e14da1c07d5b697de6caf1b9041c30581ecff102
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898078"
---
# <a name="corrected-invoices"></a><span data-ttu-id="24ecd-103">Correction de factures</span><span class="sxs-lookup"><span data-stu-id="24ecd-103">Corrected invoices</span></span>

<span data-ttu-id="24ecd-104">_**S'applique à :** Project Operations pour les scénarios basés sur les ressources/produits non stockés Déploiement simplifié – Traiter la facturation pro forma_</span><span class="sxs-lookup"><span data-stu-id="24ecd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="24ecd-105">Les factures confirmées peuvent être modifiées.</span><span class="sxs-lookup"><span data-stu-id="24ecd-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="24ecd-106">Lorsque vous modifiez une facture confirmée, un brouillon de la facture corrigée est créé.</span><span class="sxs-lookup"><span data-stu-id="24ecd-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="24ecd-107">Comme la supposition est que vous souhaitez contrepasser toutes les transactions et quantités de la facture d'origine, cette facture corrigée inclut toutes les transactions de la facture d'origine, et toutes les quantités sont de zéro (0).</span><span class="sxs-lookup"><span data-stu-id="24ecd-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="24ecd-108">Si aucune transaction ne nécessite de correction, vous pouvez la supprimer du brouillon de facture corrective.</span><span class="sxs-lookup"><span data-stu-id="24ecd-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="24ecd-109">Pour contrepasser ou ne retourner qu'une quantité partielle, vous pouvez modifier le champ Quantité sur le détail de la ligne.</span><span class="sxs-lookup"><span data-stu-id="24ecd-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="24ecd-110">Si vous ouvrez le détail de ligne de facture, la quantité de la facture d'origine s'affiche.</span><span class="sxs-lookup"><span data-stu-id="24ecd-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="24ecd-111">Vous pouvez ensuite modifier la quantité actuelle de la facture afin qu'elle soit inférieure ou supérieure à la quantité de la facture d'origine.</span><span class="sxs-lookup"><span data-stu-id="24ecd-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="24ecd-112">Lorsque vous confirmez une facture corrective, le chiffre réel facturé d'origine est contrepassé et un chiffre réel de ventes facturées est créé.</span><span class="sxs-lookup"><span data-stu-id="24ecd-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="24ecd-113">Si la quantité a été réduite, la différence aura pour effet la création d'un chiffre réel de ventes non facturées.</span><span class="sxs-lookup"><span data-stu-id="24ecd-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="24ecd-114">Par exemple, si la vente facturée d'origine était de huit heures, et que le détail de la ligne de facture corrigée dispose d'une quantité réduite de six heures, la ligne de vente facturée d'origine est contrepassée et deux chiffres réels sont créés :</span><span class="sxs-lookup"><span data-stu-id="24ecd-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="24ecd-115">Un chiffre réel de vente facturée de six heures.</span><span class="sxs-lookup"><span data-stu-id="24ecd-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="24ecd-116">Un chiffre réel de ventes non facturées de deux heures restantes.</span><span class="sxs-lookup"><span data-stu-id="24ecd-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="24ecd-117">Cette transaction peut être facturée ultérieurement ou marquée comme non facturable, selon les négociations avec le client.</span><span class="sxs-lookup"><span data-stu-id="24ecd-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>