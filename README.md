
This tutorial covers the basics to show how a Python backend works in its simplest form, yet covering avery major
concept.

Install Pycharm community edition
https://www.jetbrains.com/help/pycharm/installation-guide.html

Based on: https://fastapi.tiangolo.com/tutorial/first-steps/
And also: https://sqlmodel.tiangolo.com/tutorial/
Can also help: https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/
Manage multiple versions of Python with pyenv: https://realpython.com/intro-to-pyenv/
SQlite visualizer: https://sqlitebrowser.org/dl/

Example of pyenv

Example of virtual env.
to ENTER:source env/bin/activate
to LEAVE: deactivate


install FastAPI
pip install fastapi==0.83.0

Implement hello world with GET in FastAPI

Run Server
python3.8 -m uvicorn main:app

Go to browser and check hello world message
http://127.0.0.1:8000/

Stop Server
ctrl + c

Run Server with reload
python3.12 -m uvicorn main:app --reload

See the documentation and play with it
http://127.0.0.1:8000/docs

See alternative documentation
http://127.0.0.1:8000/redoc

Add or remove async definition

Add a /my/path endpoint

Play with insomnia

Add a POST endpoint

Show possible error with 405 response indicating method not allowed

Show how the debugger works!
1. add error
2. run server from Pycharm with Bug execution, with:
  uvicorn.run('main:app', host='0.0.0.0', port=8000, proxy_headers=True, reload=True)
3. Use smart import from pycharm
4. add breakpoint
5. run endpoint, stop and reproduce error
6. solve error: ERROR:    [Errno 48] Address already in use, solve with another script and with if __name__ == '__main__':
7. run again

install SQLModel
pip install sqlmodel==0.0.16
=> can try pycharm UI
pip install pydantic==1.10.11

show Sqlite viewer

Create DB and table

Create heroes and show, with: SELECT * from hero;

Implement POST endpoint to insert a new Hero.

Talk about async and await

Talk about commit() in a DB.

Done! Congrats! :)
