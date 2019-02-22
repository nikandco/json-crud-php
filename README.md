# json-crud-php
JSON files used as DB on your server running PHP. Perform CRUD operations and work with different files. Access / Update / delete - only parts of the JSON object. Simple to install. Just place in a folder next to your JSON file and start working. 
It functions like a REST API in the following format file / jsonKey
Example request
GET /jsonObjectFile/users
response
{
"niki":
  { 
    "todo":  "22-02-2019",
    "shopList": ['eggs','milk','water']
  }
}
would return whatever the users key holds

Example edit request
  POST /jsonObjectFile/users/niki
  data: {"todo":"22-02-2019","shopList":['eggs','milk','water']}



# Installation
Place the /json-crud-php/ in your project folder.  That's it.  Edit the config.php to match your needs. 
Atuehntication is supported. Users can access only explicitly specified files. 
