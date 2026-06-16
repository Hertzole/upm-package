# upm-package

⚠️ In development! Use at own risk! ⚠️  
Variables, outputs and more may change suddenly!

## Inputs

| Name | Description | Default | Required |
| -- | -- | -- | -- |
| `package-json` | The path to the package.json file.<br>relative to the repository root. | `*/Packages/*package.json` | No |
| `create-branch` | Whether to create a branch for the package.<br>If false, no branch will be created. | `true` | No |
| `branch-name` | The name of the branch created.<br>Only applicable if `create-branch` is true. | `upm` | No |
| `skip-ci` | If true, `[skip ci]` will be appended to the commit message. | `true` | No |
| `remove-tests` | If true, any folder called `Tests` in the package root will be removed. | `true` | No |
| `include-samples` | If true, the specified samples folder will be included, if it exists.<br>Samples will be moved to `$package_root/Samples~` | `true` | No |
| `samples-destination` | The source destination for the samples. | `Assets/Samples` | No |
| `include-plugins` | If true, any `Plugins` folder in package root will be included. | `true` | No |
| `signing-key-id` | Unity service account key ID for signing packages | - | No |
| `signing-key-secret` | Unity service account key secret for signing packages | - | No |
| `signing-org-id` | Unity organization ID for signing packages | - | No |

## Outputs

| Name | Description |
| -- | -- |
| `signed-archive` | The path to the signed package archive, if it was created. |
| `created-archive` | `true` if a signed archive was created, otherwise `false` |
