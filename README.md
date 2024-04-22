# hsa-12-redis
**Used comands:** 

redis-cli FLUSHDB
redis-cli KEYS '*'
redis-benchmark -t set -r 1000000 -n 10000

**No expirations for keys**

**noeviction -**Error from server: OOM command not allowed when used memory > 'maxmemory'.

**volatile-lru -** Error from server: OOM command not allowed when used memory > 'maxmemory'.

**allkeys-lru -** Error from server: OOM command not allowed when used memory > 'maxmemory'.

**volatile-lfu -** Error from server: OOM command not allowed when used memory > 'maxmemory'.

**allkeys-lfu** - works

**volatile-random** - Error from server: OOM command not allowed when used memory > 'maxmemory'.

**allkeys-random -** works

**volatile-ttl** - Error from server: OOM command not allowed when used memory > 'maxmemory'.

![Uploading image.png…]()

