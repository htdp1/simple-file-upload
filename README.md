# simple-file-upload

Docker container that provides an API endpoint for simple, randomize file name.

# How to Use

Basic usage is as follows:

```Dockerfile
docker run \
  -v /my_local_dir/:/uploads/ \
  -p 3000:3000 \
  htdp1/simple-file-upload
```

Call API:

```sh
 curl -XPOST -F 'data=@test.txt' "http://hostname:3000/upload"
```
