# documentation

Ce dépôt centralise tous les documents liés à l'analyse, la conception, et le rapport final de Soli-LMS.

## **Problème à fixer avec branche develop : Revenir dans l'historique**  

#### **Problème :**
En date du **samedi 16/11/2024**, une désynchronisation a été constatée entre la branche locale `develop` et son équivalent distant `origin/develop`.  

Concrètement :  
- La branche distante `origin/develop` pointe sur un commit antérieur à celui de la branche locale `develop`.  
- Cela peut arriver lorsque lorsque la branche distante a été réinitialisée à un état antérieur.
---

#### **Solution :**  
Pour résoudre ce problème et aligner la branche locale `develop` avec l’état actuel de la branche distante `origin/develop`, vous devez exécuter les commandes suivantes :  

```bash
git checkout develop
git reset --hard origin/develop
```

**`git reset --hard origin/develop`** :  
   - Cette commande force la branche locale `develop` à pointer exactement sur la même référence (commit) que la branche distante `origin/develop`.  
   - Elle supprime tous les changements locaux (commits, modifications non ajoutées ou non commitées) qui ne sont pas présents sur la branche distante.

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

git submodule add https://github.com/soli-lms/pkg_creation_tache_docs.git pkg_creation_tache
git submodule add https://github.com/soli-lms/pkg_qcm_apprenant_docs.git pkg_qcm_apprenant
git submodule add https://github.com/soli-lms/pkg_realisation_tache_docs.git pkg_realisation_tache
git submodule add https://github.com/soli-lms/pkg_formation_docs.git pkg_formation
````


## Exécution de rapport localement sans github pages



````bash
# Installation
bundle install

# Exécution
serve.ps1
````


## Rapport et Présentation 

- [Rapport](https://soli-lms.github.io/soli-lms_docs/)
- [Présentation](https://soli-lms.github.io/soli-lms_docs/)
