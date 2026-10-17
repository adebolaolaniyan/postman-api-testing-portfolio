# Phase 2 — API Testing Portfolio

## Project Overview

This project demonstrates practical API testing using Postman. It covers HTTP methods, request parameters, response validation, negative testing, and token-based authentication.

The goal is to validate API behavior, verify response structures, and test how endpoints respond to valid and invalid requests.

## Tools and APIs

- **Postman** — API requests, test scripts, and assertions
- **HTTPBin** — HTTP responses, query parameters, headers, and request behavior
- **JSONPlaceholder** — Simulated CRUD operations
- **DummyJSON** — Login authentication and protected endpoints
- **ReqRes** — Login validation and negative test scenarios

## Test Coverage

### 1. Core API Testing

- GET requests and response validation
- Query parameters: valid, empty, and missing values
- Response headers and content type
- Response-time checks
- JSON data types and nested response objects
- Request method validation
- Custom request headers

### 2. HTTP Methods and CRUD

- POST — Create-style request
- PUT — Update-style request
- PATCH — Partial-update-style request
- DELETE — Delete-style request

**Note:** JSONPlaceholder simulates write operations. Successful responses do not necessarily mean data was permanently created, updated, or deleted.

### 3. Negative Testing

- HTTP 400 Bad Request response
- HTTP 404 Not Found response
- Malformed JSON request behavior
- Missing login fields
- Invalid login input and email-format scenarios

Negative tests help examine how APIs respond to invalid input and error conditions. The malformed JSON test records HTTPBin's observed response; it does not establish that every API rejects malformed JSON.

### 4. Authentication Testing

- Successful login and token retrieval
- Access to a protected endpoint using a bearer token
- Access to a protected endpoint without a token
- Verification of the expected HTTP 401 response for an unauthenticated request

## Test Validation

Postman test scripts use assertions to check conditions such as:

- HTTP status codes
- JSON response validity
- Required response fields
- Expected values and data types
- Response headers
- Response-time limits
- Authentication error messages

## Project Structure

The Postman collection contains the core API tests, negative test scenarios, and authentication tests.

- `TC01–TC14` — Core API testing and HTTP methods
- `NT01–NT05` — Negative testing
- `AT01–AT03` — Authentication testing

## What This Project Demonstrates

- API request execution and validation
- Writing Postman test scripts
- Positive and negative test design
- HTTP status-code verification
- JSON response validation
- Authentication and authorization testing
- Identifying limitations in simulated API behavior

## Important Notes

This portfolio uses public demonstration APIs. Results may depend on the availability and behavior of those services. Demo credentials and tokens should not be treated as production secrets or used against real accounts.


