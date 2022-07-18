---
sidebar_position: 1
---

# Installation

## Récupérer le code

Le code est disponible sur Github à l'adresse : [https://github.com/Pixilabs/pixilabs](https://github.com/Pixilabs/pixilabs).

Vous pouvez, soit créer un fork, soit si vous avez les droits d'écriture sur le repository, directement cloner le repository.

```bash
git clone https://github.com/Pixilabs/pixilabs.git
```

## Préparer le code

### Variables d'environement

Vous devez ensuite créer le fichier `.env` à partir du fichier `.env.example`.

```bash
cp .env.example .env
```

Ce fichier contient vos variables d'environnement. Elles sont décrites dans le tableau ci-dessous. Toutes les variables d'environement qui ne sont pas dans ce tableau sont celles par défaut de Laravel. Pour plus d'information à leur sujet, il faut se référer à la documentation de Laravel.

| Variables               | Description     | Requis     |
|-------------------------|-----------------|------------|
| APP_DOMAIN              | Le nom de domaine de l'application. Cela peut être par exemple localhost:8000 ou www.pixilabs.local.            | Oui        |
| NOVA_DOMAIN_NAME        | Le nom de domaine sur lequel Laravel Nova doit répondre. Cela peut être par exemple console.pxlabs.local        | Oui       |
| JETSTREAM_DOMAIN_NAME   | Le nom de domaine sur lequel Laravel Jetstream doit répondre. | Oui       |
| GOOGLE_RECAPTCHA_KEY    | Clé publique de google recaptcha. | Non       |
| GOOGLE_RECAPTCHA_SECRET | Clé privée de google recaptcha. | Non       |

### Serveur DNS local

Pour que les noms de domaines www.pixilabs.local, console.pxlabs.local et my.pixilabs.local fonctionnent, vous devez modifier le fichier de configuration `/etc/hosts` avec le contenu suivant :

```text title="/etc/hosts"
127.0.0.1 www.pixilabs.local
127.0.0.1 console.pxlabs.local
127.0.0.1 my.pixilabs.local
```

## Démarrer le serveur

Vous pouvez utiliser votre outil favori pour démarrer un serveur PHP. Cependant, le code contient un fichier `docker-compose.yml` qui se charge de créer toute l'infrastructure pour vous. Si vous le souhaitez, placer vous à la racine du projet et lancez la commande suivante :

```bash
docker-compose up
```

Testez ensuite l'application en lançant la commande suivante directement depuis le conteneur PHP.


```bash
php artisan test
```

Si tous les tests passent alors vous pouvez passer à la suite.

## Administration du site

### Créer un compte administrateur

Pour créer un compte administrateur, vous pouvez utiliser la commande directement fournie par Laravel Nova.

```bash
php artisan nova:user
```

### Connexion au back office

Une fois que vous avez créé votre utilisateur, vous pouvez vous connecter au back office en utilisant ses identifiants. Pour accéder au back office, il vous suffit de vous rendre sur le domaine définie par la variable d'environnement `NOVA_DOMAIN_NAME`.

À partir de la console d'administration, vous allez pouvoir créer votre premier site web.
