# Android App Security Analysis with MobileAudit

## Project Overview

This project conducts a comprehensive security analysis of popular Android applications using MobileAudit, an open-source static analysis tool. The study aims to identify and assess potential security vulnerabilities in mobile apps, highlighting the need for improved security practices in mobile app development.

## Key Findings

The analysis revealed several concerning security issues across multiple popular Android apps:

- Widespread use of raw SQL queries, potentially leading to SQL injection vulnerabilities
- Hardcoding of sensitive information like API keys and credentials
- Unrestricted reading of clipboard data
- Collection of sensitive device information without clear justification
- Use of insecure functions that could allow arbitrary code execution
- Utilization of potentially unsafe libraries for network communication

## Methodology

1. **Tool Used**: MobileAudit (v3.0.0)
2. **Sample Size**: 11 popular Android applications from various categories
3. **Analysis Approach**: Static code analysis focusing on:
   - SQL query practices
   - Hardcoded sensitive data
   - Device information gathering
   - Use of insecure functions
   - Clipboard access
   - Network communication practices

## Key Recommendations

For Developers:
- Use parameterized queries or ORM frameworks to prevent SQL injection
- Implement secure storage for sensitive data and API keys
- Minimize collection of device-specific information
- Avoid using potentially dangerous functions like `system()`, `exec()`, etc.
- Implement proper input validation and sanitization
- Use secure communication protocols (HTTPS) consistently

For Users:
- Be cautious when granting permissions to apps
- Keep apps and OS updated
- Use apps from trusted sources only

For App Marketplaces:
- Implement stricter security vetting processes
- Provide clear security guidelines for developers
- Offer resources for security best practices

## Project Structure

- `Project Final Stage.pdf`: Comprehensive report of the final analysis
- `Project Proposal - MobileAudit.pdf`: Initial project proposal
- `Project Stage A - Kush Borikar.pdf`: First stage of the project
- `Project Stage B - Kush Borikar.pdf`: Second stage of the project

## Tool Setup and Replication Steps

Detailed instructions for setting up and using MobileAudit are provided in the project documents. Key steps include:

1. Install Docker and Docker Compose
2. Clone the MobileAudit repository
3. Build and run the Docker container
4. Access the MobileAudit dashboard at `http://localhost:8888`
5. Upload APK files for analysis

For full replication steps, refer to the "Replication Steps" section in the project documents.

## Conclusion

This project highlights significant security vulnerabilities in popular Android applications. The findings underscore the need for increased awareness and implementation of security best practices in mobile app development. By addressing these issues, developers can create a more secure and trustworthy mobile app ecosystem.

## Author

Kush Borikar (kb97)

## Acknowledgements

This project was completed as part of the CS678 - Topics in Smartphone Security & Reliability course.
