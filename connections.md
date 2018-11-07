## REDIS: Connection Count by Client
```sh
redis-cli -h myredisserver CLIENT LIST | sed -n 's|.*addr=\(.*\)\:.*|\1|p' | sort | uniq -c
```
