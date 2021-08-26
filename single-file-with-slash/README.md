## Comparison betweeen `single-file-without-slash` and `single-file-with-slash`

### `single-file-without-slash`

```
COPY file /dir1/dir2
```


### `single-file-with-slash`

```
COPY file /dir1/dir2/
```

## Build image

```
docker build -t docker-copy-quirk .
```

## Run image

```
docker run --rm -it docker-copy-quirk
```

## Inspect

```
ls -l /usr/src
```

Where is the copied `package.json` in ...?
- app
- web
