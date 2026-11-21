# LUMEN — Réunion de découverte du besoin d’intégration Peppol

**Date :** 4 novembre 2026. **Durée :** environ 35 minutes.

Cette réunion a lieu après l’arrêté de la documentation LUMEN au 27 octobre 2026 : ce qui s’y dit est nouveau et ne figure pas dans la documentation.

## Participants

| Personne | Rôle |
|---|---|
| **Claire Masson** | Product Owner, responsable administration |
| **Hugo Laurent** | Référent facturation ventes |
| **Sarah Dubois** | Gestionnaire achats |
| **Eva Leclerc** | Tech Lead |

---

## 00:00–02:30 — Pourquoi cette réunion ?

**Claire :** Bon, merci d’avoir trouvé un créneau. On s’est donné trente-cinq minutes. L’idée aujourd’hui, c’est de mettre des mots sur la demande : on veut intégrer Peppol à LUMEN. Jusqu’ici, on a surtout dit cette phrase en comité. Mais entre ce que chacun imagine derrière, je pense qu’il y a un peu de distance.

**Hugo :** Oui, moi, quand j’entends intégrer, je pense surtout arrêter de jongler. Je prépare ma facture dans LUMEN, et je voudrais pouvoir aller jusqu’au bout sans me demander dans quel outil je dois la retrouver ensuite. Mais je ne sais pas ce qu’on met exactement dans le premier morceau.

**Sarah :** Et moi, spontanément, je pense aux factures qu’on reçoit. Si on parle seulement de l’envoi, je préfère qu’on le dise tout de suite. Parce que sinon on va annoncer aux achats que leurs documents vont arriver dans LUMEN, et trois mois après on découvrira que personne n’avait prévu notre partie.

**Eva :** C’est justement la question. On n’a encore choisi ni service externe ni mode de connexion. Je peux expliquer ce que LUMEN fait aujourd’hui, mais je ne veux pas dessiner une interface sur la base d’une phrase. Qu’est-ce qu’on veut améliorer, et pour qui ?

**Claire :** Pour moi, c’est d’abord garder une maîtrise commune. Aujourd’hui, on sait préparer, finaliser, envoyer par email et conserver les pièces. Ce qu’on veut, c’est étendre ce fonctionnement aux échanges via Peppol sans créer un deuxième suivi parallèle. Et comprendre aussi ce que ça implique pour les achats.

**Sarah :** D’accord. Donc ce n’est pas simplement ajouter un bouton sur une facture.

**Claire :** Voilà. Et ce n’est pas non plus une réunion où l’on doit sortir avec toutes les décisions prises. Je voudrais qu’on distingue ce qu’on sait déjà, ce qu’on souhaite et ce qu’il faut aller demander. Benoît et Amélie ne sont pas là ; on ne répondra pas à leur place.

**Hugo :** Très bien. Je vous propose qu’on parte d’une facture réelle dans notre manière de travailler. Enfin, d’un exemple, sans les coordonnées du client. C’est plus facile pour moi que de commencer par les grands principes.

## 02:30–05:00 — Le travail actuel côté ventes

**Hugo :** Je prends Atelier Vermeil. Deux journées de conseil à cinq cents euros hors TVA. Je crée le brouillon, je vérifie les prestations, l’adresse et l’échéance. J’ai mille deux cent dix euros au total. Quand je finalise, LUMEN attribue le numéro et prépare le PDF. Ensuite, je fais une action séparée pour l’envoyer par email. Ce n’est pas la finalisation qui l’envoie.

**Eva :** Oui. Et si le PDF n’est pas encore disponible, l’envoi reste bloqué. Le numéro, lui, existe déjà. C’est important pour la suite : un problème d’envoi ne nous permet pas de repartir de zéro avec la même facture modifiée.

**Claire :** Où est-ce que tu perds du temps, aujourd’hui ? Dans l’envoi lui-même ou dans ce qui vient après ?

**Hugo :** Les deux, mais surtout après. Quelqu’un me dit : « Je ne l’ai pas reçue. » Je vérifie l’email, la bonne adresse, la tentative. Puis je renvoie, et parfois un collègue a déjà répondu entre-temps. LUMEN garde des traces, heureusement, mais on passe encore par la boîte de facturation pour comprendre la demande du client.

**Sarah :** Et quand ils disent ne pas avoir reçu, ça peut vouloir dire que la facture est arrivée chez la mauvaise personne. Ce n’est pas forcément un problème technique.

**Hugo :** Exactement. Ou alors elle est arrivée, mais il manque leur référence de commande et leur service comptable la refuse. Pour nous, l’email est parti. Pour eux, le dossier n’est pas traitable. J’aimerais éviter qu’avec Peppol on affiche un gros « réussi » qui nous fasse croire que tout est réglé.

**Eva :** Donc il faudra pouvoir distinguer l’envoi technique, les éventuels retours qu’on reçoit et le traitement commercial chez le client. On ne sait pas encore quels retours seront effectivement disponibles.

**Claire :** Oui. Et le paiement reste une autre chose. On ne veut pas qu’une transmission réussie fasse passer une facture à payée. Ça paraît évident quand on le dit, mais il faut garder cette séparation dans les écrans.

**Hugo :** Tout à fait. Ce que je voudrais voir rapidement, c’est : est-ce que j’ai encore quelque chose à faire ? Pas forcément lire un historique technique de quinze lignes.

## 05:00–07:30 — Qui est concerné et jusqu’où aller ?

**Claire :** Les volumes de départ du projet étaient autour de cent quatre-vingts factures de vente et quatre-vingt-quinze documents fournisseurs par mois. Ce ne sont pas des volumes Peppol. Il faut reprendre un échantillon récent avant de dire quelle part serait concernée.

**Hugo :** La majorité de mes factures, ce sont des entreprises belges, mais j’ai aussi des particuliers pour certaines formations. Et quelques entreprises qui ont une adresse de facturation différente du contact commercial. Je ne peux pas vous donner un pourcentage fiable ici.

**Sarah :** Aux achats, c’est encore autre chose. Certaines factures arrivent par email, d’autres sont déposées par les collègues. On a aussi des tickets et des scans. Même si on ajoute un nouveau canal, tout ça ne va pas disparaître du jour au lendemain.

**Eva :** Est-ce que vous attendez un choix de canal sur chaque document, ou quelque chose qui découle de la situation du client ? Je ne vous demande pas encore de trancher. Je veux comprendre si Hugo doit décider à chaque fois.

**Hugo :** Si je dois refaire une recherche pour chaque facture du même client, je ne vais pas gagner grand-chose. J’aimerais que LUMEN m’aide. Mais je ne veux pas qu’un canal soit choisi automatiquement sur une information qu’on a vérifiée il y a six mois et qui n’est plus correcte.

**Claire :** Et sur les obligations, on fait attention. On a des contraintes à respecter dans nos échanges, mais je ne vais pas improviser leur interprétation juridique. Benoît doit nous dire précisément quelles populations et quels documents sont concernés. Le logiciel ne doit pas transformer une préférence de l’utilisateur en autorisation de contourner une obligation.

**Eva :** D’accord. Je séparerais donc le périmètre commercial actuel, les cas concernés par l’intégration et les exceptions à faire confirmer. Pour l’instant, personne ici ne peut dire « toutes les factures » et considérer la discussion terminée.

**Sarah :** Ni « tous les documents fournisseurs ». Un ticket de parking et une facture de maintenance, ce n’est pas la même chose.

**Hugo :** Et les notes de crédit, on les met bien dans la discussion ? Sinon on sait envoyer la facture mais pas la correction.

**Claire :** Oui, on doit étudier les notes de crédit avec les factures. Ça ne veut pas dire qu’on a déjà arrêté tous leurs cas particuliers.

## 07:30–10:00 — Identités, données et choix du service externe

**Eva :** Avant même l’envoi, il faudra savoir comment notre entreprise est reconnue et comment on identifie le destinataire. Dans LUMEN, on a la société, les clients, les fournisseurs et leurs données légales. Est-ce qu’on sait aujourd’hui qui contrôle ces données quand un nouveau client est créé ?

**Hugo :** Nous, à la facturation. On reprend les informations de la commande et on fait nos vérifications. Mais le contact commercial, l’adresse email et l’identité de la société sont parfois mélangés dans la demande qu’on reçoit. Le commercial m’envoie « facturer le groupe », sans préciser l’entité.

**Sarah :** Même problème côté fournisseur. Le nom sur le bon de commande peut être une enseigne, et sur la facture on retrouve une autre raison sociale. On ne peut pas rapprocher seulement parce que le nom ressemble.

**Claire :** Je veux éviter qu’on crée un nouveau référentiel à côté des tiers existants. Si une donnée manque ou pose problème, il faut qu’on sache quelle fiche corriger et qui a le droit de le faire.

**Eva :** Oui, mais je ne sais pas encore si les champs actuels suffiront. Il faudra vérifier les identifiants attendus avec le service qu’on retiendra. Et je préfère éviter qu’on ajoute des champs obligatoires à tous les clients avant d’avoir compris à quoi ils servent.

**Hugo :** Sur la recherche du destinataire, je verrais bien une aide dans la fiche client. Mais si quelqu’un ouvre la fiche et que le partenaire ne répond pas, ça ne doit pas m’empêcher de consulter les factures déjà faites.

**Eva :** Bonne distinction. Consultation et contrôle en ligne, ce n’est pas la même opération. Il faudra également comprendre la durée de validité d’un résultat de recherche. Je n’ai pas de valeur à proposer aujourd’hui.

**Claire :** Et le fournisseur de service, personne n’a signé quoi que ce soit. J’ai reçu deux présentations commerciales, c’est tout. Ne construisons pas l’analyse autour de la première démo qu’on a vue.

**Sarah :** Donc on ne peut pas non plus me promettre qu’un portail externe résoudra tous les cas où LUMEN ne sait pas faire.

**Eva :** Non. Disponibilité, contrat, environnement de test, responsabilités de support : ce sont encore des points à établir. Et Marc devra participer sur les accès et les données échangées.

## 10:00–12:30 — Quand demander l’envoi ?

**Hugo :** Si je vous donne ma préférence, une fois la facture finalisée, j’aimerais qu’elle parte. Sinon, on va encore oublier de cliquer sur Envoyer. Je sais qu’on a séparé les deux aujourd’hui, mais c’est justement l’occasion de simplifier.

**Sarah :** Tu es sûr ? La semaine dernière, tu avais finalisé les factures d’un même client, mais tu attendais encore le nom du contact pour une d’entre elles.

**Hugo :** Oui, c’est vrai. Attends… Je dis « qu’elle parte », mais ce que je veux surtout, c’est ne pas en oublier. Ce n’est peut-être pas exactement la même chose qu’un départ automatique.

**Eva :** C’est ce que j’essayais de comprendre. On pourrait avoir un document prêt à transmettre et une action explicite. Ou autre chose. Mais si la finalisation déclenche immédiatement un échange extérieur, on change une règle importante de LUMEN.

**Claire :** Pour le premier périmètre, je préfère conserver une confirmation d’envoi par une personne habilitée. On étudie un rappel visuel des factures à traiter, mais on ne promet pas un envoi automatique à ce stade. Hugo, est-ce que ça répond à ton risque d’oubli si la liste est vraiment visible ?

**Hugo :** Oui, si je peux trouver celles qui sont finalisées et qui attendent encore. Et si je vois pourquoi une facture ne peut pas partir. Un bouton grisé sans explication, ça va finir en appel au support.

**Eva :** Le principe d’une confirmation humaine pour le premier périmètre, je le retiens. Pour l’envoi par lot, vous attendez aussi une confirmation facture par facture ?

**Claire :** Le lot, je ne veux pas le décider dans la foulée. On commence par décrire le parcours d’une facture. Ensuite, on mesurera si les volumes justifient un traitement groupé dès le départ.

**Hugo :** D’accord. En revanche, après mon clic, je ne vais pas rester devant l’écran à attendre le résultat définitif. Je dois pouvoir passer à la suivante, fermer l’onglet et retrouver le résultat plus tard.

**Eva :** Oui. Le ressenti utilisateur attendu est clair. Le détail des étapes et des retours dépendra de ce que le service externe permet. Une acceptation de la demande et le résultat final ne sont pas forcément un seul événement.

## 12:30–15:00 — Échecs, attente et risque de double envoi

**Hugo :** Voilà, prenons le cas pénible. Je clique, ça tourne, puis j’ai une erreur. Est-ce que je peux recliquer ? Parce qu’en pratique, c’est ce que les gens font.

**Eva :** Il y a au moins deux situations. On sait que rien n’est parti, ou on n’a pas reçu de réponse et on ne sait pas ce qui s’est passé à l’extérieur. Dans le deuxième cas, refaire immédiatement la même chose peut être dangereux. Il faudra comprendre comment retrouver le résultat de la première demande.

**Sarah :** Ça me parle. Quand un fournisseur dit avoir envoyé deux fois, moi, je ne sais pas si ce sont deux documents ou la même facture insistante. Et après on passe du temps à réconcilier les versions.

**Claire :** Ce qu’on ne veut pas, c’est qu’Hugo pense devoir recréer une facture parce qu’il n’a pas reçu de confirmation. Le numéro et le montant restent ceux du document finalisé. Le problème de transmission doit rester attaché à ce document.

**Hugo :** Oui. Et le message doit me dire quoi faire. « Erreur technique », je ne sais pas quoi en faire. « Résultat en cours de vérification, ne pas renvoyer », au moins je comprends que je dois attendre.

**Eva :** C’est un exemple de formulation à travailler. Je ne peux pas encore garantir comment on vérifiera le résultat ni sous quel délai. Il faut poser ces questions au partenaire. Mais on peut déjà exprimer qu’on ne veut pas présenter un échec certain quand le résultat est seulement inconnu.

**Claire :** Qui reprendrait ces cas ? Je n’ai pas envie que toute la facturation dépende d’Eva pour lire une erreur.

**Eva :** Mehdi peut être le point d’entrée support, avec une référence exploitable. Ensuite, il faut déterminer les actions qu’il peut faire seul et celles qui demandent l’équipe technique ou le partenaire. Ne lui donnons pas un droit de renvoi général avant d’avoir décrit les conséquences.

**Hugo :** Et si le retour arrive après que j’ai fermé la facture ?

**Eva :** L’historique doit rester consultable. La manière de te prévenir, bannière, liste ou notification, est encore à choisir. Je ne mettrais pas une alerte partout sans savoir combien de cas on aura.

**Sarah :** Surtout, pas un email par étape. Sinon on aura créé un nouveau travail de tri au lieu de supprimer l’ancien.

## 15:00–17:30 — Corrections, copies et notes de crédit

**Claire :** Revenons au contenu. Le client nous dit que le numéro de commande manque après l’envoi. Qu’est-ce qu’on attend ?

**Hugo :** Mon premier réflexe serait de l’ajouter et de renvoyer. Mais je sais que dans LUMEN, une facture finalisée ne se modifie plus. Aujourd’hui on traite la correction avec une note de crédit et, si nécessaire, une nouvelle facture.

**Eva :** Et on ne va pas contourner ça en modifiant seulement le document qui partirait à l’extérieur. Sinon le client reçoit une version et notre archive en montre une autre. Il faudra distinguer une correction commerciale d’un simple problème de transmission.

**Sarah :** Par exemple une mauvaise adresse de contact et un mauvais montant, ça ne se traite pas forcément de la même façon. Mais je ne veux pas qu’on décide maintenant que toute donnée peut être corrigée après coup sous prétexte qu’elle semble technique.

**Claire :** Exact. On garde l’immuabilité du document finalisé. Les cas où une correction implique un crédit ou un remplacement doivent être revus avec Benoît, en particulier les références attendues par les clients. Pas de porte dérobée dans un écran de support.

**Hugo :** Et pour les crédits, on reprend le même exemple ? Mille deux cent dix euros de facture, cent vingt et un euros de crédit. Si le client a déjà payé six cents euros, il reste quatre cent quatre-vingt-neuf. Que la facture ait été envoyée par email ou par Peppol, ce calcul ne doit pas changer.

**Eva :** Oui, c’est le calcul commercial existant. La transmission du crédit est un autre événement ; elle ne crée pas un paiement. Il faut aussi étudier à quel moment on peut transmettre le crédit si la facture d’origine a encore un résultat d’envoi incertain.

**Claire :** Celui-là, on le garde comme question. Je ne veux pas répondre « toujours » ou « jamais » sans examiner les situations.

**Hugo :** Dernier point : certains clients vont quand même demander un PDF par email, même s’ils reçoivent autrement.

**Claire :** On peut étudier une copie de confort clairement identifiée. Mais elle ne doit pas créer un autre numéro ni une autre créance. Le caractère automatique ou manuel de cette copie n’est pas décidé. Pour le premier parcours, on garde une action séparée tant qu’on n’a pas clarifié ce besoin.

## 17:30–20:00 — Réception des documents fournisseurs

**Sarah :** Alors, côté achats, je voudrais qu’une facture reçue par ce canal apparaisse dans LUMEN sans que je doive recopier tous ses montants. Aujourd’hui je dépose un PDF, je complète les informations, puis je vérifie. J’aimerais arriver directement à ce dernier travail, pas considérer que tout est correct parce que le fichier est arrivé automatiquement.

**Hugo :** Tu veux qu’elle arrive déjà avec le fournisseur et sa catégorie ?

**Sarah :** Le fournisseur, si on sait le retrouver avec certitude. La catégorie, c’est autre chose. Une même entreprise peut nous vendre du matériel un mois et une prestation le mois suivant. Je préfère une catégorie à compléter plutôt qu’une catégorie fausse qui a l’air validée.

**Eva :** Donc les données reçues peuvent préremplir, mais elles ne remplacent pas ton contrôle. Et les catégories actuelles restent celles des achats de LUMEN, sauf nouveau besoin identifié.

**Sarah :** Oui. Et je veux pouvoir voir ce qu’on a réellement reçu. Si le fournisseur a joint une annexe, un détail des prestations ou un bon de livraison, il faut le retrouver. Je ne sais pas encore quels formats le service transmettra, donc je ne vous donne pas une liste de fichiers acceptés inventée maintenant.

**Claire :** On conserve le principe actuel : d’abord un document à vérifier, ensuite une vérification ou un litige. La réception seule ne vaut ni accord sur la dépense ni paiement.

**Eva :** Il faudra préciser comment on traite une pièce illisible ou un contenu qui ne permet pas de créer un achat complet. Je distinguerais la conservation de ce qui est arrivé et sa disponibilité dans la liste métier. Mais je n’ai pas de processus final à vous présenter.

**Sarah :** Ce que je ne veux surtout pas, c’est que ça disparaisse. Même si on ne sait pas l’affecter immédiatement, il faut que quelqu’un puisse retrouver l’élément et dire ce qui bloque. Et je ne veux pas une facture avec zéro euro juste parce qu’un champ n’a pas été compris.

**Claire :** D’accord. Réception visible et problème explicable, mais pas de faux achat exploitable. Il faudra organiser la file de travail et son responsable avec Mehdi et toi.

## 20:00–22:30 — Doublons et documents qui ne correspondent pas

**Sarah :** Prenons Papier et Bureau. Ils m’envoient leur facture de deux cent quarante-deux euros, puis la personne du service interne me transfère le PDF le lendemain en disant : « À payer rapidement. » Si j’ai déjà reçu le document dans LUMEN, je ne veux pas un deuxième achat parce que l’origine du fichier est différente.

**Eva :** Dans le socle, on compare déjà le fournisseur, le type de document et le numéro externe. Il faut analyser comment étendre ce contrôle au nouveau canal. Mais une même facture et un même fichier, ce n’est pas toujours identique au niveau des octets.

**Hugo :** Parce que le PDF et les données reçues peuvent présenter la même facture différemment ?

**Eva :** Oui. On ne peut donc pas dire « fichiers différents, factures différentes ». Et on ne doit pas non plus fusionner automatiquement deux documents parce qu’ils portent le même montant. Il faudra décider ce qui constitue une correspondance suffisamment certaine et ce qui part en revue.

**Sarah :** Je vous donne la variante : même fournisseur, même numéro, mais le PDF dit deux cent quarante-deux et l’autre document deux cent soixante-six euros vingt. Là, on conserve les deux pièces et on m’affiche un conflit. Pas d’écrasement silencieux. Je contacte le fournisseur pour comprendre.

**Claire :** Oui, sur ce point on ne change pas la règle de l’existant. Et on ne compte pas deux fois la dette en attendant. La façon exacte de présenter le conflit reste à décrire.

**Sarah :** Autre cas : le fournisseur n’existe pas encore. La facture doit rester retrouvable, mais je ne veux pas qu’on crée automatiquement une nouvelle fiche avec un nom approximatif. On a justement nettoyé le référentiel pour éviter ça.

**Eva :** On pourrait avoir un élément en attente de rapprochement avec un tiers. C’est une proposition, pas encore le choix d’un nouvel écran. Et pour un fournisseur archivé, il faut décider qui vérifie la situation et qui peut le réactiver.

**Claire :** Oui. Pas de réactivation automatique par une arrivée externe. Sarah et le métier doivent pouvoir garder la main. Mais on ne promet pas non plus de supprimer un document reçu parce que la relation commerciale n’est plus active.

## 22:30–25:00 — Ce que signifie un retour métier

**Hugo :** Je reviens sur les retours. Si le client reçoit la facture mais la refuse parce qu’il conteste une prestation, est-ce que je vais le voir dans LUMEN ?

**Eva :** Je ne sais pas encore quelles informations nous recevrons du service retenu. On doit distinguer ce qu’on souhaite savoir et ce qui sera effectivement disponible. Un retour technique ne nous permet pas d’inventer une approbation du service achats du client.

**Claire :** Dans le besoin, ce qui m’importe, c’est de ne pas mélanger les choses. Si le client appelle pour contester, Hugo doit pouvoir traiter la contestation même si aucun message externe ne nous est revenu. Et une preuve de transmission ne doit pas masquer cette discussion.

**Sarah :** À l’inverse, quand moi je mets une facture fournisseur en litige, je ne veux pas qu’un message parte automatiquement chez lui. Aujourd’hui, le litige est interne à notre suivi. Parfois j’attends juste le détail d’une prestation, et je discute avec le responsable de la dépense avant de répondre.

**Hugo :** Donc pour le premier périmètre, on ne transforme pas nos actions internes en réponses à l’extérieur ?

**Claire :** Oui. Aucun changement de ce type sans analyse et validation explicites. Si on veut plus tard envoyer une réponse métier structurée, c’est un besoin à étudier. Ce n’est pas implicitement inclus parce qu’on a dit « réception ».

**Eva :** Ça nous aide à limiter le périmètre. Il reste quand même à déterminer comment présenter les retours disponibles. Par exemple, un refus technique lié aux données ne demande pas le même interlocuteur qu’un désaccord commercial communiqué par téléphone.

**Sarah :** Et qui voit quoi. Si je suis à la facturation, je dois pouvoir expliquer une erreur utile. Je n’ai pas besoin d’avoir accès à des secrets de connexion ou à une page de configuration du partenaire.

**Claire :** Exactement. Et si le comptable consulte le dossier, il doit retrouver les pièces et leur provenance. Le détail de ce qu’on lui expose dans le suivi, on le vérifiera avec Benoît. On ne lui donne pas automatiquement des droits de reprise.

## 25:00–27:30 — Droits, alertes et exploitation quotidienne

**Eva :** Aujourd’hui, on a nos quatre rôles applicatifs. L’administration technique ne donne pas automatiquement le droit de finaliser une facture ou de déclarer un paiement. Est-ce qu’on veut garder cette logique pour l’envoi ?

**Claire :** Oui. L’action d’envoi appartient au rôle Facturation dans le périmètre métier étudié. L’administrateur configure, mais ne devient pas facturier par défaut. Pour l’activation de la connexion et les accès de support, il faut une validation avec Marc. Je ne tranche pas les permissions techniques sans lui.

**Hugo :** Il faut aussi penser aux absences. Si je suis parti, Sarah peut reprendre une facture de vente avec son rôle actuel. On ne peut pas avoir une erreur visible seulement par la personne qui a cliqué.

**Sarah :** Et il nous faut une liste commune des problèmes à traiter. Mais pas un nouvel indicateur de direction qui prend trois semaines à définir. Juste pouvoir retrouver les éléments qui demandent une action, avec un filtre compréhensible.

**Eva :** L’objectif d’une file partagée est clair. Il reste à définir qui peut voir son contenu, l’affecter et clôturer un problème. Un ticket clôturé n’est pas forcément un envoi réussi : on peut aussi conclure que la facture doit être corrigée par le métier.

**Claire :** Oui. Et pas de « Résolu » qui efface l’erreur d’origine. Il nous faut l’historique : qui a demandé, à quel moment, ce qui a été reçu et ce qu’on a décidé de faire ensuite.

**Hugo :** Pour les alertes, je préfère regarder une liste au début de ma journée. Sauf incident important. Si rien ne part pendant deux heures, là j’aimerais qu’on le sache sans attendre le lendemain.

**Eva :** On peut exprimer ce besoin, mais on n’a pas encore de seuil de surveillance validé. Deux heures est ton exemple, pas un engagement de service. Mehdi devra nous aider à séparer l’alerte technique générale et la tâche métier sur une facture.

**Claire :** Et les données qu’on garde, leur durée et les traces visibles doivent être examinées avec Marc et Benoît. On a une politique existante, mais je ne veux pas annoncer que tout nouveau contenu entre automatiquement dedans sans analyse d’impact.

## 27:30–30:00 — Déploiement, reprise et priorités

**Claire :** Il nous reste quelques minutes. Si on ne peut pas tout faire d’un coup, où met-on la priorité ? Hugo, tu dirais l’envoi, je suppose.

**Hugo :** Oui. Mais pas un envoi où je dois appeler Eva pour savoir si ça a marché. Je préfère moins d’options et un suivi exploitable. La recherche du destinataire, la confirmation et le résultat vont ensemble pour moi.

**Sarah :** Et je ne veux pas que « les achats plus tard » devienne un oubli. Si on fait deux étapes, il faut quand même comprendre le parcours de réception avant de choisir un partenaire. Sinon, on en choisira un très bien pour envoyer et on découvrira ensuite les limites pour recevoir.

**Eva :** C’est raisonnable. Analyser les deux sens ne nous oblige pas à les déployer le même jour. Mais on doit vérifier les dépendances d’activation. Il peut y avoir des conditions côté service qui font qu’on ne sépare pas les choses aussi librement que dans notre planning.

**Claire :** Donc priorité proposée à l’envoi et à son suivi, avec étude de la réception dès maintenant. Le phasage de livraison sera arbitré après cette analyse. Je n’engage pas une date aujourd’hui, et je ne prends pas des jours sur R3 sans refaire le point avec Isabelle.

**Hugo :** Pour les anciennes factures, on fait quoi ? Est-ce qu’on les renvoie toutes pour avoir un historique complet dans le nouveau canal ?

**Claire :** Non, pas de campagne de renvoi des anciennes factures déjà transmises. On ne crée pas de nouvelles demandes de paiement pour remplir une liste. Pour une facture finalisée mais pas encore envoyée au moment de la bascule, en revanche, il faut établir la règle de transition.

**Sarah :** Et pour les achats, il faudra une frontière claire. Sinon le même document peut arriver avant l’ouverture, puis être récupéré une seconde fois au démarrage. Je veux un rapprochement de transition, pas un grand import aveugle.

**Eva :** Oui. Date de démarrage, documents en attente, éventuelle reprise d’historique et désactivation du traitement pendant un retour arrière : à décrire avec l’exploitation et le partenaire. On n’a pas encore choisi le mécanisme. Et revenir à une version précédente de LUMEN n’annule pas ce qu’un service extérieur a déjà transmis.

## 30:00–32:30 — Comment saura-t-on que ça fonctionne ?

**Eva :** Pour préparer la recette, j’aurais besoin de cas concrets. Pas seulement une facture qui passe. Quel résultat vous ferait dire : « Ça nous aide vraiment » ?

**Hugo :** Je peux préparer une facture simple, une note de crédit partielle et un client qui n’est pas joignable par le canal attendu. Je voudrais aussi simuler le clic répété. Et un cas où je ferme l’écran juste après ma demande : je dois retrouver ce qui s’est passé en revenant.

**Sarah :** De mon côté : une facture fournisseur connue, une facture d’un fournisseur absent, un document avec une annexe, un doublon et un conflit de montant. Je peux reprendre notre exemple à deux cent quarante-deux euros. Je veux vérifier que le conflit n’augmente pas artificiellement ce qu’on doit au fournisseur.

**Claire :** On doit aussi pouvoir expliquer le processus à quelqu’un d’autre que vous deux. Si un remplaçant ne sait pas quoi faire devant un problème, on aura seulement déplacé la complexité. Mehdi doit participer à l’essai de reprise.

**Eva :** Oui. Julien organisera la recette avec des données de test et les retours qu’on peut provoquer chez le partenaire. Pas de première tentative sur un vrai client pour voir ce qui arrive. Il faudra savoir ce que le sandbox permet de simuler, notamment les erreurs et les réponses tardives.

**Hugo :** Pour les bénéfices, je peux noter le temps qu’on passe aujourd’hui à rechercher un envoi ou à répondre à une demande de renvoi. Je n’ai pas cette mesure sous la main.

**Claire :** Très bien. On ne va pas annoncer un gain de cinquante pour cent parce que ça sonne bien dans une présentation. On fait un petit échantillon, on note les volumes et les gestes, puis on se donne une cible réaliste. La baisse des doubles traitements et la visibilité des erreurs m’intéressent autant que le temps moyen.

**Sarah :** Je peux faire la même chose sur la saisie et les recherches de doublons. Mais on distingue le temps de saisie qu’on pourrait éviter et la vérification métier qu’on doit conserver. Si on mesure seulement le temps total, on pourrait être tenté de supprimer le contrôle pour afficher un beau résultat.

## 32:30–35:00 — Reformulation et suite de l’analyse

**Claire :** Je reformule avant qu’on se quitte. Le besoin, c’est que les échanges passent dans un suivi cohérent avec LUMEN, sans double document, sans perte de pièce et sans confusion avec le paiement. On étudie les ventes, les notes de crédit et les documents fournisseurs. Mais on ne considère pas que tous les cas ont été définis aujourd’hui.

**Hugo :** Et pour le premier parcours de vente, on conserve une demande d’envoi explicite. Mon idée de départ automatique était surtout une manière de dire que je veux voir ce qui attend encore. Je ne veux pas qu’on retienne les deux comme deux consignes en même temps.

**Eva :** Oui, c’est bien clarifié. On garde ce principe pour le périmètre initial à analyser. Pour le service externe, les identifiants, les retours disponibles et la reprise après une réponse manquante, il reste des informations à obtenir. Je pourrai étudier les options avec des besoins plus précis, sans présumer du prestataire.

**Sarah :** Côté achats, préremplir n’est pas vérifier. Un document reçu doit rester retrouvable, même si un problème empêche encore de l’exploiter. Et les litiges restent internes tant qu’on n’a pas décidé et étudié autre chose. Je fournirai des exemples, y compris le fournisseur archivé.

**Claire :** Très bien. Hugo et Sarah, est-ce que vous pouvez préparer vos exemples d’ici vendredi ? Eva, on se réserve aussi un point avec Marc, Mehdi et Julien pour comprendre leurs contraintes. Je contacte Benoît sur les populations concernées, les corrections et les pièces à conserver ; Amélie sur ce qui doit rester distinct des paiements.

**Hugo :** Oui pour vendredi. Je mettrai aussi un cas où l’adresse de contact change après la finalisation, parce qu’on l’a mentionné sans aller au bout.

**Eva :** Pour le prochain échange, je voudrais surtout que les questions ouvertes soient visibles. Si on n’a pas la réponse du partenaire, on ne remplit pas le trou avec ce qui nous semblerait habituel. Et on ne transforme pas notre préférence de phasage en date promise.

**Claire :** Exactement. On relit ensuite l’analyse avec chacun sur son domaine avant de lancer le développement. Pas de commande de solution ni de date de mise en service décidée dans cette réunion. Merci à vous ; je vous envoie les invitations pour la suite.

**Sarah :** Merci. Et je garde mon histoire de facture à deux cent quarante-deux euros, elle va nous servir plus d’une fois.

**Hugo :** Oui, mais une seule dette, même si tu racontes l’histoire trois fois.

**Sarah :** Voilà. Si on arrive déjà à garder ça, ce sera un bon début.

**Eva :** On va l’écrire correctement, alors.

**Claire :** Parfait. Bonne journée.
