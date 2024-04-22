# AlexJS pre-commit mirror

Mirror of [AlexJS](https://alexjs.com) for [pre-commit](https://pre-commit.com).

## Using AlexJS with `pre-commit`

Example `.pre-commit.config.yml`:

```yaml
repos:
  - repo: "https://github.com/mfisher87/alexjs-pre-commit-mirror"
    rev: "v11.0.1"  # Use the sha / tag you prefer
    hooks:
    - id: "alex"
```

## Continuous Integration

Two example ways to run AlexJS inclusive language checks in CI for your repository using
your existing `pre-commit` configuration from the previous step:

* [The official pre-commit GitHub action](https://github.com/pre-commit/action): :rock:
  Very stable
* [pre-commit.ci](https://pre-commit.ci): :zap: Faster, but has more frequent outages.


## Troubleshooting


### I ignored a file in `.alexignore` but `pre-commit` is still failing

See this issue: <https://github.com/get-alex/alex/issues/348>
