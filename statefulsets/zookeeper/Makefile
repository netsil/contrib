VERSION=v3-epoch
PROJECT_ID=gcr.io/nutanix-epoch/zookeeper
PROJECT=gcr.io/${PROJECT_ID}

all: build

build:
	docker build --pull -t ${PROJECT}/k8szk:${VERSION} .

push: build
	gcloud docker -- push ${PROJECT}/k8szk:${VERSION}

.PHONY: all build push
