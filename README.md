### BUILDING ECOMMERCE APP BY CLONNING AMAZON USING DJANGO 3.2.X

#### 1. Initial commit

        new file:   .gitignore
        new file:   README.md

#### 2. Create virtual environment

	    > python -m venv venv3932
	    modified:   README.md

#### 3. Installing Django

	    > venv3932\Scripts\activate
	    (venv3932) ..> python -m pip install django==3.2.*
	    modified:   README.md

#### 4. Create django project 'config' inside src folder

	    (venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder\src> django-admin startproject config .

        modified:   README.md
        new file:   config/__init__.py
        new file:   config/asgi.py
        new file:   config/settings.py
        new file:   config/urls.py
        new file:   config/wsgi.py
        new file:   manage.py

#### 5. Checking the project's structure folders and files

        (venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder> tree src /f
		Folder PATH listing
		Volume serial number is DC72-8D6C
		E:\2021\DJANGO\WINDOWS\ECOM_CLONE_AMAZON_YTB_SUPERCODER\SRC
		│   .gitignore
		│   manage.py
		│   README.md
		│
		└───config
		        asgi.py
		        settings.py
		        urls.py
		        wsgi.py
		        __init__.py

#### 6. Creating django app's structure folder

        (venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder\src> mkdir app

#### 7. Create django app 'main' inside the app folder

        (venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder\src> python manage.py startapp main app\main


#### 8. Install 'main' app to the project 'config'

        modified:   README.md
        modified:   app/main/apps.py
        modified:   config/settings.py


#### 9. Checking the folder structures

        (venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder\src> tree app /f
        Folder PATH listing
        E:\2021\DJANGO\WINDOWS\ECOM_CLONE_AMAZON_YTB_SUPERCODER\SRC\APP
		└───main
		    │   admin.py
		    │   apps.py
		    │   models.py
		    │   tests.py
		    │   __init__.py
		    │
		    ├───migrations
		    │   │   __init__.py
		    │   │
		    │   └───__pycache__
		    │           __init__.cpython-39.pyc
		    │
		    └───__pycache__
		            admin.cpython-39.pyc
		            apps.cpython-39.pyc
		            models.cpython-39.pyc
		            __init__.cpython-39.pyc

        modified:   README.md

#### 10. Creating Admin app
        
        (venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder\src> python manage.py makemigrations
		No changes detected
		(venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder\src> python manage.py migrate
		Operations to perform:
		  Apply all migrations: admin, auth, contenttypes, sessions
		  ...
		  Applying sessions.0001_initial... OK

		> Create super user  
		(venv3932) PS E:\2021\DJANGO\WINDOWS\ecom_clone_amazon_ytb_supercoder\src> python manage.py createsuperuser
		Username (leave blank to use '62812'): admin
		Email address: admin@admin.com
		Password:
		Password (again):		
		        modified:   db.sqlite3



















































































































































































































