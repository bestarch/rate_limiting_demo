# rate limiting demo
###### The demo showcases subscription based API rate limiting using fixed window algorithm. Application also implements authentication and session externalisation using Redis and Spring.

###### Run using docker

	docker run -p 127.0.0.1:8080:8080 -e SPRING_REDIS_HOST=<HOST> -e SPRING_REDIS_PORT=<PORT> -e SPRING_REDIS_PASSWORD=<PSWD> abhishekcoder/rate_limiting_app:latest

###### Execute Redis script
	cd inside /src/main/resources and execute following command
 	cat script.txt | redis-cli -h <HOST> -p <PORT> -a <PASSWORD> --pipe
