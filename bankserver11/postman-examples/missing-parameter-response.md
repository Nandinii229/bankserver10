# Missing Parameter Response in Postman

When executing a request without the required zipcode parameter (e.g., `http://localhost:8081/maps/banksIn10Miles`), Postman will show:

## Request
![Postman Request](https://i.imgur.com/placeholder.png)

## Response
- **Status**: 400 Bad Request
- **Time**: 87 ms
- **Size**: 167 B

```json
{
  "timestamp": "2025-04-21T02:41:09.441083",
  "status": 400,
  "error": "Missing Parameter",
  "message": "Required parameter 'zipcode' is missing",
  "path": "/maps/banksIn10Miles"
}
```

## How to execute in Postman:
1. Open Postman
2. Create a new GET request
3. Enter URL: `http://localhost:8081/maps/banksIn10Miles` (without any parameters)
4. Click "Send"
5. View the error response in the lower panel 