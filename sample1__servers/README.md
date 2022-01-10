# servers

## run
```
docker run --rm -d --name nginx \
-p 80:80 -p8080:8080 \
-v $(pwd)/nginx.conf:/etc/nginx/nginx.conf \
-v $(pwd)/conf.d:/etc/nginx/conf.d \
nginx 
```

## Test on browser
```
http://127.0.0.1
http://127.0.0.1:8080
http://localhost
http://localhost:8080
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
