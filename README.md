# retrieve-oidc-token-action

Retrieve OIDC token's claims for GitHub.

<!-- actdocs start -->

## Description

This action retrieves and decodes an OIDC token from the GitHub OpenID Connect Provider, exposing its JWT payload as JSON for workflows.
It simplifies managing OIDC tokens in GitHub Actions and enables secure access to JWT claims.

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
