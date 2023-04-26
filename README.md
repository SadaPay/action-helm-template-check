# action-helm-template-check

<!-- action-docs-description -->
## Description

Verify helm generation template
<!-- action-docs-description -->

<!-- action-docs-inputs -->
## Inputs

| parameter | description | required | default |
| --- | --- | --- | --- |
| aws-access-key-id | AWS access key ID to perform the helm login (if empty no login will be performed) | `false` |  |
| aws-region | AWS region where the ECR repo is | `false` | me-south-1 |
| aws-secret-access-key | AWS secret access key to perform the helm login (if empty no login will be performed) | `false` |  |
| chart-path | Path of the helm chart | `false` | chart |
| disable-checkout | Set to true to disable the code checkout step | `false` | false |
| service-name | Defining service-name for charts | `true` | ${{ github.event.repository.name }} |
| values-staging | Helm values for staging | `true` | chart/values-staging.yaml |
| values-production | Helm values for production | `true` | chart/values-production.yaml |
<!-- action-docs-inputs -->

<!-- action-docs-outputs -->

<!-- action-docs-outputs -->

<!-- action-docs-runs -->
## Runs

This action is a `composite` action.
<!-- action-docs-runs -->
