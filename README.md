This Repo describes [organization-wide health files](https://github.blog/changelog/2019-02-21-organization-wide-community-health-files/) (eg `CONTRIBUTING`, `SUPPORT`, `CODE_OF_CONDUCT`, `ISSUE_TEMPLATE`, or `PULL_REQUEST_TEMPLATE`).

We are also using this Repo for organization-wide tickets/issues.

## Labels
All repos in the organization have the same labels for pull requests and issues. 

If you want to update them:

1. Install `github-label-sync`
```
npm install -g github-label-sync
```

2. Get the GITHUB_ACCESS_TOKEN environment variable for access to fetch and update labels.The token must have permission to write to the repository. See https://github.com/settings/tokens on how to create this token. The token GITHUB_ACCESS_TOKEN can be passed in the command line or defined in ~/.profile (see https://help.ubuntu.com/community/EnvironmentVariables#A.2BAH4-.2F.profile).

3. Run 
```
github-label-sync --access-token $GITHUB_ACCESS_TOKEN --labels labels.json drift-org/demo-app
```
and replace `drift-org/demo-app` with whatever repo you are updating.