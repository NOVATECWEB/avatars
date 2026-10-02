# avatars

Les images publiques qui servent d'avatar aux applications et aux webhooks Google Chat de Novatec.

## À quoi sert ce dépôt

Google Chat ne permet pas de téléverser l'avatar d'une application ou d'un webhook. Il demande une
**URL HTTPS publique** vers une image PNG carrée, qu'il va chercher lui-même, sans être connecté à
aucun compte. Ce dépôt fournit ces URL :

```
https://raw.githubusercontent.com/NOVATECWEB/avatars/main/<fichier>
```

Pourquoi un dépôt plutôt qu'un fichier Drive : le 2 octobre 2026, la même icône partagée depuis
Google Drive avec « Tous les utilisateurs disposant du lien » (en 128 px) s'affichait dans Chat avec
l'avatar par défaut. Servie depuis ce dépôt en 512 px, elle s'affiche.

## Règles

- ⚠ **Ce dépôt est public.** N'y déposer que des images destinées à être vues de tous : rien
  d'interne, aucun document, aucune configuration.
- Une image par application ou par webhook, en **PNG carré**, de préférence en **512 × 512**.
  Google recommande au moins 256 × 256.
- Le fichier porte le nom de l'application, en minuscules (`stewart.png`).
- Remplacer un fichier garde la même URL. Chat peut mettre quelques minutes à rafraîchir l'icône.

## Inventaire

| Fichier | Taille | Utilisé par |
|---|---|---|
| `stewart.png` | 512 × 512 | l'application Google Chat « Stewart » |

Où coller l'URL :
- **une application** : console Google Cloud › API Google Chat › onglet *Configuration* › champ
  *Avatar URL* ;
- **un webhook** : dans le salon › *Applis et intégrations* › *Webhooks* › modifier le webhook ›
  *URL de l'avatar*.

## Crédits

Icône de Stewart : « Butler », [IconScout](https://iconscout.com/icon/butler-icon_4121435).
