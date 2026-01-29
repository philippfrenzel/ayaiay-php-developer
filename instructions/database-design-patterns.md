---
name: 'database-design-patterns'
description: 'Database design patterns and audit history implementation'
---

# Database Design Patterns

## Audit History Patterns

### Temporal Table Pattern
- Maintain historical versions of records
- Include valid_from and valid_to timestamps
- Use triggers or application logic for versioning

### Audit Log Table
- Separate table for tracking all changes
- Include: user_id, table_name, record_id, action, old_values, new_values, timestamp
- Index on table_name, record_id, and timestamp for efficient queries

### Event Sourcing
- Store all changes as immutable events
- Rebuild current state by replaying events
- Useful for complex audit requirements and temporal queries

### Shadow Table Pattern
- Mirror table structure with _history suffix
- Copy records to history table on update/delete
- Include operation type and timestamp

## Common Database Patterns

### Repository Pattern
- Abstract data access layer
- Centralize data access logic
- Enable easy testing with mock repositories

### Unit of Work
- Track changes during business transaction
- Commit all changes together
- Maintain consistency across multiple operations

### Data Mapper
- Separate domain objects from database
- Map between domain and persistence layers
- Allow domain model evolution independently

### Query Object
- Encapsulate complex queries
- Reusable query logic
- Type-safe query building

## Optimization Strategies
- Proper indexing (B-tree, Hash, Full-text)
- Denormalization for read-heavy workloads
- Partitioning for large tables
- Caching strategies (query cache, result cache)
- Connection pooling
- Read replicas for scaling reads
