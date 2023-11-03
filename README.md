# fastapi-react

This is a FullStack project with a FastAPI Backend with PostGresSql database and a React Frontend.
This application got auth, authorizazation. This application is about a millitary school logistic system.

Steps:
You need to download and install a Python interpreter and Node.js and PostgresSQL too (Maybe We need Docker later).

1. Create a (venv)
    1.Create a Python Virtual Environment
    Ctrl + Shift + P in vsCode
    Python: Create Environment
    Select Venv Creates a '.venv' ......
    Select The installed Python interpreter

2. Open the .venv \ Scripts folder on the terminal
    cd .venv\Scripts
    Type activate
    If You get an error type .\activate
    Now You see (.venv) on the console with green

3. Create a fastAPI foolder to the root.
   Create a React folder to the root.

4. Let's create The FASTAPI Backend
    pip install FASTAPI
    pip install uvicorn
    pip install slqalchemy
    pip install pydantic
    pip install psycopg2-binary (Connection port that connects FASTAPI TO psSQL Server)
    FASTAPI is the framework and uvicorn is the ASGI web server

5. Check the install is ok. Sometimes vscode doesn't wanna import the fastAPI modules. Watch out for the green text in the first row.

6. Init fastAPI APP.

    from fastapi import FastAPI   #watch that

    app = FastAPI()

    @app.get('/')
    def sayHello():
    return "Hello:" 

7. Start the server from the console
    uvicorn fastAPI.main:app --reload
