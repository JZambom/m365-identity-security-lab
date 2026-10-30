# Portfolio safety and publishing policy

## Scope

This is an independent personal learning project. Publish original lab work and clearly labelled synthetic data only. Do not connect its scripts to an employer's tenant or copy material out of an employer's systems.

## Before every commit or browser upload

- [ ] Every file is original personal lab material or an appropriately attributed public reference.
- [ ] No employer documents, internal code, ticket records or company exports are included.
- [ ] No real employee, customer or supplier details are included.
- [ ] No company domains, internal hostnames, network details or tenant configurations are exposed.
- [ ] No passwords, access tokens, client secrets, private keys or sensitive connection strings are present.
- [ ] Example identities and datasets are synthetic and explicitly labelled as such.
- [ ] Screenshots, logs, notebook outputs and metadata have been reviewed; no company screenshots are used.
- [ ] Proposed changes and filenames have been inspected, including any newly added files.
- [ ] Documentation distinguishes planned work, simulated tests and verified tenant experiments.

## Local Git workflow

Review `git status --short` and `git diff` before staging. Stage only intended files, then review `git diff --cached --stat` and `git diff --cached` before committing. Review any new file's complete contents, not just its name.

The `.gitignore` patterns are an extra precaution, not a substitute for review or secret scanning. They do not untrack existing files or erase history. Do not rely on `.gitignore` when choosing files for a browser upload; inspect the upload selection itself.

A private repository is not permission to upload employer-owned or confidential material.

## Test environment boundaries

Use a separate personal test tenant with fictitious accounts and the permissions needed for the specific experiment. Start with read-only reporting. Before making configuration changes, document the test scope, expected behaviour, recovery steps and results. Keep credentials outside the repository.

## Accidental exposure

Stop publishing. Treat any exposed credential as compromised and revoke or rotate it through the relevant service. Removing the current file alone is not sufficient because repository history may retain it. For any suspected employer information, follow the employer's incident-reporting process. Do not include secrets or personal data in public issues.

## Reference guidance

- [GitHub: Ignoring files](https://docs.github.com/en/get-started/git-basics/ignoring-files)
- [GitHub: Adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
- [GitHub: Removing sensitive data from a repository](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository)
