# BharatFD Backend Assignment

This repository contains the backend implementation for the BharatFD assignment. The project is built as per the provided guidelines and is designed to run locally.

## Table of Contents

- [Setup and Installation](#setup-and-installation)
- [Admin Panel Access](#admin-panel-access)
- [Features](#features)
- [Running Without Docker](#running-without-docker)
- [Running With Docker](#running-with-docker)
- [API Endpoints](#api-endpoints)
- [Schema](#schema)
- [Contributing](#contributing)
- [Contact](#contact)

---

## Setup and Installation

Follow these steps to set up and run the project on your local machine:

```bash
git clone https://github.com/Harsh-Kesharwani/bharatfd-assignment.git
cd bharatfd-assignment
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

To run tests, use:

```bash
pytest
```

---

## Admin Panel Access

You can access the Django admin panel by navigating to:

**URL:** `http://localhost:8000/admin`

Use the following credentials:
- **Username**: `admin`
- **Password**: `admin123`

*(Ensure you create a superuser if necessary by running `python manage.py createsuperuser`.)*

---

## Features

- Automatic translation during FAQ creation
- Optimized database queries using `Prefetch`
- Efficient schema design for scalability
- Multi-language support via Google Translate API
- REST API with language selection
- Caching with Redis for better performance
- Unit tests for models and API endpoints

---

## Running Without Docker

To run the project without Docker:

```bash
git https://github.com/Harsh-Kesharwani/bharatfd-assignment.git
cd bharatfd-assignment
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

---

## Running With Docker

To run the project using Docker:

```bash
docker compose up --build
```

The application will be accessible at `http://localhost:8000`.

---

## API Endpoints

Examples for making API requests:

```bash
# Get FAQs in default language (English)
curl http://localhost:8000/api/faqs/

# Get FAQs in Hindi
curl http://localhost:8000/api/faqs/?lang=hi

# Get FAQs in Bengali
curl http://localhost:8000/api/faqs/?lang=bn
```

---

## Schema

*(Include schema details here if needed.)*

---

## Contributing

Interested in contributing? Follow these steps:

1. **Fork the repository**
2. **Clone your fork**
   ```bash
   git clone https://github.com/Harsh-Kesharwani/bharatfd-assignment.git
   ```
3. **Create a new branch**
   ```bash
   git checkout -b feature-branch
   ```
4. **Make your changes** and follow best coding practices
5. **Run tests** to ensure stability
6. **Commit and push**
7. **Create a pull request** for review

---

## Contact

For queries or suggestions, feel free to reach out at `harshkesharwani777@gmail.com`. Happy coding! 🚀

