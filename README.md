# Mise en place d'un SOC Cloud Sentinel pour la sécurisation d'infrastructures Linux

Projet réalisé par **HAMEG Sami**.

## Objectif
Déployer et valider un SOC Cloud basé sur **Microsoft Sentinel** pour détecter et traiter des tentatives de compromission SSH sur une infrastructure Linux.

## Étapes du projet
1. **Création d'une VM Ubuntu** dans Azure pour servir de cible Linux.
2. **Déploiement de Microsoft Sentinel** sur un workspace Log Analytics.
3. **Configuration de l'agent AMA et des DCR** pour la collecte des logs Linux.
4. **Création d'une règle KQL** pour détecter les attaques par force brute SSH.
5. **Réalisation d'un test d'intrusion** (tentatives SSH invalides) pour valider la détection.
6. **Hardening réseau via NSG** pour réduire la surface d'attaque.
7. **Extinction propre des ressources** afin de limiter les coûts et clôturer le projet.

## Tableau des screenshots
| Étape | Screenshot attendu | Emplacement |
|---|---|---|
| 1 | VM Ubuntu déployée | `screenshots/01-vm-ubuntu.png` |
| 2 | Sentinel activé sur le workspace | `screenshots/02-sentinel-deploiement.png` |
| 3 | AMA + DCR configurés | `screenshots/03-ama-dcr.png` |
| 4 | Règle KQL brute force SSH | `screenshots/04-regle-kql.png` |
| 5 | Résultats du test d'intrusion | `screenshots/05-test-intrusion.png` |
| 6 | Règles NSG renforcées | `screenshots/06-hardening-nsg.png` |
| 7 | Ressources arrêtées proprement | `screenshots/07-extinction-propre.png` |

## Compétences démontrées
- Déploiement d'une architecture SOC Cloud sur Azure.
- Intégration de sources Linux dans Microsoft Sentinel via AMA/DCR.
- Écriture de requêtes KQL orientées détection sécurité.
- Validation opérationnelle par simulation d'attaque (brute force SSH).
- Renforcement de la posture sécurité réseau avec NSG.
- Gestion du cycle de vie des ressources cloud (arrêt et maîtrise des coûts).
