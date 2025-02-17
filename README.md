# Segmentation des Clients avec K-Means

## 📌 Présentation
Ce projet vise à analyser et segmenter des clients en fonction de leurs comportements d'achat et de leurs caractéristiques démographiques. Nous utilisons **l'algorithme K-Means** pour identifier des groupes de clients ayant des profils similaires, ce qui permet d'optimiser les stratégies marketing et d'améliorer la compréhension des tendances d'achat.

## 📂 Contenu du dépôt
- **Mall_Customers.csv** : Dataset utilisé pour l'analyse.
- **Segmentation_Client.ipynb** : Notebook Jupyter contenant l'analyse, la segmentation et les visualisations.
- **requirements.txt** : Liste des dépendances nécessaires à l'exécution du projet.
- **README.md** : Documentation du projet.

## 📊 Données utilisées
Le dataset comprend les colonnes suivantes :
- **CustomerID** : Identifiant unique du client
- **Genre** : Sexe du client (Male/Female)
- **Age** : Âge du client
- **Annual Income (k$)** : Revenu annuel du client en milliers de dollars
- **Spending Score (1-100)** : Score de dépense attribué par le magasin (basé sur le comportement d'achat et la fidélité)

## 🔍 Méthodologie
1. **Prétraitement des données** : Nettoyage, gestion des valeurs manquantes, normalisation si nécessaire.
2. **Exploration des données** : Analyse statistique et visualisation des distributions.
3. **Application de K-Means** : Détermination du nombre optimal de clusters (méthodes du coude et silhouette) et exécution de l'algorithme.
4. **Analyse des clusters** : Interprétation des résultats et visualisation des groupes.

## 📌 Segmentation des Clients
Nous avons identifié **5 groupes de clients distincts** :

### 1️⃣ Cluster 0 (Violet) :
- Très large dispersion des âges, de moins de 20 ans à plus de 70 ans.
- Médiane autour de 45 ans.
- Cluster avec la plus grande diversité d’âges.

### 2️⃣ Cluster 1 (Bleu foncé) :
- Jeunes adultes (~25-40 ans).
- Moins dispersé que le Cluster 0.
- Médiane autour de 35 ans.

### 3️⃣ Cluster 2 (Bleu clair) :
- Population très jeune, majoritairement sous 30 ans.
- Faible dispersion, bien concentré autour de la vingtaine.
- Médiane autour de 25 ans.

### 4️⃣ Cluster 3 (Vert foncé) :
- Regroupe principalement des personnes autour de 40-50 ans.
- Dispersion modérée (20-60 ans).
- Légère dominance des hommes dans ce groupe.

### 5️⃣ Cluster 4 (Vert clair) :
- Population majoritairement plus âgée (~45-50 ans).
- Très grande dispersion (moins de 20 ans à plus de 70 ans).
- Médiane légèrement plus élevée que celle du Cluster 0.



## 📊 Résultats de la segmentation

Voici les visualisations des graphiques obtenus :
![Scatterplot-clustering](https://github.com/Paul-Buchholz/Segmentation-Clients-KMeans/blob/main/images/Scatterplot-clustering.png?raw=true)
![boxplot_clustering](https://github.com/Paul-Buchholz/Segmentation-Clients-KMeans/blob/main/images/boxplot_clustering.png?raw=true)


## 🎯 Applications Business
Grâce à cette segmentation, plusieurs stratégies marketing peuvent être mises en place :
- **Personnalisation des offres** : Adapter les promotions et les services en fonction du profil du client.
- **Optimisation du ciblage publicitaire** : Mieux cibler les campagnes selon les segments les plus rentables.
- **Fidélisation des clients** : Créer des programmes adaptés à chaque type de consommateur.
- **Amélioration de l'expérience client** : Offrir des services plus pertinents et mieux adaptés aux attentes des consommateurs.

## 🚀 Installation et Exécution
1. Clonez le projet :
   ```bash
   git clone https://github.com/Paul-Buchholz/Segmentation-Clients-KMeans.git
   cd Segmentation-Clients-KMeans
   ```
2. Installez les dépendances :
   ```bash
   pip install -r requirements.txt
   ```
3. Ouvrez et exécutez le notebook :
   ```bash
   jupyter notebook Segmentation_Client.ipynb
   ```

## 🛠 Technologies utilisées
- **Python**
- **Pandas, NumPy** (Manipulation des données)
- **Matplotlib, Seaborn** (Visualisation des données)
- **Scikit-learn** (Modélisation et K-Means clustering)

## 📜 Licence
Ce projet est sous licence MIT.

---
💡 *N'hésitez pas à contribuer et à partager vos améliorations !*



English Version 


# Customer segmentation with K-Means

## 📌 Presentation
This project aims to analyze and segment customers based on their purchasing behavior and demographic characteristics. We use **the K-Means algorithm** to identify groups of customers with similar profiles, allowing us to optimize marketing strategies and improve our understanding of purchasing trends.

## 📂 Repository content
- **Mall_Customers.csv**: Dataset used for analysis.
- **Segmentation_Client.ipynb**: Jupyter notebook containing analysis, segmentation and visualizations.
- **requirements.txt** : List of dependencies required to run the project.
- **README.md** : Project documentation.

## 📊 Data used
The dataset includes the following columns:
- **CustomerID**: Customer's unique identifier.
- **Gender**: Customer's gender (Male/Female)
- **Age**: Customer's age
- **Annual Income (k$)**: Customer's annual income in thousands of dollars
- **Spending Score (1-100)** : Spending score assigned by the store (based on buying behavior and loyalty)

## 🔍 Methodology
1. **Data pre-processing**: Cleaning, management of missing values, normalization if necessary.
2. **Data exploration**: Statistical analysis and visualization of distributions.
3. **Application of K-Means**: Determination of the optimal number of clusters (elbow and silhouette methods) and execution of the algorithm.
4. **Cluster analysis**: Interpretation of results and visualization of clusters.

## 📌 Customer segmentation
We have identified **5 distinct customer clusters**:

### 1️⃣ Cluster 0 (Violet):
- Very wide age dispersion, from under 20 to over 70.
- Median around 45.
- Cluster with greatest age diversity.

### 2️⃣ Cluster 1 (Dark Blue):
- Young adults (~25-40 years).
- Less dispersed than Cluster 0.
- Median around 35.

### 3️⃣ Cluster 2 (Light blue):
- Very young population, mostly under 30.
- Low dispersion, well concentrated around 20.
- Median around 25.

### 4️⃣ Cluster 3 (dark green):
- Mainly people around 40-50 years old.
- Moderate dispersion (20-60 years).
- Slight male dominance in this cluster.

### 5️⃣ Cluster 4 (Light green):
- Predominantly older population (~45-50 years).
- Very wide dispersion (under 20 to over 70).
- Median slightly higher than Cluster 0.



## 📊 Segmentation results

Here are the visualizations of the graphs obtained:
![Scatterplot-clustering](https://github.com/Paul-Buchholz/Segmentation-Clients-KMeans/blob/main/images/Scatterplot-clustering.png?raw=true)
![boxplot_clustering](https://github.com/Paul-Buchholz/Segmentation-Clients-KMeans/blob/main/images/boxplot_clustering.png?raw=true)


## 🎯 Business Applications
Thanks to this segmentation, several marketing strategies can be implemented:
- **Personalization of offers**: tailor promotions and services to the customer's profile.
- **Optimized advertising targeting**: Better target campaigns to the most profitable segments.
- **Customer loyalty**: Create programs adapted to each type of consumer.
- **Enhanced customer experience**: Offer services that are more relevant and better adapted to consumer expectations.

## 🚀 Installation and operation
1. Clone the project :
   ```bash
   git clone https://github.com/Paul-Buchholz/Segmentation-Clients-KMeans.git
   cd Segmentation-Clients-KMeans
   ```
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the notebook:
   ```bash
   jupyter notebook Segmentation_Client.ipynb
   ```

## 🛠 Technologies used
- **Python**
- **Pandas, NumPy** (Data manipulation)
- **Matplotlib, Seaborn** (Data visualization)
- **Scikit-learn** (Modeling and K-Means clustering)

## 📜 License
This project is licensed under the MIT License.

---
💡 *Feel free to contribute and share your improvements!*
