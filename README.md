LAB-2 : Rooting Android
Étape 1 : Rooter l'AVD
<img width="1090" height="574" alt="image" src="https://github.com/user-attachments/assets/8ee8d5f7-d245-4241-9380-c6c092667f0a" /> <img width="1104" height="382" alt="image" src="https://github.com/user-attachments/assets/2b5afeb8-7b41-4756-94c3-859b5eebf99b" /> <img width="843" height="229" alt="image" src="https://github.com/user-attachments/assets/bd9fa342-618d-4244-9d0f-337330da98ab" />

App + version : DivaApplication v1.0
Support : AVD Android 12 / Device labo
Objectif : Comprendre le rooting et ses impacts
Données : Fictives
Réseau : Test

<img width="1545" height="903" alt="image" src="https://github.com/user-attachments/assets/d15607f6-14b8-4371-978b-a48414e4042c" /> <img width="924" height="144" alt="image" src="https://github.com/user-attachments/assets/e62d677f-72de-4cbb-a9b8-ba7776fae148" />
I. Architecture de Confiance : Focus sur AVB

Android Verified Boot (AVB) est le mécanisme clé de sécurité au démarrage.
Il utilise une signature cryptographique pour vérifier l’intégrité de chaque partition avant son chargement.

Objectifs :

Validation d’intégrité : Assurer qu’aucun fichier système n’a été modifié ou corrompu.

Protection Anti-Rollback : Empêcher le retour vers une version ancienne vulnérable.

Remarque en labo : L’état de l’AVB peut être vérifié sur un appareil de test pour confirmer l’intégrité du système.

II. Méthodologie du Rooting en Audit

Le rooting permet d’obtenir les droits de super-utilisateur, offrant un contrôle total sur le système Android et brisant le modèle de confiance standard.

Utilité :

Analyse approfondie des comportements internes des applications

Audit de zones normalement verrouillées

Gestion des risques :

Environnement strictement isolé

Documentation détaillée de chaque modification

Réinitialisation complète après chaque test

III. Protocole de Sécurité du Laboratoire

Pour garantir la sécurité et l’intégrité des tests :

Confinement : Utilisation de réseaux dédiés et d’appareils réservés aux tests

Hygiène des données : Données fictives uniquement, aucun compte personnel

Gestion des traces : Snapshots ou wipes fréquents pour effacer toute empreinte

Maîtrise logicielle : Contrôle strict des APK installées pour éviter l’introduction de codes non audités

IV. Référentiel OWASP (MASVS & MASTG)
Analyse du Stockage (MSTG-STORAGE-1)

Principe : Interdiction de stocker des secrets (mots de passe, clés API) sans protection cryptographique.

Test en audit : Exploration du stockage local de l’application. Toute donnée sensible lisible en clair indique une non-conformité.

Analyse Réseau (MSTG-NETWORK-1)

Principe : Toutes les communications doivent être chiffrées via TLS (HTTPS).

Test audit : Toute interception lisible via proxy constitue une non-conformité.

Analyse des Flux Logcat

Principe : L’application ne doit pas divulguer d’informations sensibles dans les journaux système.

Test audit : Toute fuite d’identifiants ou de clés dans les logs indique une vulnérabilité.

V. Bonnes pratiques en environnement de test

Réseau isolé et données fictives

Appareil dédié ou AVD réservé aux tests

Snapshots ou wipes après chaque session

Journal détaillé pour audit et reproductibilité

Aucun compte personnel utilisé

Contrôle strict des APK installées

VI. Fiche Environnement : Pixel 6 (AVD)
<img width="363" height="790" alt="image" src="https://github.com/user-attachments/assets/a985725f-7671-4463-9f76-1e6a99ba9f77" /> <img width="357" height="785" alt="image" src="https://github.com/user-attachments/assets/94cd27cb-99df-458e-9aa4-7239f204084a" />
