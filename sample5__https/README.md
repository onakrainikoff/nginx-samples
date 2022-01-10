# https

## run
```
docker run --rm -d --name nginx \
-p 443:443 \
-v $(pwd)/nginx.conf:/etc/nginx/nginx.conf \
-v $(pwd)/cert:/etc/nginx/cert \
nginx 
```

## Test on browser
```
https://localhost
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