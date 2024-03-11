# Why E-Commerce Security?
- Customer PII & Financial Information
- Financial Loss
- Regulatory compliance requirements
- Brand Protection

# Common E-Commerce Security Threats
- Data Leaks
- Skimming
- Financial Frauds
- Bots
- DoS & DDoS Attacks
- Brute Force Attacks
- Known Vulnerabilities -> SQLi, XSS, CSRF, SSRF, IDOR, etc

# Basic Terminology
## CIA+ Triad
- Confidentiality
- Integrity
- Availability
- Authenticity
- Accountability
- Non-repudiation

> Risk = Impact  x Likelihood

## Common Web Security Vulnerabilities

- Authentication means who are you
- Authorization means what can you access

1. **Insecure Direct Object Reference (IDOR):** Authentication but no Authorization where the attacker who is authenticated can access information for the unauthorized user. (Implement Principle of Least Privilege (PoLP) to avoid this)
2. **Server-Side Request Forgery (SSRF):** Changing the payload of a legitimate HTTP request
3. **SQL Injection:** (SQLi) Sending SQL Query as input to manipulate the functioning of server/database.
	1. First-order SQL Injection
	2. Second-order SQL Injection