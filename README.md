This application is an Inventory Management System for a real time hardware store that stores the application data to your google drive. 

**Application User(s):**

This application can be used by one or more users, for setting up a user the admin needs to follow these steps: 
1. generate a hashed password using [`auth/hasher.py`](auth/hasher.py) and copy it.
2. Go to [`config/auth_config.yaml`](config/auth_config.yaml) and add a new user with its details in it.
3. Paste the copied hashed password for the respective user.

**Application features:**
| Menu Option | Options                                                 | Status    | 
| ----------- | ------------------------------------------------------- | --------- | 
| [Inventario](app_pages/Inventario.py)  | Summary Dashboard                                       | Completed | 
| [Inventario](app_pages/Inventario.py)  | List of products with current totals                    | Completed | 
| [Inventario](app_pages/Inventario.py)  | Edit Inventory (Add, Edit, Delete)                      | Completed | 
| [Ventas](app_pages/Ventas.py)      | Weekly Sales and Losses Report with Dashboard           | Completed | 
| [Ventas](app_pages/Ventas.py)      | Weekly Summary                                          | Completed | 
| [Ventas](app_pages/Ventas.py)      | Historical Sales Log                                    | Completed | 
| Whole App   | Responsive for Mobile and Web                          | Completed | 

**Project Structure:**
- `app_pages:` contains the main 3 application pages source code
- `auth:` contains the authorization checks for system login and logout
- `configs:` configuration files for system users, pages, styling and google drive
- `controllers:` authorization, data and google drive synchronization controllers
- `nav_bar:` main and sub-navigation bar source codes
- `res:` sample database file templates

**Pre-requisites:**

      ﻿streamlit==1.38.0
      pandas==2.2.2
      numpy==2.1.1
      streamlit-extras==0.4.7
      streamlit-authenticator==0.3.3
      streamlit-navigation-bar==3.3.0
      streamlit-option-menu==0.3.13
      PyYAML==6.0.2
      openpyxl==3.1.5
      google-api-python-client==2.146.0
      google-auth-httplib2==0.2.0
      google-auth-oauthlib==1.2.1

you can install these by using the command: `pip install -r requirements.txt`

**How to run the app:**

This is a streamlit app, either you can run it directly via command-line using the command: `streamlit run main.py` OR you can run it in VS code by simply running the `run.py` file through its GUI or `python run.py`
