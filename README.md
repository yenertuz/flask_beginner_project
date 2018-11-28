# Flask_Hello_World

```
from flask import Flask
app = Flask(__name__)

@app.route("/")
def hello():
    return "Hello World!"

if __name__ == "__main__":
    app.run(ssl_context='adhoc')
```

To use ad hoc certificates with Flask, you need to install an additional dependency in your virtual environment:

```
$ pip install pyopenssl
```

When you run the script, you will notice that Flask indicates that it is running an https:// server:
```
$ python hello.py
 * Running on https://127.0.0.1:5000/ (Press CTRL+C to quit) ```
