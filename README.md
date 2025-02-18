# Architectures Sécurisées

MARINE NATIONALE

Pôle Écoles Méditerranée

---

## Architecture sécurisée

![Image: VLAN Utilisateurs, DMZ Serveurs]

**Éléments clés:**

*   VLAN Utilisateurs
*   VLAN Administrateurs Bureautique
*   Interfaces Admin Réseaux
*   Zone Admin
*   Zone Applis
*   Zone Services
*   DMZ Serveurs

---

## Architecture sécurisée

Connaitre son SI

*   Bien ou actif
*   Quelles sont les vulnérabilités ?
*   Types de réseau ?
*   Quelles peuvent être les menaces ?
*   Quelles peuvent être les sources de menaces ?
*   On en déduit des risques
*   On met en place les mesures de sécurité adaptées
    *   Besoin, niveau de sécurité
    *   Compétence en SSI
    *   Coût financier

---

## Architecture sécurisée

![Image: Applications, Systemes, Securite]

Périmètre d'un équipement

---

## Principe de défense en profondeur

![Image: Citadelle, château]

Sébastien Le Prestre, Marquis de Vauban

---

## Défense En Profondeur en SSI

Ce principe peut être divisée en trois domaines :

*   Administratif
*   Physique
*   Technique

![Image: Cercles Defense en Profondeur]

---

## Défense En Profondeur en SSI

![Image: Conférence]

*   Administratif
    *   La sensibilisation
    *   Connaissance de la PSSI-A
    *   La formation

---

## Défense En Profondeur en SSI

![Image: Militaire, Digicode]

*   Physique
    *   Protection des locaux et des biens matériels.
    *   Déploiement de lecteurs biométriques pour réguler l'accès des zones sensibles

---

## Défense En Profondeur en SSI

![Image: Defense en Profondeur 2]

*   Sécurité technique

---

## Défense En Profondeur en SSI

![Image: Firewall Schemas]

*   Firewall
*   DMZ
*   Proxys
*   IDS/IPS
*   Etc

Contrôle qui a le droit d'accéder à quoi

---

## Défense En Profondeur en SSI

![Image: Schema reseau bloqué]

*   Réseau externe

---

## Défense En Profondeur en SSI

![Image: Schema reseau DMZ]

*   Réseau externe

Déplacés les serveurs devant être accessibles de l'extérieur

Architecture << accès DMZ via le pare-feu >>

---

## Principe de défense en profondeur

![Image: Schema reseau interne]

DMZ + base interne

---

## Principe de défense en profondeur

![Image: Schema deux Firewall]

*   Réseau externe

Architecture basée sur deux pare-feux

---

## Principe de défense en profondeur

![Image: Schema deux Firewall Mandataire]

*   Réseau externe

Architecture basée sur deux pare-feux avec serveur mandataire

---

## Principe de défense en profondeur

![Image: Schema deux DMZ]

*   Réseau externe

Architecture avec deux DMZ en coupure physique

---

## Principe de défense en profondeur

*   Réseau externe

Principes de sécurisation appliquées sur les pare feux et les serveurs ?

*   Pare feux
    *   Principe de la diversité à tous les niveaux
        *   au niveau du système d'exploitation
        *   au niveau du moteur de filtrage
        *   au niveau du matériel.
    *   Principe de la panne sans danger
    *   Principe de l'interdiction par défaut

---

## Principe de défense en profondeur

*   Réseau externe

Principes de sécurisation appliquées sur les pare feux et les serveurs ?

*   Serveurs
    *   Principe de l'unicité de fonction,
    *   Principe du moindre privilège,
    *   Principe du maillon le plus faible

---

## Principe de défense en profondeur

![Image: Schema Interne]

*   Réseau Interne
    *   Sécuriser les équipements d'interconnexion
    *   Gérer les utilisateurs
    *   Sécuriser les terminaux
    *   Sécuriser les services et processus

---

## Principe de défense en profondeur

![Image: Schema VLAN]

*   Réseau Interne

Sécuriser les équipements d'interconnexion

Recommandations de l'ANSSI

---

## Principe de défense en profondeur

*   Réseau Interne

Sécuriser les équipements d'interconnexion

Exigences de sécurité des routeurs :

*   Séparer les adresses internes des adresses publiques tout en assurant la correspondance entre elles.
*   Filtrer le trafic entre réseaux IP en tenant compte des connexions et de leur sens.
*   Préserver la confidentialité et l'intégrité des échanges.
*   Disposer d'une redondance IP sûre pour la route par défaut.
*   Sécuriser les protocoles de routage
*   Désactiver les protocoles et services non utiles et non utilisés
*   Se protéger des attaques TCP
*   Etc

---

## Principe de défense en profondeur

![Image: ACL]

ACL ?

---

## Principe de défense en profondeur

*   ACL (Acces Control List)

Il existe deux types d'ACLs :

*   ACL simple (standard)
*   ACL plus complexe (étendue)

Peuvent être identifiées soit par un numéro ACL « numériques » soit par un nom ACL « nommées »

*   Les numéros 1 à 99 et 1300 à 1999 sont réservés aux ACL standards.
*   Les numéros 100 à 199 et 2000 à 2699 sont réservés aux ACL étendues.

---

## Principe de défense en profondeur

*   Réseau Interne

ACL (Acces Control List)

*   ACL simple (standard)
    *   uniquement adresse IPv4 source
*   ACL plus complexe (étendue)
    *   type de protocole,
    *   adresses IPv4 source ou destination
    *   et ports source ou destination

---

## Principe de défense en profondeur

ACL (Acces Control List)

Les listes d'accès utilisent des masques génériques (wildcard mask)

*   Permet le filtrage
*   Permet de mettre en évidence les bits hôtes
*   Lorsqu'un bit aura une valeur de 0 dans le masque, il y aura vérification de ce bit

---

## Conception d'un réseau local

![Image: Schema reseau local]

Redondance de passerelles de routeurs

HSRP Hot Standby Routing Protocol

GLBP Gateway Load Balancing Protocol

VRRP Virtual Router Redundancy Protocol

---

## Principe de défense en profondeur

![Image: Logos antivirus]

---

## Principe de défense en profondeur

![Image: couches défense en profondeur]

---

## Principe de défense en profondeur

![Image: couches défense en profondeur data]

---

## Principe de défense en profondeur

![Image: couches défense en profondeur sauvegarde]

---

## Principe de défense en profondeur

Plan de secours

Plan de secours en cas de dysfonctionnement important (électrique, télécom...) :

*   Double alimentation
*   Onduleur, batterie de secours, groupe électrogène

Accès Internet :

*   Souscription à une offre Internet comme ligne de secours fournie par un opérateur différent.

Avoir une sauvegarde de ses données

*   PRA : Plan de Reprise d'Activité
*   PCA : Plan de Continuité d'Activité

---

## Architecture sécurisée

![Image:Architecture securisée plus complexe]

---

## Architecture sécurisée

![Image:Architecture securisée avec dmz]

---

## Conclusion

Le S.I. est un tout, un maillon faible affaiblir tout l'ensemble.

*   L'attaque peut réussir par l'exploitation d'une seule vulnérabilité ;
*   Tandis que la défense doit prendre en compte l'ensemble du système.

---

## Conclusion

Appliquez la DEP sur le modèle OSI

*   Couches hautes
    *   Séparation fonctionnelle, filtrage applicatif
*   4 Transport
    *   Chiffrement de la communication
*   3 Réseau
    *   Filtrage, segmentation sous rzo, chiffrement de la com
*   2 Liaison
    *   Cloisonnement virtuel, contrôle d'accès logique
*   1 Physique
    *   Utilisation d'équipement différents, contrôle d'accès physique

---

## Architecture sécurisée

Norme et guides nationaux

La réglementation:

*   Référentiel Général de Sécurité (RGS),
*   II 901 systèmes d'information dit << sensibles »
*   Systèmes classifiés de défense: IGI 1300, II 920, etc.
*   Les normes: ISO 2700X (27001, 27002, 27005, etc.), etc.
*   Les méthodes:
    *   Les méthodes de gestion des risques (par ex: EBIOS) ;
    *   Le guide d'intégration de la SSI dans les projets;
    *   Le guide externalisation
*   Les guides de sécurisation (ANSSI, CLUSIF, etc.)
    *   mementodep-v1-1
    *   anssi-guide-passerelle\_internet\_securisee-v3 (Plus de 50 recommandations)
    *   nt commutateurs
*   ETC

---

## Maintenant, c'est à vous !

A vos souris !
