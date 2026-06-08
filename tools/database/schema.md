# Database Guidelines

1. **Migrations**: All schema changes must be managed via migrations.
2. **Indexing**: Always index foreign keys and columns frequently used in WHERE clauses.
3. **Security**: Validate data before insertion; enforce relationships.
