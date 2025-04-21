# Invalid Zipcode Response in Postman

When executing a request with an invalid zipcode (e.g., `http://localhost:8081/maps/banksIn10Miles?zipcode=invalid`), Postman will show:

## Request
![Postman Request](https://i.imgur.com/placeholder.png)

## Response
- **Status**: 400 Bad Request
- **Time**: 98 ms
- **Size**: 189 B

```json
{
  "timestamp": "2025-04-21T02:40:21.780363",
  "status": 400,
  "error": "Invalid Input",
  "message": "Invalid zipcode format. Expected 5 digits or 5+4 digits (e.g., 12345 or 12345-6789)",
  "path": "/maps/banksIn10Miles"
}
```

## How to execute in Postman:
1. Open Postman
2. Create a new GET request
3. Enter URL: `http://localhost:8081/maps/banksIn10Miles?zipcode=invalid`
4. Click "Send"
5. View the error response in the lower panel 