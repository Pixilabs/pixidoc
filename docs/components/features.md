---
sidebar_position: 1
---

# Fonctionnalités

You have just learned the **basics of Docusaurus** and made some changes to the **initial template**.

Docusaurus has **much more to offer**!

## Fonctionnalités 2

![Capture d'écran Fonctionnalités 2](./img/feature-2.png)

**Nom :** `feature-2`

**Fichier :** `resources/views/components/features/features-2.blade.php`

### Propriétés

---

#### id

**Requis :** Non

---

#### style

**Requis :** Non

---

#### features

**Requis :** Oui

---

#### features.icon

**Requis :** Non

---

#### features.icon.svg

**Requis :** Oui

**Description :** Code HTML de l'icône au format SVG.

---

#### features.icon.style

**Requis :** Non

---

#### features.title

**Requis :** Oui

---

#### features.title.text

**Requis :** Oui

---

#### features.title.style

**Requis :** Non

---

#### features.paragraph

**Requis :** Oui

---

#### features.paragraph.text

**Requis :** Oui

---

#### features.paragraph.style

**Requis :** Non

---

### Examples

![Capture d'écran Fonctionnalités 2](./img/feature-2.png)

```json
{
    "type": "features.features-2",
    "style": {
        "background-color": "#F3F4F6"
    },
    "features": [
        {
            "icon": {
                "svg": "<svg aria-hidden='true' focusable='false' data-prefix='fal' data-icon='cube' role='img' xmlns='http:\/\/www.w3.org\/2000\/svg' viewBox='0 0 512 512' class='h-6 w-6'><path fill='currentColor' d='M239.1 6.3l-208 78c-18.7 7-31.1 25-31.1 45v225.1c0 18.2 10.3 34.8 26.5 42.9l208 104c13.5 6.8 29.4 6.8 42.9 0l208-104c16.3-8.1 26.5-24.8 26.5-42.9V129.3c0-20-12.4-37.9-31.1-44.9l-208-78C262 2.2 250 2.2 239.1 6.3zM256 34.2l224 84v.3l-224 97.1-224-97.1v-.3l224-84zM32 153.4l208 90.1v224.7l-208-104V153.4zm240 314.8V243.5l208-90.1v210.9L272 468.2z'><\/path><\/svg>",
                "style": []
            },
            "title": {
                "text": "Votre 1er argument",
                "style": []
            },
            "paragraph": {
                "text": "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maiores impedit perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.",
                "style": []
            }
        },
        {
            "icon": {
                "svg": "<svg aria-hidden='true' focusable='false' data-prefix='fal' data-icon='cube' role='img' xmlns='http:\/\/www.w3.org\/2000\/svg' viewBox='0 0 512 512' class='h-6 w-6'><path fill='currentColor' d='M239.1 6.3l-208 78c-18.7 7-31.1 25-31.1 45v225.1c0 18.2 10.3 34.8 26.5 42.9l208 104c13.5 6.8 29.4 6.8 42.9 0l208-104c16.3-8.1 26.5-24.8 26.5-42.9V129.3c0-20-12.4-37.9-31.1-44.9l-208-78C262 2.2 250 2.2 239.1 6.3zM256 34.2l224 84v.3l-224 97.1-224-97.1v-.3l224-84zM32 153.4l208 90.1v224.7l-208-104V153.4zm240 314.8V243.5l208-90.1v210.9L272 468.2z'><\/path><\/svg>",
                "style": []
            },
            "title": {
                "text": "Votre 2eme argument",
                "style": []
            },
            "paragraph": {
                "text": "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maiores impedit perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.",
                "style": []
            }
        },
        {
            "icon": {
                "svg": "<svg aria-hidden='true' focusable='false' data-prefix='fal' data-icon='cube' role='img' xmlns='http:\/\/www.w3.org\/2000\/svg' viewBox='0 0 512 512' class='h-6 w-6'><path fill='currentColor' d='M239.1 6.3l-208 78c-18.7 7-31.1 25-31.1 45v225.1c0 18.2 10.3 34.8 26.5 42.9l208 104c13.5 6.8 29.4 6.8 42.9 0l208-104c16.3-8.1 26.5-24.8 26.5-42.9V129.3c0-20-12.4-37.9-31.1-44.9l-208-78C262 2.2 250 2.2 239.1 6.3zM256 34.2l224 84v.3l-224 97.1-224-97.1v-.3l224-84zM32 153.4l208 90.1v224.7l-208-104V153.4zm240 314.8V243.5l208-90.1v210.9L272 468.2z'><\/path><\/svg>",
                "style": []
            },
            "title": {
                "text": "Votre 3eme argument",
                "style": []
            },
            "paragraph": {
                "text": "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maiores impedit perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.",
                "style": []
            }
        }
    ]
}
```
