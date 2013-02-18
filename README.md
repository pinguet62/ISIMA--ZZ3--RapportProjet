Notes :
    Retour à la ligne (sans alinéat) : passer 1 ligne blanche
    Sauter une ligne (avec alinéat) : mettre \\ en début de ligne suivante
    Citer avec lien en bas de page: \textit{Python}\footnote{Site web : \href{http://www.python.org}{http://www.python.org}}

Glossaire:
    XMPP
    


A ajouter :
    iChat (Apple)



Plan:
    Remerciements
    Résumé
    Abstract
    Table des matières
    Introduction
    I- Introduction de l'étude
        A- Besoin de l'utilisateur
        B- Solution envivagée
    II- Etude de fonctionnement
        A- Protocole XMPP
        B- GTalk
    III- Réalisation de la solution
        A- Site web
        B- Applications mobiles
            a- Androïd
            b- iOS
            c- Windows Phone
    IV- Résultats obtenus
        A- Site web
        B- Applications mobiles
    Conclusion
    Bibliographie



TODO:
    Page de garde :
        Fillières : box (pour alignés)
        Bas de page : colonnes flexibles (pours prénoms sur même ligne)



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