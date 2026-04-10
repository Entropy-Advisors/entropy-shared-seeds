# entropy-shared-seeds

Shared reference data (labels, entities, tokens) for Entropy dbt projects.

## Install

Add to your dbt project's `packages.yml`:

```yaml
packages:
  - git: "git@github.com:Entropy-Advisors/entropy-shared-seeds.git"
    revision: main
```

Then run `dbt deps && dbt seed`.

## Contributing

Open a PR with the label change. Both the Dune and ClickHouse projects will
pick it up on their next `dbt deps` run.
