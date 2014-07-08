Create a virtual environment: `virtualenv env`
Activate: `source env/bin/activate`
Install uwsgi in virtualenv env: `pip install uwsgi`
Run app: `uwsgi --socket 127.0.0.1:9000 --protocol=http --module wsgi --callable app`
