## 占位符

## go

### revel

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

https://github.com/asim/go-micro/tree/master/config/source/env

非传统占位符，而是根据下划线，展开成对应的 json 格式，再 Merge 的过程中如何和其他源冲突则按照源的顺序覆盖

```env
DATABASE_ADDRESS=127.0.0.1
DATABASE_PORT=3306
```

对应 JSON

```json
{
    "database": {
        "address": "127.0.0.1",
        "port": 3306
    }
}
```

### beego

https://github.com/beego/beego

```ini
token = ${TOKEN}
token = ${TOKEN||default-value}
```

## php

### symfony

https://github.com/symfony/symfony

```yaml
key: %kernel.project_dir%
env: %env(ENV_VAR_NAME)%
```

## Java

### Spring

https://github.com/spring-projects/spring-framework

```
FOO=${FOO}
```
