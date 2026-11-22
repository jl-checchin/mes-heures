# Mes Heures – Aide à domicile

Appli téléphone pour les aides à domicile (FPT) : planning, heures effectuées, kilomètres,
congés, jours fériés, panier d'heures complémentaires.

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html` | L'appli complète |
| `manifest.webmanifest` | Nom et icône quand on l'installe sur le téléphone |
| `sw.js` | Fonctionnement sans réseau |
| `icon-*.png`, `apple-touch-icon.png`, `icon.svg` | Icônes |

## Mise en ligne (une seule fois)

1. Sur GitHub, créer un dépôt **public** nommé `mes-heures`.
2. Y déposer **tous** les fichiers de ce dossier (bouton *Add file → Upload files*).
3. Dans le dépôt : *Settings → Pages* → *Source : Deploy from a branch* → branche `main`, dossier `/ (root)` → *Save*.
4. Après 1 ou 2 minutes, l'appli est en ligne à l'adresse :
   `https://jl-checchin.github.io/mes-heures/`

## Installer sur le téléphone

- **Android (Chrome)** : ouvrir le lien → menu ⋮ → *Ajouter à l'écran d'accueil* (ou *Installer l'application*).
- **iPhone (Safari)** : ouvrir le lien → bouton *Partager* → *Sur l'écran d'accueil*.

Ouvrir l'appli une première fois avec du réseau. Ensuite elle fonctionne même sans réseau.

## Mettre à jour l'appli

Remplacer `index.html` (et les autres fichiers modifiés) sur GitHub.
Les téléphones récupèrent la nouvelle version à la prochaine ouverture avec du réseau.
**Les données des aides ne sont pas effacées.**

## Les données

- Elles restent **uniquement sur le téléphone** de chaque aide (rien n'est envoyé ailleurs).
- *Réglages → Sauvegarder dans un fichier* : à faire au moins une fois par mois.
- *Réglages → Restaurer une sauvegarde* : pour un nouveau téléphone.
- Attention : vider les données du navigateur ou désinstaller l'appli efface tout → d'où la sauvegarde.

## Règles de calcul utilisées

- Heures d'une journée = contrat mensuel ÷ (jours travaillés par semaine × 52 ÷ 12).
- Congés, fériés non travaillés, maladie et ASA comptent comme des heures faites (au forfait journée).
- Panier d'heures complémentaires = total du mois au-delà du contrat (jauge pleine à 10 h).
- Droit à congés = 5 × jours travaillés par semaine (décret n° 85-1250, art. 1), au prorata en cas d'arrivée en cours d'année.
- Congés décomptés en jours ouvrés (jours travaillés de l'agent, hors fériés).
- Jours de fractionnement (règle de la collectivité) : jours posés en janvier–mars et octobre–décembre ;
  5 ou 6 jours → +1 jour, 7 jours et plus → +2 jours (maximum 2).
- Maladie : 1 jour de carence signalé (non rémunéré).
