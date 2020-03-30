[![Build Status](https://travis-ci.com/Jebay/Instance-Configuration.svg?branch=master)](https://travis-ci.com/Jebay/Instance-Configuration)

# Instance-Configuration
Creation d'une instance sur Scaleway

## Token
Créer un token sur le site de Scaleway pour les accès distants et le stocker dans un fichier scaleway_token
`export SCW_API_KEY='aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa'`

Sourcer le fichier
`source scaleway_token`

## Création d'une VM
Le playbook [`00_scaleway_setup.yml`](00_scaleway_setup.yml) permet de générer une instance sur [Scaleway](https://console.scaleway.com).

## Configuration de la VM
Le playbook [`10_configure.yml`](10_configure.yml) permet de configurer l'instance précédement créée.

## Destruction de la VM
Le playbook [`00_scaleway_destroy.yml`](00_scaleway_destroy.yml) permet de supprimer l'instance.