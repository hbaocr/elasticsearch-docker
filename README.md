### To Success mount the host folder to docker volume. You might need to change these folder volume to be owned by 1000:1000

```
mkdir app_volume

sudo chown 1000:1000 <directory you wish to mount>

```


### ES cluster require vm.max_map_count=262144. You might to set your host VPS before start docker-compose to launch vm

sudo sysctl -w vm.max_map_count=262144

### elasticsearch-docker

```

const {
    Client
} = require('@elastic/elasticsearch')
const client = new Client({
    node: 'http://192.168.1.57:9200',
    auth: {
        username: "elastic",// default user of es when initating with docker
        password: "password"
    }
})
```
