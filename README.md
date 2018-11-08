# Node 11 with Textract
Based on debian:wheezy image to support [Textract](https://github.com/dbashford/textract).

## Update
``` docker push czconsultants/node11-textract ```

## Build
``` docker build -t czconsultants/node11-textract . ```

## Packages
We install the following packages within our image.

* [catdoc](http://www.wagner.pp.ru/%7Evitus/software/catdoc/)
* [pdftotext](http://www.foolabs.com/xpdf/download.html)
* [tesseract](http://code.google.com/p/tesseract-ocr/)

Currently not supporting [drawingtotext](https://github.com/davidworkman9/drawingtotext).


## Useful commands
Some helpful commands for maintaining docker containers and images.

### docker images
List your docker images

### docker rm $(docker ps -a -q)
Remove all containers from your system

### docker rmi $(docker images -q)
Remove all images from your system but remember to remove containers before.
