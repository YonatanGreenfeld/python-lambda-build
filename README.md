# python-lambda-build
Docker images for building python aws lambda containers
These images are meant to be used with the 
[serverless-python-requirements-plugin](https://www.serverless.com/plugins/serverless-python-requirements).

### Supported versions:
- 3.11
- 3.10
- 3.9
- 3.8
### Supported architectures:
- x86_64
- arm64

### Usage
Pulling the image:
```shell
docker pull ghcr.io/yonatangreenfeld/python-lambda-build/python:3.10-x86_64
```

In the `serverless.yml` file:
```yaml
custom:
  pythonRequirements:
    dockerizePip: true
    dockerImage: ghcr.io/yonatangreenfeld/python-lambda-build/python:3.10-x86_64
```
