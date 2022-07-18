---
sidebar_position: 2
---

# Créer un site web

Nous allons voir comment créer un site nouveau site web sur la plateforme **Pixilabs**.

## Prérequis

Pour suivre cette partie, assurez-vous que les prérequis suivants soient satisfaits :

- vous devez avoir suivi le guide d'installation,
- connectez-vous à la console d'administration.

## Préparation des données

Pour créer un site web, vous devez d'abord vous rendre dans la partie site web de la console d'administration et créer un site web. Vous devez ensuite vous rendre dans les pages pour en créer une nouvelle et l'attacher au nouveau site web.

## Structure de base d'un site web

La structure de base d'une page web est la suivante :

```json
{
    "meta": {
        "favicon": "images/placeholders/logo_placeholder.png"
    },
    "social": {
        "twitter": "",
        "facebook": "",
        "linkedin": "",
        "whatsapp": "",
        "instagram": "",
        "pinterest": ""
    },
    "navigation": {
        "style": {},
        "responsive-style": {},
        "logo": "images/placeholders/logo_placeholder.png",
        "items": [
            {
                "link": "#accueil",
                "text": "Accueil",
                "style": {},
                "responsive-style": {}
            }
        ]
    },
    "components": []
}
```

## Recaptcha

Pour faire fonctionner le Google Recaptcha avec le nouveau site qui vient d'être créé, il faut ajouter le nom de domaine à la console d'administration de Google Recaptcha.
