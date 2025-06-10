# Successful Login – API Test

**Test Case ID**: API-LOGIN-001  
**Module**: Login  
**Reported by**: oZelloX  
**Date**: 2025-06-10  
**Environment**: https://reqres.in/api/login, Postman  

---

## Use Case  
Проверка, что пользователь может успешно войти в систему с валидными учетными данными через API.

---

## Request

**Method**: `POST`  
**URL**: `https://reqres.in/api/login`  
**Headers**: `Content-Type: application/json`  
**Body** (JSON):
```json
{
  "email": "eve.holt@reqres.in",
  "password": "cityslicka"
}
Expected Result

Ответ от API:

Status Code: 200 OK
Response Body:
{
  "token": "QpwL5tke4Pnpja7X4"
}
Actual Result

Успешный ответ с токеном получен.
Status: 200 OK
Response:

{
  "token": "QpwL5tke4Pnpja7X4"
}
Notes

Токен — это строка, которая выдается сервером после успешной авторизации.
Он используется для дальнейших запросов от имени пользователя без повторного ввода логина и пароля.
Обычно токен передаётся в заголовке Authorization: Bearer <token> при следующих API-запросах.

Сохраняешь это в `api_testing/login_success_test.md`.  
Если надо — сделаю аналогично ещё.
