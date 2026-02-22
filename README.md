# JSONPlaceholder API – CRUD Testing Project

##  Project Overview
This project demonstrates functional and API testing of CRUD operations using JSONPlaceholder public API.

Tool used:
- Postman
- Manual Test Case Design
- Basic automated validations using Postman Scripts

---

##  Scope

The following endpoints were tested:

- GET /posts/1
- POST /posts
- PUT /posts/1
- DELETE /posts/1
- Negative scenario validation

---

##  Test Coverage

### 1 GET – Read Operation
Validated:
- Status code 200
- ID value consistency
- Required fields presence (title, body, userId)
- Response time < 500ms

### 2 POST – Create Operation
Validated:
- Status code 201
- Resource creation confirmation
- Title consistency
- ID auto-generation

### 3 PUT – Update Operation
Validated:
- Status code 200
- Updated title and body
- ID integrity remains unchanged

### 4 DELETE – Delete Operation
Validated:
- Status code 200
- Empty response body

Post-deletion validation:
- Executed GET request to verify persistence behavior
- Observed that JSONPlaceholder is a mock API and does not persist changes
- In a real environment, expected result would be 404 Not Found

---

##  Observations

JSONPlaceholder is a mock API.
CRUD operations simulate responses but do not persist data.
Post-deletion GET returned 200, confirming non-persistent behavior.

---

##  Skills Demonstrated

- REST API Testing
- CRUD validation
- Positive and negative test scenarios
- Response structure validation
- Performance validation (response time)
- Understanding of mock vs real APIs
- Basic test automation using Postman scripts
