# Security Guidelines

1. **Rate Limiting**: Configure rate limiting by default on all endpoints.
2. **OWASP Top 10**: Ensure code adheres to OWASP guidelines (prevent SQLi, XSS, CSRF).
3. **Bot Mitigation**: Configure Cloudflare Turnstile on sensitive components (login, checkout, etc).
4. **Observability**: Configure Sentry in production with feedback options and recommended metrics.
5. **Webhooks**: 
   - Never name a callback simply "callback" as it is guessable.
   - Use a secret token in the URL or header.
   - Configure IP whitelisting in CIDR notation if supported by the provider.
6. **Secrets**: Never hardcode security keys. Always use `.env`.
7. **Input Validation & Sanitization**: Never trust client data. Validate all incoming data against strict schemas on the backend, and sanitize inputs to prevent injection attacks.
8. **Data at Rest**: Ensure all sensitive data (PII, financial information, tokens) is encrypted at rest using industry-standard algorithms (e.g., AES-256) at the database or storage volume level.
