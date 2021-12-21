
# SimpleText@CLEF-2022 Tâches

[Accueil](./) | [Appel à communication](./CFP) | [Dates importantes](./dates) | [Tâches](./tasks)  
[Programme](./program) | [Publications](./publications) | [Organisation](./organisation) | [Contacts](./contacts) | [Affiche](./affiche) | [Poster](./poster) | [Video](./video) | [<img src="./en.png" width="30">](../en/CFP)


---

## Directives pour les tâches pilotes de SimpleText

Nous vous invitons à soumettre aussi bien des passages automatiques que manuels ! Les interventions manuelles doivent être signalées.

---

<button>[Accès](./tasks)</button> | <button>[Tâche partagée 1](./task1)</button> | <button>[Tâche partagée 2](./task2)</button> | <button>[Tâche partagée 3](./task3)</button> | <button> [Tâche non partagée](./task4) </button>

<br>

## Accès
Veuillez vous inscrire à l'atelier SimpleText@CLEF afin d'accéder aux données : [https://clef2022.clef-initiative.eu](https://clef2022.clef-initiative.eu/)  
Après l'inscription, vous recevrez un courriel contenant les informations nécessaires pour vous connecter au serveur de données.

### Soumission des résultats :
Les participants doivent placer leurs résultats dans le dossier Documents créé pour leur utilisateur.

### 2022 - Dataset
Pour cette édition, nous utilisons le Citation Network Dataset : DBLP+Citation, ACM Citation network ([https://www.aminer.org/citation](https://www.aminer.org/citation)). Un index Elasticsearch est mis à la disposition des participants et est accessible via une API GUI. Cet index est adapté pour :
*	appliquer des méthodes de base de recherche de passages basées sur des modèles de RI vectoriels ou linguistiques,
*	générer des modèles d'allocation de Dirichlet latente,
*	former des Graph Neural Networks pour la recommandation de citations, comme c'est le cas sur [https://stellargraph.readthedocs.io/](https://stellargraph.readthedocs.io/) par exemple, 
*	appliquer des Transformers bidirectionnels profonds pour l'expansion des requêtes,
*	et bien plus encore...

### 2022 - Requêtes
Pour cette édition, les requêtes sont une sélection de titres de presse récents du Guardian enrichis de mots-clés extraits manuellement du contenu de l'article. Il a été vérifié que chaque mot-clé permet d'extraire au moins 5 résumés pertinents. L'utilisation de ces mots-clés est facultative.

*Format d'entrée pour toutes les tâches :*
* Sujets au format MD

<img src="../Query1.png">

* Articles en texte intégral du Guardian (lien, dossier query_related_content avec textes intégraux au format MD)
* Index ElasticSearch sur le serveur de données suivant (par exemple) : [https://guacamole.univ-avignon.fr/nextcloud/index.php/apps/files/?dir=/simpleText/queries&fileid=570352](https://guacamole.univ-avignon.fr/nextcloud/index.php/apps/files/?dir=/simpleText/queries&fileid=570352)
* Dépôt complet du DBLP au format JSON.GZ
* Extraction des résumés DBLP pour chaque sujet dans le format MD suivant (doc_id, year, abstract) :

<img src="../MDformat.png">
