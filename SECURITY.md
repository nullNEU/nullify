# Security Policy for the official null NEU website aka 'nullify'

## Repository

**Name:** nullify

**Description:** This repository houses all code (and data) related to the official website of the Northeastern University chapter of the [null community](https://null.community).

## Tech Stack

The website is built with Hugo, a popular static site generator written in Go. All the data displayed on the website is stored in `.md` files or `.yaml` files. The website is deployed using Cloudflare pages, ensuring high security, availability in different regions, and improved performance.

## Privacy and Security Highlights

*   **User Privacy Centric**: Our website is designed with user privacy as a top priority, ensuring minimal data collection and usage.
*   **Minimalistic Design**: The site is intentionally minimalistic, making it easy for users to navigate and understand our content.
*   **No JavaScript Dependency**: We have avoided using JavaScript in our codebase, ensuring that the website remains fully functional even if all scripts are blocked on a user's browser.

## Security Measures

1.  **Data Integrity and Confidentiality:**
    *   All data files (`.md` and `.yaml`) are regularly reviewed to ensure they do not contain sensitive information.
    *   Sensitive information should never be hardcoded into the codebase or configuration files.
    *   Sensitive data, if required, should be encrypted and stored securely.

2.  **Access Control:**
    *   Only authorized members of the null NEU chapter should have write access to the repository.
    *   Access permissions are reviewed regularly to ensure they align with the current team structure.
    *   Two-factor authentication (2FA) is enforced for all accounts with write access to the repository.

3.  **Code Review and Approval:**
    *   All code changes must go through a peer review process before being merged into the main branch.
    *   Use GitHub's pull request feature to facilitate code reviews and discussions.
    *   Reviewers should have the necessary security knowledge to identify and address potential security concerns.

4.  **Issue and Bug Reporting:**
    *   If you find a bug or a security vulnerability, please raise a new issue on GitHub.
    *   For sensitive security issues, please report them via our secure communication channel: [Signal Group](https://signal.group/#CjQKIIKg1u8zMBSIY9f73mTfjfIYKDaJpKAhSAWItBwoVDswEhBlW_zswdgeQrlDMGxEpavy)
    *   Before creating a new issue, check if the bug or feature has already been reported to avoid duplicates.

5.  **Dependencies and Updates:**
    *   Regularly update Hugo and any other dependencies to their latest stable versions to ensure security patches are applied.
    *   Use tools like Dependabot to monitor and automate dependency updates.

6.  **Deployment Security:**
    *   The website is deployed using Cloudflare pages, which provides DDoS protection and enhances the security of our site.
    *   Deployment credentials and secrets are stored securely and not exposed in the codebase.
    *   Secure communication channels (HTTPS) are used for all data transmissions during deployment.

7.  **Monitoring and Logging:**
    *   Security monitoring tools are implemented to detect and respond to security incidents promptly.
    *   Logs of access and changes to the repository are maintained for auditing and investigating suspicious activities.
    *   Regular reviews of logs are conducted to identify potential security breaches or unauthorized access attempts.

## Contributing

If you wish to contribute to the project:

*   Follow the detailed guidelines provided in the contribution guidelines for setting up the project locally and contributing.
*   Ensure all contributions comply with the security measures outlined in this policy.
*   Adhere to the security best practices and guidelines specific to this project.

## Note

Please ensure that the bug/feature you are raising/requesting has not already been reported before you create a new issue!

By adhering to this security policy, we aim to maintain a secure, privacy-centric, and user-friendly website for the null NEU community.
