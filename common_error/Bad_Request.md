## Failure Response

**Condition** : 올바른 요청이 아닐때 - 해당 필드값이 없거나, 지원되지 않는 형식일 때

**Code** : `400 Bad Request`

**Content**

```json
{
    "errMsg" : [
      "<FieldName> is required\n",
      "<FieldName>/<Type> is not supported / Recommended : <Type>\n",
    ]
}
```
