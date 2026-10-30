# Microsoft 365 Identity & Security Lab

> **Status: planning and documentation.** No tenant configuration, automation scripts or test results have been implemented or validated yet.

## Project purpose

An independent personal lab to develop and demonstrate practical Microsoft 365 identity administration, security fundamentals and IT operations automation. The focus is on repeatable processes, clear documentation and useful business reporting.

## Fictional business scenario

A fictional small business has office-based and remote employees using Microsoft 365. Its IT team needs consistent onboarding and offboarding, appropriate access permissions, stronger sign-in controls and clearer visibility of user access.

This scenario is invented. It does not reproduce an employer's environment, processes, incidents or data.

## Planned technologies

| Technology | Intended use |
| --- | --- |
| Microsoft 365 and Microsoft Entra ID | Identity, group and role administration in a separate personal test tenant |
| PowerShell and Microsoft Graph | Read-only lab inventory and repeatable reporting |
| Python | Validate synthetic records and generate reports |
| SQL / SQLite | Query synthetic identity records locally; not a production database |
| Git and GitHub | Version control, documentation and evidence of progress |

## Intended deliverables

- A documented joiner, mover and leaver workflow, with approval and verification steps.
- A least-privilege access design covering standard users and administrative roles.
- An MFA design and a comparison of security defaults with Conditional Access.
- A synthetic identity dataset, data dictionary and repeatable Python/SQL reporting example.
- Read-only PowerShell/Microsoft Graph reporting in an isolated test tenant, when available.
- Test cases, expected and observed results, limitations, and troubleshooting or rollback notes for any configuration changes.

## Intended business value

The project aims to make account administration more consistent, reduce manual reporting effort and improve visibility of access risks. These are intended outcomes, not measured achievements.

Future evidence will distinguish simulated results from tenant-tested results. Any time-saving claim will include a measured manual baseline and a comparable automated test.

## Roadmap

- [x] Define the fictional scenario, scope and planned technologies.
- [x] Document confidentiality and publishing rules.
- [ ] Create synthetic records and expected test outcomes.
- [ ] Build and test the first Python/SQL report.
- [ ] Add read-only Graph reporting in a personal test tenant.
- [ ] Document identity-security experiments and verified results.

## Environment and licensing boundaries

Start with documentation and offline synthetic data. A Microsoft 365 subscription is not needed for those activities.

Live tenant experiments must use a separate personal test environment, never an employer's tenant. Conditional Access testing requires appropriate licensing, such as Microsoft Entra ID P1 or a plan that includes it. Security defaults are a separate baseline option; they are not presented here as something to run alongside Conditional Access. Tenant-dependent work remains design-only until a suitable environment is available. See Microsoft's [security defaults guidance](https://learn.microsoft.com/en-us/entra/fundamentals/security-defaults) and [licensing guidance](https://learn.microsoft.com/en-us/entra/fundamentals/licensing).

## Confidentiality and safe publishing

Only original personal lab material and clearly labelled synthetic data belong in this repository. Do not include employer documents, internal code, tickets, exports, screenshots, real employee/customer records or company-specific configurations.

Never commit passwords, access tokens, client secrets, private keys or connection strings. Review every proposed change before publishing. The included `.gitignore` is a convenience, not a security guarantee; it does not remove information already committed. See [GitHub's guidance on ignored files](https://docs.github.com/en/get-started/git-basics/ignoring-files).

See [SECURITY.md](SECURITY.md) for the publishing checklist. This is an independent learning project, not a production security deployment or a representation of any employer's systems.
