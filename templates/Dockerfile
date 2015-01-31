FROM gitinsky/baseimage:0.1.1
MAINTAINER Git In Sky <support@gitinsky.com>

RUN apt-get update && apt-get -y install python3 python3-setuptools python3-pip cython3 libacl1-dev && ln -s /usr/bin/pip3 /usr/bin/pip && cd /root && git clone https://github.com/msgpack/msgpack-python.git && cd /root/msgpack-python && python3 ./setup.py build && python3 ./setup.py install && pip install attic
VOLUME /repositories
