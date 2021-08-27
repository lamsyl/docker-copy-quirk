## Takeaway

Copy a directory will copy its content to the destination.

`COPY src dest` is same as

```
mkdir src dest
touch src/main.cpp
cp -r src/ dest
```

OR

```
mkdir src
touch src/main.cpp
cp -r src dest
```

But is different from

```
mkdir src dest
touch src/main.cpp
cp -r src dest
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
ls -l .
```

What will you see in /usr/src/app?

a. `v1.cpp` (content inside `v1/`)

b. `v1/` (`v1/` directory itself)

c. `v2.cpp` (content inside `v2/`)

d. `v2/` (`v2/` directory itself)
