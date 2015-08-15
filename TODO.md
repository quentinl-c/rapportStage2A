#TODO : Rapport de satge

##Plan du rapport

Introduction

* Les enjeux de l'édition collaborative
* Exemples d'éditeurs (google doc)
* Problématique du passage à l'échelle et limitation des systèmes actuels
* Problématique de la gestion et du contrôle des données 

**Problématique : Implémentation d'un système p2P pour l'édition collaborative**

###I. Présentation du Loria(et de COAST)

####1. Présentation du Loria

* Présentation générale (done)
* Présentation des différents départements (done)

####2. Présentation de l'équipe COAST 

* Présentation générale
* Les différents axes de recherche
* Ma place dans l'équipe

###II. État de l'art

####1.Présentation de MUTE
* Avantage de l'approche CRDT par rapport à l'approche OT (présentation rapide de ses deux approches)
* Présentation de l'architecture de MUTE
* Présentation des limites d'un tel système 

####2. Présentation des technologies webrtc
* Qu'est-ce qu'un réseau pair-à-pair ?
* Détails sur la technologie webrtc

###III. Réalisation

####1. Présentation de la problématique détaillée et du contexte

* Implémentation d'un système pair-à-pair
* Système développé en nodeJS -> développement en JavaScript
* Utilisation de webrtc

####2. Réalisation d'un système de communication pair-à-pair pour l'outil MUTE

#####1. Choix de la librairie et développement d'un prototype pour valider le choix

* Difficultés liées à la recherche d'une librairie
	* Maintenabilité/ Support existant? Beaucoup de librairies encore disponibles ne sont plus supportées
	* Degré d'abstraction
* Choix de la librairie PeerJS
	* Librairie JavaScript
	* Support actif
	* API documentée
	* Offrant un service de signaling distant, MAIS proposant aussi un serveur de signaling utilisable sous nodeJS
	* Un très bon compromis pour du prototypage 
* Développement d'un prototype pour valider le choix de la librairie 
	* Présentation du prototype

#####2. Implémentation du système pair-à-pair dans MUTE
	
* Implémentation d'un module pair-à-pair dans l'architecture de mute
* Description du fonctionnement du système p2p

#####3. présentation du résultat (et limites d'un tel système)

* Système fonctionnalité
* Qui n'est pas dépendant du serveur
* Toplogie "fully-meshed" pas assez efficace (transisiton vers les algorithmes de gossiping)

####3. Implémentation d'un système de gossiping pour MUTE

#####1. Présentation rapide des algorithmes de Gossiping

* Qu'est-ce qu'un algorithme de gossiping
* Leur utilisation (big data, cloud cpmputing ...)

#####2. Choix d'un algorithme SCAMP

* un grand nombre d'algorithmes (SCAMP CYCLON et cie..)
* De nombreuses recherches dans le domaine
* CRATE éditeur p2p utilisant déjà un algo de gossiping
* Choix de SCAMP
* Présentation de SCAMP

#####3. Adaptation de SCAMP

* Reflexion autour de l'algorithme et présentation des mécanismes
* Place de SCAMP dans MUTE, présentation du travail effectué

###Conclusion

* SCAMP (gossiping en général), une piste de réflexion qui mériterait d’être approfondie
* La sécurité dans ces réseaux ...


##Biblio :
* http://www.journaldunet.com/solutions/0601/060105_tribune-sqli-web-20.shtml


