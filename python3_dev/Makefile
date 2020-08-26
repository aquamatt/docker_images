REPO_NAME=rtl
VERSION=1.0

ALL: Dockerfile
	docker build -t $(REPO_NAME)/python3 .
	docker image tag $(REPO_NAME)/python3:latest $(REPO_NAME)/python3:$(VERSION)

clean:
	docker image rm $(REPO_NAME)/python3
