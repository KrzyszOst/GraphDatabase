# 🧠 Graph Database Project – Movies, Users & Recommendations 🎬

This project was developed for the **Graph Databases** course.  
It explores relationships between users, movies, actors, directors, and genres using a **graph-based model** in Neo4j.

---

## 🎯 Project Goal

The aim was to uncover hidden patterns in movie ratings and preferences using a flexible, query-friendly graph structure.  
We implemented realistic connections to support **recommendations, trend analysis, and genre-based exploration**.

---

## 🗃️ Data Model

### 📌 Node Types:
- **User** – name, surname, birthDate  
- **Movie** – title, releaseYear  
- **Actor / Director** – name, surname  
- **Genre** – name  

### 🔗 Relationship Types:
- `(:User)-[:RATED {rating}]->(:Movie)`  
- `(:User)-[:LIKES]->(:Genre)`  
- `(:Actor)-[:ACTED_IN]->(:Movie)`  
- `(:Director)-[:DIRECTED]->(:Movie)`  
- `(:Movie)-[:IN_GENRE]->(:Genre)`

---

## 📥 Files Included

- `creates.txt` – Cypher script for full graph setup  
- `questions.txt` – Cypher queries answering business questions  
- `raport graph database project.pdf` – Full project documentation  
- `Graph database project presentation.pdf` – Visual walkthrough of the project

---

## 🧠 Competency Questions (with Cypher)

1. 📊 What is the average rating for each movie?  
2. 🎟️ How many movies did each user rate and what’s their average?  
3. 🎬 What movies belong to each genre?  
4. ⭐ Which movie has the most ratings?  
5. 🧑‍🎤 Which actors appeared in Sci-Fi or Action movies?  
6. 🏆 What’s the top-rated movie in each genre?  
7. 👵 What’s the average rating for movies rated by users older than 30?  
8. 🎯 Movie recommendations based on users who rated the same movie

---

## 🚀 How to Run

1. Open Neo4j Desktop or Neo4j Sandbox  
2. Copy & run the queries from `creates.txt` to build the graph  
3. Use the queries in `questions.txt` to interact with the data

---

## 👥 Team

- **Krzysztof Ostrzycki**  
- **Łukasz Turek**

