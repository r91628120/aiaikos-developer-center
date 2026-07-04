# API Design Standard

## 原則

- API 回傳 JSON。
- 所有回傳需包含 success。
- 錯誤需包含 error message。

## 建議格式

```json
{
  "success": true,
  "result": {},
  "meta": {
    "version": "1.0",
    "updatedAt": "YYYY-MM-DD"
  }
}
```
