Project Setup and Usage
This guide will help you set up the project, run the server, and troubleshoot any issues you may encounter.

Prerequisites
Before you start, ensure you have the following installed:

Node.js for running front-end build scripts.
Python (version 3.8 or higher) for running the back-end Django server.
Conda for managing Python environments.
Git for version control.
Project Setup
1. Clone the Repository
bash
Copy code
git clone <repository_url>
cd ecom-proj-master
2. Install Node Dependencies
To build the front-end assets, run the following command:

bash
Copy code
npm run build
3. Start the Front-End Server
To start the front-end server, run:

bash
Copy code
npm run start
4. Set Up Python Virtual Environment
Create and activate a Python virtual environment to isolate dependencies:

bash
Copy code
# Create a new virtual environment
python -m venv test

# Activate the environment
test\Scripts\activate  # On Windows
source test/bin/activate  # On Mac/Linux
5. Install Python Dependencies
If you are using Django and need to install required dependencies, run:

bash
Copy code
pip install django
6. Check Django Version
To verify the installed Django version:

bash
Copy code
django-admin --version
7. Run Django Development Server
To run the Django server:

bash
Copy code
python manage.py runserver
Git Submodules
If the project uses Git submodules, you may need to check their status or update them. Use the following commands:

bash
Copy code
# Check the status of submodules
git submodule status

# List staged files with submodules
git ls-files --stage | grep 160000
Deactivating the Virtual Environment
When you're done, you can deactivate the virtual environment by running:

bash
Copy code
conda deactivate
# or
deactivate
Troubleshooting
Issue: ModuleNotFoundError: No module named 'django'
If you see the error message:

vbnet
Copy code
ModuleNotFoundError: No module named 'django'
This indicates that Django is not installed in your virtual environment. You can resolve this by running:

bash
Copy code
pip install django
Notes
If you encounter issues with the version of pip, upgrade it by running:
bash
Copy code
python -m pip install --upgrade pip
Ensure your virtual environment is activated before running Django commands.
