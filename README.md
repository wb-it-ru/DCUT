# HTTP-services Personal аccount

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

---


## Approval of repairs
### Описание
Предназначен для согласования/отмены согласования заказ-наряда в 1С по переданному GUID
Метод - PUT

### Описание шаблона
**_URL_**: 
```html
https://<domen>.ru/<base>/hs/PersAcc/repairs/approval/{guid}
```
где guid уникальный идентификатор заказ-наряда (строка 36 знаков)


**Ответ в формате _JSON_**: 
```json
{
    "response": {
        "TransactionID": "0d2fd304-07ef-4f32-9a76-2b7d820e2c64",
        "SourceID": "0d2fd304-07ef-4f32-9a76-2b7d820e2c64",
        "OrderStatus": "Ожидает оплаты",
        "NewOrderGUIDDocument": ""
    },
    "error": null,
    "errorCode": null
}
```
