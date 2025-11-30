# My Remnawave

## Страницы подписки

- [Моя]()
- [Orion](https://github.com/legiz-ru/Orion)

## Кастомный app-config

1. Копировать `app-config.json` в контейнер
```shell
curl -O https://raw.githubusercontent.com/mitsuha44/my-remnawave/refs/heads/main/subscription-page/app-config.json
```

2. Добавить файл в контейнер

```yaml
remnawave-subscription-page:
...
    volumes:
      - ./app-config.json:/opt/app/frontend/assets/app-config.json
...

```

3. Перезапустить контейнер

```shell
docker compose down remnawave-subscription-page && docker compose up -d remnawave-subscription-page
```
## Полезные ссылки
- [Legiz my-remnawave](https://github.com/legiz-ru/my-remnawave)
