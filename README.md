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

