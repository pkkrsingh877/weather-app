# Documentation

## 1. Create a Virtual Environment

```Python
py -m venv .venv
```

## 2. Activate The Virtual Environment

```Python
source .venv/Scripts/activate
```

The above written commands are supposed to be run on a Windows OS and on Git Bash.

## 3. Install Some Important Packages

```Python
pip install requests python-dotenv Flask
```

## 4. Update pip version if update available

```Python
python.exe -m pip install --upgrade pip
```

## 5. Create requirements.txt file

```Python
pip freeze > requirements.txt
```

This lists down all of the installed packages or dependencies required to run our application.

## 6. Create .gitignore file 

Create that file(.gitignore) and add .venv and .env to make sure that these files are not shared on GitHub or any other platform alternative to GitHub.

```
.venv/
.env
```
This will be the content of your .gitignore file.

## 7. Initialize Git Repository Locally and link to GitHub Repository Online

## 8. Get API Key and Put in .env file

Create an account on openweathermap.org and get an api key from there. 

Next Step is to put that api key in the .env file

```
API_KEY = a12398721397asd
```

Something like this should be in the .env file.

## 9. Create Some New Folders

a. static
b. templates
