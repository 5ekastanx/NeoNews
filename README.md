# 📰 NeoNews
NeoNews is a backend project designed to provide APIs for news management, including authorization, authentication, favorites functionality, and Swagger documentation. The project is containerized using Docker for easy deployment.
 
## 🚀 Features
News API: Endpoints for creating, retrieving, updating, and deleting news articles.
Authorization & Authentication: Secure access with JWT.  
Favorites: API endpoints for managing favorite news articles.
Swagger: API documentation with Swagger UI.
Docker: Containerized application for easy deployment. 

## 📁 Project Structure 

   neonews/
   ├── main/
   │   ├── __pycache__/
   │   ├── migrations/
   │   ├── templates/
   │   ├── __init__.py
   │   ├── admin.py
   │   ├── apps.py
   │   ├── models.py
   │   ├── tests.py
   │   ├── urls.py
   │   ├── views.py
   ├── neonews/
   │   ├── __pycache__/
   │   ├── __init__.py
   │   ├── asgi.py
   │   ├── settings.py
   │   ├── urls.py
   │   ├── wsgi.py
   ├── news/
   │   ├── __pycache__/
   │   ├── migrations/
   │   ├── __init__.py
   │   ├── admin.py
   │   ├── apps.py
   │   ├── models.py
   │   ├── serializers.py
   │   ├── tests.py
   │   ├── urls.py
   │   ├── views.py
   ├── news_images/
   ├── venv/
   │   ├── Include/
   │   ├── Lib/
   │   ├── Scripts/
   │   ├── pyvenv.cfg
   ├── .dockerignore
   ├── db.sqlite3
   ├── Dockerfile
   ├── manage.py
   ├── requirements.txt
   ├── rundocker.sh
   ├── runsite.sh

## 🛠️ Setup and Installation
Prerequisites
Docker
Docker Compose
Installation
1. Clone the repository: 
   git clone https://github.com/5ekastanx/NeoNews.git
   cd NeoNews
2. Create and activate a virtual environment:
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
3. Install the dependencies:
   pip install -r requirements.txt
4. Run the application with Docker:
   docker-compose up --build

## 🧩 Usage
   Access the API at http://localhost:8000/news/.
   Access Swagger UI for API documentation at http://localhost:8000/swagger/.
## 🗂️ API Endpoints
## News
   GET /news/list/ - List all news articles
   GET /news/detail/<id>/ - Retrieve a specific news article
   GET /news/category/ - List all category articls

## Authentication
POST /token/ - Obtain JWT token
POST /token/refresh/ - Refresh JWT token
## Favorites
GET //favorites/ - List all favorite news articles
POST /favorites/ - Add a news article to favorites
DELETE /favorites/<id>/ - Remove a news article from favorites

## 📜 License
This project is licensed under the MIT License.

## ✨ Acknowledgements
This project was purchased and further developed by 5ekastanx.
