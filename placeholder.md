## 占位符

### beego

https://github.com/beego/beego

```ini
token = ${TOKEN}
token = ${TOKEN||default-value}
```

### revel (go)

https://github.com/revel/revel

```ini
# key
app.name = myapp
log.warn.output = %(app.name)s.log

# env
db.driver = ${CHAT_DB_DRIVER}
db.spec = ${CHAT_DB_SPEC}
```


### go-micro

https://github.com/asim/go-micro

非传统占位符，而是根据下划线，展开成对应的 json 格式，再 Merge 的过程中如何和其他源冲突则按照源的顺序覆盖

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
