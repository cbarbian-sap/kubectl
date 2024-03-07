# kubectl

How to build:

```bash
VERSION=1.28.6
docker buildx --builder march build \
  --platform linux/amd64,linux/arm64 \
  --build-arg KUBECTL_VERSION=v$VERSION \
  -t ghcr.io/cbarbian-sap/kubectl:$VERSION \
  --push \
  .
```
