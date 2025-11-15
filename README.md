Parfait ! 😄 Voici une **version finale ultra-pro et complète** du README pour ton projet BDA, avec :

* Badges GitHub (stats, stars, forks, issues)
* Section démo visuelle (GIF/screenshot)
* Style clair et attractif pour GitHub
* Explication complète du projet, technologies, et usage

---

````md
# 🚆 Advanced Databases Project – Smart City Transport System

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

---

## 👩‍💻 About the Project

This project was developed as part of the **Advanced Databases (BDA)** course.  
It provides a **web interface to execute and visualize queries** on **two types of databases**:

1. **SQL3 (Oracle)** – relational-object model  
2. **NoSQL (MongoDB)** – document-oriented model  

The system simulates a **smart city urban transport network**, including:

- Metro (MET), Tramway (TRA), Bus (BUS), Train (TRN)  
- Lines with departure/arrival stations and segments  
- Stations (main/secondary) with spatial coordinates  
- Shuttles performing multiple trips with tracking: duration, date, passengers, observations  
- Travel time estimation via **CalculerDurée**  

The interface allows selecting queries from a **menu**, executing them, and viewing results interactively.

---

## 🛠 Features & Functionality

- **Two database models**:  
  - Part I: SQL3 (Oracle)  
  - Part II: MongoDB  
- Clear, user-friendly displays and messages  
- **Interactive menu** to select queries  
- Execute queries with **one click**  
- Display results dynamically in tables/cards  
- **Pre-fill scripts** to populate both SQL and NoSQL databases before execution  
- Frontend built with **React + Tailwind CSS**  
- Backend using **Node.js + Express.js**  
- Connects seamlessly with both **SQL3 and MongoDB**  

---

## 🖥 Demo

![BDA Demo](assets/demo.gif)

**Demo description**:  
- Navbar to choose SQL3 or MongoDB  
- Cards for each query  
- Click a card to see the query  
- Execute with a button and view results  

> ⚡ Replace the GIF with your own demo for live visualization

---

## ⚙️ Tech Stack

| Frontend | Backend | Databases |
|----------|--------|-----------|
| ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) | ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white) | ![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white) |
| ![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white) | Express.js | ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white) |

---

## 🚀 Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/<your-username>/BDA-Project.git
cd BDA-Project
````

2. **Install Node.js dependencies**

```bash
npm install
```

3. **Configure databases**

* **Oracle SQL3**:

  * Ensure Oracle 11g is installed locally
  * Update `db-sql3.js` with your credentials and TableSpaces
* **MongoDB**:

  * Ensure MongoDB is running at `mongodb://127.0.0.1:27017`
  * Database: `smartcity`

4. **Populate databases**

```bash
# Run provided scripts to pre-fill SQL3 and MongoDB with realistic data
```

5. **Start backend server**

```bash
node index.js
```

6. **Start frontend**

```bash
cd client
npm start
```

7. Open [http://localhost:3000](http://localhost:3000)

---

## 🔍 Usage

* Use **navbar** to select SQL3 or MongoDB
* Click a **query card** to view the query text
* Click **Execute** to run the query
* Results are displayed dynamically
* Example queries:

  * List trips with issues (panne, retard, accident)
  * Lines with main stations
  * Shuttles with max trips
  * Stations with multiple transport modes
  * Aggregate trips per line

---

## 📌 Code Snippets

**MongoDB connection**

```javascript
import { MongoClient } from "mongodb";

const client = new MongoClient("mongodb://127.0.0.1:27017");
const dbName = "smartcity";
let db;

async function getMongoDB() {
  if (!db) {
    await client.connect();
    db = client.db(dbName);
  }
  return db;
}

export default getMongoDB;
```

**Oracle SQL3 connection**

```javascript
import oracledb from 'oracledb';

export async function getOracleConnection() {
  return await oracledb.getConnection({
    user: 'SQL3',
    password: 'password',
    connectString: 'localhost/XEPDB1'
  });
}
```

---

## 📈 Project Status

![GitHub repo size](https://img.shields.io/github/repo-size/<your-username>/BDA-Project)
![GitHub contributors](https://img.shields.io/github/contributors/<your-username>/BDA-Project)
![GitHub stars](https://img.shields.io/github/stars/<your-username>/BDA-Project?style=social)
![GitHub forks](https://img.shields.io/github/forks/<your-username>/BDA-Project?style=social)

* ✅ Backend connected to Oracle SQL3 & MongoDB
* ✅ Frontend with React + Tailwind CSS
* ✅ Query execution and result display
* ✅ Pre-fill scripts for databases
* 🚧 Future improvements: authentication, enhanced UI/UX, advanced visualizations


