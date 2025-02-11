# AI-Powered Chatbot for Supplier and Product Information  

## 📌 Overview  
This project is an AI-powered chatbot that enables users to query a product and supplier database using natural language. The chatbot interacts with an open-source Large Language Model (LLM) and utilizes the LangGraph framework to fetch relevant information from a MySQL/PostgreSQL database, summarizing results using the LLM.  

## 🎯 Features  
✅ **Natural Language Querying** – Users can ask product- and supplier-related queries.  
✅ **LLM-Powered Summarization** – Enhances responses using context from the LLM.  
✅ **Database Integration** – Retrieves structured data from MySQL/PostgreSQL.  
✅ **Interactive UI** – A React-based frontend for seamless interaction.  
✅ **Query History** – Displays recent queries for reference.  

## 🚀 Tech Stack  
### **Frontend**  
- React (Material UI / Tailwind CSS)  
- Axios (for API calls)  
- Redux / Context API (for state management)  

### **Backend**  
- Python (FastAPI / Flask)  
- LangGraph (for chatbot workflow)  
- Open-source LLM (LLaMA 2) 

### **Database**  
- MySQL / PostgreSQL  

## 🛠️ Functional Requirements  
- Users can ask questions like:  
  - _"Show me all products under brand X."_  
  - _"Which suppliers provide laptops?"_  
  - _"Give me details of product ABC."_  
- The chatbot should:  
  - Retrieve relevant data from the database.  
  - Enhance responses using LLM context.  
  - Return structured and meaningful results.  
  - Handle incorrect or incomplete queries gracefully.  

## 📊 Database Schema  
### **Products Table**  
| ID  | Name  | Brand  | Price  | Category  | Description  | Supplier ID  |
|-----|------|--------|--------|-----------|--------------|-------------|

### **Suppliers Table**  
| ID  | Name  | Contact Info  | Product Categories  |
|-----|------|--------------|--------------------|

## 📌 Installation & Setup  

# Project Setup Guide  

## Backend Setup  

- Clone the repository:  
  - `git clone <repository-url>`  
  - `cd backend`  

- Install Python dependencies:  
  - `pip install -r requirements.txt`  

- Set up the MySQL database:  
  - Create a database named `supplierproductdb`.  
  - Import the schema and sample data using the provided SQL scripts.  

- Configure the database connection in `main.py`:  
  - Set the `DB_CONFIG` as follows:
  - DB_CONFIG = {
    "host": "localhost",
    "port": 5000,
    "user": "root",
    "password": "********",
    "database": "supplierproductdb"
}



- Run the FastAPI server:  
  - `uvicorn main:app --reload`  

---

## Frontend Setup  

- Navigate to the frontend directory:  
  - `cd frontend`  

- Install Node.js dependencies:  
  - `npm install`  

- Install Material-UI:  
  - `npm install @mui/material @emotion/react @emotion/styled @mui/icons-material`  

- Run the React app:  
  - `npm start`  

- Access the frontend at:  
  - `http://localhost:3000`  



