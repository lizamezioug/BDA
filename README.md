# 🚆 Advanced Databases Project – Smart City Transport System

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)


## 👩‍💻 About the Project

This project was developed as part of the **Advanced Databases (BDA)** course.  
It provides a **Full-Stack web interface** to **execute and visualize queries** on **two types of databases**:

1. **SQL3 (Oracle)** – relational-object model  
2. **NoSQL (MongoDB)** – document-oriented model  

The system simulates a **smart city urban transport network**, including:

- Metro (MET), Tramway (TRA), Bus (BUS), Train (TRN)  
- Lines with departure/arrival stations and segments  
- Stations (main/secondary) with spatial coordinates  
- Shuttles performing multiple trips with tracking: duration, date, passengers, observations  
- Travel time estimation via **CalculerDurée**  

The interface allows selecting queries from a **menu**, executing them, and viewing results interactively.  
**Pre-fill scripts** are provided to populate DBs ( SQL3 and MongoDB) before executing queries.



## 🛠 Features & Functionality

- **Two database models**: SQL3 (Oracle) & MongoDB  
- Clear, user-friendly displays  
- **Interactive menu** to select queries  
- Execute queries with **one click**  
- Display results dynamically 
- **Full-Stack interface** using React + Tailwind CSS + Node.js + Express.js  
- Seamless connection to **SQL3 and MongoDB**  
- Pre-fill scripts for database initialization  
- **Dynamic execution** and visualization of queries  

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

* **Oracle SQL3**: Ensure Oracle 11g is installed locally and update `db-sql3.js` with your credentials.
* **MongoDB**: Ensure MongoDB is running at `mongodb://127.0.0.1:27017` with database `smartcity`.

4. **Populate databases**

```bash
# Run the provided scripts to pre-fill SQL3 and MongoDB with realistic data
```

5. **Run the full-stack application**

```bash
npm run dev
```

* This starts the **React frontend (Vite)** and **Node.js backend**.
* Open your browser at: [http://localhost:5173/](http://localhost:5173/) to access the interface.

---

## 🔍 Usage

**How to execute queries:**

1. Use the **navbar** to select either **SQL3 (Oracle)** or **MongoDB**.
2. Click a **query card** to view the full query.
3. Press **Execute** to run the query on the selected database.
4. View results dynamically.




