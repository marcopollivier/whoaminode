# Who am I, Go? 

Simple HTTP project written in [Node](https://nodejs.org/en/) 

See other _**Who am I?**_ options
- [Who am I, Go?](https://github.com/marcopollivier/whoamigo)
- [Who am I, Java?](https://github.com/marcopollivier/whoamijava)
- [Who am I, Clojure?](https://github.com/marcopollivier/whoamiclojure)

## Docker

### Build Docker image

```bash
$ docker build -t marcopollivier/whoami:node-latest .
```

or [Download the Docker Image](https://hub.docker.com/r/marcopollivier/whoami)

### Push Docker Image

```bash
$ docker push marcopollivier/whoami:node-latest
```

### Run Docker container

```bash
$ docker run --name whoami_go -d -p 8082:8082 marcopollivier/whoami:node-latest
```

## API REST

### Response

- **me**: hostname (container ID for example)
- **timestamp**: execution start time 

```json
{
  "me": "RJ-MB2680.lan",
  "timestamp": "2019-02-12T10:00:00.000Z"
}
```
