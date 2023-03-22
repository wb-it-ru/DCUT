# DCUT

# DCUT HTTP-services
---
## Ping
### Описание
Предназначен для проверки доступности сервиса
Метод - GET

### Описание шаблона
**_URL_**: 
```html
https://<domen>.ru/<base>/hs/PersAcc/ping/
```

**Ответ в формате _JSON_**: 
```json
{
    "response": {
        "result": "ok",
        "ver": "1.1.1.1",
    }
}
```
