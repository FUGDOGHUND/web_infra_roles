# Web Infra Deployment

## Состав инфраструктуры:
- NGINX (веб-сервер)
- PHP-FPM (бэкенд)
- PostgreSQL (база данных)
- Kafka + ZooKeeper (брокеры сообщений)

## Развёртывание:
```bash
sudo ansible-playbook -i inventory.ini deploy.yml

docker-compose down --rmi all -v
docker rm -f $(docker ps -aq) 2>/dev/null || true