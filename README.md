# (Setup)

* Create a virtual environment: `virtualenv env`
* Activate: `source env/bin/activate`
* Install uwsgi in virtualenv env: `pip install uwsgi`


# Run the simplest possible wsgi app:

(see `wsgi.py`)

* Run app: `uwsgi --http 127.0.0.1:9000 -w wsgi:app`


# Run the simplest possible flask app:

(see `f.py`)

* Install flask in virtual env: `pip install flask`
* Run app: `uwsgi -H env --http 127.0.0.1:9000 -w f:app`
