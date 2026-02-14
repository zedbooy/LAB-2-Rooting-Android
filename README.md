LAB-2-Rooting-Android
Étape 1 : Rooter l'AVD
<img width="1090" height="574" alt="image" src="https://github.com/user-attachments/assets/8ee8d5f7-d245-4241-9380-c6c092667f0a" /> <img width="1104" height="382" alt="image" src="https://github.com/user-attachments/assets/2b5afeb8-7b41-4756-94c3-859b5eebf99b" /> <img width="843" height="229" alt="image" src="https://github.com/user-attachments/assets/bd9fa342-618d-4244-9d0f-337330da98ab" />

App + version : DivaApplication v1.0
Support : AVD Android 12 / Device labo
Objectif : Comprendre rooting et impacts
Données : Fictives
Réseau : Test

<img width="1545" height="903" alt="image" src="https://github.com/user-attachments/assets/d15607f6-14b8-4371-978b-a48414e4042c" /> <img width="924" height="144" alt="image" src="https://github.com/user-attachments/assets/e62d677f-72de-4cbb-a9b8-ba7776fae148" />
AVB – Android Verified Boot

AVB est la version moderne de Verified Boot. Il vérifie l’intégrité du système au démarrage pour s’assurer que les partitions n’ont pas été modifiées et inclut une protection anti-rollback pour empêcher l’installation de versions vulnérables.

Rooting (Privilèges Super-Utilisateur)

Le rooting permet d’obtenir un contrôle total sur Android, en accédant et modifiant toutes les ressources du système. Utile en laboratoire pour analyser et tester la sécurité, mais risqué en environnement réel, nécessitant isolement, traçabilité et réinitialisation après usage.

Bonnes pratiques en environnement de test

Réseau isolé et données fictives

Appareil dédié ou AVD pour tests

Snapshots ou wipe après chaque session

Journal détaillé pour audit et reproductibilité

Pas de compte personnel

Contrôle strict des APK

Exigences OWASP MASVS

Stockage sécurisé : Ne jamais enregistrer de mots de passe ou clés API en clair.

Communication sécurisée : Toutes les communications doivent utiliser TLS (HTTPS).

Tests recommandés

Stockage local : Vérifier si des secrets sont stockés sans chiffrement.

Logs système : Contrôler que l’application ne divulgue pas d’informations sensibles dans les journaux.

Fiche Environnement : Pixel 6 (AVD)
<img width="363" height="790" alt="image" src="https://github.com/user-attachments/assets/a985725f-7671-4463-9f76-1e6a99ba9f77" /> <img width="357" height="785" alt="image" src="https://github.com/user-attachments/assets/94cd27cb-99df-458e-9aa4-7239f204084a" />
