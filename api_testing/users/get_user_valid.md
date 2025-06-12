# Get User by ID – Valid Case

**Method**: GET  
**Endpoint**: `https://reqres.in/api/users/2`  
**Description**: Verifies that the API returns correct user data when a valid user ID is provided.

## Request
No request payload required.

## Expected Result  
- Status code: **200 OK**  
- Response body includes valid user object with fields:
  - id, name, year, color, pantone_value
  - and a support block

## Actual Result  
- Status code: **200 OK**  
- Response body:
```json
{
  "data": {
    "id": 2,
    "name": "fuchsia rose",
    "year": 2001,
    "color": "#C74375",
    "pantone_value": "17-2031"
  },
  "support": {
    "url": "https://contentcaddy.io?utm_source=reqres&utm_medium=json&utm_campaign=referral",
    "text": "Tired of writing endless social media content? Let Content Caddy generate it for you."
  }
}
```

## Notes
This confirms that the API correctly returns a user object for a valid ID.
