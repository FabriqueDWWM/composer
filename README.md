# Composer

## Installation

L'univers (on dit aussi écosystème) **PHP** est empreint de références musicales.

A tout seigneur, tout honneur, voici **Composer** !

Allez, on l'installe => [Composer](https://getcomposer.org/). Cliquer dur Download. Pour **Linux**, c'est le paragraphe intitulé **Command-line installation**. ;-)

Ok, maintenant, assurez-vous que **Composer** est intallé globalement en tapant la commande `composer -v` dans un terminal.

## A quoi ça sert ?

Bon d'accord, mais ça sert à quoi ?

Tu connais **npm** le gestionnaire de librairies de **NodeJs** ? Ben c'est la même chose, mais pour **PHP**.

Avec **Composer**, on peut donc installer n'importe quelle librairie hébergée sur **Packagist** pour l'utiliser dans notre projet. Enorme !

Allez, on se lance, on va installer une librairie (on dit package aussi) qui sert à afficher des **var_dump** plus jolis !

## Création d'un projet Php

Ben, on crée juste un dossier dans notre répertoire web.

## Installation du package VarDumper

On va sur [Packagist](https://packagist.org/packages/symfony/var-dumper). On trouve le package **symfony/var-dumper**.

Dans le terminal (dans le répertoire du projet), on colle la commande `composer require symfony/var-dumper`.

Et bam, le package est installé ! On a un répertoire **vendor** qui contient les fichiers du package (on dit aussi Component chez **Symfony**), un fichier **composer.json** et un fichier **composer.lock**. Allez donc voir ce que contiennent ces 2 fichiers !

## Utilisation du package

Sur la page [Packagist](https://packagist.org/packages/symfony/var-dumper), il y a un lien [Documentation](https://symfony.com/doc/current/components/var_dumper.html) qui dirige vers la doc de **Symfony** :-o.

Testez la fonction dump().

...si vous n'y arrivez pas, parlez-vous ! ;-)

Lorsque vous utiliserez **Symfony**, vous vous servirez beaucoup de la commande `composer require` pour installer des packages (ou encore components, ou encore bundles...jargon quoi...).

Bon c'est bien, c'est un peu magique, alors jetez quand même un oeil au code du fichier `vendor/autoload.php`, c'est quand même lui qui fait le taf ( on voit ça juste après ;-) ) !

## Un autre : Monolog

La librairie Monolog permet d'enregistrer des messages (des logs) dans un fichier pour pouvoir consulter les erreurs produites par le code. C'est très utile en production, car les erreurs ne s'affichent pas dans le navigateur !

Même chose que précédemment, on l'installe avec Composer et on voit comment l'utiliser.

L'objectif est d'enregistrer les erreurs dans un fichier dans l'environnement de production, et de les afficher dans le navigateur dans l'environnement de développement.

## Encore un : GuzzleClient

Cette bibliothèque sert à créer des requêtes Http, par exemple pour récupérer des données sur une Api.

Nous allons l'utiliser de la manière suivante :

-   création d'une api sur [mockaroo](https://mockaroo.com/)
-   récupération des données au format json
-   enregistrement des données en bdd
    -   création de la bdd
    -   création de la table
    -   enregistrement des données
