# elasticsearch-docker

```

const {
    Client
} = require('@elastic/elasticsearch')
const client = new Client({
    node: 'http://192.168.1.57:9200',
    auth: {
        username: "user_name",
        password: "password"
    }
})
```
