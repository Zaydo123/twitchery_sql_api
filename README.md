# SQL API TWICHERY
ik i spelled it wrong in the repo name but whatever.

## Basics
First, if the database doesn't exist yet, we need to call the ```create_db()``` function to create the database.

After calling ```create_db()```, you need to connect to the database via the ```connect()``` function.

# User Table
the user table stores information about each registered user. This includes information in the order of **Discord ID** *(stored as string)*, **Token Balance** *(integer)*, and **Premium Status** *(bit)*

In the database they are formally named as ```discord_id```, ```token_count```, and ```premium```.

## User Table Functions
```tokens``` is the amount of tokens the user will start of with, and ```is_premium``` and ```boolean_bit``` are bits representing whether or not the user is a premium member. 1 = yes, 0 = no

1. Create a new user object `new_user(user_id,tokens,is_premium)`
2. Add amount to token balance `add_tokens(user_id,amount)` 
3. Subtract amount from token balance `subtract_tokens(user_id,amount)` 
4. Set token balance to specific integer `set_tokens(user_id,amount)` 
5. Set premium membership status `set_premium(user_id,boolean_bit)` 
