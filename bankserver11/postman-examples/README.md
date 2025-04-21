# Postman Response Examples

This directory contains visual examples of how responses will appear in Postman when testing the Bank Finder API.

## Available Examples

1. [Successful Response](./successful-response.md) - Response when using a valid zipcode
2. [Invalid Zipcode Response](./invalid-zipcode-response.md) - Error response when using an invalid zipcode format
3. [Missing Parameter Response](./missing-parameter-response.md) - Error response when the zipcode parameter is missing
4. [Service Unavailable Response](./service-unavailable-response.md) - Error response when the Maps Service is down

## How to Import Collection to Postman

1. Open Postman
2. Click on "Import" in the upper left corner
3. Select the file `BankFinder.postman_collection.json` from the project root
4. Click "Import"
5. You should now see a "Bank Finder" collection in your Postman workspace
6. The collection contains ready-to-use requests for both services

## Testing All Response Types

To test all the different response types:

1. **Successful Response**: 
   - Make sure both services are running
   - Send a request with a valid zipcode (e.g., 98390)

2. **Invalid Zipcode Response**:
   - Make sure both services are running
   - Send a request with an invalid zipcode (e.g., "invalid")

3. **Missing Parameter Response**:
   - Make sure both services are running
   - Send a request without the zipcode parameter

4. **Service Unavailable Response**:
   - Stop the Maps Service (keep Banks Service running)
   - Send a request to the Banks Service with any zipcode 