# Expérimentations en cours au SSP Lab

Le SSP Lab participe à des expérimentations, dont le but est de tester la possibilité d'utiliser une méthode innovante dans un processus de production. Cette page décrit les expérimentations actuellement en cours.

---

## Quel est le parc de véhicules roulants ?

Le Sdes a entrepris la refonte du répertoire des véhicules routiers (RSVERO). Ce projet consiste à apparier les données administratives d'immatriculation des véhicules, utilisées de longue date, à celles des contrôles techniques. L'enjeu est de  distinguer plus précisément les véhicules roulants de ceux retirés de la circulation et de connaître les distances parcourues entre deux contrôles techniques. Mais que ce se passe-t'il avant ou entre deux contrôles techniques ? L'objectif de l'expérimentation est d'essayer d’estimer au 31 décembre de chaque année, pour chaque véhicule routier, une probabilité d’existence et un nombre de kilomètres parcourus au cours des 12 mois précédents, indépendemment de la date effective du contrôle technique.

<u> Méthode utilisée :</u> Machine Learning 
<br>
<u> Date de fin d'expérimentation estimée : </u> Avril 2021
<br>
<u> Conditions de l'expérimentation : </u> Partenariat SSP Lab/SDES

---

## Prévoir la croissance en lisant le journal (extensions et approfondissements)

 L’information produite par les media présente l’avantage d’être réactive, fournie et aborde de nombreux domaines économiques. En outre les techniques récentes d’analyse textuelle (text mining) et de collecte automatisée des données en ligne (web scraping) permettent d’élaborer des indicateurs synthétisant cette richesse. Plus généralement, l’estimation en continu d’un indicateur médiatique associé à l’activité économique peut présenter un intérêt de par sa complémentarité avec les autres enquêtes de conjoncture existantes. Dans l’article [« Prévoir la croissance du PIB en lisant le journal »](https://www.insee.fr/fr/statistiques/fichier/3705976/505-506_Bortoli-Combes-Renault-FR.pdf) de C. Bartoli, S. Combes et T. Renault, les archives du journal Le Monde sont utilisées afin de construire un indicateur aidant à prédire le PIB. Le but de l’expérimentation est de mettre à jour les modèles estimés dans cette étude en mobilisant des sources journalistiques complémentaires et dans un contexte conjoncturel qui s’est depuis un peu assombri. A ce titre, une analyse particulière des périodes de crise passées, notamment celle de 2008, pourrait aider à interpréter les messages issus de l’indicateur construit, en particulier pour pouvoir distinguer les ralentissements modérés des récessions brutales. Des améliorations pourront ensuite être envisagées en utilisant par exemple les méthodes les plus récentes de text mining ou en ciblant mieux les données en entrée.

<u> Méthode utilisée :</u> Text Mining
<br>
<u> Date de fin d'expérimentation estimée : </u> Mars 2021
<br>
<u> Conditions de l'expérimentation : </u> Partenariat SSP Lab/Département de la Conjoncture (Insee)
---

## Utilisation des données de caisse pour évaluer le chiffre d'affaires

 Les données de caisse donnent pour chaque code-barres (ou GTIN), chaque jour et chaque point de ventes les quantités vendues ainsi que le chiffre d’affaires et/ou le prix auquel le produit est vendu. Pour exploiter ces données, il est toutefois nécessaire de savoir quel produit se trouve derrière un code-barres. A cet effet, un référentiel, acheté à un prestataire extérieur, est actuellement  utilisé. Il est toutefois incomplet, et ne permet de toute façon pas de classer les données dans d'autre nomenclature que celle de l'indice des prix à la consommation.

 L'expérimentation en cours vise à tenter de classifier automatiquement les données de caisse dans un référentiel permettant la reconstruction de chiffres d'affaires. Pour cela, un premier échantillon d'entrainement associant description textuelle du produit, code barre, et catégorie de chiffres d'affaires est tout d'abord construit. Cet échantillon est ensuite utilisé pour parvenir à ventiler chaque produit dans une catégorie de chiffres d'affaires. A terme, l'expérimentation devrait ainsi permettre de reconstituer des séries de chiffres d'affaires avec une précision élevée, et avec une capacité d'actualisation et de fréquence optimale.
 
<u> Méthode utilisée :</u> NLP, Machine Learning
<br>
<u> Date de fin d'expérimentation estimée : </u> Été 2021
<br>
<u> Conditions de l'expérimentation : </u> Partenariat SSP Lab/Divsion (Insee)

 ---

## Amélioration de l'identification de l'établissement employeur dans les données du recensement de la population

 L’enjeu de l’expérimentation est d’améliorer le codage automatique de l’établissement employeur, avec l’ambition à terme de réduire la charge de recodage manuel. Il s’agit notamment de retrouver dans le répertoire Sirus l’établissement employeur à partir des informations déclarées dans les enquêtes annuelles de recensement qui peuvent comporter des  erreurs, des inversions de champs, et qui ne sont pas normalisées au sens des nomenclatures. L’expérimentation s’appuie sur les idées et les résultats du hackathon “Les champs de Sirene” ([github](https://github.com/SSP-Lab/Hackathon-2018)) et poursuit les pistes qui y ont été développées.