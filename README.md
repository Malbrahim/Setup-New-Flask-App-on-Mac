# How to Setup a New Flask App on a Mac

### Quickstart reference for myself or anyone else out there on the internet to get up and running with Python and Flask on a Mac (assumes you’ve already installed Python 3, if you haven’t, please visit https://python.org):


**First, make sure virtualenv is installed**

``` $ pip3 install virtualenv```


**Then create a directory for your new Flask project**

```$ mkdir MyNewFlaskApp```


**Navigate to your newly created directory**

```$ cd MyNewFlaskApp```


**Create your virtual environment**

```$ virtualenv venv --system-site-packages```


**Activate the virtual environment**

```$ source venv/bin/activate```


**Make sure Flask is installed**

```(venv) $ pip3 install Flask```


**Now write the actual python code for your flask application. We’ll call our python script my_new_flask_app.py. Save this script in your MyNewFlaskApp directory.**

```from flask import Flask

app = Flask(__name__)

@app.route('/')
def index():
    return 'hello, world'
view rawmy_new_flask_app.py hosted with ❤ by GitHub
```


**Set the FLASK_APP system variable**

```(venv) $ export FLASK_APP=my_new_flask_app.py```


**Run Flask**

```(venv) $ python3 -m flask run```


**Visit http://127.0.0.1:5000 to see your app in action**



Resource: https://topherpedersen.blog/2019/12/28/how-to-setup-a-new-flask-app-on-a-mac/ 
