# Yugabyte Python ORM implementation sample using sqlalchemy

This example project shows you how you can use Python with sqlalchemy to connect to a Yugabyte cluster and perform various ORM operations.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

* Yugabyte
* Python3
* sqlalchemy

### Installing

## Install the Python requirements

Use the pip command to install all
of the Python dependencies listed in the requrements.txt file

```
pip3 install -r requirements.txt
```

This environment is now configured to run the python code.  

## Open src/config.py and update the database settings:

```
listen_port = 8000
db_user = 'postgres'
db_password = None
database = 'postgres'
db_host = 'localhost'
db_port = 5433
```

---
### Your environment should now be ready!
It is time to run the client application that will create and list objects from the Yugabyte database.  The Python application listens on a port (configured to port 8000) for Post/Get commands and it will interact with the Yugabyte database to create the required User, Product and order objects.

### Start the server that will listen for your commands: 

```
./src/rest-service.py
```

Note that the rest-service.py file contains the "shebang" that defines Python3 to be the program loader for this file.
