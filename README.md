# Senior PHP Developer Agent

An AI agent profile for [AyAiAy.org](https://ayaiay.org) that embodies a senior PHP developer with 10+ years of experience.

## Repository Structure

This package follows the [AyAiAy pack structure](https://github.com/ayaiayorg/ayaiay-cli/blob/main/docs/PACKS.md):

```
ayaiay-php-developer/
├── ayaiay.yaml                          # Pack manifest with metadata
├── agents/
│   └── senior-php-developer.md          # Agent definition with YAML frontmatter
├── instructions/
│   ├── clean-code-principles.md         # Clean code instruction pack
│   ├── database-design-patterns.md      # Database design instruction pack
│   └── api-design-best-practices.md     # API design instruction pack
└── prompts/
    ├── code-review-request.md           # Code review prompt template
    ├── architecture-review.md           # Architecture review prompt template
    ├── database-schema-review.md        # Database schema review prompt template
    └── api-endpoint-design.md           # API endpoint design prompt template
```

### Agent File Format

Agent files use YAML frontmatter followed by Markdown content:

```markdown
---
name: 'Agent Name'
description: 'Agent description'
model: gpt-4
temperature: 0.7
tools:
  - tool1
  - tool2
---

# Agent markdown content...
```

## Overview

This agent is designed to assist with professional PHP development tasks, bringing expertise in:

- **Object-Oriented Programming**: SOLID principles, design patterns, clean architecture
- **PHP Frameworks**: Laravel, Symfony, Yii/Yii2 - expert-level knowledge
- **Clean Code**: Best practices, code quality, maintainability, and PSR standards
- **Database Design**: Operational database design, audit history patterns, optimization
- **API Development**: RESTful and GraphQL API design, security, and best practices
- **Enterprise Architecture**: DDD, CQRS, Event Sourcing, Hexagonal Architecture

## Installation

This package is designed to work with the [AyAiAy CLI](https://github.com/ayaiayorg/ayaiay-cli).

> ⚠️ **Note**: The AyAiAy CLI is not yet published to PyPI. Until then, you can use it directly from GitHub:
> ```bash
> pip install git+https://github.com/ayaiayorg/ayaiay-cli.git
> ```

**Once the CLI is available:**

```bash
# Install the CLI
pip install ayaiay

# Install this agent pack
ayaiay install philippfrenzel/ayaiay-php-developer

# Or add to your project's ayaiay.json
ayaiay add philippfrenzel/ayaiay-php-developer
```

## Features

### Agent Profile

The **senior-php-developer** agent includes:

- Comprehensive system prompt with 10+ years of experience knowledge
- Expert-level guidance on PHP frameworks (Laravel, Symfony, Yii)
- Database design expertise including audit history patterns
- API design best practices (REST and GraphQL)
- Security-first approach following OWASP guidelines
- Performance optimization strategies

### Instruction Packs

1. **clean-code-principles**: PHP-specific clean code practices and conventions
2. **database-design-patterns**: Database design patterns including audit history implementations
3. **api-design-best-practices**: Comprehensive REST and GraphQL API design guidelines

### Prompt Templates

1. **code-review-request**: Template for requesting detailed code reviews
2. **architecture-review**: Template for reviewing system architecture
3. **database-schema-review**: Template for evaluating database schemas
4. **api-endpoint-design**: Template for designing API endpoints

## Tags

- php
- senior-developer
- laravel
- symfony
- yii
- clean-code
- object-oriented
- database-design
- api-design
- audit-history
- architecture
- best-practices
- design-patterns
- solid-principles
- rest-api
- graphql

## Usage Examples

### Code Review

```
Use the code-review-request template to get expert feedback on PHP code:
- Focus on SOLID principles
- Security vulnerabilities
- Performance optimization
- Framework best practices
```

### Architecture Design

```
Use the architecture-review template for system design review:
- Scalability considerations
- Database design patterns
- API integration strategies
- Security architecture
```

### Database Schema Design

```
Use the database-schema-review template for:
- Audit history implementation
- Query optimization
- Indexing strategies
- Data integrity patterns
```

## Requirements

- Compatible with AyAiAy CLI version 1.0+
- Designed for GPT-4 or similar language models

## License

MIT License - see [LICENSE](LICENSE) file for details

## Author

Philipp Frenzel

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## Links

- [AyAiAy.org Marketplace](https://ayaiay.org)
- [AyAiAy CLI](https://github.com/ayaiayorg/ayaiay-cli)
- [Repository](https://github.com/philippfrenzel/ayaiay-php-developer)
