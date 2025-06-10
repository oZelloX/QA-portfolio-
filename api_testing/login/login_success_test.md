# API Test: Successful Login

**Method**: POST  
**Endpoint**: `https://reqres.in/api/login`  
**Description**: This test verifies that a user can successfully log in using valid credentials.

---

## Request

**Headers**:
- Content-Type: `application/json`

**Body (JSON)**:
```json
{
  "email": "eve.holt@reqres.in",
  "password": "cityslicka"
}

