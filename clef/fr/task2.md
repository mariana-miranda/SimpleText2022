
# SimpleText@CLEF-2022 Tâche 2

[Accueil](./) | [Appel à communication](./CFP) | [Dates importantes](./dates) | [Tâches](./tasks) | [Outils](./tools)  
[Programme](./program) | [Publications](./publications) | [Organisation](./organisation) | [Contacts](./contacts) | [Affiche](./affiche) | [Poster](./poster) | [Video](./video) | [<img src="./en.png" width="30">](../en/CFP)


---

## Directives pour les tâches partagées de SimpleText

Nous vous invitons à soumettre aussi bien des passages automatiques que manuels ! Les interventions manuelles doivent être signalées.

---

<button>[Accès](./tasks)</button> | <button>[Tâche partagée 1](./task1)</button> | <button>[Tâche partagée 2](./task2)</button> | <button>[Tâche partagée 3](./task3)</button> | <button> [Tâche non partagée](./task4) </button>

<br>

## Tâche partagée 2 : Qu'est-ce qui n'est pas clair? Ayant un passage et une requête, classe les termes/concepts à expliquer pour comprendre ce passage (définitions, contexte, applications,...).

L'objectif de cette tâche partagée est de déterminer quels termes (jusqu'à 10) nécessitent une explication et une contextualisation pour aider un lecteur à comprendre un texte scientifique complexe ; par exemple, en ce qui concerne une requête, les termes qui doivent être contextualisés (avec une définition, un exemple et/ou un cas d'utilisation). La regroupement des termes et les métriques automatiques (NDCG,…) seront utilisées pour évaluer ces résultats.


*Fomat de sortie :*  

Liste des termes à contextualiser dans un fichier TSV tabulé avec les champs suivants&nbsp;:
* *run_id* : ID du passage commençant par team_id_
* *manual* : Si l'exécution est manuelle {0,1}
* *topic_id* : ID du sujet
* *passage_text* : Texte du passage
* *term* : Terme ou autre expression à expliquer
* *rank* : Importance de l'explication du terme

Run_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; manual &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; topic_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; passage_text &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; term &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; rank

### Évaluation
Le regroupement de termes et les métriques automatiques (NDCG,...) seront utilisés pour évaluer ces résultats.

Exemple de SORTIE :

| run_id | manual | topic_id | passage_text | term | rank |
|:-------|:-------|:---------|:-------------|:-----|:-----|
| ST_1 | 1 | 1 | Automated decision making based on big data and machine learning (ML) algorithms can result in discriminatory decisions against certain protected groups defined upon personal data like gender, race, sexual orientation etc. Such algorithms designed to discover patterns in big data might not only pick up any encoded societal biases in the training data, but even worse, they might reinforce such biases resulting in more severe discrimination. The majority of thus far proposed fairness-aware machine learning approaches focus solely on the pre-, in- or post-processing steps of the machine learning process, that is, input data, learning algorithms or derived models, respectively. However, the fairness problem cannot be isolated to a single step of the ML process. Rather, discrimination is often a result of complex interactions between big data and algorithms, and therefore, a more holistic approach is required. The proposed FAE (Fairness-Aware Ensemble) framework combines fairness-related interventions at both pre- and postprocessing steps of the data analysis process. In the preprocessing step, we tackle the problems of under-representation of the protected group (group imbalance) and of class-imbalance by generating balanced training samples. In the post-processing step, we tackle the problem of class overlapping by shifting the decision boundary in the direction of fairness.| machine learning | 1 |
| ST_1 | 1 | 1 | Automated decision making based on big data and machine learning (ML) algorithms can result in discriminatory decisions against certain protected groups defined upon personal data like gender, race, sexual orientation etc. Such algorithms designed to discover patterns in big data might not only pick up any encoded societal biases in the training data, but even worse, they might reinforce such biases resulting in more severe discrimination. The majority of thus far proposed fairness-aware machine learning approaches focus solely on the pre-, in- or post-processing steps of the machine learning process, that is, input data, learning algorithms or derived models, respectively. However, the fairness problem cannot be isolated to a single step of the ML process. Rather, discrimination is often a result of complex interactions between big data and algorithms, and therefore, a more holistic approach is required. The proposed FAE (Fairness-Aware Ensemble) framework combines fairness-related interventions at both pre- and postprocessing steps of the data analysis process. In the preprocessing step, we tackle the problems of under-representation of the protected group (group imbalance) and of class-imbalance by generating balanced training samples. In the post-processing step, we tackle the problem of class overlapping by shifting the decision boundary in the direction of fairness.| societal biases | 2 |
| ST_1 | 1 | 1 | Automated decision making based on big data and machine learning (ML) algorithms can result in discriminatory decisions against certain protected groups defined upon personal data like gender, race, sexual orientation etc. Such algorithms designed to discover patterns in big data might not only pick up any encoded societal biases in the training data, but even worse, they might reinforce such biases resulting in more severe discrimination. The majority of thus far proposed fairness-aware machine learning approaches focus solely on the pre-, in- or post-processing steps of the machine learning process, that is, input data, learning algorithms or derived models, respectively. However, the fairness problem cannot be isolated to a single step of the ML process. Rather, discrimination is often a result of complex interactions between big data and algorithms, and therefore, a more holistic approach is required. The proposed FAE (Fairness-Aware Ensemble) framework combines fairness-related interventions at both pre- and postprocessing steps of the data analysis process. In the preprocessing step, we tackle the problems of under-representation of the protected group (group imbalance) and of class-imbalance by generating balanced training samples. In the post-processing step, we tackle the problem of class overlapping by shifting the decision boundary in the direction of fairness. | ML | 3 |  
