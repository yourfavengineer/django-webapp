FROM python:3.10-slim  

COPY . /app

WORKDIR /app

RUN  python3 -m venv /opt/venv && \
        pip install pip-upgrade && \
        /opt/venv/bin/pip install -r requirements.txt && \
        chmod +x entrypoint.sh 

CMD ["/app/entrypoint.sh"]