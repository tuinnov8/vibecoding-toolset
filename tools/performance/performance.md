# Performance Guidelines

1. **Background Tasks**: Use background workers (e.g., Celery, BullMQ) for heavy processing.
2. **Modularity**: Break files into smaller components and modules to ensure maintainability.
3. **Pagination**: Ensure list and table data is paginated depending on the database used.
4. **Concurrency**: Use transaction pooling (like PgBouncer) for production database concurrency if applicable.
5. **Caching**: Utilize caching (Redis, CDN) depending on the deployment environment.
