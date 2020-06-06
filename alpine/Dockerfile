FROM alpine 
RUN apk add curl
RUN apk add python
RUN apk add python-dev
#RUN apk add python-utils
RUN apk add g++
RUN apk add gcc
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN python2.7 get-pip.py
RUN pip install django==1.8.16
RUN pip install requests==2.2.1
RUN echo "Create a layer" >  /etc/testfile
COPY ./file.tar /tmp/
RUN pip install django -U 
RUN pip install requests -U
