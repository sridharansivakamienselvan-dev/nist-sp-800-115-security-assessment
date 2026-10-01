# Security Assessment to NIST SP 800-115

Technical lead on a simulated client security assessment for a UK managed security provider, planned and executed against NIST SP 800-115 with OWASP testing guidance.

## Status

Work in progress. This repository is being built from scratch and will hold the methodology, tooling notes, and sanitised findings from the engagement.

## Scope and approach

Test planning followed the phases set out in NIST SP 800-115, covering planning, execution, post-execution, and reporting. An isolated Docker lab hosted the target environment so that testing stayed contained. Services and versions were enumerated with Nmap, and every finding was manually verified rather than accepted from scanner output.

## Findings and reporting

Five vulnerabilities were demonstrated and scored under CVSS v3.1, including SQL injection and command injection, both rated 9.8. Findings were recorded in a risk register that ties each issue to business impact, alongside a compliance gap analysis against Cyber Essentials, ISO/IEC 27001:2022, the NCSC CAF, and UK GDPR, and a phased remediation roadmap.

## Planned repository layout

Documentation of the test plan and methodology will live under docs, lab build files under lab, enumeration and verification notes under findings, and the risk register and remediation roadmap under reporting.

## Note

This was an academic, consent-based exercise against a simulated client environment. No real client data or live third-party systems are included.
