# Hearthstats

**Assistant et tracker de statistiques pour Hearthstone Battlegrounds (Duos & Solo) — 100 % local.**

Hearthstats lit les journaux de partie de Hearthstone **en temps réel** pour construire
automatiquement ton historique, calculer tes statistiques par carte et par héros, et
t'aider à décider quels serviteurs prendre pendant le recrutement.

> ⚠️ **Version alpha.** Le projet est en développement actif : des bugs sont possibles, et le format
> des données peut évoluer entre versions. Tes retours sont les bienvenus.

---

## 📥 Téléchargement

➡️ **[Télécharger la dernière version](../../releases/latest)** → récupère le fichier
`Hearthstats-Setup-<version>.exe` dans la section *Assets*, puis lance-le.

### Premier lancement : avertissement Windows
L'application n'est pas (encore) signée par un certificat payant. Au premier lancement, Windows
SmartScreen peut afficher **« Windows a protégé votre ordinateur »**. C'est normal pour une app
indépendante :

1. Clique sur **Informations complémentaires**.
2. Puis sur **Exécuter quand même**.

Les mises à jour suivantes se font ensuite automatiquement dans l'app (voir plus bas).

---

## ✨ Fonctionnalités

- **Conseil en temps réel** : pendant le recrutement, une fenêtre flottante affiche, pour chaque
  serviteur proposé par Bob, ton taux de victoire en combat **à ce stade de la partie** (par tour /
  palier), avec le nombre de combats observés. Descriptif, jamais prescriptif.
- **Filtre serviteurs** : détecte les tribus actives du lobby au fil des tours et permet de filtrer
  les serviteurs pertinents (tribus / palier / pool actif).
- **Historique des parties** : héros, coéquipier (Duos), placement, déroulé des combats tour par tour,
  plateaux adverses vus, achats et sorts joués.
- **Revoir un combat** : un moteur de **replay** rejoue n'importe quel combat de ton historique
  (attaques, dégâts, morts, râles d'agonie, réincarnations…).
- **Statistiques** : taux de victoire par carte **ventilé par tour**, bilan par héros (placement moyen,
  top-2 en Duos / top-4 en Solo), le tout filtrable par patch.
- **Marquage de cartes** : favori / à tester / à éviter.
- **Référentiel toujours à jour** : les cartes (noms FR, paliers, tribus, mots-clés, images) sont
  dérivées automatiquement des données du jeu et mises à jour à chaque patch.
- **Duos & Solo** pris en charge.

---

## 🔄 Mises à jour automatiques

L'application vérifie au démarrage s'il existe une version plus récente. Si c'est le cas, une bannière
te propose de **télécharger** la mise à jour ; une barre de progression s'affiche, puis un bouton
**Redémarrer** installe la nouvelle version et relance l'app. Rien à faire manuellement.

---

## 🔒 Confidentialité & données

- **100 % local** : ton historique et tes statistiques sont stockés sur ta machine
  (`%AppData%/Hearthstats`), dans une base SQLite. **Aucun compte, aucun serveur, aucune télémétrie.**
- Les seules connexions réseau sortantes sont :
  - le téléchargement des **données de cartes et images** (HearthstoneJSON, licence CC0) ;
  - la **vérification de mise à jour** (lecture anonyme de ce dépôt GitHub).
- Aucune donnée personnelle ni de partie n'est envoyée où que ce soit.

> Tes données restent dans `%AppData%/Hearthstats` même après une mise à jour ou une réinstallation.

---

## 🖥️ Prérequis

- **Windows 10 / 11**.
- **Hearthstone** installé. L'application lit automatiquement les journaux de partie écrits par le jeu
  (`Power.log`) — aucune configuration manuelle nécessaire dans la majorité des cas.

---

## ℹ️ À propos

Le **code source est privé** ; ce dépôt n'héberge que les installeurs et les notes de version.

Hearthstats est un projet indépendant, sans lien avec Blizzard Entertainment. Hearthstone® est une
marque de Blizzard Entertainment, Inc.
