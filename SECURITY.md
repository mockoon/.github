# Security Policy

This document outlines the security practices and incident response procedures followed by the Mockoon team to ensure the safety and integrity of our open-source applications. This policy does not cover our cloud services, which have their own dedicated security measures and protocols.

---

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

To report a vulnerability in Mockoon's desktop application or packages (CLI, serverless, etc.) please send an email to security@mockoon.com.
You should receive a response from us within 48 hours.

Please include the requested information listed below to help us better understand the nature and scope of the possible issue:

- The application and/or library version where the issue was identified.
- Any special configuration required to reproduce the issue.
- Step-by-step instructions to reproduce the issue.
- Impact of the issue, including how an attacker might exploit the issue.
- Your recommended remediation if any.

---

## Open Source Security Incident Response Process

This document outlines the process the Mockoon team follows when handling security vulnerabilities reported in our open-source applications and libraries (CLI, etc.). Our goal is to be transparent with our community about how we triage, fix, and disclose security issues.

This process applies only to the open-source tools maintained by the Mockoon team not the Cloud services.

---

### Phase 1: Triage & Validation

This initial phase begins when we receive a security vulnerability report. The primary goal is to understand, reproduce, and assess the potential impact of the reported issue.

**Process Overview:**

When a report is received, a designated security lead from the core team will:

1. **Acknowledge the Report**: Privately acknowledge receipt of the report to the person who submitted it.
2. **Validate the Vulnerability**: Thoroughly review the report and work to reproduce the vulnerability. This helps us understand the conditions required for an exploit.
3. **Assess Impact**: Determine the potential impact on the confidentiality, integrity, and availability (CIA) of a user's environment. We analyze what data could be at risk and what an attacker might be able to achieve.
4. **Determine Severity**: Assign an initial severity level (e.g., Critical, High, Medium, Low) based on the impact and exploitability.
5. **Decision**:

- If the report is not a vulnerability or is otherwise invalid, we will inform the reporter with our reasoning.
- If the vulnerability is validated, we will proceed to the Mitigation & Remediation phase.

---

### Phase 2: Mitigation & Remediation

Once a vulnerability is confirmed, our focus shifts to fixing the issue and preventing potential exploitation.

**Process Overview:**

Our remediation efforts include the following steps:

1. **Develop a Fix**: The team will identify the root cause and develop a code patch to resolve the vulnerability.
2. **Code Review**: The proposed fix will be submitted as a pull request and undergo a thorough review by core team members to ensure it is effective and does not introduce new issues.
3. **Testing**: The patch is tested to confirm that it successfully resolves the vulnerability.
4. **Merge and Release**: Once approved, the fix is merged into the main codebase and scheduled for inclusion in the next official release of the application.

---

### Phase 3: Scoping & Impact Analysis

During this phase, we analyze the codebase to understand the full scope of the vulnerability.

**Process Overview:**

The team will perform an analysis to determine:

1. **Affected Versions**: Identify all previous versions of the Mockoon open-source application that contain the vulnerability.
2. **Introduction Point**: Pinpoint when the vulnerability was first introduced into the codebase.
3. **User Impact**: Define the potential impact on users running affected versions. This includes clarifying what an attacker could do and what conditions must be met to exploit the vulnerability.

---

### Phase 4: Notification & Disclosure

Transparency with our users is critical. This phase is about communicating the vulnerability and its solution to the community in a clear and timely manner.

**Process Overview:**

Following the release of a patched version, we will execute our public disclosure process.

1. **Publish Security Advisory**: We will publish a detailed security advisory on GitHub. This advisory will serve as the single source of truth and will contain:

   - A description of the vulnerability and its potential impact.
   - A list of all affected application versions.
   - The version number that contains the fix.
   - Instructions and recommendations for users to upgrade.
   - Credit to the security researcher who discovered and reported the issue (with their permission).

2. **Community Communication**: We will announce the security patch through our public channels, including the application's release notes and our blog, directing users to the official GitHub Security Advisory for details.
