# locations match

## run
```
docker run --rm -d --name nginx \
-p 80:80 \
-v $(pwd)/nginx.conf:/etc/nginx/nginx.conf \
nginx 
```

## Test on browser
```
http://localhost
http://localhost/1
http://localhost/static/
http://localhost/static/text/
http://localhost/static/text/1.txt
http://localhost/metod1/doc
http://localhost/metod2/doc
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