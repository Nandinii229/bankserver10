# Service Unavailable Response in Postman

When executing a request to the Banks Service while the Maps Service is down, Postman will show:

## Request
![Postman Request](https://i.imgur.com/placeholder.png)

## Response
- **Status**: 503 Service Unavailable
- **Time**: 1203 ms
- **Size**: 189 B

```json
{
  "timestamp": "2025-04-21T02:45:00.123456",
  "status": 503,
  "error": "Service Unavailable",
  "message": "Could not connect to Maps Service: Connection refused: localhost/127.0.0.1:8081",
  "path": "/banks/nearby"
}
```

## How to reproduce in Postman:
1. Stop the Maps Service (if it's running)
2. Keep the Banks Service running
3. Open Postman
4. Create a new GET request
5. Enter URL: `http://localhost:8082/banks/nearby?zipcode=60601`
6. Click "Send"
7. View the error response in the lower panel 