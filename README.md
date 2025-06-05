How to set the App Up?

-> Pre req

  Python3
  
  Postgres DB(DB of your choice) -> Note for different dbs there will be a slight change in setup of line 24 database file. Refer Fastapi docs

Step 1

  Make a python virtual env
  Change to venv 

    python -m venv myenv
    source myenv/bin/activate (For linux)
    ./myenv/Scripts/activate (For windows)


Step 2

  install all the requirements from requirements.txt
  
    pip install -r requirements.txt

Step 3
  Add the below environment variables

          DATABASE_HOSTNAME=
          DATABASE_USERNAME=
          DATABASE_NAME=
          DATABASE_PORT=
          DATABASE_PASSWORD=
          SECRET_KEY=
          ALGORITHM =
          ACCESS_TOKEN_EXPIRE_MINUTES=



Stpe 4
  Run the server via uvicorn/fastapi form the root directory{directory contatning app folder} after populating the table via alembic.

    alembic upgrade head #db migration tool
    uvicorn app.main:app / fastapi app.main:app

Step 5
  If ur running in localhost check -> 127.0.0.1:8000/docs for interactive documnets 
  Alternativly you can use postman

!! Check for any typos !!


  
