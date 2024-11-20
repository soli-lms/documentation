# documentation

Ce dépôt centralise tous les documents liés à l'analyse, la conception, et le rapport final de Soli-LMS.

## Cloner le dépôt

````bash
git clone https://github.com/soli-lms/soli-lms_documentation.git
#Initialiser et mettre à jour les sous-modules
git submodule init
git submodule update
````

## Insertion des modules au dépôt

````bash
git submodule add https://github.com/soli-lms/pkg_rh_docs.git pkg_rh
git submodule add https://github.com/soli-lms/pkg_competences_docs.git pkg_competences
git submodule add https://github.com/soli-lms/pkg_creation_projets_docs.git pkg_creation_projets
git submodule add https://github.com/soli-lms/pkg_realisation_projets_docs.git pkg_realisation_projets
git submodule add https://github.com/soli-lms/pkg_validations_docs.git pkg_validations
git submodule add https://github.com/soli-lms/pkg_suivi_docs.git pkg_suivi
git submodule add https://github.com/soli-lms/pkg_autorisation_docs.git pkg_autorisation
````


## Exécution de rapport localement sans github pages
 
````bash

# Installation de bundler 
gem install bundler

````

````bash
# Installation
bundle install

# Exécution
serve.ps1
````


## Rapport et Présentation 

- [Rapport](https://soli-lms.github.io/soli-lms_docs/)
- [Présentation](https://soli-lms.github.io/soli-lms_docs/)
