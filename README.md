# python-namespace-demo

This GIT repo combines all sub-command projects together with base GIT repo.

**Note 1:** We have `namespace_demo.main_demo.py` to wrap CLI. We are not overwriting base module `namespace_demo.main`.

**Note 2**: main cli is still from base module `demo-cli = "namespace_demo.main_demo:cli"` so that all sub-commands are available.

## Run

```shell
$ poetry run demo-cli
Usage: demo-cli [OPTIONS] COMMAND [ARGS]...

Options:
  --help  Show this message and exit.

Commands:
  app1
  app2
```