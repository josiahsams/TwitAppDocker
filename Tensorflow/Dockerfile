FROM tensorflow/tensorflow

RUN mkdir /code

RUN mkdir /tf_files

RUN pip install --upgrade pip

RUN pip install --upgrade tensorflow

RUN pip install Flask

ADD https://raw.githubusercontent.com/josiahsams/TwitApp/master/predict.py /code

COPY ./tf_files /tf_files

CMD ["/usr/bin/python", "-u", "/code/predict.py" ]
