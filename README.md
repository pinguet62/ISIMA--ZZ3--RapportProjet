



Glossaire:
    JSON
    XMPP



A ajouter :
    iChat (Apple)



TODO:
    Mettre en commun le fonctionnement général des application Androïd et iOS -> ça évite de répéter les mêmes choses...
    Page de garde :
        Fillières : box (pour alignés)
        Bas de page : colonnes flexibles (pours prénoms sur même ligne)
    Glossaire
    Parler de la licence



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