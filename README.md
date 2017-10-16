# Google gcr.io container mirrors

https://hub.docker.com/r/jungleran/gcr

## Mapping rules:

```
Image name: jungle/gcr
Tag name: [ORIGINAL_IMAGE_NAME]-[ORIGINAL_TAG_NAME]
```

For example:

Original:

```
docker pull gcr.io/google_containers/echoserver:1.4
```

Mirror:

```
docker pull jungleran/gcr:echoserver-1.4
```

## References

- `--image-pull-policy=IfNotPresent` https://github.com/kubernetes/kubernetes/issues/24903#issuecomment-274319080
- Added a `--registry-mirror` flag to minikube start https://github.com/kubernetes/minikube/blob/master/CHANGELOG.md#version-080---8172016
