# Development Environment

## Commands

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

### Login mysql root

Container:

- rails
- db

```bash
mysql -h db -u root -ppassword
```