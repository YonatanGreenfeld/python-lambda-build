# python-lambda-build
Docker images for building python aws lambda containers
These images are meant to be used with the 
[serverless-python-requirements-plugin](https://www.serverless.com/plugins/serverless-python-requirements).

### Supported versions:
- 3.12
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
docker ghcr.io/jitsecurity/python-lambda-build/python:3.8-x86_64
```

In the `serverless.yml` file:
```yaml
custom:
  pythonRequirements:
    dockerizePip: true
    dockerImage: ghcr.io/jitsecurity/python-lambda-build/python:3.8-x86_64
```
