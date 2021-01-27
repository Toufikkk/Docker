# Docker
<p align="center">
  <h1 align="center">Docker Project</h1>
</p>

## Table des matières
>   * [Infos Générales / Prérequis]
>   * [Architecture du projet]
	- [Installation]
		- Variables d'environnement
		- Docker
>	* Notes supplémentaires

## Infos Générales / Prérequis
Prérequis : PHP 7.2.9 ou supérieur, Docker, Composer, Symfony CLI

- Création d'un projet symfony "symfony-demo" à partir d'un projet démo :
https://github.com/symfony/demo

## Architecture du projet
1/ ./symfony-demo/: contient tous les codes sources
2/ ./data/: contient la database sqlite
3/ .gitignore: afin d'extraire les fichiers de git
4/ docker-compose.yml: contient les configurations des conteneurs
5/ README: documentation pour les devs du projet

## Installation
Installation : Symfony, PHP, Composer

## Variables Environnement
KERNEL_CLASS = 'App\Kernel'
APP_SECRET = '$ecretf0rt3st'
SYMFONY_DEPRECATIONS_HELPER = 999999
PANTHER_APP_ENV = panther
DATABASE_URL = sqlite:///%kernel.project_dir%/data/database_test.sqlite

## Docker
- Pour lancer docker : docker-compose up -d
- Pour construire : docker build -t iddockerhub/name .
- Pour mettre sur dockerhub : docker push iddockerhub/name

## Notes supplémentaires
Deux images ont été push sur dockerhub "docker_project" & "docker_project2"
