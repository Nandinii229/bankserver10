# Successful Response in Postman

When executing a request with a valid zipcode (e.g., `http://localhost:8082/banks/nearby?zipcode=60601`), Postman will show:

## Request
![Postman Request](https://i.imgur.com/placeholder.png)

## Response
- **Status**: 200 OK
- **Time**: 123 ms
- **Size**: 175 B

```json
[
  "Chase Bank",
  "Bank of America Financial Center",
  "Wells Fargo Bank",
  "US Bank",
  "KeyBank"
]
```

## How to execute in Postman:
1. Open Postman
2. Create a new GET request
3. Enter URL: `http://localhost:8082/banks/nearby?zipcode=60601`
4. Click "Send"
5. View the response in the lower panel 