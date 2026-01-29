---
name: 'api-design-best-practices'
description: 'Best practices for designing RESTful and GraphQL APIs'
---

# API Design Best Practices

## RESTful API Design

### Resource Naming
- Use nouns, not verbs (e.g., /users, not /getUsers)
- Use plural names for collections (e.g., /users)
- Use hierarchical structure (e.g., /users/{id}/orders)
- Keep URLs lowercase and use hyphens for readability

### HTTP Methods
- GET: Retrieve resources (idempotent, cacheable)
- POST: Create new resources
- PUT: Update entire resource (idempotent)
- PATCH: Partial update
- DELETE: Remove resource (idempotent)

### Status Codes
- 200 OK: Success
- 201 Created: Resource created
- 204 No Content: Success with no body
- 400 Bad Request: Validation error
- 401 Unauthorized: Authentication required
- 403 Forbidden: Insufficient permissions
- 404 Not Found: Resource doesn't exist
- 422 Unprocessable Entity: Semantic errors
- 429 Too Many Requests: Rate limit exceeded
- 500 Internal Server Error: Server error

### Response Format
- Consistent JSON structure
- Include metadata (pagination, timestamps)
- Use snake_case or camelCase consistently
- Provide meaningful error messages
- Include error codes for client handling

### Versioning
- URI versioning: /api/v1/users
- Header versioning: Accept: application/vnd.api.v1+json
- Query parameter: /users?version=1
- Choose one strategy and be consistent

### Pagination
- Cursor-based for real-time data
- Offset-based for static datasets
- Include total count and next/previous links

### Filtering & Sorting
- Use query parameters: ?status=active&sort=-created_at
- Support multiple filters
- Document filter capabilities

### Security
- Always use HTTPS
- Implement authentication (OAuth2, JWT)
- Rate limiting and throttling
- Input validation and sanitization
- CORS configuration
- API key rotation

## GraphQL API Design

### Schema Design
- Strong typing with GraphQL schema
- Clear field descriptions
- Proper nullability definitions
- Use interfaces for polymorphic types

### Query Optimization
- Implement DataLoader to prevent N+1 queries
- Query complexity analysis
- Depth limiting
- Pagination with connections (cursor-based)

### Error Handling
- Use GraphQL errors with extensions
- Provide meaningful error codes
- Distinguish between client and server errors

## General API Principles
- Document with OpenAPI/Swagger
- Provide SDKs and code examples
- Version APIs appropriately
- Monitor and log API usage
- Implement health check endpoints
- Use API gateways for complex systems
- Consider backward compatibility
- Test thoroughly (unit, integration, contract)
