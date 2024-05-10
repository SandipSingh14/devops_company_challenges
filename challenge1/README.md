## Challenge 1. Docker and CI/CD

> Estimated time: 30 minutes

Now, show us your skills with Python (or whatever language you are most comfortable with) to develop a webserver (using `HTTPServer` python library) which listens on port `8000`. When you make a request to the server, it will return the following information:

![webserver-example.png](images/ch1-webserver-example.png "Example output Challenge-1")

Once you have it finished, can you create a Dockerfile and build an image with your application?

Helpers:

- [HTTPServer library](https://docs.python.org/3/library/http.server.html)
- [Dockerfile instructions](https://docs.docker.com/develop/develop-images/instructions/)

Optional:

- Application accepts arguments. Example: `--host`, `--port`
- Securize your Dockerfile
- Allow pass arguments when executing `docker run`. For example: `docker run <your-image-tag> --port 8081`
- Pass coverage with `dive` ([wagoodman/dive](https://github.com/wagoodman/dive)). Use `.dive-ci` that is provided in the repository

```bash
# command
CI=true dive <your-image-tag>

# result
Result:PASS [Total:3] [Passed:3] [Failed:0] [Warn:0] [Skipped:0]
```

- Upload your image to Docker Hub account with Github Actions ([docker/build-push-action](https://github.com/docker/build-push-action))
