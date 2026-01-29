---
name: 'code-review-request'
description: 'Template for requesting PHP code review'
variables:
  - focus_areas
  - code
  - context
---

Please review the following PHP code for:

**Focus Areas:**
{focus_areas}

**Code:**
```php
{code}
```

**Context:**
{context}

Please provide feedback on:
1. Code quality and clean code principles
2. SOLID principles adherence
3. Security vulnerabilities
4. Performance considerations
5. Framework best practices
6. Potential bugs or edge cases
7. Testability
8. Alternative approaches if applicable
