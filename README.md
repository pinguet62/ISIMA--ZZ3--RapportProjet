Je pense que �a serait mieux de faire une partie "Applications mobiles" qui regroupent Android et iOS car au final c'est le m�me principe de fonctionnement.

J'ai quelques bugs dans la compilation du glossaire, donc j'ai comment� les lignes qui pour l'instant ne servent pas.
Je ne sais pas si �a vient de mon compilateur, je regarderai �a � la fin quand on aura fini et qu'il ne restera plus que le glossaire.










Glossaire:
    XMPP
    


A ajouter :
    iChat (Apple)



TODO:
    Page de garde :
        Filli�res : box (pour align�s)
        Bas de page : colonnes flexibles (pours pr�noms sur m�me ligne)
    Glossaire



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