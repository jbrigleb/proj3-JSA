FROM python:3.6
MAINTAINER Jack Brigleb "jbrigleb@uoregon.edu"
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
COPY . /vocab
WORKDIR /vocab
RUN pip install -r requirements.txt
ENTRYPOINT ["python"]
CMD ["flask_vocab.py"]
