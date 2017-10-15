# gcr

Google gcr.io container mirrors https://hub.docker.com/r/jungleran/gcr


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
