### Sujet : Plateforme générique de partage de ressources


    La mobilité partagée (vélos, trottinettes) n'est qu'un cas d'une famille de services : prêt de matériel, location
    de voitures en libre-service, réservation d'espaces. Le groupe conçoit une plateforme générique de partage
    de ressources, configurée pour chaque opérateur et chaque type de ressource sans modifier le noyau.

- **Ce qui doit être configurable**
    • Les types de ressources et leurs attributs (un vélo a une batterie, une salle a une capacité), décrits par
        un métamodèle.
    • Le cycle de vie d'une ressource (états et transitions), défini par configuration et non codé en dur.
    • Les règles de tarification, composées à partir de règles élémentaires (durée, horaire, profil,
        abonnement).
    • Les règles d'usage par zone ou par site : zones hiérarchiques, horaires, quotas.
- **Points d'extension attendus**
    • Prestataires de paiement, sources de localisation et capteurs, ajoutés comme modules.
    • Nouvelles règles de tarification ou d'usage, ajoutées par extension.
- **Instanciations à démontrer** : 
    la mobilité urbaine partagée, plus un second domaine choisi par le groupe (prêt
    de matériel sur un campus, location de voitures en libre-service, réservation de salles...).
    Les demandes de changement seront communiquées en semaines 5, 7 et 8. Chacune devra être absorbée
    par configuration ou par extension, sans modifier le noyau.

