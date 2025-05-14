# 🔧 Gas Utility Customer Service Portal

A Django-based web application to streamline and improve customer service operations for gas utility companies. This system allows customers to submit service requests, track the progress, and view their account information. Additionally, it provides an administrative interface for support representatives to manage and resolve customer issues efficiently.

---

## 🚀 Features

### 🧑‍💻 Customer Portal
- **Submit Service Requests**
  Customers can log in and submit requests for various services (e.g., gas leak, billing issue, connection request).
- **Request Tracking**
  View real-time status updates of submitted requests.
- **Account Overview**
  Access personal information and a history of past service requests.

### 🛠️ Admin/Support Panel
- **Request Management**
  Customer support representatives can view, update, and resolve service requests.
- **User Management**
  Admins can manage customer accounts and permissions.
- **Status Updates & Communication**
  Notify customers of changes via email or internal messages.

---

## 📁 Project Structure
```
gas_utility_portal/
│
├── accounts/
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   └── urls.py
│
├── service_requests/
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   └── urls.py
│
├── support_dashboard/
│   ├── views.py
│   └── urls.py
│
├── templates/
├── static/
│
├── gas_utility_portal/  # Your main config folder
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── manage.py
└── README.md
```


---

## 🛠️ Tech Stack

- **Backend**: Django (Python)
- **Frontend**: HTML5, CSS3, Bootstrap
- **Database**: SQLite (default, can be switched to PostgreSQL/MySQL)
- **Authentication**: Django's built-in User model
- **File Uploads**: Handled via Django FileField

---

## 🧑‍💻 Installation & Setup

### 📦 Prerequisites
- Python 3.8+
- pip
- Virtualenv (optional but recommended)

### ⚙️ Setup

```bash
# Clone the repo
git clone https://github.com/your-username/gas-utility-portal.git
cd gas-utility-portal

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py makemigrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Run the server
python manage.py runserver
