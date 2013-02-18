Notes :
    Retour � la ligne (sans alin�at) : passer 1 ligne blanche
    Sauter une ligne (avec alin�at) : mettre \\ en d�but de ligne suivante
    Citer avec lien en bas de page: \textit{Python}\footnote{Site web : \href{http://www.python.org}{http://www.python.org}}

Glossaire:
    XMPP
    


A ajouter :
    iChat (Apple)



Plan:
    Remerciements
    R�sum�
    Abstract
    Table des mati�res
    Introduction
    I- Introduction de l'�tude
        A- Besoin de l'utilisateur
        B- Solution envivag�e
    II- Etude de fonctionnement
        A- Protocole XMPP
        B- GTalk
    III- R�alisation de la solution
        A- Site web
        B- Applications mobiles
            a- Andro�d
            b- iOS
            c- Windows Phone
    IV- R�sultats obtenus
        A- Site web
        B- Applications mobiles
    Conclusion
    Bibliographie



TODO:
    Page de garde :
        Filli�res : box (pour align�s)
        Bas de page : colonnes flexibles (pours pr�noms sur m�me ligne)



Diagramme de classe :
    http://www.websequencediagrams.com/#
    Sources :
        GTalk :
            R�ception :
                
            Emission :
                
        Site web :
            R�ception :
                title R�ception d'un SMS
                Exp�diteur->Smartphone: SMS
                Smartphone->Application mobile: Ev�nement r�ception SMS
                Application mobile->+Smartphone: Lecture du SMS
                Smartphone-->-Application mobile: Exp�diteur + contenu
                Application mobile->Compte Google: message XMPP
                Compte Google->Site web: message XMPP
                Site web->Utilisateur: Affiche le SMS
            Emission :
                title Envoi d'un SMS
                Utilisateur->Site web: Saisie du SMS
                Site web->Compte Google: message XMPP
                Compte Google->Application mobile: message XMPP
                Application mobile->Smartphone: Envoi du SMS
                Smartphone->Exp�diteur: SMS