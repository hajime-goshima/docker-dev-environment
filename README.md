# Development Environment

## Commands

### Run docker-compose

```bash
docker-compose build
```

```bash
docker-compose up -d
```

```bash
docker-compose start
```

```bash
docker-compose stop
```

### Enter rails shell

```bash
docker-compose exec rails /bin/bash
```

### Enter db shell

```bash
docker-compose exec db /bin/bash
```

### Enter redis shell

```bash
docker-compose exec redis /bin/bash
```

### Login mysql

Container:
- rails

```bash
mysql -h db -u root -ppassword
```

### Login redis

Container:
- rails

```bash
redis-cli -h redis
```