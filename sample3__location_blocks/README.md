# location blocks

## run
```
docker run --rm -d --name nginx \
-p 80:80 \
-v $(pwd)/nginx.conf:/etc/nginx/nginx.conf \
-v $(pwd)/html:/usr/share/nginx/html \
nginx 
```

## Test on browser
```
http://localhost
http://localhost/files/
http://localhost/api/v1/
http://localhost/api/v2/
http://localhost/api/v3/
```
## Test on postman

```
GET http://localhost/api/
HEADER API-VERSION 1
```

## management

### CLI
```
docker exec -it nginx bash 
```

### Test config
```
nginx -t
```

### Reload config
```
nginx -s reload
```

### Logs
```
docker logs nginx
```