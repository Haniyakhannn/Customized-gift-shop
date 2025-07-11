

# 🎁 Customized Gift Store

A full-stack web application for a **Customized Gift Store** built using **Django** (Backend) and **MySQL** (Database). This platform allows users to browse, personalize, and purchase custom gifts while providing an intuitive admin dashboard for product management.


## 🛠️ Tech Stack

* **Backend**: Django (Python)
* **Database**: MySQL
* **Frontend**: HTML, CSS, JavaScript, Bootstrap
* **ORM**: Django ORM
* **Authentication**: Django Auth System
* **Hosting**: (Add if deployed — e.g., Heroku, PythonAnywhere, etc.)



## ✨ Features

### 🧑‍💻 User Side:

* Browse various gift items
* Filter & search products
* Customize gifts (name, message, images, etc.)
* Add to cart & wishlist
* User registration & login
* Place orders with order tracking
* View order history

### 🛍️ Admin/Manager Side:

* Secure admin panel
* Add, edit, delete gift products
* Manage users, orders, and inventory
* View order statuses and history


## 🚀 Setup Instructions

### Prerequisites

* Python 
* MySQL Server
* pip (Python package manager)

### 1. Clone the Repository

bash
git clone https://github.com/yourusername/customized-gift-store.git
cd customized-gift-store


### 2. Create Virtual Environment

bash
python -m venv venv
source venv/bin/activate  # On Windows use venv\Scripts\activate


### 3. Install Dependencies

bash
pip install -r requirements.txt


### 4. Configure Database (MySQL)

* Create a MySQL database (e.g., `giftstore`)
* Update `settings.py` with your database credentials:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'giftstore',
        'USER': 'yourusername',
        'PASSWORD': 'yourpassword',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### 5. Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Create Superuser (for Admin Panel)

```bash
python manage.py createsuperuser
```

### 7. Run Server

bash
python manage.py runserver
Visit [http://127.0.0.1:8000](http://127.0.0.1:8000)


📂 Project Structure


customized-gift-store/
│
├── giftstore/              # Main Django project
├── store/                  # App handling products, orders, users
├── templates/              # HTML templates
├── static/                 # CSS, JS, images
├── media/                  # Uploaded media files
├── requirements.txt
└── manage.py

## 📌 Future Improvements

* Payment Gateway Integration
* Email Notifications
* Review and Ratings System
* REST API for mobile apps

