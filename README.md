# openshift-ex288-training

## Install s2i on ubuntu -- repo location
- https://github.com/openshift/source-to-image
- https://github.com/openshift/source-to-image/releases
- https://github.com/openshift/source-to-image/releases/download/v1.3.0/source-to-image-v1.3.0-eed2850f-linux-amd64.tar.gz

## script
- wget https://github.com/openshift/source-to-image/releases/download/v1.3.0/source-to-image-v1.3.0-eed2850f-linux-amd64.tar.gz
- tar xvf https://github.com/openshift/source-to-image/releases/download/v1.3.0/source-to-image-v1.3.0-eed2850f-linux-amd64.tar.gz

## s2i study notes
- ## from s2i github repo
- s2i build https://github.com/sclorg/django-ex centos/python-35-centos7 hello-python
- docker run -p 8080:8080 hello-python
- ## to see s2i run/assemble execution path
- docker inspect <image> | grep openshift
