# Dockerfile starts here
FROM centos:7
LABEL "about" = "This is a sample application file"
RUN yum -y update
RUN yum -y install python
RUN yum -y install epel-release && yum clean all
RUN yum -y install python-pip 
RUN pip install flask
COPY ./app.py /app.py
CMD ["echo", "File copied"]
ENTRYPOINT FLASK_APP = /app.py flask run --host 0.0.0.0
# Dockerfile ends here
