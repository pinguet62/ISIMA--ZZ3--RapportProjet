



Glossaire:
    JSON
    XMPP



A ajouter :
    iChat (Apple)



TODO:
    Mettre en commun le fonctionnement g�n�ral des application Andro�d et iOS -> �a �vite de r�p�ter les m�mes choses...
    Page de garde :
        Filli�res : box (pour align�s)
        Bas de page : colonnes flexibles (pours pr�noms sur m�me ligne)
    Glossaire
    Parler de la licence



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