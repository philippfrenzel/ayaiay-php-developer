---
name: 'database-schema-review'
description: 'Template for reviewing database schema design'
variables:
  - database_type
  - schema
  - use_cases
  - load_description
---

Please review the following database schema:

**Database Type:** {database_type}

**Schema:**
```sql
{schema}
```

**Use Cases:**
{use_cases}

**Expected Load:**
{load_description}

Please evaluate:
1. Normalization and data integrity
2. Indexing strategy
3. Audit history implementation
4. Query performance considerations
5. Scalability for expected load
6. Data consistency and locking strategy
7. Suggested optimizations
