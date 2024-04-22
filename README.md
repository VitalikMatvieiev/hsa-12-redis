# hsa-12-redis
**Used comands:** 

redis-cli FLUSHDB
redis-cli KEYS '*'
redis-benchmark -t set -r 1000000 -n 10000

**With epirations** 
only noeviction doesn't work - Error from server: OOM command not allowed when used memory > 'maxmemory'.

**No expirations for keys**

**noeviction -**Error from server: OOM command not allowed when used memory > 'maxmemory'.

**volatile-lru -** Error from server: OOM command not allowed when used memory > 'maxmemory'.

**allkeys-lru -** Error from server: OOM command not allowed when used memory > 'maxmemory'.

**volatile-lfu -** Error from server: OOM command not allowed when used memory > 'maxmemory'.

**allkeys-lfu** - works

**volatile-random** - Error from server: OOM command not allowed when used memory > 'maxmemory'.

**allkeys-random -** works

**volatile-ttl** - Error from server: OOM command not allowed when used memory > 'maxmemory'.

![image](https://github.com/VitalikMatvieiev/hsa-12-redis/assets/77060767/ec968432-5774-4ed8-aa86-389031532dd1)




