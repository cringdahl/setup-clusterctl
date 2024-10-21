# Setup Clusterctl

This action sets up clusterctl for use in actions by:

- Downloading and caching a version of `clusterctl`, optionally by version, and adding to `$PATH`

```yaml
steps:
  - uses: cringdahl/setup-clusterctl@v1
  - run: clusterctl version
```

```yaml
steps:
  - uses: cringdahl/setup-clusterctl@v1
    with:
      clusterctl-version: 1.4.8
  - run: clusterctl version
```
