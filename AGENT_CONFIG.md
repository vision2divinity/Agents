# Banking AQA Specialist Agent - Complete Configuration

## Agent Metadata
- **Agent Name:** Banking AQA Specialist (or your exact name)
- **Agent Type:** Agent (with tools)
- **Created:** [Date]
- **Last Modified:** [Date]
- **Version:** 1.0.0

---

## Model Configuration

### Provider: Groq
- **Model:** gpt-oss-120b
- **Temperature:** 0.7
- **Max Tokens:** 4096
- **Top P:** 1.0

---

## Instructions / System Prompt
```
[PASTE YOUR ENTIRE SYSTEM PROMPT HERE - the one I just provided about banking domain]
```

---

## Opening Statement
```
Welcome! I'm your Banking QA Expert Assistant. I specialize in comprehensive testing for financial services and can help you with:

🏦 Core Banking Operations Testing
💳 Card Services & ATM Testing  
📱 Digital/Mobile Banking Testing
💰 Payment Systems & Transfers
🔒 Security & Fraud Prevention Testing
📊 Investment & Wealth Management Testing
⚖️ Regulatory Compliance Testing
🔌 API & Integration Testing
⚡ Performance & Load Testing

What banking module or feature would you like to test today?
```

---

## Variables

### 1. banking_module
- **Type:** Select
- **Options:** 
  - Core Banking
  - Digital Banking
  - Card Services
  - Payments & Transfers
  - Loans & Credit
  - Investments
  - Security & Fraud
  - Compliance & Regulatory
- **Default:** Core Banking
- **Description:** Select the banking domain you want to test

### 2. test_framework
- **Type:** Select
- **Options:**
  - Selenium
  - Appium
  - REST Assured
  - JMeter
  - Postman
  - Cypress
  - Playwright
- **Default:** Selenium
- **Description:** Preferred test automation framework

### 3. programming_language
- **Type:** Select
- **Options:**
  - Java
  - Python
  - JavaScript
  - C#
- **Default:** Java
- **Description:** Programming language for test scripts

### 4. test_type
- **Type:** Select
- **Options:**
  - Functional Testing
  - API Testing
  - Security Testing
  - Performance Testing
  - Integration Testing
  - Compliance Testing
- **Default:** Functional Testing
- **Description:** Type of testing to perform

### 5. environment
- **Type:** Select
- **Options:**
  - Development
  - QA
  - UAT
  - Pre-Production
  - Production
- **Default:** QA
- **Description:** Target test environment

---

## Tools Enabled

### 1. Code Interpreter
- **Status:** Enabled
- **Purpose:** Execute Python code for calculations, data analysis, test data generation

### 2. Web Scraper
- **Status:** Enabled
- **Purpose:** Extract information from banking documentation or web sources

### 3. HTTP Request (if added)
- **Status:** Enabled/Disabled
- **Purpose:** Make API calls for testing or data retrieval

---

## Knowledge Base

### Documents Uploaded:
- [List any documents you've uploaded]
- Banking API documentation
- Testing standards
- Compliance guidelines
- etc.

### Future Additions:
- ISO 20022 standards
- PCI-DSS documentation
- OWASP banking security guidelines
- Core banking system documentation

---

## Features Configuration

### Response Mode
- **Type:** Streaming (real-time response)

### Conversation History
- **Enabled:** Yes
- **Max Messages:** [Check your setting]

### File Upload
- **Enabled:** Yes/No
- **Allowed Types:** [If enabled]

---

## API Configuration (if using)

### Endpoint
- Check "Access API Reference" in Publish menu for your specific endpoint

### Authentication
- API Key required
- [Document your API key location - don't include actual key]

---

## Usage Examples

### Example 1: Generate Selenium Test
**Input:**
```
Generate a Selenium test script in Java for testing fund transfer between accounts.
Variables: banking_module=Core Banking, test_framework=Selenium, programming_language=Java
```

**Expected Output:**
- Complete Java class with Page Object Model
- TestNG annotations
- Proper assertions
- Error handling

### Example 2: Create API Test Cases
**Input:**
```
Create test cases for payment API endpoint including security scenarios.
Variables: banking_module=Payments & Transfers, test_type=API Testing
```

**Expected Output:**
- Comprehensive test case table
- Security-focused scenarios
- Compliance checks

---

## Deployment Information

### Hosting
- **Platform:** Docker (local)
- **URL:** http://localhost:8081
- **Port:** 8081

### Dependencies
- Docker containers: nginx, api, web, db, redis, etc.
- Groq API key configured

---

## Maintenance & Updates

### Version History
- v1.0.0 (Initial release) - [Date]
  - Banking domain specialization
  - Comprehensive testing coverage
  - Multiple framework support

### Planned Enhancements
- [ ] Add more banking modules
- [ ] Integration with test management tools
- [ ] Custom tool for WooCommerce integration
- [ ] Jenkins CI/CD integration
- [ ] Test execution capabilities

---

## Testing & Validation

### Test Scenarios Validated
- [ ] Core banking test generation
- [ ] Card services testing
- [ ] API test script generation
- [ ] Security test cases
- [ ] Performance test plans

### Known Limitations
- [Document any limitations you discover]

---

## Support & Documentation

### Related Resources
- Main repository: https://github.com/[your-username]/dify-aqa-agents
- Dify documentation: https://docs.dify.ai
- Banking testing standards: [Links]

---

## Notes
[Add any additional notes, observations, or important information]