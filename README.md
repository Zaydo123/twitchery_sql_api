# SQL API TWICHERY
ik i spelled it wrong in the repo name but whatever.

## Basics
First, if the database doesn't exist yet, we need to call the ```create_db()``` function to create the database.

After calling ```create_db()```, you need to connect to the database via the ```connect()``` function.

# User Table
the user table stores information about each registered user. This includes information in the order of **Discord ID** *(stored as string)*, **Token Balance** *(integer)*, and **Premium Status** *(bit)*

In the database they are formally named as ```discord_id```, ```token_count```, and ```premium```.
