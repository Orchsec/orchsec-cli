# Coordinated Vulnerability Disclosure Policy

## Our Commitment to Security

OrchSec Inc. is committed to ensuring the security of our customers and the broader open-source community. We believe that responsible disclosure of security vulnerabilities helps us maintain the trust and safety of all users of the OrchSec platform and its associated open-source projects.

## Reporting a Vulnerability

If you believe you have discovered a security vulnerability in any OrchSec-owned repository, open-source project, or infrastructure component, **please do not open a public issue**. Instead, report it directly to our security team by sending an email to:

**security@orchsec.com**

To help us respond effectively, please include the following details in your report:

- **Type of vulnerability** (e.g., buffer overflow, SQL injection, cross-site scripting, privilege escalation, etc.)
- **Affected component** (repository name, file path, module, or endpoint)
- **Steps to reproduce** — provide a clear, minimal, and reproducible test case
- **Proof of concept** — any PoC code or payload that demonstrates the issue
- **Impact assessment** — your estimation of the potential damage or exploitation scenario
- **Environment details** — operating system, runtime version, dependency versions, and configuration

## Disclosure Process

1. **Initial Report:** You send your findings to security@orchsec.com.
2. **Acknowledgment:** We will acknowledge receipt of your report **within 48 hours** of submission.
3. **Triage & Validation:** Our security team will validate the report and assess its severity and impact.
4. **Remediation:** We will develop and test a fix. The timeline depends on severity:
   - **Critical/High:** Patch within 7 days
   - **Medium:** Patch within 30 days
   - **Low:** Patch within 90 days
5. **Coordinated Disclosure:** Once a fix is deployed, we will coordinate a public disclosure timeline with you.

## Scope

This policy applies to all repositories and public-facing services owned or operated by OrchSec Inc., including but not limited to:

- All repositories under the `orchsec` GitHub Organization
- The OrchSec CLI (`orchsec-cli`)
- Documentation and configuration files in official OrchSec repositories
- OrchSec-hosted API endpoints and SaaS infrastructure

## Out of Scope

- Issues in third-party dependencies — please report those to the respective maintainers
- Exploitation of vulnerabilities against production systems without prior authorization
- Social engineering attacks against OrchSec employees or contractors

## Safe Harbor

OrchSec Inc. will not pursue legal action against individuals who report security vulnerabilities in accordance with this policy. We consider research and reporting conducted under this policy as:

- Authorized conduct under applicable computer fraud and abuse laws
- A exempt from any restrictions in our Terms of Service that would otherwise prohibit security testing

We will not initiate a Digital Millennium Copyright Act (DMCA) takedown request against researchers acting in good faith under this policy.

## Recognition

We believe in crediting security researchers who help us improve our security posture. With your permission, we will:

- Add your name and affiliation to our Hall of Fame
- Acknowledge your contribution in release notes or advisories related to your finding
- Offer swag or bounty consideration on a case-by-case basis

---

*OrchSec Inc. — Building a safer future for autonomous AI systems.*
