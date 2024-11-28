🎉 Project Setup & Usage Guide
Welcome to the project! This guide will walk you through setting up the project, running the development server, and resolving any common issues you might encounter.

📋 Prerequisites
Make sure you have the following installed before proceeding:

Node.js for running front-end build scripts.
Python (version 3.8 or higher) for running the back-end Django server.
Conda for managing Python environments.
Git for version control.
🛠️ Project Setup
1️⃣ Clone the Repository
Start by cloning the repository to your local machine:

bash
Copy code
git clone <repository_url>
cd ecom-proj-master
2️⃣ Install Front-End Dependencies
Run the following command to build the front-end assets:

bash
Copy code
npm run build
3️⃣ Start the Front-End Development Server
Start the server for the front-end:

bash
Copy code
npm run start
4️⃣ Set Up a Python Virtual Environment
To ensure project dependencies are isolated, create and activate a Python virtual environment:

bash
Copy code
# Create a new virtual environment
python -m venv test

# Activate the virtual environment
test\Scripts\activate  # On Windows
source test/bin/activate  # On Mac/Linux
5️⃣ Install Python Dependencies
Once the environment is activated, install Django and other Python dependencies:

bash
Copy code
pip install django
6️⃣ Check Django Version
Verify that Django is installed correctly:

bash
Copy code
django-admin --version
7️⃣ Run the Django Development Server
Start the Django development server:

bash
Copy code
python manage.py runserver
The server should now be running at http://127.0.0.1:8000/.

⚙️ Git Submodules
If the project includes Git submodules, follow these steps to manage them:

bash
Copy code
# Check the status of submodules
git submodule status

# List staged files, including submodules
git ls-files --stage | grep 160000
❌ Deactivating the Virtual Environment
When you are done working, deactivate your virtual environment:

bash
Copy code
conda deactivate
# or
deactivate  # For virtualenv
🛑 Troubleshooting
🔧 Issue: ModuleNotFoundError: No module named 'django'
If you encounter the following error:

vbnet
Copy code
ModuleNotFoundError: No module named 'django'
It means Django is not installed in your virtual environment. To fix this, run:

bash
Copy code
pip install django
📦 Additional Notes
Upgrading pip: If you see a notice about an outdated pip version, update it with:
bash
Copy code
python -m pip install --upgrade pip
Ensure the virtual environment is active: Always activate the virtual environment before running Django commands.
🔗 Useful Links
Django Documentation
Node.js Documentation
💡 Tips & Tricks
To check if your virtual environment is active, you should see (test) in your terminal prompt.
If you face any other issues, consult the logs or search for the error message in Google for a solution.
