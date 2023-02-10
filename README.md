# nginx-image-resize

Simple docker container for dynamic image resizing with nginx image_filter module

## .env

example

```.env
PORT=80
QUALITY=80
IMAGE_HOST=https://{storage_account}.blob.core.windows.net/{container}
NGINX_HOST=localhost
```

## Build and Run

```
$ docker-compose build
$ docker-compose up
```

## Usage

In case your .env is as above example.

If you want to get https://{storage_account}.blob.core.windows.net/{container}/your/file/name.jpg`  
just GET `http://localhost/your/file/name.jpg`

If you want to resize.  
just GET `http://localhost/500x500/your/file/name.jpg`
