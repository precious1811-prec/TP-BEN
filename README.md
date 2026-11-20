# CV Flutter — AMINI-TU BEN

Application de CV et de présentation personnelle réalisée avec Flutter. Le
design a été volontairement simplifié : fond uni, couleurs de base et cartes
rectangulaires. L’application n’utilise plus de photos personnelles.

## Résumé

AMINI-TU BEN est présenté comme étudiant en informatique et développeur en
devenir à Goma, en République démocratique du Congo. Le CV présente une
formation en informatique, des projets académiques, des compétences techniques,
des langues et des centres d’intérêt.

La rubrique famille contient des noms d’exemple utilisant tous le nom
« AMINI-TU ». Les informations de formation, de famille et de contact sont des
exemples à vérifier et à remplacer avant de partager l’application.

## Fonctionnalités

- Écran de connexion de démonstration avec validation des champs.
- Page **Mon CV** : profil, formation, projets, compétences et intérêts.
- Page **Ma famille** : membres présentés avec des initiales, sans photos.
- Page **Contact** : actions pour appeler, envoyer un e-mail, copier l’adresse
  et consulter des liens sociaux.
- Menu latéral et barre de navigation.
- Présentation responsive pour petits et grands écrans.

### Identifiants de démonstration

| Champ | Valeur |
|---|---|
| Identifiant | `amini` |
| Mot de passe | `ben2026` |

Ces identifiants sont codés dans l’application pour la démonstration. La
connexion ne constitue pas un système d’authentification sécurisé.

## Technologies

- Flutter et Dart
- Material 3
- [`url_launcher`](https://pub.dev/packages/url_launcher) pour les actions de
  contact
- `flutter_test` pour les tests d’interface

Le projet inclut des configurations pour Android, iOS, le Web, Windows, macOS
et Linux. La compilation de chaque cible nécessite les outils correspondants.

## Prérequis

- Flutter installé et configuré (`flutter doctor`)
- Une version de Dart compatible avec la contrainte du projet (`^3.14.0`)
- Un navigateur, un appareil ou un émulateur pour la cible choisie

## Installation et lancement

Depuis le dossier du projet :

```bash
flutter pub get
flutter run
```

Pour lancer la version Web dans Chrome :

```bash
flutter devices
flutter run -d chrome
```

## Tests et analyse

```bash
flutter test
flutter analyze
```

Le test d’interface vérifie la connexion de démonstration et la navigation
entre les pages CV, famille et contact.

## Structure du projet

```text
.
├── lib/main.dart       # Écrans et composants de l’application
├── test/               # Tests d’interface
├── android/            # Configuration Android
├── ios/                # Configuration iOS
├── linux/              # Configuration Linux
├── macos/              # Configuration macOS
├── web/                # Configuration Web
├── windows/            # Configuration Windows
├── pubspec.yaml        # Dépendances Flutter
└── pubspec.lock        # Versions résolues des dépendances
```

Les photos du profil et de la famille, les captures d’écran et leur archive ZIP
ont été retirées. Les icônes techniques nécessaires aux plateformes sont
conservées.

## Personnalisation

Les noms, descriptions, coordonnées et liens sont définis dans
`lib/main.dart`. Modifiez les identifiants de démonstration dans le même fichier
si vous souhaitez en utiliser d’autres.
