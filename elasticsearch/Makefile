.PHONY:	build push save load

VENDOR = kuberdock
NAME = elasticsearch
VERSION = 2.2
TAG = $(VENDOR)/$(NAME):$(VERSION)
TAR = $(VENDOR)_$(NAME)_$(VERSION).tar

build:
	docker build -t $(TAG) .

push:
	docker push $(TAG)

save:
	docker save -o $(TAR) $(TAG)

load:
	docker load -i $(TAR)
