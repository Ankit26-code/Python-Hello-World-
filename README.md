# Python-Hello-World-
Python Hello World


Steps 

Create Dockerfile 

FROM python
WORKDIR /myapp
COPY . .
RUN pip install -r requirements.txt
EXPOSE 5000
CMD ["python", "app.py"]

Now Creating Docker Image using Dockerfile

command : docker build -t pythonapp .

once image is build now we run the container

Command  : docker run -d -p 5000:5000 pythonapp

Now Docker Container Up 

We Check Container up or Down

Docker ps 

now we check on a browser 

localhost:5000
