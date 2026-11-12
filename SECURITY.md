# Security reporting

[English](SECURITY.md) | [Português](SECURITY.pt.md) | [Español](SECURITY.es.md)

Use the target repository's security instructions when present. Ordinary functional bugs belong in its **Bug report** issue form. Suspected vulnerabilities must not be disclosed in public issues, discussions or pull requests.

The relevant CODEOWNERS are responsible for monitoring, triaging and coordinating the resolution of security reports for their owned components, through both public-repository PVR and private-repository internal email. Maintainers configure the necessary permissions and notifications; CODEOWNERS assignment alone does not configure GitHub delivery.

## Public repositories

Use the affected public repository's **Security and quality → Report a vulnerability** flow when Private Vulnerability Reporting is enabled. Submit the affected version, summary, safe reproduction and impact through that private form. Reports may be written in English, Portuguese or Spanish. Do not include secrets, customer data or unnecessary sensitive attachments.

The organization provides a default `.github/VULNERABILITY_REPORT.yml`; a repository-specific form takes precedence. A template does not enable the feature or prove that responders are monitoring it. If the private reporting option is absent or unavailable, request private reporting instructions from a maintainer without disclosing the vulnerability. Do not substitute an ordinary issue containing security details.

## Private repositories

Email the relevant **CODEOWNERS** using existing internal Versat channels. Identify the owners responsible for the affected paths from the repository's CODEOWNERS file, then obtain their email addresses through the internal directory or an established internal contact. Do not guess email addresses from GitHub usernames or publish internal contacts.

If CODEOWNERS is missing, ownership is unclear or internal contact access is unavailable, ask the repository maintainer or your existing Versat contact for private routing instructions without disclosing sensitive details. A private repository issue is not a substitute for this route: its audience may exceed the intended recipients.

## Receipt and scope

This policy does not grant access to private repositories or permission to conduct tests. No response deadline or continuous monitoring is promised here. Maintainers must establish permitted recipients, notifications and actual receipt before claiming a route is verified. Keep vulnerability details private while coordinating remediation.
