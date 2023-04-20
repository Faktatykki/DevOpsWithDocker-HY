FROM python:latest

WORKDIR /usr/src/app

EXPOSE 8000

ENV PYTHONUNBUFFERED=1

COPY ./hy-cyber-security-project/brokensite/requirements.txt .

RUN apt-get update                                              && \
    apt-get -y install libpq-dev gcc                            && \
    pip3 install --no-cache-dir --upgrade -r ./requirements.txt && \
    rm -rf /var/lib/apt/lists/*

COPY ./hy-cyber-security-project/brokensite .

RUN python3 manage.py migrate

CMD [ "python3", "manage.py", "runserver", "0.0.0.0:8000" ]

#Commands to make the image:
#git clone git@github.com:Faktatykki/hy-cyber-security-project.git
#docker build . -t "cbs-project"
#docker login
#docker tag cbs-project faktatykki/cbs-project
#docker push faktatykki/cbs-project
