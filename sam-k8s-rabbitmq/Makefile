package:
	mvn package

build: package
	docker build . --tag myguddy/sam-springboot-redis:latest
	docker push myguddy/sam-springboot-redis:latest
run:
	docker run -d --name rabbitmq  -p 15672:15672 -p 5672:5672 rabbitmq:3.7-management