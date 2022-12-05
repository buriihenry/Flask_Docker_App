## Building our Flask App and connecting it to Postgres db using Docker Compose
In this project I will show you how to deploy ML model using Flask 

### Requirements
You must create a vitual environment for the app to run

You must have Docker, Python and Flask installed.

Flask version: 2.2.2
pip install Flask==2.2.2

### Running the project
1. Ensure that you are in the project home directory. Run Docker file "docker-compose.yml" first

The command for running docker is 

```
docker-compose up.
```

2. After running the docker container, Login in to the PgAdmin4 
```
Create a server for this app then create a database called "students"
```
3. On the Terminal run below commands to activate the connection and create a db

```
python
app.app_context().push()
db.create_all()
```
4. After the connecting to our schema,run below command to start our app

```
python app.py
```

5. Navigate to URL http://127.0.0.1:5000/

You should be able to view the homepage.

Enter valid values in the form and hit Submit.

If everything goes well, you should  be able to see submitted vaules in the Postgres database page!



