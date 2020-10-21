# openshift-ex288-training

## 10/21/20 READER NOTE: This repo is a WIP while I study for the ex288 exam

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

## config map
- kubectl create cm config-map-demo --from-literal=key1=value1
- kubectl create -f bbox1.yaml
- kubectl exec -it bbox1 -- env

## useful links
- This Repo: https://github.com/rlaskew/openshift-ex288-training
- 4.2 Playground (exam version I'm taking): https://learn.openshift.com/playgrounds/openshift42/
- Exam Objectives: https://www.redhat.com/en/services/training/ex288-red-hat-certified-specialist-openshift-application-development-exam?section=Objectives
- Main Repo is also good: https://github.com/luckylittle/openshift-cheatsheet/blob/master/DO288.md
