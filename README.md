**A Simple Blog Application built using [Django](https://docs.djangoproject.com/en/3.9/) Framework.**

                                      Hit the ⭐ button to show some ❤️           

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See [deployment](#Deployment) for notes on how to deploy the project on a live system.

### Prerequisites
```
Any Code Editor (VS Code preferred)
Python version 3.7 or higher
Latest version of Git
A PythonAnywhere Account (for deploying the project on a live system)
```

### Development Environment Setup : Windows
**Step 1** : Downloading and Installing the Code Editor

| **Code Editor** | **Link** 	|
|-	|-	|
| Visual Studio Code 	| [Download it from here](https://code.visualstudio.com/)	|
| Sublime Text 3 	| [Download it from here](https://www.sublimetext.com/3) |
| Atom 	| [Download it from here](https://atom.io/)	|

---
**Step 2** : Installing Python
* Click on [Download Python](https://www.python.org/downloads/windows/).
* Click on the "Latest Python 3 Release - Python x.x.x" link.
   * * Download the Windows x86-64 executable installer for 64-bit version of Windows
   * * Download the Windows x86 executable installer for 32-bit version of Windows.


* Make sure to check "Add Python 3.x to Path" in the setup window of the Installer.

Verify the installation from the command prompt using following command :
```
python --version
```
And the installed version of python will be printed.


---
**Step 3**: Creating Project Directory 


(Note : We are creating project directory in the desktop for ease of access)

```
cd desktop

mkdir mydblogtask

cd mydblogtask
```
---
**Step 4**: Cloning Repository using Git
```
git clone https://github.com/Favy-source/My-Django-BlogTask.git
```
Note: The cloned repo directory need to be renamed as "My-Django-BlogTask".

---
**Step 5**: Creating Virtual Environment

Change the directory to the required one where the virtual environment will be created :
```
cd My-Django-BlogTask
```
Creating Virtual Environment named "myvenv" :
```
python -m venv myvenv
```
Activating "myvenv" :
```
myvenv\Scripts\activate
```
Command to deactivate "myvenv" :
```
deactivate
```
---
**Step 6**: Installing Requirements


Note: Virtual Environment should be activated.


Upgrading pip to the latest version :
```
python -m pip install --upgrade pip
```


Installing requirements :
```
pip install -r requirements.txt
```
**Step 7**: Creating Superuser and making database migrations to access the default Admin Panel
```
python manage.py createsuperuser
```
```
python manage.py makemigrations blog
python manage.py migrate blog
```

---
**Step 8**: Running the Project in local server


Note: Virtual Environment should be activated.


Run the following command in the terminal :
```
python manage.py runserver
```

---
## Deployment

Sign Up for a free account in Pythonanywhere.com and generate an API token.

```
pip3.7 install --user pythonanywhere

pa_autoconfigure_django.py --python=3.7 https://github.com/<your-github-username>/<your-github-repo-link>.git

python manage.py createsuperuser

python manage.py collectstatic
```


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* I4G ZuriTrainin and HNG Internship, Django Girls Tutorial
