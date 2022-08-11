FROM python:3.11-rc-bullseye
RUN apt update && apt install -y python3 python3-dev python3-distutils uwsgi uwsgi-src uuid-dev libcap-dev libpcre3-dev python3-pip python3-venv uwsgi uwsgi-plugin-python3
RUN python -m pip install --upgrade pip && python -m pip install flask
COPY uwsgi.ini wsgi.py /
