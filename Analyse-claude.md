2. Analyse du sujet
Nature du problème
Le sujet porte moins sur un domaine métier que sur la conception d'une plateforme réutilisable. La mobilité partagée sert d'exemple, mais la vraie question est : comment séparer ce qui est stable (le noyau) de ce qui varie (les opérateurs, les types de ressources, les règles) ? C'est un problème d'abstraction et de généricité, avec le risque classique de la sur-généralisation.
Les quatre axes de variabilité
Le sujet identifie quatre dimensions qui doivent varier sans toucher au noyau :
1. Les données : types de ressources et attributs (métamodèle).
2. Le comportement : cycle de vie des ressources (états et transitions).
3. Les règles économiques : tarification composable.
4. Les règles d'accès : zones hiérarchiques, horaires, quotas.
Ces axes sont de natures différentes (structure, dynamique, calcul, contrainte). Chacun pose ses propres questions, et ils interagissent entre eux. Par exemple, la tarification peut dépendre de la zone, et le cycle de vie dépend du type de ressource.
Deux mécanismes distincts à ne pas confondre
Le sujet distingue explicitement :
• la configuration (faire varier le comportement par des paramètres ou des descriptions) ;
• l'extension (ajouter du code ou des modules sans modifier l'existant).
Savoir où passe la frontière entre les deux, et ce qui relève de l'un ou de l'autre, est une question centrale du sujet.
Contrainte structurante : l'invariance du noyau
La phrase décisive est : « sans modifier le noyau ». Elle sert aussi de critère d'évaluation, puisque les changements des semaines 5, 7 et 8 testeront la conception. Les changements étant inconnus à l'avance, la plateforme sera jugée sur sa capacité à absorber l'imprévu.
Difficultés et tensions identifiables
• Généricité vs simplicité : un métamodèle trop abstrait devient difficile à utiliser, un métamodèle trop spécifique perd son intérêt.
• Configuration vs code déguisé : une configuration très expressive peut devenir un langage de programmation à part entière, avec ses propres problèmes (validation, lisibilité, tests).
• Composition des règles : combiner des règles élémentaires soulève des questions d'ordre, de priorité, de conflit et de cumul.
• Hiérarchie de zones : l'héritage et la surcharge des règles entre niveaux peuvent créer des ambiguïtés.
• Cohérence entre axes : un cycle de vie configurable doit rester cohérent avec les règles d'usage et la tarification.
• Hétérogénéité des intégrations : paiement, localisation et capteurs ont des contrats très différents d'un prestataire à l'autre.
• Validation de la généricité : deux instanciations seulement ne prouvent pas qu'une plateforme est réellement générique.
Ce que le choix du second domaine implique
Le second domaine n'est pas neutre. Un domaine trop proche de la mobilité urbaine démontrera peu de choses, alors qu'un domaine très différent (par exemple la réservation de salles, où la notion de créneau remplace celle de trajet) mettra davantage la généricité à l'épreuve. Ce choix doit être fait en pensant à ce qu'il permet de démontrer.
Éléments non précisés dans le sujet
• Le périmètre exact du « noyau » : qu'est-ce qui en fait partie ?
• Le niveau d'exécution attendu : modèle conceptuel, prototype, application complète ?
• Le degré de configuration visé : fichiers, interface d'administration, ou autre ?
• Les critères d'évaluation précis (qualité de l'architecture, démonstration, documentation).
• La nature des demandes de changement des semaines 5, 7 et 8.
• Les exigences non fonctionnelles : performance, multi-opérateurs, sécurité, volumétrie.
Risques pour l'équipe
• Passer trop de temps sur l'abstraction au détriment d'une démonstration concrète.
• Sous-estimer l'impact des changements tardifs sur les choix initiaux.
• Concevoir uniquement à partir du cas de la mobilité, puis constater que le second domaine ne rentre pas.
• Confondre « flexible » et « générique » : on peut tout rendre paramétrable sans que le système soit pour autant bien conçu.
Compétences mobilisées
Modélisation (métamodèles), architecture logicielle et modularité, conception de systèmes extensibles, gestion du changement, travail en équipe sur un temps long avec des évolutions imposées.
