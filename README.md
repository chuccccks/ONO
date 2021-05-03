# ONO OFFICIAL DEVELOPEMENT
<img src="https://github.com/chukkyiii/ONO/blob/main/static/img/ono_logo.png?raw=true" alt="ONO" width="256" height="256" >

```python
  status: 'underdevelopment'
  path: 'still deciding'
  goal: 'not sure yet'
```
This is just the current goal I have in mind not sure, where this is going will update this soon. 

## RUNNING 
```shell
bash ono.sh 

or 

zsh ono.sh
```
Should start running on your localhost...

# DATABASE (MONGODB)

Set up a mongo collection and make a database with two collection called `users` and `messages` 
Then create a file called `config.py` and connect it to your database like so: 

```python 
  import ssl
  from pymongo import MongoClient

  client = MongoClient( 
      'Insert Connection String Here',
      ssl = True,
      ssl_cert_reqs=ssl.CERT_NONE
      ) 
```