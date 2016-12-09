# Docker image to ml-foundations

  Coursera [Machine Learning Foundations: A Case Study Approach](https://www.coursera.org/learn/ml-foundations/) docker image.

  Help paulof at gmail.com or open a issue!

  [my blog](http://www,paulorcf.com)
  Happy learning! :-)


## Based on docker hub

continuumio/anaconda
Official https://docs.continuum.io/anaconda/docker

### Before start

* Change **ENV graphLabLicense**

**Example "YOUREMAIL@DOMAIN.com/YOUR_LICENSE"** at Dockerfile

Get on https://turi.com/download/install-graphlab-create.html

### Read to rock!

* Build

> docker build -t coursera/ml-foundations .

* Running

> docker run -d -p 8888:8888 -v $(pwd)/ml-foundations-week-files:/opt/ml-foundations-week-files -d coursera/ml-foundations

 **Open browser**: http://localhost:8888

 *ml-foundations-week-files* folder is where you need to put your ipynb files.

Your "notebook" is mount at */opt/ml-foundations-week-files* inside docker machine

* Debug

> docker run -i -p 8888:8888 coursera/ml-foundations

* Bashfy :-)

> docker exec -it $YOUR_ID_CONTAINER /bin/bash
