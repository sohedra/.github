# Sohedra community files

Default community health files for the [Sohedra](https://github.com/sohedra) organization. GitHub
shows them in every repository that has no file of its own of the same kind.

- [Code of Conduct](./CODE_OF_CONDUCT.md): Contributor Covenant 3.0
- [Security policy](./SECURITY.md)
- [Funding](./FUNDING.yml): the **Sponsor** button, shown on repositories with Sponsorships turned
  on
- [Issue settings](./.github/ISSUE_TEMPLATE/config.yml)
- [Organization profile](./profile/README.md)
- [Renovate preset](./renovate-preset.json): shared dependency-update settings. A repository uses it
  with `"extends": ["local>sohedra/.github:renovate-preset"]` in its `renovate.json`.
