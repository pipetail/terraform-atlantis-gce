## Providers

| Name | Version |
|------|---------|
| google | ~> 3.32 |
| null | ~> 2.1 |
| random | ~> 2.3 |
| tls | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:-----:|
| client\_email | Service account email address | `string` | `""` | no |
| cos\_image\_name | The forced COS image to use instead of latest | `string` | `"cos-stable-77-12371-89-0"` | no |
| github\_token | GitHub API token | `string` | n/a | yes |
| github\_user | GitHub user | `string` | n/a | yes |
| image | docker image ref to be used | `string` | `"runatlantis/atlantis:v0.15.1"` | no |
| image\_port | The port the image exposes for HTTP requests | `number` | `4141` | no |
| instance\_name | The desired name to assign to the deployed instance | `any` | n/a | yes |
| network | The GCP network | `string` | `"default"` | no |
| project | GCP project id | `string` | n/a | yes |
| region | GCP region | `string` | `"us-central1"` | no |
| repo\_allowlist | GitHub repo allow list | `string` | n/a | yes |
| webhook\_secret | GitHub webhook secret | `string` | n/a | yes |
| zone | The GCP zone to deploy instances into | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| atlantis\_ip | The public IP address of the deployed instance |

