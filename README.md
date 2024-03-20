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

    - Create a static folder
        - Create a css folder inside static
            - Create a style.css file and add css in there from above shown folder
    - Create a templates folder
        - Create index.html and add this code
            - ```
            <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A weather app to check current weather conditions and forecasts.">
    <meta name="keywords" content="weather, weather app, forecast, temperature, humidity, wind speed">
    <meta name="author" content="Your Name">
    <meta property="og:title" content="Your Weather App">
    <meta property="og:description" content="Check current weather conditions and forecasts with our weather app.">
    <meta property="og:image" content="https://example.com/your-app-icon.png">
    <meta property="og:url" content="https://example.com">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="Your Weather App">
    <meta name="twitter:description" content="Check current weather conditions and forecasts with our weather app.">
    <meta name="twitter:image" content="https://example.com/your-app-icon.png">
    <title>Your Weather App</title>
    <link rel="stylesheet" href="{{ url_for('static', filename='styles/style.css')}}" />
</head>
<body>
    <h1>Get Weather Conditions</h1>
    <form action="/weather">
        <input type="text" name="city" id="city" placeholder="Enter a City">
        <button type="submit">Submit</button>
    </form>
</body>
</html>
```
