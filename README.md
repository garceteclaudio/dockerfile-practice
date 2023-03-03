## Docker image commands

Download docker images from the internet

```bash
docker pull {image}
Examples: 
docker pull mongo
docker pull jenkins/jenkins
docker run --add-host="localhost:192.168.x.x" -p 8080:8080 -p 50000:50000 --name jenkins -d -v /Users/myuserr/Desktop/jenkins/jenkins_home:/var/jenkins_home jenkins/jenkins

        		//nombre contenedor
docker exec -it jenkins bash


docker logs -f nombreContainer
```

List Docker images

```bash
docker images
```

Remove one or more images

```bash
docker rmi {nombreImagen}
```

## Docker container commands

Create and run a new container from an image

```bash
docker run -d -p 27017:27017 mongo
```

List Docker containers that are currently running.

```bash
docker ps
```

Docker start command will start any stopped container.

```bash
docker start {containerID}
```

Stop one or more running containers

```bash
docker stop {containerID}
```

Remove one or more containers

```bash
docker rm {containerID}
```

## Docker compose commands

```bash
docker-compose up
```


## Usage

```python
import foobar

# returns 'words'
foobar.pluralize('word')

# returns 'geese'
foobar.pluralize('goose')

# returns 'phenomenon'
foobar.singularize('phenomena')
```
