# Install Verilator Action

Install Verilator for use in a Github Action workflow.

## Usage

See [`action.yml`](./action.yaml)

Here's a basic example:

```yaml
name: Using Verilator example
on:
  pull_request:
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@master
    - uses: v0xnihili/install-verilator-action@main
    - run: verilator --version
```
