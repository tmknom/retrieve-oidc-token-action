# retrieve-oidc-token-action

Retrieve OIDC token's claims for GitHub.

<!-- actdocs start -->

## Description

This action retrieves an OIDC token from the GitHub OpenID Connect Provider,
decodes its payload, and extracts claims such as actor, repository, and workflow metadata.
The data is organized into structured outputs for easier integration with external systems or workflow debugging.

## Usage

```yaml
  steps:
    - name: Retrieve OIDC Token
      uses: tmknom/retrieve-oidc-token-action@v0
```

## Inputs

N/A

## Outputs

| Name | Description |
| :--- | :---------- |
| actor | The `actor` claim is the name of the person or app that initiated the workflow. |
| actor_id | The `actor_id` claim is the account ID of the person or app that triggered the initial workflow run. |
| aud | The `aud` claim identifies the recipients that the JWT is intended for. |
| base_ref | The `base_ref` claim is the name of the base ref or target branch of the pull request in a workflow run. |
| event_name | The `event_name` claim is the name of the event that triggered the workflow. |
| exp | The `exp` claim is the expiry time of the JWT. |
| head_ref | The `head_ref` claim is the head ref or source branch of the pull request in a workflow run. |
| iat | The `iat` claim is the time when the JWT was issued. |
| iss | The `iss` claim is the issuer of the OIDC token. |
| job_workflow_ref | The `job_workflow_ref` claim is the ref path to the reusable workflow. |
| job_workflow_sha | The `job_workflow_sha` claim is the commit SHA for the reusable workflow file. |
| jti | The `jti` claim is a unique identifier for the OIDC token. |
| nbf | The `nbf` claim is the time before which the token cannot be used. |
| payload | The JWT payload included OIDC token as plain JSON. |
| ref | The `ref` claim is the fully-formed ref of the branch or tag that triggered the workflow run. |
| ref_protected | The `ref_protected` claim is `true` if branch protections or rulesets are configured for the ref that triggered the workflow run. |
| ref_type | The `ref_type` claim is the type of ref that triggered the workflow run. |
| repository | The `repository` claim is the owner and repository name. |
| repository_id | The `repository_id` claim is the ID of the repository. |
| repository_owner | The `repository_owner` claim is the repository owner's name. |
| repository_owner_id | The `repository_owner_id` claim is the  repository owner's account ID. |
| repository_visibility | The `repository_visibility` claim is the visibility of the repository where the workflow is running. |
| run_attempt | The `run_attempt` claim is a unique number for each attempt of a particular workflow run in a repository. |
| run_id | The `run_id` claim is a unique number for each workflow run within a repository. |
| run_number | The `run_number` claim is a unique number for each run of a particular workflow in a repository. |
| runner_environment | The `runner_environment` claim is the environment of the runner executing the job. |
| sha | The `sha` claim is the commit SHA that triggered the workflow. |
| sub | The `sub` claim identifies the principal that is the subject of the JWT. |
| workflow | The `workflow` claim is the name of the workflow. |
| workflow_ref | The `workflow_ref` claim is the ref path to the workflow. |
| workflow_sha | The `workflow_sha` claim is the commit SHA for the workflow file. |

<!-- actdocs end -->

## Permissions

| Scope    | Access |
| :------- | :----- |
| id-token | write  |

## FAQ

N/A

## Related projects

N/A

## Release notes

See [GitHub Releases][releases].

[releases]: https://github.com/tmknom/retrieve-oidc-token-action/releases
