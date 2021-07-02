## 占位符

### go-micro

非传统占位符，而是根据下划线，展开成对应的 json 格式

```env
DATABASE_ADDRESS=127.0.0.1
DATABASE_PORT=3306
```

```json
{
    "database": {
        "address": "127.0.0.1",
        "port": 3306
    }
}
```
