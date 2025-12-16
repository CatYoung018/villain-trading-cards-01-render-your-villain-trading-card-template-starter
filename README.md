# 🦹 Villain Trading Cards - Rendering Templates

Introduction to Flask web development by creating and rendering villain trading card templates. This project focuses on the fundamentals of Flask, including setting up a Flask application, creating routes, and rendering Jinja2 templates.

![Languages](https://img.shields.io/badge/HTML-41.5%25-orange)
![Languages](https://img.shields.io/badge/CSS-33.1%25-blue)
![Languages](https://img.shields.io/badge/Python-25.4%25-yellow)

## 📋 Project Overview

This is **Part 1** of the Villain Trading Cards series, introducing Flask fundamentals through a simple villain trading card application. The project demonstrates how to set up Flask, create basic routes, and render HTML templates with Jinja2.

### Key Features

- **Flask Setup**: Basic Flask application structure
- **Template Rendering**: Using `render_template()` to serve HTML
- **Jinja2 Basics**: Introduction to Flask's templating engine
- **Static Assets**: Serving CSS and images
- **Development Server**: Using Flask's built-in development server

## 🛠️ Technologies Used

- **Backend**: Python, Flask
- **Templating**: Jinja2
- **Frontend**: HTML5, CSS3
- **Development**: Virtual environments, Flask debugger

## 📚 Learning Outcomes

This project demonstrates:

- Installing and setting up Flask
- Creating a basic Flask application
- Understanding Flask routing with decorators
- Rendering HTML templates with `render_template()`
- Organizing project structure (templates, static files)
- Working with virtual environments
- Using Flask's development server

## 🚀 Installation & Setup

### Prerequisites

Check if Python is installed:

**On Mac:**
```bash
python3 --version
```

**On Windows:**
```bash
python --version
```

Ensure you have Python 3.8 or higher installed (3.11 recommended). If you need to install Python on Windows, see [this guide](https://docs.google.com/document/d/14diNu_g6uhouBscRt8zIezolANTRQA6HobKRP4Lgu5Q/copy).

### Step 1: Clone the Repository

```bash
git clone https://github.com/CatYoung018/villain-trading-cards-01-render-your-villain-trading-card-template-starter.git
cd villain-trading-cards-01-render-your-villain-trading-card-template-starter
```

### Step 2: Create Virtual Environment

**On Mac:**
```bash
python3 -m venv venv
```

**On Windows:**
```bash
python -m venv venv
```

### Step 3: Activate Virtual Environment

**On Mac:**
```bash
source venv/bin/activate
```

**On Windows:**
```bash
source venv/Scripts/activate
```

Once activated, you'll see `(venv)` at the beginning of your terminal prompt.

### Step 4: Install Dependencies

```bash
pip install flask flask-sqlalchemy
```

### Step 5: Run the Application

**Without debugger:**
```bash
flask run
```

**With debugger (recommended for development):**
```bash
flask run --debug
```

The app will run at: `http://127.0.0.1:5000/`

### Step 6: View the App

Open your browser and navigate to `http://127.0.0.1:5000/` to see your villain trading card template.

### Stopping the Application

- Press `Ctrl + C` to stop the server
- Run `deactivate` to close the virtual environment

**Note:** When not using the debugger, you'll need to stop and restart the server after making code changes. Remember to hard refresh your browser (`Ctrl + F5` or `Cmd + Shift + R`).

## 📁 Project Structure

```
villain-trading-cards-01-render-your-villain-trading-card-template-starter/
├── static/              # Static assets
│   ├── css/            # Stylesheets
│   │   └── style.css   # Main stylesheet
│   └── images/         # Card images
├── templates/           # HTML templates (Jinja2)
│   └── index.html      # Main template
├── app.py              # Flask application entry point
├── .gitignore          # Git ignore file
├── README.md           # Project documentation
└── venv/               # Virtual environment (after setup)
```

## 🎯 Core Flask Concepts

### 1. Basic Flask Application
```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html')
```

### 2. Routing
Flask uses decorators to map URLs to functions:
```python
@app.route('/')  # Maps root URL to index()
def index():
    return render_template('index.html')
```

### 3. Rendering Templates
The `render_template()` function renders HTML templates from the `templates/` folder:
```python
return render_template('index.html')
```

### 4. Static Files
CSS and images are served from the `static/` folder and accessed in templates:
```html
<link rel="stylesheet" href="{{ url_for('static', filename='css/style.css') }}">
```

## 💡 Usage

1. **Start the server**: Run `flask run --debug`
2. **View the card**: Open browser to `http://127.0.0.1:5000/`
3. **Make changes**: Edit HTML/CSS files
4. **Refresh**: Hard refresh browser to see changes (with debugger, changes appear automatically)

## 🔄 Series Progression

This is **Part 1** in the Villain Trading Cards series:
- **Part 1: Rendering templates** (this project) - Flask basics
- Part 2: Building a Flask static site - Multiple pages and routing
- Part 3: Adding forms and user input - Form handling
- Part 4: Database integration - SQLAlchemy and CRUD operations

## 🔮 Next Steps

After completing this project, you'll be ready to:
- Add more routes and pages (Part 2)
- Work with forms and user input (Part 3)
- Integrate a database (Part 4)
- Deploy your Flask application

## 🎓 Acknowledgments

This project was created as part of a Skillcrush coding bootcamp, introducing Flask web development fundamentals through a hands-on project.

## 📝 License

This project is open source and available for educational purposes.

## 📧 Contact

**Cat Young**  
Email: cat@catyoungconsulting.com  
Portfolio: [catyoung018.github.io/Cat-Young-Dev](https://catyoung018.github.io/Cat-Young-Dev/)  
GitHub: [@CatYoung018](https://github.com/CatYoung018)

---

⭐ **If you found this project helpful, please consider giving it a star!**
