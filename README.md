# Exploration des données de prêt de Prosper

### Présenté par Aby DIOUF


### Données des prêt de Prosper

Cet ensemble de données contient 113 937 prêts avec 81 variables sur chaque prêt, y compris le montant du prêt, le taux de l'emprunteur (ou taux d'intérêt), le statut actuel du prêt, le revenu de l'emprunteur, et bien d'autres.

Nous ne sommes pas censé explorer toutes les variables de l'ensemble de données ! Nous avons concentrer notre explorartion sur les  14 variables que voici : le montant initial des emprunts (**LoanOriginalAmount**), le  rendement du prêteur sur le prêt(**LenderYield**), le taux d'intérêt de l'emprunteur sur un emprunt (**BorrowerRate**), le taux annuel effectif global (TAEG) de l'emprunteur pour le prêt (**BorrowerAPR**), le numéro qui identifie de manière unique le listing pour le public tel qu'il est affiché sur le site web (**ListingNumber**), le numéro unique associé à chaque prêt (**LoanNumber**), le status de l'emploi des emprunteurs (**EmploymentStatus**), le status du prêt (**LoanStatus**), la profession des emprunteurs (**Occupation**), le classement de prosper attribué à chaque prêt (**ProsperRating (Alpha)**), de l' adresse de l'emprunteurs (**BorrowerState**), la duréé de chaque prêt (**Term**), le score attribué à chaque prêt (**ProsperScore**) et du nombre d'investisseurs qui ont financé le prêt (**Investors**).

Cette ensemble de données ce trouve sur cette [archive ](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1581581520570000). Vous pouvez consulter ce [dictionnaire](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554486256024000) de données pour comprendre la définition des variables de l'ensemble de données.


### Résumé des resultats

Au cours de mes recherche, j'ai decouvert qu'il existait une forte relation entre le rendement du prêteur, le taux d'intérêt de l'emprunteur, le taux annuel effectif global des prêts et le montant des prêts. Cette relation est approximativement linéaire lorsque le montant est transformé en une échelle logarithmique et que le rendement à l'échelle de la racine cubique. La profession des emprunteurs et le status de l'emploi de l'emprunteur ont aussi un impacte sur les préts et le rendement du prêteur.En plus le status des prêt à une relation claire avec le taux d'interêt des emprunteur.

En dehors des principales variables d'intérêt, j'ai vérifié la relation entre le classement de prosper attribué à chaque prêt et l'addresse des emprunteurs. Pour l'ensemble de données , il y avait une interaction intéressante dans les caractéristiques catégoriques des prêt. Les prêt de plus faible montant semblaient avoir une distribution du rendement et du status de l'emploi de l'emprunteur légèrement moyen important.


### Principales idées pour la présentation

Pour la présentation, je me concentre uniquement sur l'influence des variables comme  le montant initiale de chaque prêt,le rendement du prêteur pour chaque prêt, le taux d'intérêt de l'emprunteur sur le prêt et taux annuel effectif global (TAEG) de l'emprunteur pour le prêt des données de prêt de Prosper et laisse de côté les autres variables numérique. Je commence par introduire la variable montant, suivie par les modèles de distributions du rendement, du taux d'intérêt, taux annuel effectifs puis je trace le diagramme de dispersion transformé du rendement en fonction de chaque prêt.

Ensuite, j'introduis chacune des variables catégorielles une par une. Pour commencer, j'utilise les diagrammes de violon du montant et du rendement en fonction du status du prêt.La proffession des emprunteurs, le statut de l'emploi de l'emprunteur affectent le montants des prêts. Les autres variables catégorielles sont traitées plus loin, à l'aide de graphiques ponctuels.