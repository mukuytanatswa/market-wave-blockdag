# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |

## Reporting a Vulnerability

If you discover a security vulnerability, please report it responsibly:

1. **DO NOT** create a public GitHub issue
2. Email us at: [your-email@example.com]
3. Include:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if any)

## Security Best Practices

### API Keys
- Never commit API keys to version control
- Use environment variables for all sensitive data
- Rotate API keys regularly
- Use different keys for development and production

### Environment Variables
- Store sensitive data in `.env` files (not committed)
- Use GitHub Secrets for deployment
- Never log API keys or sensitive data

### Dependencies
- Keep dependencies updated
- Use `npm audit` to check for vulnerabilities
- Review dependency changes before updating

## Data Privacy

This application:
- Does not store personal data
- Does not collect user information
- Only fetches public market data
- All API calls are made client-side

## API Rate Limits

Be aware of API rate limits:
- **CoinGecko**: 10-50 calls/minute (free tier)
- **Alpha Vantage**: 5 calls/minute (free tier)
- **Metals API**: 100 calls/month (free tier)

## Reporting Security Issues

We take security seriously. If you find a vulnerability:

1. **Immediate**: Don't exploit it
2. **Report**: Contact us privately
3. **Wait**: Give us time to fix it
4. **Disclose**: We'll coordinate public disclosure

Thank you for helping keep this project secure!
