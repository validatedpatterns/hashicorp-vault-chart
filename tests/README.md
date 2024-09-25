# Unit tests for the pattern-install chart with helm-unittest framework

## Testing documentation

The syntax for writing tests can be found [here](https://github.com/helm-unittest/helm-unittest/blob/main/DOCUMENT.md)

## Run tests

The following will use a containerized version:
```bash
make helm-unittest
```

## Install framework as helm plugin

```bash
helm plugin install https://github.com/helm-unittest/helm-unittest.git
```

### Run unittest with locally installed helm and helm plugin
```bash
helm unittest .
```

## Run unittests with docker
```bash
docker run -ti --rm -v $(pwd):/apps:z helmunittest/helm-unittest .
```
