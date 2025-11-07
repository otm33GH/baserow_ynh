### Utilisateur administrateur

Rendez-vous sur la page [__DOMAIN__](__DOMAIN__) pour créer le premier utilisateur.
❗Le **premier** utilisateur créé aura des droits d'administration, les suivants seront des utilisateurs normaux.

### Configuration
Le panneau de configuration permet d'éditer les paramètres suivants :
* Relais SMTP pour l'envoi de courriel
* Limite de la taille d'import des fichiers
* Stockage AWS
* Modèles AI

### Génération d'applications
Les applications créées avec Baserow peuvent être déployées sur des sous domaines de [__DOMAIN__](__DOMAIN__).
Par défaut, ces sous-domaines ne seront pas couverts par un certificat reconnu par les navigateurs.
Pour les rendre accessibles en https, il convient de suivre les étapes suivantes :
- créer le sous-domaine correspondant à l'application dans yunohost et y installer un certificat Let's Encrypt.
- installer l'application _Redirect_ en mode `reverse_proxy`et la faire pointer sur http://127.0.0.1:__PORT_FRONTEND__
