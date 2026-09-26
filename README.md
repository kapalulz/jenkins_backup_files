# Jenkins Backup Files — Educational Snapshot

An example Jenkins backup captured while testing a backup-and-restore workflow.

## Purpose

The snapshot demonstrates the kinds of controller files and plugins involved in a Jenkins restore. It was paired with a pipeline that archived selected data and transferred the resulting backup.

Related Jenkins plugins:

- [ThinBackup](https://plugins.jenkins.io/thinBackup/)
- [HTTP Request](https://www.jenkins.io/doc/pipeline/steps/http_request/)

## Important security warning

Do not use a public Git repository for Jenkins backups. Jenkins home data may contain encrypted credentials, controller secrets, user records, job configuration, and plugin binaries.

For a real environment:

- Store encrypted backups in a private bucket or backup system.
- Restrict access with least-privilege IAM.
- Exclude credentials, controller secrets, user data, caches, and plugin binaries.
- Rotate every credential that was ever committed.
- Test recovery in an isolated environment.
- Define retention and deletion policies.

> This repository should be treated as a historical learning artifact. Its contents require sanitization before they can be shared safely.
