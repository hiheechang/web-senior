# Performance3 :: BackEnd

Backend : CDNs, Caching, LoadBalancing, DB Scaling, GZIP

## CDN 

caching files to nearby CDN server ex) CloudFlare, AWS(cloudFront), Azure(CDN)

## GZIP 

- compressing file ex)using compression in gzip
- alternative :: Brotli

```javascript
const compression = require('compression')
const express = require('express')
const app = express()

app.use(compression())
```

## Database Scaling

- identify inefficient Query
- Increase Memory
- vertical Scaling (Redis, Memcached)
- Sharding : breaking down into pieces
- More DBs
- Database Type

## Caching

- CDN : cache html,css,javascript
- server : store in redis, database .... instead of slow APIs
- browser : cache in client side <--by ServiceWorker

## Load Balancing

- handle multiple requests
- for static files : NGINX, ApacheServer

npm install -g loadtest

loadtest -t 5 -c 100 --rps 100 http://localhost:80
-time -numOfClient --requestPerSecond

