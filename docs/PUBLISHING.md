# Maintaining public releases

1. Update the workflow and relevant examples without adding private operational records.
2. Update `VERSION`, `CHANGELOG.md`, `.zenodo.json` and `CITATION.cff` together. Use the actual public release date.
3. Parse JSON/YAML, review internal links and scan the staged file list for private identifiers, artwork, credentials and local paths.
4. Commit the public files to the GitHub repository.
5. Enable only the intended public repository in the owner's existing Zenodo GitHub integration before publishing its first GitHub release.
6. Publish a GitHub release tagged `v<version>` from the reviewed commit. Zenodo should ingest the release archive. Inspect the actual Zenodo result before reporting a DOI.
7. Verify the record title, creator, resource type, version, license, archived files and GitHub relationship. If ingestion fails or remains pending, inspect that release's integration status before retrying; avoid creating duplicate Zenodo records.
8. Add the actual DOI to the repository citation and README once assigned. Do not move an existing version tag to include later metadata edits. Record future substantive changes in a new version.

`.zenodo.json` controls the Zenodo metadata when both it and `CITATION.cff` are present. The citation file also supports GitHub's citation display. This package describes a workflow and requests the Workflow resource type; inspect the deposited record rather than assuming the integration preserved the type.

Official guidance:

- [Enable a repository](https://help.zenodo.org/docs/github/enable-repository/)
- [Describe GitHub releases](https://help.zenodo.org/docs/github/describe-software/)
- [Manage versions](https://help.zenodo.org/docs/deposit/manage-versions/)

Publication on Zenodo supplies an archival identifier. It does not itself validate the workflow's scientific novelty, correctness or operating guarantees.
