FROM centos 
RUN yum -y upgrade 
RUN yum install -y python3
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
RUN chmod 666 get-pip.py
RUN python3 get-pip.py
RUN pip install django==1.8.16
RUN pip install requests==2.2.1
RUN echo "Create a layer" >  /etc/testfile
COPY ./file.tar /tmp/
RUN pip install django -U 
RUN pip install requests -U
