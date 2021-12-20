
# SimpleText@CLEF-2021 Tâches pilotes

[Accueil](./) | [Appel à communication](./CFP) | [Dates importantes](./dates) | [Tâches pilotes](./tasks)  
[Programme](./program) | [Publications](./publications) | [Organisation](./organisation) | [Contacts](./contacts) | [<img src="../EN.png" width="30">](../en/task3)

---

## Directives pour les tâches pilotes de SimpleText

Nous vous invitons à soumettre aussi bien des passages automatiques que manuels ! Les interventions manuelles doivent être signalées.

---

<button>[Accès](./tasks)</button> | <button>[Tâche pilote 1](./task1)</button> | <button>[Tâche pilote 2](./task2)</button> | <button>[Tâche pilote 3](./task3)</button>

<br>

## Tâche pilote 3 : Simplification de textes scientifiques – Simplification de la langue

L'objectif de cette tâche pilote est de fournir une version simplifiée des passages de texte. Les participants recevront des requêtes et des résumés d'articles scientifiques. Les résumés peuvent être divisés en phrases comme dans l'exemple : [https://guacamole.univ-avignon.fr/nextcloud/index.php/s/SQTdS2Yowf9dxNa](https://guacamole.univ-avignon.fr/nextcloud/index.php/s/SQTdS2Yowf9dxNa).

*Format de sortie :*  

Passages simplifiés dans un fichier TSV tabulé avec les champs suivants :
* *run_id* : ID du passage commençant par team_id_
* *manual* : Si l'exécution est manuelle {0,1}
* *topic_id* : ID du sujet
* *topic_text* : Sujet
* *source_passage* : Texte du passage source
* *simplified_passage* : Texte du passage simplifié

run_id &nbsp;&nbsp;&nbsp;&nbsp; manual &nbsp;&nbsp;&nbsp;&nbsp; topic_id &nbsp;&nbsp;&nbsp;&nbsp; topic_text &nbsp;&nbsp;&nbsp;&nbsp; doc_id &nbsp;&nbsp;&nbsp;&nbsp; source_passage &nbsp;&nbsp;&nbsp;&nbsp; simplified_passage

### Évaluation
Les passages simplifiés seront évalués manuellement avec l'utilisation éventuelle de métriques d'agrégation.

Exemple de SORTIE :

| run_id | manual | topic_id | topic_text | doc_id | source_passage | simplified_passage |
|:-------|:-------|:---------|:-----------|:-------|:---------------|:-------------------|
| BTU | 1 | 1 | Digital assistants like Siri and Alexa entrench gender biases, says UN | 3003409254 | Automated decision making based on big data and machine learning (ML) algorithms can result in discriminatory decisions against certain protected groups defined upon personal data like gender, race, sexual orientation etc. Such algorithms designed to discover patterns in big data might not only pick up any encoded societal biases in the training data, but even worse, they might reinforce such biases resulting in more severe discrimination. | Automated decision-making may include sexist and racist biases and even reinforce them because their algorithms are based on the most prominent social representation in the dataset they use. |
