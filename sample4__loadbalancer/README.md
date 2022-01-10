# loadbalancer

## run
```
docker run --rm -d --name nginx \
-p 80:80 \
-v $(pwd)/nginx.conf:/etc/nginx/nginx.conf \
nginx 
```

## Test on postman
```
GET http://localhost
```

```
GET http://localhost/header
HEADER USER-ID 1
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