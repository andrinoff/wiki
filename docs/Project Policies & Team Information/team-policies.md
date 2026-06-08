# Oreon Team Policies

## Contributions and maintaining

All commits must be signed with a PGP key. See [oreonhq/how-pgp](https://github.com/oreonhq/how-pgp) for a guide on setting up PGP signing.

All changes must be submitted through a pull request. Direct pushes to protected branches are not permitted.

All changes must be approved by the repository maintainer before merging.

If a commit from an external contributor is not PGP-signed, the approving maintainer must re-sign it before merging:

```
git commit --amend -S --no-edit
```

## Repository creation

New repositories must follow the standard setup process:

1. Create a new repository from the [oreonhq/default-repo](https://github.com/oreonhq/default-repo) template.
2. Clone the repository locally and remove the `.git` directory.
3. Import the JSON ruleset: go to **Settings → Rules → Rulesets → New Ruleset → Import from JSON** and select `rules.json`.
4. Delete `rules.json` after the ruleset has been imported.
5. Create a team named after the repository.
6. Edit `.github/CODEOWNERS` and set the default owner: `* @oreonhq/<repo_name>`
