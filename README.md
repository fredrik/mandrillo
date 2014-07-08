

Run the simplest possible wsgi app:

(see `wsgi.py`)

Create a virtual environment: `virtualenv env`
Activate: `source env/bin/activate`
Install uwsgi in virtualenv env: `pip install uwsgi`
Run app: `uwsgi -s 127.0.0.1:9000 --protocol=http --module wsgi --callable app`


Run the simplest possible flask app:

(see `f.py`)

Install flask in virtual env: `pip install flask`
Run app: `uwsgi -H env -s 127.0.0.1:9000 --protocol=http --module f --callable app`
