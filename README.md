
## Boilerplate

Inspect your environment
docker run -it -p 9000:9000 -p 35729:35729 -d -v $(pwd)/app:/src/app deanvn/docker-web-app 

Gulp Serve
docker run -it -p 9000:9000 -p 35729:35729 -d -v $(pwd)/app:/src/app deanvn/docker-web-app gulp serve
docker run -it -p 9000:9000 -p 35729:35729 -d -v $(pwd)/app:/src/app --name <your-app-name> deanvn/docker-web-app gulp serve

Need to run an additional command in the running container like gulp assemble:
docker exec -it docker-web-app gulp assemble

Or run a bash shell in the running container
docker exec -it docker-web-app /bin/bash 
