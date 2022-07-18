---
sidebar_position: 3
---

# Créer un composant

## Structure de base

La structure de base d'un composant est la suivante :

```json
{
    "id": "custom_id",
    "type": "folder.component-name",
    "style": {},
    "spacing": {
        "top": "y",
        "bottom": "n"
    },
    "options": {} 
}
```

### Propriétés

---

#### id

**Requis :** Non

---

#### type

**Requis :** Oui

**Description :** Représente le composant à afficher. Le nom est formatté ainsi : `nom_du_dossier.nom_du_fichier`. Il représente l'aborescence du fichier contenant le composant. `nom_du_fichier` est le nom du fichier sans l'extension.

---

#### style

**Requis :** Non

---

#### spacing

**Requis :** Non

**Description :** Représente les marges intérieures verticales des composants. `spacing` peut prendre les valeur `y` pour qu'il y ai des marges intérieures, `n` pour qu'il n'y ai pas de marges intérieures ou un object contenant les propriétés `top` et `bottom` pour dissocier le comportement des marges intérieures hautes et basses.

---

#### options

**Requis :** Non

**Description :** Représente les options de configuration proposées par le composant. C'est un objet qui défini les valeurs des options de chaques composants.

---

## Méthodes

### Formatter le style

```html
<div style="{{ @inlineStyle($component['style']) }}">...</div>
```

### Afficher les images

```html
<img src="{{ @loadImage($component['image']) }}" />
```
