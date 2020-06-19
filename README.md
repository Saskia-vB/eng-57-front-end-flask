# Build a website with Flask

## What is Flask? 
Flask is a micro web framework written in Python. It's a microframework because it does not require particular tools or libraries. 

## Install
Install with pip in terminal: pip install Flask

### Minimal application 
```python
from flask import Flask
app = Flask(__name__)

@app.route('/')
def hello_world():
    return 'Hello, World!'

```

Once you import Flask you need to create an instance of the Flask class for the web app. 

```python
if __name__ == '__main__':
    app.run(debug=True)
```
Python assigns "__main__" to the script when the script is being executed. Here, __name__ is equal to __main__ which means the conditions statement is satisfied and the app.run() method will be exectued. 

Setting the debug parameter to True will print out possible Python errors on the web page helping us trace errors. But in a production environment set it to False to avoid security issues. 

## What is Bootstrap? 
A popular framework for building responsive websites. 

### Application 

On your CSS stylesheet: 
```CSS
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
```

On your html page, use JS right before the closing </body> tag:

```JS
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
```