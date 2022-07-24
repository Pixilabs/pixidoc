---
sidebar_position: 3
---

# Créer une brique

## Structure de base

La structure de base d'un composant est la suivante :

```json
{
    "id": "custom_id",
    "type": "folder.component-name",
    "style": {},
    "spacing": "tb", // ou "bt" ou "t" ou "b"
    "boxed": "y"
}
```

et voici le code HTML associé :

```html
<div
    @isset($component['id'])
        id="{{ $component['id'] }}"
    @endisset
    @isset($component['style'])
        style="{{ @inlineStyle($component['style']) }}"
    @endisset
    class="
        @isset($component['spacing'])
            @if($component['spacing'] == 't')
                pt-12 md:pt-24
            @elseif($component['spacing'] == 'b')
                pb-12 md:pb-24
            @elseif($component['spacing'] == 'tb' || $component['spacing'] == 'bt')
                py-12 md:py-24
            @endif
        @endif
    ">
    ...
</div>
```

et enfin voici le code pour les briques dites `boxed` :

```html
<div
    class="
        @isset($component['boxed'])
            @if($component['boxed'] == 'y')
                max-w-7xl mx-auto px-4 sm:px-6 lg:px-8
            @endif
        @endisset
    ">
    ...
</div>
```

### Propriétés

---

#### `id`

**Requis :** Non

---

#### `type`

**Requis :** Oui

**Description :** Représente le composant à afficher. Le nom est formatté ainsi : `nom_du_dossier.nom_du_fichier`. Il représente l'aborescence du fichier contenant le composant. `nom_du_fichier` est le nom du fichier sans l'extension.

---

#### `style`

**Requis :** Non

---

#### `spacing`

**Requis :** Non

**Description :** Représente les marges intérieures verticales des composants. `spacing` peut prendre les valeur `t` pour qu'il y ai des marges intérieures supérieures, `b` pour qu'il y ai des marges intérieures inférieures et `tb` ou `bt` pour qu'il y ai des marges intérieures supérieures et inférieures.

---

#### `boxed`

**Requis :** Non

**Description :** La propriété `boxed` permet d'indiquer que l'on veut que la brique soit contrainte au niveau de la largeur.

---

## Javascript

Si une brique a besoin d'utiliser une librairie JavaScript alors il faut regarder en bas du fichier `welcome.blade.php` au niveau des scripts et suivre la même méthode que ce qui est utilisé.

## Méthodes

### Formatter le style

```html
<div style="{{ @inlineStyle($component['style']) }}">...</div>
```

### Afficher les images

```html
<img src="{{ @loadImage($component['image']) }}" />
```
