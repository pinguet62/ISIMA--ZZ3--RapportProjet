Je pense que ça serait mieux de faire une partie "Applications mobiles" qui regroupent Android et iOS car au final c'est le même principe de fonctionnement.

J'ai quelques bugs dans la compilation du glossaire, donc j'ai commenté les lignes qui pour l'instant ne servent pas.
Je ne sais pas si ça vient de mon compilateur, je regarderai ça à la fin quand on aura fini et qu'il ne restera plus que le glossaire.










Glossaire:
    XMPP
    


A ajouter :
    iChat (Apple)



TODO:
    Page de garde :
        Fillières : box (pour alignés)
        Bas de page : colonnes flexibles (pours prénoms sur même ligne)
    Glossaire



Diagramme de classe :
    http://www.websequencediagrams.com/#
    Sources :
        GTalk :
            Réception :
                
            Emission :
                
        Site web :
            Réception :
                title Réception d'un SMS
                Expéditeur->Smartphone: SMS
                Smartphone->Application mobile: Evénement réception SMS
                Application mobile->+Smartphone: Lecture du SMS
                Smartphone-->-Application mobile: Expéditeur + contenu
                Application mobile->Compte Google: message XMPP
                Compte Google->Site web: message XMPP
                Site web->Utilisateur: Affiche le SMS
            Emission :
                title Envoi d'un SMS
                Utilisateur->Site web: Saisie du SMS
                Site web->Compte Google: message XMPP
                Compte Google->Application mobile: message XMPP
                Application mobile->Smartphone: Envoi du SMS
                Smartphone->Expéditeur: SMS