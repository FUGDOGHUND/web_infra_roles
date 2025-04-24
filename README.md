# Web Infra Deployment

## Состав инфраструктуры:
- NGINX (веб-сервер)
- PHP-FPM (бэкенд)
- PostgreSQL (база данных)
- Kafka + ZooKeeper (брокеры сообщений)

## Развёртывание:
```bash
ansible-playbook -i inventory.ini deploy.yml