# GitHub Action: [building_blocks]

[![GitHub Actions status](https://github.com/iahmedelbayaa/github-actions-course/workflows/building_blocks/badge.svg)](https://github.com/iahmedelbayaa/github-actions-course/actions)

## Overview

[building_blocks] is a GitHub Action that show structure of Github actions and how did work. This action helps to study and show steps tp create a yml file that will work on actions.

## Features

- building blocks
- use events like push or etc...
- Feature 3

## Usage

To use this GitHub Action, you need to add a new workflow file to your repository under `.github/workflows` directory. Below is an example of how to configure this action:

```yaml
name: [building_blocks]

on: 
  push:
    branches:
      - main

jobs:
  [job_name]:
    runs-on: ubuntu-latest
    
    steps:
      - name: Checkout repository
        uses: actions/checkout@v2

      - name: Run [Action Name]
        uses: [OWNER]/[REPOSITORY]@v1
        with:
          # Add required inputs here
          input1: value1
          input2: value2
```

## Inputs

| Input Name | Description           | Required | Default |
|------------|-----------------------|----------|---------|
| `input1`   | Description of input1 | true     |         |
| `input2`   | Description of input2 | false    | value2  |

## Outputs

| Output Name | Description            |
|-------------|------------------------|
| `output1`   | Description of output1 |
| `output2`   | Description of output2 |

## Example Workflow

Here is an example of a complete workflow using this action:

```yaml
name: Example Workflow

on: 
  pull_request:
    branches:
      - main

jobs:
  example:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v2

      - name: Run [Action Name]
        uses: [OWNER]/[REPOSITORY]@v1
        with:
          input1: value1
          input2: value2
```

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.

## License

This project is licensed under the [LICENSE_NAME] License - see the [LICENSE](LICENSE) file for details.
