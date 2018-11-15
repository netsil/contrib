VERSION=v3-epoch
PROJECT_ID=nutanix-epoch
PROJECT=gcr.io/${PROJECT_ID}

all: build

build:
	docker build --pull -t ${PROJECT}/k8szk:${VERSION} .

push: build
	docker push ${PROJECT}/k8szk:${VERSION}

.PHONY: all build push
