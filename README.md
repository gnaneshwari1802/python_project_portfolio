


# 🛠️ **Project Setup & Usage Guide**

Welcome to the project! This guide will help you set up and run the project, including common troubleshooting steps.

---

## 📋 **Prerequisites**

Before you begin, ensure the following are installed on your machine:

- **Node.js**: Required to run front-end build scripts.
- **Python 3.8+**: For running the back-end Django server.
- **Conda**: For managing Python environments.
- **Git**: For version control.

---

## 🏁 **Project Setup**

### 1️⃣ **Clone the Repository**

Clone the project from GitHub and navigate to the project folder:

```bash
git clone <repository_url>
cd ecom-proj-master
```

---

### 2️⃣ **Install Front-End Dependencies**

Run the following command to build the front-end assets:

```bash
npm run build
```

---

### 3️⃣ **Start the Front-End Server**

To start the front-end development server, use:

```bash
npm run start
```

---

### 4️⃣ **Set Up Python Virtual Environment**

Create and activate a Python virtual environment to manage dependencies:

```bash
# Create a new virtual environment
 cd D:\telusko\telusko                                                                                                                      
(base) PS D:\telusko\telusko> test\Scripts\activate
python -m venv test

# Activate the virtual environment
test\Scripts\activate  # On Windows
source test/bin/activate  # On macOS/Linux
```

---

### 5️⃣ **Install Python Dependencies**

After activating the environment, install Django and other required Python packages:

```bash
pip install django
```

---

### 6️⃣ **Check Django Version**

Ensure Django is installed by checking its version:

```bash
django-admin --version
```

You should see the version number, e.g., `5.0.3`.

---

### 7️⃣ **Run the Django Development Server**

Start the Django development server:

```bash
python manage.py runserver
```

You can now access the project at `http://127.0.0.1:8000/`.

---

## 🔄 **Git Submodules**

If the project uses Git submodules, you can manage them with these commands:

```bash
# Check the status of submodules
git submodule status

# List staged files with submodules
git ls-files --stage | grep 160000
```

---

## ❌ **Deactivating the Virtual Environment**

When you're done working, deactivate your virtual environment:

```bash
conda deactivate  # If using Conda
# or
deactivate  # For virtualenv
```

---

## ⚠️ **Troubleshooting**

### 1. **ModuleNotFoundError: No module named 'django'**

If you encounter the error:

```
ModuleNotFoundError: No module named 'django'
```

It means Django is not installed in your virtual environment. To fix this, run:

```bash
pip install django
```

---

## 📝 **Additional Notes**

- **Upgrade pip**: If you see a message about an outdated version of `pip`, upgrade it by running:

```bash
python -m pip install --upgrade pip
pip install gunicorn uvicorn
pip freeze > requirements.txt
pip install fcntl
python -m gunicorn telusko.asgi:application -k uvicorn.workers.UvicornWorker
pip install dj-database-url
pip install psycopg2-binary
```

- **Virtual Environment**: Always ensure your virtual environment is activated before running Django commands.

---

## 🔗 **Useful Links**

- [Django Documentation](https://docs.djangoproject.com/)
- [Node.js Documentation](https://nodejs.org/en/docs/)

---

### 💡 **Tips & Tricks**

- Check if your virtual environment is active: The terminal prompt should include `(test)` or the name of your environment.
- If you encounter other errors, Google the error message or consult the logs for more information.

---

```

### Key Changes:
1. **Clear section headers** for each task, such as "Prerequisites", "Project Setup", "Git Submodules", and "Troubleshooting".
2. **Code blocks** for each command that users need to run, ensuring readability and easy copying.
3. **Bullet points** and numbered lists make the steps easy to follow.
4. **Helpful links** and **tips** at the end to guide the user through any issues they may face.
5. **Emojis** to visually organize the document and add a fun touch.

Simply copy this into your `README.md` file, and you’ll have a well-organized, editable, and user-friendly guide for anyone setting up or using the project!
