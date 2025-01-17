 <!-- Space: TerraformGrafanaDashboard -->
<!-- Title: Project -->

<!--


  ** DO NOT EDIT THIS FILE
  **
  ** 1) Make all changes to `provision/generator/README.yaml`
  ** 2) Run`task readme` to rebuild this file.
  **
  ** (We maintain HUNDREDS of open source projects. This is how we maintain our sanity.)
  **


  -->

[![Latest Release](https://img.shields.io/github/release/hadenlabs/terraform-grafana-dashboard)](https://github.com/hadenlabs/terraform-grafana-dashboard/releases) [![Lint](https://img.shields.io/github/workflow/status/hadenlabs/terraform-grafana-dashboard/lint-code)](https://github.com/hadenlabs/terraform-grafana-dashboard/actions?workflow=lint-code) [![CI](https://img.shields.io/github/workflow/status/hadenlabs/terraform-grafana-dashboard/ci)](https://github.com/hadenlabs/terraform-grafana-dashboard/actions?workflow=ci) [![Test](https://img.shields.io/github/workflow/status/hadenlabs/terraform-grafana-dashboard/test)](https://github.com/hadenlabs/terraform-grafana-dashboard/actions?workflow=test) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit) [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow)](https://conventionalcommits.org) [![KeepAChangelog](https://img.shields.io/badge/changelog-Keep%20a%20Changelog%20v1.0.0-orange)](https://keepachangelog.com) [![Terraform Version](https://img.shields.io/badge/terraform-1.x%20|%200.15%20|%200.14%20|%200.13%20|%200.12.20+-623CE4.svg?logo=terraform)](https://github.com/hashicorp/terraform/releases)

# terraform-grafana-dashboard

terraform-grafana-dashboard for project

## Requirements

This is a list of plugins that need to be installed previously to enjoy all the goodies of this configuration:

- [terraform](https://github.com/hashicorp/terraform)
- [taskfile](https://github.com/go-task/task)

## Usage

```hcl
  module "main" {
    source  = "hadenlabs/dashboard/grafana"
    version = "0.0.0"
  }
```

Full working examples can be found in [examples](./examples) folder.

## Examples

<!-- Space: TerraformGrafanaDashboard -->
<!-- Parent: Project -->
<!-- Title: Project Examples -->

<!-- Label: Examples -->
<!-- Include: docs/disclaimer.md -->
<!-- Include: ac:toc -->

### common

```hcl
  module "main" {
    source  = "hadenlabs/dashboard/grafana"
    version = "0.0.0"
  }
```

 <!-- BEGIN_TF_DOCS -->

## Requirements

| Name                                                                     | Version           |
| ------------------------------------------------------------------------ | ----------------- |
| <a name="requirement_terraform"></a> [terraform](#requirement_terraform) | >= 0.12.20, < 2.0 |
| <a name="requirement_grafana"></a> [grafana](#requirement_grafana)       | >=1.19.0, < 2.0   |

## Providers

| Name                                                         | Version         |
| ------------------------------------------------------------ | --------------- |
| <a name="provider_grafana"></a> [grafana](#provider_grafana) | >=1.19.0, < 2.0 |

## Modules

No modules.

## Resources

| Name | Type |
| --- | --- |
| [grafana_dashboard.this](https://registry.terraform.io/providers/grafana/grafana/latest/docs/resources/dashboard) | resource |

## Inputs

| Name | Description | Type | Default | Required |
| --- | --- | --- | --- | :-: |
| <a name="input_enabled"></a> [enabled](#input_enabled) | Set to false to prevent the module from creating any resources | `bool` | `true` | no |
| <a name="input_file_dashboard"></a> [file_dashboard](#input_file_dashboard) | JSON file to Grafana dashboard | `string` | n/a | yes |
| <a name="input_folder"></a> [folder](#input_folder) | ID folder to save the dashboard | `number` | `0` | no |

## Outputs

| Name                                                     | Description                |
| -------------------------------------------------------- | -------------------------- |
| <a name="output_enabled"></a> [enabled](#output_enabled) | Enabled property of module |
| <a name="output_id"></a> [id](#output_id)                | Grafana dashboard ID       |
| <a name="output_uid"></a> [uid](#output_uid)             | Grafana dashboard UID      |
| <a name="output_version"></a> [version](#output_version) | Grafana dashboard version  |

<!-- END_TF_DOCS -->

## Help

**Got a question?**

File a GitHub [issue](https://github.com/hadenlabs/terraform-grafana-dashboard/issues).

## Contributing

See [Contributing](./docs/contributing.md).

## Module Versioning

This Module follows the principles of [Semantic Versioning (SemVer)](https://semver.org/).

Using the given version number of `MAJOR.MINOR.PATCH`, we apply the following constructs:

1. Use the `MAJOR` version for incompatible changes.
1. Use the `MINOR` version when adding functionality in a backwards compatible manner.
1. Use the `PATCH` version when introducing backwards compatible bug fixes.

### Backwards compatibility in `0.0.z` and `0.y.z` version

- In the context of initial development, backwards compatibility in versions `0.0.z` is **not guaranteed** when `z` is increased. (Initial development)
- In the context of pre-release, backwards compatibility in versions `0.y.z` is **not guaranteed** when `y` is increased. (Pre-release)

## Copyright

Copyright © 2018-2022 [Hadenlabs](https://hadenlabs.com)

## Trademarks

All other trademarks referenced herein are the property of their respective owners.

## License

The code and styles are licensed under the LGPL-3.0 license [See project license.](LICENSE).

## Don't forget to 🌟 Star 🌟 the repo if you like terraform-grafana-dashboard

[Your feedback is appreciated](https://github.com/hadenlabs/terraform-grafana-dashboard/issues)
