# Employee Management System (CRUD) – Streamlit & PostgreSQL

<img width="1536" height="1024" alt="crud diagram" src="https://github.com/user-attachments/assets/a7d9c23b-88f5-49a1-86f2-b6d1b140e468" />

A full-stack CRUD (Create, Read, Update, Delete) web application for managing employee records, built using **Python**, **Streamlit**, and **PostgreSQL**.  
This project demonstrates database integration, backend logic, and interactive UI development.

---

## 🚀 Features

- Add new employees
- View all employees in a dynamic table
- Update existing employee information
- Delete employee records
- Persistent data storage using PostgreSQL
- Clean and interactive UI with Streamlit

---

## 🛠️ Tech Stack

- **Frontend:** Streamlit
- **Backend:** Python
- **Database:** PostgreSQL
- **Database Driver:** psycopg2
- **Data Handling:** pandas

---

## 🏗️ Architecture Overview

User (Web Browswer)  ->
StreamLit App (Python)  ->
PostgreSQL (Database)

- The Streamlit app handles UI and user interaction
- SQL queries are executed using `psycopg2`
- PostgreSQL stores employee data persistently

---

## 📂 Project Structure

├── app.py # Main Streamlit application
├── db.py # Database connection logic
├── requirements.txt # Python dependencies
└── README.md

---

## 🗄️ Database Schema

```sql
CREATE TABLE employee (
    emp_id SERIAL PRIMARY KEY,
    emp_name VARCHAR(100),
    email VARCHAR(100),
    department VARCHAR(50),
    salary NUMERIC,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

---

⚙️ Setup & Installation
1️⃣ Clone the Repository
git clone https://github.com/your-username/employee-crud-streamlit-postgres.git
cd employee-crud-streamlit-postgres

2️⃣ Create a Virtual Environment (Optional but Recommended)
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Configure PostgreSQL
Ensure PostgreSQL is running
Create a database named employee_db
Create the employee table using the schema above

⚠️ Security Note:
Database credentials should be stored in environment variables instead of hardcoded values for production use.

5️⃣ Run the Application
streamlit run app.py

🧪 Example Use Cases
HR employee tracking
Learning full-stack Python development
CRUD application demonstration for resumes
PostgreSQL + Python integration practice

📈 What This Project Demonstrates
Full CRUD operations with SQL
Backend–database integration
State management in Streamlit
Clean project organization
Real-world data workflows

🔮 Future Improvements
Authentication & user roles
Input validation
Pagination & search
Dockerization
Deployment to cloud (AWS / GCP / Streamlit Cloud)

📄 License
This project is open-source and available for learning and portfolio use.
