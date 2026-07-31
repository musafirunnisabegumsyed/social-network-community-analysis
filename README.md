# Comparative Analysis of Louvain and Girvan–Newman for Community Detection and Influential Node Identification in Social Networks

## 📌 Project Overview

This project focuses on **Social Network Analysis (SNA)** using the **Zachary Karate Club Network**.

The objective is to compare the **Louvain** and **Girvan–Newman** community detection algorithms and identify influential nodes in the social network using different centrality measures.

The project also evaluates the quality of the detected communities using modularity, community density, community size, and execution time.

---

## 🎯 Objectives

* Detect communities using the **Louvain algorithm**
* Detect communities using the **Girvan–Newman algorithm**
* Compare the communities detected by both algorithms
* Evaluate community quality
* Calculate different centrality measures
* Identify influential nodes
* Identify bridge nodes
* Compare the performance of both community detection algorithms

---

## 📊 Dataset

### Zachary Karate Club Network

The dataset represents the social relationships between members of a university karate club.

| Property     |         Value |
| ------------ | ------------: |
| Nodes        |            34 |
| Edges        |            78 |
| Network Type |    Undirected |
| Data Format  | CSV Edge List |

Each row represents a connection between two nodes.

```text
id1,id2
0,1
0,2
0,3
...
```

The dataset is stored in:

```text
data/karate_club.csv
```

---

## 🧠 Community Detection

### Louvain Algorithm

The Louvain algorithm detects communities by optimizing **modularity**. It is efficient and widely used for community detection in networks.

### Girvan–Newman Algorithm

The Girvan–Newman algorithm detects communities by repeatedly removing edges with high **edge betweenness centrality**, causing the network to split into communities.

---

## 📈 Community Quality Analysis

The communities detected by both algorithms are compared using:

### 1. Modularity

Measures the strength of the community structure. Higher modularity generally indicates better separation between communities.

### 2. Community Density

Measures how strongly connected the nodes within each community are.

### 3. Community Size

Measures the number of nodes belonging to each detected community.

### 4. Execution Time

Measures the time required by each algorithm to detect communities.

---

## ⭐ Influential Node Identification

Four centrality measures are used to identify important nodes.

### Degree Centrality

Measures the number of direct connections of a node.

### Betweenness Centrality

Measures how frequently a node lies on shortest paths between other nodes.

It is also used to identify potential **bridge nodes**.

### Closeness Centrality

Measures how efficiently a node can reach other nodes in the network.

### Eigenvector Centrality

Measures the importance of a node based on its connections to other important nodes.

---

## 🏆 Influence Score

A combined influence score is calculated using the four centrality measures:

```text
Influence Score =
0.25 × Degree Centrality
+ 0.30 × Betweenness Centrality
+ 0.20 × Closeness Centrality
+ 0.25 × Eigenvector Centrality
```

Nodes are ranked according to their influence score.

---

## 🔗 Bridge Node Identification

Nodes with high **betweenness centrality** are analyzed as potential bridge nodes.

These nodes can connect different communities and may play an important role in information flow across the network.

---

## 🔬 Project Workflow

```text
Dataset
   ↓
Network Construction
   ↓
Louvain Community Detection
   ↓
Girvan–Newman Community Detection
   ↓
Community Quality Analysis
   ↓
Centrality Analysis
   ↓
Influential Node Ranking
   ↓
Bridge Node Identification
   ↓
Algorithm Comparison
   ↓
Final Analysis
```

---

## 📁 Project Structure

```text
social-network-community-analysis/
│
├── README.md
│
├── data/
│   └── karate_club.csv
│
├── notebooks/
│   └── social_network_analysis.ipynb
```

---

## 🛠️ Technologies Used

* Python
* NetworkX
* Pandas
* NumPy
* Matplotlib
* Google Colab
* Git
* GitHub

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/musafirunnisabegumsyed/social-network-community-analysis.git
```

### 2. Navigate to the project

```bash
cd social-network-community-analysis
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the notebook

Open:

```text
notebooks/social_network_analysis.ipynb
```

The notebook contains the complete implementation of the project.

---



---

## 📌 Expected Analysis

The project aims to determine:

* Which algorithm detects better-defined communities
* Which algorithm achieves higher modularity
* Which algorithm produces denser communities
* Which algorithm is computationally faster
* Which nodes are the most influential
* Which nodes act as bridges between communities

---

## 🔮 Future Enhancements

* Apply the methodology to larger social-network datasets
* Compare additional community detection algorithms
* Analyze weighted and directed networks
* Perform dynamic community detection
* Study information propagation across communities
* Develop an interactive Social Network Analysis dashboard

---

## 📚 References

1. Zachary, W. W. (1977). *An Information Flow Model for Conflict and Fission in Small Groups.*
2. Girvan, M., & Newman, M. E. J. (2002). *Community Structure in Social and Biological Networks.*
3. Blondel, V. D., Guillaume, J.-L., Lambiotte, R., & Lefebvre, E. (2008). *Fast Unfolding of Communities in Large Networks.*
4. NetworkX documentation.

---

## 👩‍💻 Author

**Musafirunnisa Begum**

Social Network Analysis Project

**Python | NetworkX | Community Detection | Centrality Analysis**
