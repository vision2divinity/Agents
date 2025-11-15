# Banking AQA Specialist Agent

**Version:** 1.0.0  
**Status:** Production Ready  
**Domain:** Banking & Financial Services  
**Model:** Groq gpt-oss-120b / OpenAI GPT-4 / Anthropic Claude

---

## Overview

Specialized AI agent for comprehensive banking and financial services quality assurance testing.

## Capabilities

### Testing Domains Covered
- Core Banking Operations
- Digital/Mobile Banking
- Card Services (Debit, Credit, ATM, POS)
- Payment & Transfer Systems
- Loan & Credit Services
- Investment & Wealth Management
- Security & Fraud Prevention
- Regulatory Compliance

### Test Automation
- Selenium WebDriver (Java, Python, JavaScript)
- Appium (Mobile testing)
- REST Assured, Postman, Karate (API testing)
- JMeter, Gatling (Performance testing)
- Cucumber/BDD frameworks
- TestNG, JUnit, PyTest

## Files in This Directory

- `banking-aqa-agent.yml` - Dify DSL export (importable configuration)
- `AGENT_CONFIG.md` - Complete manual configuration guide
- `README.md` - This file

## Setup Instructions

See `AGENT_CONFIG.md` for detailed setup instructions.

## Usage Examples

### Example 1: Generate Selenium Test
```
Generate a Selenium WebDriver test in Java for ATM cash withdrawal including:
- PIN validation (3 attempts max)
- Balance check
- Daily limit verification
- Transaction receipt generation
Use Page Object Model pattern.
```

### Example 2: API Testing
```
Create REST Assured tests for fund transfer API:
POST /api/v1/transfer
Include authentication, input validation, idempotency, and error scenarios.
```

### Example 3: Performance Testing
```
Generate JMeter test plan for 1000 concurrent users performing login and balance inquiry.
Test duration: 15 minutes. Include assertions for <2 second response time.
```

## Variables

The agent uses the following variables for context:
- `banking_module` - Target banking domain
- `test_framework` - Preferred automation framework
- `programming_language` - Code language preference
- `test_type` - Type of testing (functional, security, etc.)
- `environment` - Target test environment

## Tools Enabled

- Code Interpreter (for calculations and data generation)
- Web Scraper (for documentation research)
- HTTP Request (optional, for API calls)

## Version History

- **v1.0.0** (Nov 2025) - Initial release with comprehensive banking domain coverage

## Support

For issues or questions, please open an issue in the main repository.