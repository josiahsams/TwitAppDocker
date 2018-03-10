# TwitAppDocker

Steps to run:

1. Export the Twitter API keys:

- export CONSUMER_SECRECT=ABC
- export ACCESS_TOKEN_SECRECT=ABC

2. Clone this repo.

- git clone https://github.com/josiahsams/TwitAppDocker.git
- cd TwitAppDocker

3. Prepare a pre-trained tensorflow model and place it under ./Tensorflow/tf_files
```
$ ls -l Tensorflow/tf_files
total 180040
-rw-r--r--  1 joe  staff  87434154 Mar  6 13:04 retrained_graph.pb
-rw-r--r--  1 joe  staff        19 Mar  6 13:02 retrained_labels.txt
```

4. To persist the mongodb data, create a directory "db",

- mkdir db

5. build the docker image
- docker-compose build

6. Start all the services,

- docker-compose up

7. Web Application is running in port 3000

http://localhost:3000
