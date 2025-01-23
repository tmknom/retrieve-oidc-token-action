# retrieve-oidc-token-action

Retrieve OIDC token's claims for GitHub.

<!-- actdocs start -->

## Description

This action retrieves OIDC token's claims from GitHub OpenID Connect Provider.
Use this action, you can get JWT claims such as `sub`, `workflow` and `job_workflow_ref`.

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
| payload | The JWT payload included OIDC token as plain JSON. |

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
